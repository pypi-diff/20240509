# Comparing `tmp/readfish-2024.1.0.tar.gz` & `tmp/readfish-2024.2.0.tar.gz`

## Comparing `readfish-2024.1.0.tar` & `readfish-2024.2.0.tar`

### file list

```diff
@@ -1,155 +1,157 @@
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 readfish-2024.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 readfish-2024.1.0/CITATION.cff
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq.yml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq/FAQ.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/faq/suggest.md
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/faqtory.yml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 readfish-2024.1.0/.github/workflows/stale.yml
--rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish.jpg
--rw-r--r--   0        0        0   164136 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_dark.png
--rw-r--r--   0        0        0   190609 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_light.png
--rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_logo.jpg
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/readfish_small.jpg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/example_tomls/COSMIC_cancer_panel.bed
--rw-r--r--   0        0        0   228736 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackControlRun30Minutes.png
--rw-r--r--   0        0        0   206755 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargeted.png
--rw-r--r--   0        0        0   222323 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargetedPeak.png
--rw-r--r--   0        0        0   224078 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunTargetedUnblockPeak.png
--rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunUnblock.png
--rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackRunUnblockCloseUp.png
--rw-r--r--   0        0        0   202426 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackUnblockAll30minutes.png
--rw-r--r--   0        0        0   211500 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/PlaybackUnblockAllCloseUp.png
--rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/Unblock.png
--rw-r--r--   0        0        0   151624 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/UnblockAllMessages.png
--rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/Unblock_closeup.png
--rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/control.png
--rw-r--r--   0        0        0   284161 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model.png
--rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model.svg
--rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/data_model_no_bg.svg
--rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/message.png
--rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/minknow_messages.png
--rw-r--r--   0        0        0   103153 2020-02-02 00:00:00.000000 readfish-2024.1.0/_static/images/simulated_playback_run_options.png
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/FAQ.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/changelog.md
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/conf.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/developers-guide.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/development.yml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/getting-started.md
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/guppy-params.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/make.bat
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/post-analysis.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.console.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.plugins.rst
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/readfish.rst
--rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/toml.md
--rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/PlaybackRunUnblock.png
--rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/PlaybackRunUnblockCloseUp.png
--rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/Unblock.png
--rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/Unblock_closeup.png
--rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/control.png
--rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/message.png
--rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/minknow_messages.png
--rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish.jpg
--rw-r--r--   0        0        0   237831 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish.png
--rw-r--r--   0        0        0   217946 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_dark.png
--rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_logo.jpg
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/images/readfish_small.jpg
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/batch-times.question.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/creating_readfish-environment.question.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/key_error_adapter.md
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/py-guppy-client-error.question.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/py-guppy-client-version.question.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2024.1.0/docs/questions/readfish-branches.question.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__about__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/__main__.py
--rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_channels.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_cli_args.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_cli_base.py
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_config.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_loggers.py
--rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_read_until_client.py
--rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_statistics.py
--rw-r--r--   0        0        0    15654 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/demultiplex.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/stats.py
--rw-r--r--   0        0        0    30418 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/targets.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/unblock_all.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/entry_points/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_filter.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_mappy.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/_no_op.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/deepnano_blitz.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/guppy.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/mappy.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/mappy_rs.py
--rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/plugins/utils.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/_version.py
--rw-r--r--   0        0        0    25181 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/base.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 readfish-2024.1.0/src/readfish/read_until/read_cache.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/describe_test.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/stats_test.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/utils_test.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/validation_test.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_aligner_regions_expected.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_barcoded_experiment_expected.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/describe_experiment_regions_expected.txt
--rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/README.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/001_no_write_socket.txt
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/002_missing_socket.txt
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/003_no_read_socket.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/5555_fail_nr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/fail/5555_fail_nw
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/001_correct_debug.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/002_correct_no_debug.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/guppy_validation_test/pass/5555_pass
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/README.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/001_wrong_reference_type.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/002_reference_not_exist.txt
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/003_wrong_reference_type_mmi_gz.txt
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/004_bad_reference_file_extension.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/bad_extension.mmi.cabbage
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.mmi.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/001_correct_reference_mmi.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/002_correct_reference_fasta.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/003_correct_reference_fastq.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/004_correct_reference_fasta_gz.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/005_correct_reference_fastq_gz.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/006_passing_fna_mmi.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.mmi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fasta
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fasta.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fastq
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.fastq.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/mappy_validation_test/pass/hello.mmi
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/expected_summary.txt
--rw-r--r--   0        0        0   997010 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/simulated_reads.fastq
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/stats.tsv
--rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/README.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/001_missing_keys.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/002_wrong_types.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/003_plugin_fail_0.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/003_plugin_fail_1.txt
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/fail/COSMIC_cancer_panel_errors.bed
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 readfish-2024.1.0/tests/static/toml_validation_test/pass/001_simple_toml.txt
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 readfish-2024.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 readfish-2024.1.0/LICENSE
--rw-r--r--   0        0        0    69691 2020-02-02 00:00:00.000000 readfish-2024.1.0/README.md
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 readfish-2024.1.0/pyproject.toml
--rw-r--r--   0        0        0    72472 2020-02-02 00:00:00.000000 readfish-2024.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 readfish-2024.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 readfish-2024.2.0/CITATION.cff
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/faq.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/faq/FAQ.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/faq/suggest.md
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/workflows/faqtory.yml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 readfish-2024.2.0/.github/workflows/stale.yml
+-rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/readfish.jpg
+-rw-r--r--   0        0        0   164136 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/readfish_dark.png
+-rw-r--r--   0        0        0   190609 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/readfish_light.png
+-rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/readfish_logo.jpg
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/readfish_small.jpg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/example_tomls/COSMIC_cancer_panel.bed
+-rw-r--r--   0        0        0   228736 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackControlRun30Minutes.png
+-rw-r--r--   0        0        0   206755 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackRunTargeted.png
+-rw-r--r--   0        0        0   222323 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackRunTargetedPeak.png
+-rw-r--r--   0        0        0   224078 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackRunTargetedUnblockPeak.png
+-rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackRunUnblock.png
+-rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackRunUnblockCloseUp.png
+-rw-r--r--   0        0        0   202426 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackUnblockAll30minutes.png
+-rw-r--r--   0        0        0   211500 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/PlaybackUnblockAllCloseUp.png
+-rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/Unblock.png
+-rw-r--r--   0        0        0   151624 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/UnblockAllMessages.png
+-rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/Unblock_closeup.png
+-rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/control.png
+-rw-r--r--   0        0        0   284161 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/data_model.png
+-rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/data_model.svg
+-rw-r--r--   0        0        0    38123 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/data_model_no_bg.svg
+-rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/message.png
+-rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/minknow_messages.png
+-rw-r--r--   0        0        0   103153 2020-02-02 00:00:00.000000 readfish-2024.2.0/_static/images/simulated_playback_run_options.png
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/FAQ.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/changelog.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/conf.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/developers-guide.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/development.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/getting-started.md
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/guppy-params.md
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/make.bat
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/post-analysis.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/readfish.console.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/readfish.plugins.rst
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/readfish.rst
+-rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/toml.md
+-rw-r--r--   0        0        0   155966 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/PlaybackRunUnblock.png
+-rw-r--r--   0        0        0   156826 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/PlaybackRunUnblockCloseUp.png
+-rw-r--r--   0        0        0   145644 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/Unblock.png
+-rw-r--r--   0        0        0   155720 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/Unblock_closeup.png
+-rw-r--r--   0        0        0   151990 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/control.png
+-rw-r--r--   0        0        0    69772 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/message.png
+-rw-r--r--   0        0        0   143794 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/minknow_messages.png
+-rw-r--r--   0        0        0    82708 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/readfish.jpg
+-rw-r--r--   0        0        0   237831 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/readfish.png
+-rw-r--r--   0        0        0   217946 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/readfish_dark.png
+-rw-r--r--   0        0        0    12731 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/readfish_logo.jpg
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/images/readfish_small.jpg
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/batch-times.question.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/creating_readfish-environment.question.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/key_error_adapter.md
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/py-guppy-client-error.question.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/py-guppy-client-version.question.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 readfish-2024.2.0/docs/questions/readfish-branches.question.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/__about__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/__main__.py
+-rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_channels.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_cli_args.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_cli_base.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_compatibility.py
+-rw-r--r--   0        0        0    19444 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_config.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_loggers.py
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_read_until_client.py
+-rw-r--r--   0        0        0    19105 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_statistics.py
+-rw-r--r--   0        0        0    15655 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/demultiplex.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/stats.py
+-rw-r--r--   0        0        0    31420 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/targets.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/unblock_all.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/entry_points/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/_filter.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/_mappy.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/_no_op.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/deepnano_blitz.py
+-rw-r--r--   0        0        0    19356 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/dorado.py
+-rw-r--r--   0        0        0    12892 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/guppy.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/mappy.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/mappy_rs.py
+-rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/plugins/utils.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/read_until/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/read_until/_version.py
+-rw-r--r--   0        0        0    25181 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/read_until/base.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 readfish-2024.2.0/src/readfish/read_until/read_cache.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/describe_test.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/stats_test.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/utils_test.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/validation_test.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_aligner_regions_expected.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_barcoded_experiment_expected.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/describe_experiment_regions_expected.txt
+-rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/fail/001_no_write_socket.txt
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/fail/002_missing_socket.txt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/fail/003_no_read_socket.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/fail/5555_fail_nr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/fail/5555_fail_nw
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/pass/001_correct_debug.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/pass/002_correct_no_debug.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/guppy_validation_test/pass/5555_pass
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/README.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/001_wrong_reference_type.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/002_reference_not_exist.txt
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/003_wrong_reference_type_mmi_gz.txt
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/004_bad_reference_file_extension.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/bad_extension.mmi.cabbage
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.mmi.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/fail/i_am_a_fail_reference.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/001_correct_reference_mmi.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/002_correct_reference_fasta.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/003_correct_reference_fastq.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/004_correct_reference_fasta_gz.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/005_correct_reference_fastq_gz.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/006_passing_fna_mmi.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.mmi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/hello.fasta
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/hello.fasta.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/hello.fastq
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/hello.fastq.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/mappy_validation_test/pass/hello.mmi
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/stats_test/expected_summary.txt
+-rw-r--r--   0        0        0   997010 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/stats_test/simulated_reads.fastq
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/stats_test/stats.tsv
+-rw-r--r--   0        0        0   531281 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/README.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/001_missing_keys.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/002_wrong_types.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/003_plugin_fail_0.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/003_plugin_fail_1.txt
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/fail/COSMIC_cancer_panel_errors.bed
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 readfish-2024.2.0/tests/static/toml_validation_test/pass/001_simple_toml.txt
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 readfish-2024.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 readfish-2024.2.0/LICENSE
+-rw-r--r--   0        0        0    71996 2020-02-02 00:00:00.000000 readfish-2024.2.0/README.md
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 readfish-2024.2.0/pyproject.toml
+-rw-r--r--   0        0        0    74974 2020-02-02 00:00:00.000000 readfish-2024.2.0/PKG-INFO
```

### Comparing `readfish-2024.1.0/.pre-commit-config.yaml` & `readfish-2024.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/CITATION.cff` & `readfish-2024.2.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.github/CONTRIBUTING.md` & `readfish-2024.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.github/faq/suggest.md` & `readfish-2024.2.0/.github/faq/suggest.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.github/workflows/CI.yml` & `readfish-2024.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.github/workflows/faqtory.yml` & `readfish-2024.2.0/.github/workflows/faqtory.yml`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.github/workflows/stale.yml` & `readfish-2024.2.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/readfish.jpg` & `readfish-2024.2.0/_static/readfish.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/readfish_dark.png` & `readfish-2024.2.0/_static/readfish_dark.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/readfish_light.png` & `readfish-2024.2.0/_static/readfish_light.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/readfish_logo.jpg` & `readfish-2024.2.0/_static/readfish_logo.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/readfish_small.jpg` & `readfish-2024.2.0/_static/readfish_small.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackControlRun30Minutes.png` & `readfish-2024.2.0/_static/images/PlaybackControlRun30Minutes.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackRunTargeted.png` & `readfish-2024.2.0/_static/images/PlaybackRunTargeted.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackRunTargetedPeak.png` & `readfish-2024.2.0/_static/images/PlaybackRunTargetedPeak.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackRunTargetedUnblockPeak.png` & `readfish-2024.2.0/_static/images/PlaybackRunTargetedUnblockPeak.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackRunUnblock.png` & `readfish-2024.2.0/_static/images/PlaybackRunUnblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackRunUnblockCloseUp.png` & `readfish-2024.2.0/_static/images/PlaybackRunUnblockCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackUnblockAll30minutes.png` & `readfish-2024.2.0/_static/images/PlaybackUnblockAll30minutes.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/PlaybackUnblockAllCloseUp.png` & `readfish-2024.2.0/_static/images/PlaybackUnblockAllCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/Unblock.png` & `readfish-2024.2.0/_static/images/Unblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/UnblockAllMessages.png` & `readfish-2024.2.0/_static/images/UnblockAllMessages.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/Unblock_closeup.png` & `readfish-2024.2.0/_static/images/Unblock_closeup.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/control.png` & `readfish-2024.2.0/_static/images/control.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/data_model.png` & `readfish-2024.2.0/_static/images/data_model.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/data_model.svg` & `readfish-2024.2.0/_static/images/data_model.svg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/data_model_no_bg.svg` & `readfish-2024.2.0/_static/images/data_model_no_bg.svg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/message.png` & `readfish-2024.2.0/_static/images/message.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/minknow_messages.png` & `readfish-2024.2.0/_static/images/minknow_messages.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/_static/images/simulated_playback_run_options.png` & `readfish-2024.2.0/_static/images/simulated_playback_run_options.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/FAQ.md` & `readfish-2024.2.0/docs/FAQ.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/Makefile` & `readfish-2024.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/conf.py` & `readfish-2024.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/developers-guide.md` & `readfish-2024.2.0/docs/developers-guide.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 ```console
 conda env create -f docs/development.yml
 ```
 
 ## Readfish versioning
 Readfish uses [calver](https://calver.org/) for versioning. Specifically the format should be
-`YYYY.MINOR.MICRO.Modifier`, where `MINOR` is the feature addiiton, `MICRO` is any hotfix/bugfix, and `Modifier` is the modifier (e.g. `rc` for release candidate, `dev` for development, empty for stable).
+`YYYY.MINOR.MICRO.Modifier`, where `MINOR` is the feature addition, `MICRO` is any hotfix/bugfix, and `Modifier` is the modifier (e.g. `rc` for release candidate, `dev` for development, empty for stable).
 
 ## Changelog
 
 We are generally trying to follow the guidance here. https://keepachangelog.com/en/1.0.0/
 
 Notably we should correctly update the Unreleased section for things added in the PRs that are inbetween releases.
```

### Comparing `readfish-2024.1.0/docs/getting-started.md` & `readfish-2024.2.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/guppy-params.md` & `readfish-2024.2.0/docs/guppy-params.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/make.bat` & `readfish-2024.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/post-analysis.md` & `readfish-2024.2.0/docs/post-analysis.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/readfish.console.rst` & `readfish-2024.2.0/docs/readfish.console.rst`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/readfish.plugins.rst` & `readfish-2024.2.0/docs/readfish.plugins.rst`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/readfish.rst` & `readfish-2024.2.0/docs/readfish.rst`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/toml.md` & `readfish-2024.2.0/docs/toml.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/PlaybackRunUnblock.png` & `readfish-2024.2.0/docs/images/PlaybackRunUnblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/PlaybackRunUnblockCloseUp.png` & `readfish-2024.2.0/docs/images/PlaybackRunUnblockCloseUp.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/Unblock.png` & `readfish-2024.2.0/docs/images/Unblock.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/Unblock_closeup.png` & `readfish-2024.2.0/docs/images/Unblock_closeup.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/control.png` & `readfish-2024.2.0/docs/images/control.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/message.png` & `readfish-2024.2.0/docs/images/message.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/minknow_messages.png` & `readfish-2024.2.0/docs/images/minknow_messages.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/readfish.jpg` & `readfish-2024.2.0/docs/images/readfish.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/readfish.png` & `readfish-2024.2.0/docs/images/readfish.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/readfish_dark.png` & `readfish-2024.2.0/docs/images/readfish_dark.png`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/readfish_logo.jpg` & `readfish-2024.2.0/docs/images/readfish_logo.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/images/readfish_small.jpg` & `readfish-2024.2.0/docs/images/readfish_small.jpg`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/questions/batch-times.question.md` & `readfish-2024.2.0/docs/questions/batch-times.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/questions/creating_readfish-environment.question.md` & `readfish-2024.2.0/docs/questions/creating_readfish-environment.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/questions/key_error_adapter.md` & `readfish-2024.2.0/docs/questions/key_error_adapter.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/questions/py-guppy-client-error.question.md` & `readfish-2024.2.0/docs/questions/py-guppy-client-error.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/docs/questions/py-guppy-client-version.question.md` & `readfish-2024.2.0/docs/questions/py-guppy-client-version.question.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_channels.py` & `readfish-2024.2.0/src/readfish/_channels.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_cli_args.py` & `readfish-2024.2.0/src/readfish/_cli_args.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_cli_base.py` & `readfish-2024.2.0/src/readfish/_cli_base.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_config.py` & `readfish-2024.2.0/src/readfish/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         plugin modules are loaded dynamically at runtime. The builtins dictionary maps
         the names of built-in plugins to the actual module names, and is used to avoid
         having to specify the full module name when loading a built-in plugin. If
         override=True, the builtin module names are ignored.
         """
         builtins = {
             "guppy": "guppy",
+            "dorado": "dorado",
             "mappy": "mappy",
             "mappy_rs": "mappy_rs",
             "no_op": "_no_op",
         }
         if self.name in builtins and not override:
             return importlib.import_module(f"readfish.plugins.{builtins[self.name]}")
         return importlib.import_module(self.name)
```

### Comparing `readfish-2024.1.0/src/readfish/_loggers.py` & `readfish-2024.2.0/src/readfish/_loggers.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_read_until_client.py` & `readfish-2024.2.0/src/readfish/_read_until_client.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_statistics.py` & `readfish-2024.2.0/src/readfish/_statistics.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/_utils.py` & `readfish-2024.2.0/src/readfish/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import zlib
 
 import numpy as np
 import numpy.typing as npt
 from minknow_api.manager import Manager, FlowCellPosition
 from minknow_api import Connection
 
+
 if sys.version_info < (3, 11):
     from exceptiongroup import BaseExceptionGroup
 
 from readfish._channels import FLONGLE_CHANNELS, MINION_CHANNELS
 
 
 MODULE_LOGGER = logging.getLogger(__name__)
```

### Comparing `readfish-2024.1.0/src/readfish/entry_points/stats.py` & `readfish-2024.2.0/src/readfish/entry_points/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 To run and output PAF alignments and demutiplexed FASTQ, and output a HTML summary file at summary_adaptive.html
 
 .. code-block:: bash
 
     readfish stats --toml tests/static/stats_test/yeast_summary_test.toml --fastq-directory tests/static/stats_test/ --html summary_adaptive
 
 """
+
 from __future__ import annotations
 import argparse
 from pathlib import Path
 import sys
 import logging
 
 if sys.version_info < (3, 11):
```

### Comparing `readfish-2024.1.0/src/readfish/entry_points/targets.py` & `readfish-2024.2.0/src/readfish/entry_points/targets.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,21 @@
 from minknow_api import protocol_service
 
 # Library
 from readfish._cli_args import DEVICE_BASE_ARGS, Chemistry
 from readfish._read_until_client import RUClient
 from readfish._config import Action, Conf, make_decision, _Condition
 from readfish._statistics import ReadfishStatistics
+from readfish.__about__ import __version__
+from readfish._compatibility import (
+    _get_minknow_version,
+    check_compatibility,
+    MINKNOW_COMPATIBILITY_RANGE,
+    DIRECTION,
+)
 from readfish._utils import (
     get_device,
     send_message,
     ChunkTracker,
     Severity,
 )
 from readfish.plugins.abc import AlignerABC, CallerABC
@@ -193,24 +200,26 @@
             f"{self.run_information.run_id}_readfish.tsv" if debug_log else None
         )
 
         self.logger.info("Fetching Run Configuration")
         self.break_reads_after_seconds = (
             self.client.connection.analysis_configuration.get_analysis_configuration().read_detection.break_reads_after_seconds.value
         )
+        self.sample_rate = self.client.connection.device.get_sample_rate().sample_rate
         self.logger.info("Run Configuration Received")
         self.logger.info(f"run_id={self.run_information.run_id}")
         self.logger.info(f"break_reads_after_seconds={self.break_reads_after_seconds}")
+        self.logger.info(f"sample_rate={self.sample_rate}")
         # Create our statistics tracker
         self.loop_statistics = ReadfishStatistics(
             read_log_name, self.break_reads_after_seconds
         )
         logger.info("Initialising Caller")
         self.caller: CallerABC = self.conf.caller_settings.load_object(
-            "Caller", run_information=self.run_information
+            "Caller", run_information=self.run_information, sample_rate=self.sample_rate
         )
         logger.info("Caller initialised")
         caller_description = self.caller.describe()
         self.logger.info(caller_description)
         send_message(self.client.connection, caller_description, Severity.INFO)
         logger.info("Initialising Aligner")
         self.mapper: AlignerABC = self.conf.mapper_settings.load_object("Aligner")
@@ -569,14 +578,32 @@
     :param extras: Extra stuff, I guess
 
     :returns: An exit code integer, 0 for success
     """
     # Setup logger used in this entry point, this one should be passed through
     logger = logging.getLogger(f"readfish.{args.command}")
 
+    # Check MinKNOW version
+
+    minknow_version = _get_minknow_version(host=args.host, port=args.port)
+    if (
+        action := check_compatibility(minknow_version, MINKNOW_COMPATIBILITY_RANGE)
+    ) in (
+        DIRECTION.UPGRADE,
+        DIRECTION.DOWNGRADE,
+    ):
+        lower_bound, upper_bound = MINKNOW_COMPATIBILITY_RANGE
+        logger.warning(
+            f"""This readfish version ({__version__}) is tested for compatibility with MinKNOW v{lower_bound} to v{upper_bound}.
+This version of minknow is {minknow_version}.
+If readfish fails please try to {action.value} readfish.
+If there isn't a newer version of readfish and readfish is failing, please open an issue:
+    https://github.com/LooseLab/readfish/issues"""
+        )
+
     # Fetch sequencing device
     position = get_device(args.device, host=args.host, port=args.port)
 
     # Create a read until client
     read_until_client = RUClient(
         mk_host=position.host,
         mk_port=position.description.rpc_ports.secure,
@@ -600,17 +627,14 @@
         read_until_client.connection,
         f"'readfish {args.command}' connected to this device.",
         Severity.WARN,
     )
 
     # start the client running
     read_until_client.run(
-        # TODO: Set correct channel range
-        # first_channel=186,
-        # last_channel=187,
         first_channel=1,
         last_channel=read_until_client.channel_count,
         max_unblock_read_length_seconds=args.max_unblock_read_length_seconds,
     )
 
     worker = Analysis(
         read_until_client,
```

### Comparing `readfish-2024.1.0/src/readfish/entry_points/unblock_all.py` & `readfish-2024.2.0/src/readfish/entry_points/unblock_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 The unblock all command only requires the target device and a small description of the experiment, for example:
 
 .. code-block:: bash
 
    readfish unblock-all --device X3 --experiment-name "test unblock all"
 """
+
 from tempfile import NamedTemporaryFile
 
 from readfish._cli_args import DEVICE_BASE_ARGS
 from readfish.entry_points import targets
 
 _help = "Unblock all reads"
 _cli = DEVICE_BASE_ARGS + (
```

### Comparing `readfish-2024.1.0/src/readfish/entry_points/validate.py` & `readfish-2024.2.0/src/readfish/entry_points/validate.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,15 +77,22 @@
     if args.no_check_plugins:
         logger.info("Plugin initialisation and testing was skipped.")
     else:
         logger.info("Initialising Caller")
         try:
             _ = conf.caller_settings.load_object("Caller")
         except Exception as exc:
-            logger.error("Caller could not be initialised, see below for details")
+            logger.error("Caller could not be initialised.")
+            logger.error(
+                "Possible reasons for this include a mismatch between the ont basecaller client and the versions of guppy or dorado you are connecting to."
+            )
+            logger.error(
+                "Additional information is available here: https://looselab.github.io/readfish/FAQ.html#connection-error-bad-reply-could-not-interpret-message-from-server-for-request-load-config-reply-invalid-protocol"
+            )
+            logger.error("See below for further details on this specific error.")
             logger.error(str(exc))
             errors += 1
         else:
             logger.info("Caller initialised")
 
         logger.info("Initialising Aligner")
         try:
```

### Comparing `readfish-2024.1.0/src/readfish/plugins/_filter.py` & `readfish-2024.2.0/src/readfish/plugins/_filter.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/plugins/_mappy.py` & `readfish-2024.2.0/src/readfish/plugins/_mappy.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/plugins/_no_op.py` & `readfish-2024.2.0/src/readfish/plugins/_no_op.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/plugins/abc.py` & `readfish-2024.2.0/src/readfish/plugins/abc.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/plugins/guppy.py` & `readfish-2024.2.0/src/readfish/plugins/guppy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """Guppy plugin module
 
 Extension of pyguppy Caller that maintains a connection to the basecaller
 """
+
 from __future__ import annotations
 import logging
 import os
 import time
 from collections import namedtuple
 from pathlib import Path
 from typing import Iterable, TYPE_CHECKING
+from packaging.version import parse as parse_version
 
 import numpy as np
 import numpy.typing as npt
 from minknow_api.protocol_pb2 import ProtocolRunInfo
-from pyguppy_client_lib.helper_functions import package_read
-from pyguppy_client_lib.pyclient import PyGuppyClient
+
+try:
+    from pyguppy_client_lib.helper_functions import package_read
+    from pyguppy_client_lib.pyclient import PyGuppyClient
+except ImportError:
+    pass
 
 from readfish._loggers import setup_logger
 from readfish.plugins.abc import CallerABC
 from readfish.plugins.utils import Result
 from readfish._utils import nice_join
 
 
@@ -52,17 +58,34 @@
     def __init__(
         self, run_information: ProtocolRunInfo = None, debug_log=None, **kwargs
     ):
         self.logger = setup_logger("readfish_guppy_logger", log_file=debug_log)
         self.supported_barcode_kits = None
         self.supported_basecall_models = None
         self.run_information = run_information
+        logging.warn(
+            "Deprecation warning - As ONT has moved fully to dorado, this plugin is no longer maintained, and will be deprecated in a future release of readfish."
+        )
+        if self.run_information:
+            self.guppy_version = (
+                self.run_information.software_versions.guppy_connected_version
+            )
+
+            if parse_version(self.guppy_version) < parse_version("7.3.9"):
+                logging.info(f"Connected to caller version {self.guppy_version}.")
+            else:
+                logging.info(
+                    f"Trying to connect to minKNOW with caller version {self.guppy_version}. This plugin requires a version of Dorado or Guppy < 7.3.9. If this is stopping readfish from running try changing [caller_settings.guppy] to [caller_settings.dorado]. You should also check for any updates available to readfish."
+                )
 
         # Set our own priority
         self.guppy_params = kwargs
+
+        # Remove the sample rate from the guppy params as it isn't required for the PyGuppyClient
+        self.guppy_params.pop("sample_rate", None)
         self.guppy_params["priority"] = PyGuppyClient.high_priority
         # Set our own client name to appear in the guppy server logs
         self.guppy_params["client_name"] = "Readfish_connection"
         self.validate()
         self.caller = PyGuppyClient(**self.guppy_params)
         self.caller.connect()
```

### Comparing `readfish-2024.1.0/src/readfish/plugins/utils.py` & `readfish-2024.2.0/src/readfish/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/read_until/base.py` & `readfish-2024.2.0/src/readfish/read_until/base.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/src/readfish/read_until/read_cache.py` & `readfish-2024.2.0/src/readfish/read_until/read_cache.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/describe_test.py` & `readfish-2024.2.0/tests/describe_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/stats_test.py` & `readfish-2024.2.0/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/utils_test.py` & `readfish-2024.2.0/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/validation_test.py` & `readfish-2024.2.0/tests/validation_test.py`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt` & `readfish-2024.2.0/tests/static/describe_test/describe_aligner_barcoded_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt` & `readfish-2024.2.0/tests/static/describe_test/describe_aligner_barcoded_regions_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt` & `readfish-2024.2.0/tests/static/describe_test/describe_barcoded_regions_experiment_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/describe_test/describe_experiment_regions_expected.txt` & `readfish-2024.2.0/tests/static/describe_test/describe_experiment_regions_expected.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi` & `readfish-2024.2.0/tests/static/describe_test/yeast_8kb_contigs_test.mmi`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/guppy_validation_test/README.md` & `readfish-2024.2.0/tests/static/guppy_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/mappy_validation_test/README.md` & `readfish-2024.2.0/tests/static/mappy_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/stats_test/expected_summary.txt` & `readfish-2024.2.0/tests/static/stats_test/expected_summary.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/stats_test/simulated_reads.fastq` & `readfish-2024.2.0/tests/static/stats_test/simulated_reads.fastq`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/stats_test/stats.tsv` & `readfish-2024.2.0/tests/static/stats_test/stats.tsv`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi` & `readfish-2024.2.0/tests/static/stats_test/yeast_8kb_contigs_test.mmi`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/toml_validation_test/README.md` & `readfish-2024.2.0/tests/static/toml_validation_test/README.md`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt` & `readfish-2024.2.0/tests/static/toml_validation_test/fail/004_target_interval_check.txt`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/.gitignore` & `readfish-2024.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/LICENSE` & `readfish-2024.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readfish-2024.1.0/README.md` & `readfish-2024.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 MinKNOW server to obtain read data in real-time. The data can be analysed in the
 way most fit for purpose, and a return call can be made to the server to unblock
 the read in progress and so direct sequencing capacity towards reads of interest.
 
 
 **This implementation of readfish requires Guppy version >= 6.0.0 and MinKNOW version core >= 5.0.0 . It will not work on earlier versions.**
 
+**Since MinKNOW version core >=5.9.0 and Dorado server version >=7.3.9, Dorado requires an alternate library, `ont-pybasecall-client-lib`. We have introduced a new`dorado` module to handle this.**
+
 
 The code here has been tested with Guppy in GPU mode using GridION Mk1 and
 NVIDIA RTX2080 on live sequencing runs and an NVIDIA GTX1080 using playback
 on a simulated run (see below for how to test this).
 This code is run at your own risk as it DOES affect sequencing output. You
 are **strongly** advised to test your setup prior to running (see below for
 example tests).
@@ -117,17 +119,17 @@
 
 ```bash
 curl -LO https://raw.githubusercontent.com/LooseLab/readfish/e30f1fa8ac7a37bb39e9d8b49251426fe1674c98/docs/development.yml?token=GHSAT0AAAAAACBZL42IS3QVM4ZGPPW4SHB6ZE67V6Q
 conda env create -f development.yml
 conda activate readfish_dev
 ```
 
-| <h2>‼️ Important! </h2> |
-|:---------------------------|
-|  The listed `ont-pyguppy-client-lib` version will probably not match the version installed on your system. To fix this, Please see this [issue](https://github.com/LooseLab/readfish/issues/221#issuecomment-1381529409)     |
+| <h2>‼️ Important !! </h2>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| MinKNOW is transitioning from Guppy to Dorado. Until MinKNOW version 5.9 both Guppy and Dorado used ont-pyguppy-client-lib.<br/>As of MinKNOW version 5.9 and Dorado server version 7.3.9 and greater Dorado requires an alternate library, `ont-pybasecall-client-lib`.<br/>The listed `ont-pyguppy-client-lib` or `ont-pybasecaller-client-lib` version may not match the version installed on your system. To fix this, Please see this [issue](https://github.com/LooseLab/readfish/issues/221#issuecomment-1381529409), using the appropriate library. |
 
 
 [ONT's Guppy GPU](https://community.nanoporetech.com/downloads) should be installed and running as a server.
 
 <details style="margin-top: 10px">
 <summary><span id="py-ve">Alternatively, install readfish into a python virtual-environment</span></summary>
 
@@ -329,29 +331,33 @@
 
 Note: The plots here are generated from running readfish unblock-all on an Apple Silicon laptop. The unblock response may be faster on a GPU server.
 </details>
 
 <details style="margin-top: 10px">
 <summary id="testing-basecalling-and-mapping"><h3 style="display: inline;">Testing base-calling and mapping</h3></summary>
 
-To test selective sequencing you must have access to a
-[guppy basecall server](https://community.nanoporetech.com/downloads/guppy/release_notes) (>=6.0.0)
+To test selective sequencing you must have access to either a
+[guppy basecall server](https://community.nanoporetech.com/downloads/guppy/release_notes) (>=6.0.0) or a [dorado basecall server](https://community.nanoporetech.com/downloads/dorado/release_notes). 
 
 and a readfish TOML configuration file.
 
 NOTE: guppy and dorado are used here interchangeably as the basecall server. Dorado is gradually replacing guppy. All readfish code is compatible with Guppy >=6.0.0 and dorado >=0.4.0
 
 1. First make a local copy of the example TOML file:
     ```console
     curl -O https://raw.githubusercontent.com/LooseLab/readfish/master/docs/_static/example_tomls/human_chr_selection.toml
     ```
 1. If on PromethION, edit the `mapper_settings.mappy` section to read:
     ```toml
     [mapper_settings.mappy-rs]
     ```
+1. If on MinKNOW core>=5.9.0 and Dorado server version >=7.3.9, edit the `basecaller` section to read:
+    ```toml
+    [caller_settings.dorado]
+    ```
 1. Modify the `fn_idx_in` field in the file to be the full path to a [minimap2](https://github.com/lh3/minimap2) index of the human genome.
 
 1. Modify the `targets` fields for each condition to reflect the naming convention used in your index. This is the sequence name only, up to but not including any whitespace.
 e.g. `>chr1 human chromosome 1` would become `chr1`. If these names do not match, then target matching will fail.
 
 We can now validate this TOML file to see if it will be loaded correctly.
 
@@ -549,17 +555,23 @@
 And for our Awesome Logo please checkout out [@tim_bassford](https://twitter.com/tim_bassford) from [@TurbineCreative](https://twitter.com/TurbineCreative)!
 
 <!-- end-epilog -->
 [ONT]: https://nanoporetech.com
 
 <!-- start-changelog -->
 # Changelog
+## 2024.2.0
+1. Add a dorado base-caller which addressed issue [#347](https://github.com/LooseLab/readfish/issues/347) - chiefly in Dorado 7.3.9 ONT have moved to `ont-pybasecall-client-lib`, 
+  and connections from `ont_pyguppy_client_lib` raise `Connection error. ...  LOAD_CONFIG. Reply: INVALID_PROTOCOL` [(#344)](https://github.com/LooseLab/readfish/pull/344)
+1. Adds version checking for MinKNOW and Guppy/Dorado, logs if not compatibile [(#351)](https://github.com/LooseLab/readfish/pull/351)
+
 ## 2024.1.0
 1. bug fix type for `--wait-on-ready` type and actual function [(#327)](https://github.com/LooseLab/readfish/pull/327), [(#323)](https://github.com/LooseLab/readfish/pull/323)
 1. mutiple suffix `.mmi` support [(#330)](https://github.com/LooseLab/readfish/pull/330)
 1. Change the default `unblock_duration` on the `Analysis` class to use `DEFAULT_UNBLOCK` value defined in `_cli_args.py`. Change type on the Argparser for `--unblock-duration` to float. [(#313)](https://github.com/LooseLab/readfish/pull/313)
 1. Big dog Duplex feature - adds ability to select duplex reads that cover a target region. See pull request for details [(#324)](https://github.com/LooseLab/readfish/pull/324)
+
 ## 2023.1.1
 1. Fix Readme Logo link 🥳 (#296)
-1. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
-1. Correctly handle overriding a decision in internal statistics tracking. (#299)
+2. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
+3. Correctly handle overriding a decision in internal statistics tracking. (#299)
 <!-- end-changelog -->
```

### Comparing `readfish-2024.1.0/pyproject.toml` & `readfish-2024.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 tests = ["pytest", "coverage[toml]"]
 tests-mappy = ["readfish[tests,mappy,guppy]"]
 dev = ["readfish[all,docs,tests]", "pre-commit"]
 # Running dependencies, this is a little bit clunky but works for now
 mappy = ["mappy"]
 mappy-rs = ["mappy-rs >= 0.0.6"]
 guppy = ["ont_pyguppy_client_lib"]
-all = ["readfish[mappy,mappy-rs,guppy]"]
+dorado = ["ont-pybasecall-client-lib"]
+all = ["readfish[mappy,mappy-rs,guppy,dorado]"]
 
 [project.urls]
 Documentation = "https://looselab.github.io/readfish"
 "Bug Tracker" = "https://github.com/LooseLab/readfish/issues"
 "Source Code" = "https://github.com/LooseLab/readfish"
 
 [tool.hatch.metadata]
@@ -79,7 +80,14 @@
     "tests/*test.py",
     "src/readfish",
 ]
 markers = [
     "alignment: marks tests which rely on loading or using Mappy or Mappy-rs aligners, used to test with both. (deselect with '-m \"not slow\", select with '-k alignment')",
 ]
 addopts = ["-ra", "--doctest-modules", "--ignore=src/readfish/read_until/base.py"]
+
+[tool.coverage.report]
+omit = [
+    "src/readfish/plugins/dorado.py",
+    "src/readfish/_read_until_client.py",
+    "src/readfish/plugins/guppy.py",
+]
```

### Comparing `readfish-2024.1.0/PKG-INFO` & `readfish-2024.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: readfish
-Version: 2024.1.0
+Version: 2024.2.0
 Summary: ONT adaptive sampling
 Project-URL: Documentation, https://looselab.github.io/readfish
 Project-URL: Bug Tracker, https://github.com/LooseLab/readfish/issues
 Project-URL: Source Code, https://github.com/LooseLab/readfish
 Author: Alexander Payne
 Author-email: Rory Munro <rory.munro@nottingham.ac.uk>, Matt Loose <matt.loose@nottingham.ac.uk>
 License-Expression: MIT
@@ -30,31 +30,35 @@
 Requires-Dist: numpy
 Requires-Dist: readfish-summarise>=0.2.5
 Requires-Dist: readfish[all]
 Requires-Dist: rtoml
 Provides-Extra: all
 Requires-Dist: mappy; extra == 'all'
 Requires-Dist: mappy-rs>=0.0.6; extra == 'all'
+Requires-Dist: ont-pybasecall-client-lib; extra == 'all'
 Requires-Dist: ont-pyguppy-client-lib; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == 'dev'
 Requires-Dist: faqtory; extra == 'dev'
 Requires-Dist: furo; extra == 'dev'
 Requires-Dist: mappy; extra == 'dev'
 Requires-Dist: mappy-rs>=0.0.6; extra == 'dev'
 Requires-Dist: myst-parser; extra == 'dev'
+Requires-Dist: ont-pybasecall-client-lib; extra == 'dev'
 Requires-Dist: ont-pyguppy-client-lib; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: sphinx-copybutton; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: faqtory; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
+Provides-Extra: dorado
+Requires-Dist: ont-pybasecall-client-lib; extra == 'dorado'
 Provides-Extra: guppy
 Requires-Dist: ont-pyguppy-client-lib; extra == 'guppy'
 Provides-Extra: mappy
 Requires-Dist: mappy; extra == 'mappy'
 Provides-Extra: mappy-rs
 Requires-Dist: mappy-rs>=0.0.6; extra == 'mappy-rs'
 Provides-Extra: tests
@@ -90,14 +94,16 @@
 MinKNOW server to obtain read data in real-time. The data can be analysed in the
 way most fit for purpose, and a return call can be made to the server to unblock
 the read in progress and so direct sequencing capacity towards reads of interest.
 
 
 **This implementation of readfish requires Guppy version >= 6.0.0 and MinKNOW version core >= 5.0.0 . It will not work on earlier versions.**
 
+**Since MinKNOW version core >=5.9.0 and Dorado server version >=7.3.9, Dorado requires an alternate library, `ont-pybasecall-client-lib`. We have introduced a new`dorado` module to handle this.**
+
 
 The code here has been tested with Guppy in GPU mode using GridION Mk1 and
 NVIDIA RTX2080 on live sequencing runs and an NVIDIA GTX1080 using playback
 on a simulated run (see below for how to test this).
 This code is run at your own risk as it DOES affect sequencing output. You
 are **strongly** advised to test your setup prior to running (see below for
 example tests).
@@ -186,17 +192,17 @@
 
 ```bash
 curl -LO https://raw.githubusercontent.com/LooseLab/readfish/e30f1fa8ac7a37bb39e9d8b49251426fe1674c98/docs/development.yml?token=GHSAT0AAAAAACBZL42IS3QVM4ZGPPW4SHB6ZE67V6Q
 conda env create -f development.yml
 conda activate readfish_dev
 ```
 
-| <h2>‼️ Important! </h2> |
-|:---------------------------|
-|  The listed `ont-pyguppy-client-lib` version will probably not match the version installed on your system. To fix this, Please see this [issue](https://github.com/LooseLab/readfish/issues/221#issuecomment-1381529409)     |
+| <h2>‼️ Important !! </h2>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| MinKNOW is transitioning from Guppy to Dorado. Until MinKNOW version 5.9 both Guppy and Dorado used ont-pyguppy-client-lib.<br/>As of MinKNOW version 5.9 and Dorado server version 7.3.9 and greater Dorado requires an alternate library, `ont-pybasecall-client-lib`.<br/>The listed `ont-pyguppy-client-lib` or `ont-pybasecaller-client-lib` version may not match the version installed on your system. To fix this, Please see this [issue](https://github.com/LooseLab/readfish/issues/221#issuecomment-1381529409), using the appropriate library. |
 
 
 [ONT's Guppy GPU](https://community.nanoporetech.com/downloads) should be installed and running as a server.
 
 <details style="margin-top: 10px">
 <summary><span id="py-ve">Alternatively, install readfish into a python virtual-environment</span></summary>
 
@@ -398,29 +404,33 @@
 
 Note: The plots here are generated from running readfish unblock-all on an Apple Silicon laptop. The unblock response may be faster on a GPU server.
 </details>
 
 <details style="margin-top: 10px">
 <summary id="testing-basecalling-and-mapping"><h3 style="display: inline;">Testing base-calling and mapping</h3></summary>
 
-To test selective sequencing you must have access to a
-[guppy basecall server](https://community.nanoporetech.com/downloads/guppy/release_notes) (>=6.0.0)
+To test selective sequencing you must have access to either a
+[guppy basecall server](https://community.nanoporetech.com/downloads/guppy/release_notes) (>=6.0.0) or a [dorado basecall server](https://community.nanoporetech.com/downloads/dorado/release_notes). 
 
 and a readfish TOML configuration file.
 
 NOTE: guppy and dorado are used here interchangeably as the basecall server. Dorado is gradually replacing guppy. All readfish code is compatible with Guppy >=6.0.0 and dorado >=0.4.0
 
 1. First make a local copy of the example TOML file:
     ```console
     curl -O https://raw.githubusercontent.com/LooseLab/readfish/master/docs/_static/example_tomls/human_chr_selection.toml
     ```
 1. If on PromethION, edit the `mapper_settings.mappy` section to read:
     ```toml
     [mapper_settings.mappy-rs]
     ```
+1. If on MinKNOW core>=5.9.0 and Dorado server version >=7.3.9, edit the `basecaller` section to read:
+    ```toml
+    [caller_settings.dorado]
+    ```
 1. Modify the `fn_idx_in` field in the file to be the full path to a [minimap2](https://github.com/lh3/minimap2) index of the human genome.
 
 1. Modify the `targets` fields for each condition to reflect the naming convention used in your index. This is the sequence name only, up to but not including any whitespace.
 e.g. `>chr1 human chromosome 1` would become `chr1`. If these names do not match, then target matching will fail.
 
 We can now validate this TOML file to see if it will be loaded correctly.
 
@@ -618,17 +628,23 @@
 And for our Awesome Logo please checkout out [@tim_bassford](https://twitter.com/tim_bassford) from [@TurbineCreative](https://twitter.com/TurbineCreative)!
 
 <!-- end-epilog -->
 [ONT]: https://nanoporetech.com
 
 <!-- start-changelog -->
 # Changelog
+## 2024.2.0
+1. Add a dorado base-caller which addressed issue [#347](https://github.com/LooseLab/readfish/issues/347) - chiefly in Dorado 7.3.9 ONT have moved to `ont-pybasecall-client-lib`, 
+  and connections from `ont_pyguppy_client_lib` raise `Connection error. ...  LOAD_CONFIG. Reply: INVALID_PROTOCOL` [(#344)](https://github.com/LooseLab/readfish/pull/344)
+1. Adds version checking for MinKNOW and Guppy/Dorado, logs if not compatibile [(#351)](https://github.com/LooseLab/readfish/pull/351)
+
 ## 2024.1.0
 1. bug fix type for `--wait-on-ready` type and actual function [(#327)](https://github.com/LooseLab/readfish/pull/327), [(#323)](https://github.com/LooseLab/readfish/pull/323)
 1. mutiple suffix `.mmi` support [(#330)](https://github.com/LooseLab/readfish/pull/330)
 1. Change the default `unblock_duration` on the `Analysis` class to use `DEFAULT_UNBLOCK` value defined in `_cli_args.py`. Change type on the Argparser for `--unblock-duration` to float. [(#313)](https://github.com/LooseLab/readfish/pull/313)
 1. Big dog Duplex feature - adds ability to select duplex reads that cover a target region. See pull request for details [(#324)](https://github.com/LooseLab/readfish/pull/324)
+
 ## 2023.1.1
 1. Fix Readme Logo link 🥳 (#296)
-1. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
-1. Correctly handle overriding a decision in internal statistics tracking. (#299)
+2. Fix bug where we had accidentally started requiring barcoded TOMLs to specify a region. Thanks to @jamesemery for catching this. (#299)
+3. Correctly handle overriding a decision in internal statistics tracking. (#299)
 <!-- end-changelog -->
```

