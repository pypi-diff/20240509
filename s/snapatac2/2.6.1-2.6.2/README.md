# Comparing `tmp/snapatac2-2.6.1.tar.gz` & `tmp/snapatac2-2.6.2.tar.gz`

## Comparing `snapatac2-2.6.1.tar` & `snapatac2-2.6.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0     1001      127      994 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/LICENSE
--rw-r--r--   0     1001      127      724 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/embedding.rs
--rw-r--r--   0     1001      127    12674 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/export.rs
--rw-r--r--   0     1001      127     2687 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/knn.rs
--rw-r--r--   0     1001      127      117 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/lib.rs
--rw-r--r--   0     1001      127    10767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/motif.rs
--rw-r--r--   0     1001      127     2765 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/network.rs
--rw-r--r--   0     1001      127    19661 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
--rw-r--r--   0     1001      127     5504 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam.rs
--rw-r--r--   0     1001      127    18667 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/coverage.rs
--rw-r--r--   0     1001      127    31384 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/genome.rs
--rw-r--r--   0     1001      127     9610 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/import.rs
--rw-r--r--   0     1001      127     7967 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/matrix.rs
--rw-r--r--   0     1001      127     6990 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data.rs
--rw-r--r--   0     1001      127      427 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/mod.rs
--rw-r--r--   0     1001      127    12773 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/qc.rs
--rw-r--r--   0     1001      127    13427 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/utils/similarity.rs
--rw-r--r--   0     1001      127     5168 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/utils.rs
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 snapatac2-2.6.1/snapatac2-python/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/LICENSE
--rw-r--r--   0     1001      127       85 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/README.md
--rw-r--r--   0     1001      127      655 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127     2616 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/_io.py
--rw-r--r--   0     1001      127     3767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127    11895 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     7376 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127     6145 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     7190 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127    11034 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127    16396 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127     2911 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127      204 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127    37676 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127     3509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127     3031 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127     6030 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127     5005 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127    14260 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127      324 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127     8737 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127    11325 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127     9283 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127    19537 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127     1251 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127    11022 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127     4509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127    19618 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127     2078 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127    13935 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/call_peaks.rs
--rw-r--r--   0     1001      127    15184 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/embedding.rs
--rw-r--r--   0     1001      127     3156 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/export.rs
--rw-r--r--   0     1001      127      748 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/knn.rs
--rw-r--r--   0     1001      127     3451 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/lib.rs
--rw-r--r--   0     1001      127     4759 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/motif.rs
--rw-r--r--   0     1001      127     1195 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/network.rs
--rw-r--r--   0     1001      127    11649 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/preprocessing.rs
--rw-r--r--   0     1001      127     8499 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/utils/anndata.rs
--rw-r--r--   0     1001      127    10859 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/utils.rs
--rw-r--r--   0     1001      127     2015 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_func.py
--rw-r--r--   0     1001      127     2195 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_pipeline.py
--rw-r--r--   0     1001      127     4262 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_similarity.py
--rw-r--r--   0     1001      127      132 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test.bam
--rw-r--r--   0     1001      127      130 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test.bed.gz
--rw-r--r--   0     1001      127      131 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test_clean.tsv.gz
--rw-r--r--   0     1001      127     4668 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools.py
--rw-r--r--   0     1001      127    99127 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/Cargo.lock
--rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 snapatac2-2.6.1/pyproject.toml
--rw-r--r--   0     1001      127    11325 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127     1251 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127     8737 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127     4509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127     9283 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127     2078 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127    19537 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127      324 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127    19618 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127    11022 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127    16396 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127    11034 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127     2911 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127    11895 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     7190 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127     2616 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/_io.py
--rw-r--r--   0     1001      127      655 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127    14260 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127     6030 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127      204 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127     5005 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127     3509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127     3031 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127    37676 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127     3767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127     6145 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     7376 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127       85 2024-05-03 00:36:51.000000 snapatac2-2.6.1/README.md
--rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/LICENSE
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 snapatac2-2.6.1/PKG-INFO
+-rw-r--r--   0     1001      127      995 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/LICENSE
+-rw-r--r--   0     1001      127      724 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/embedding.rs
+-rw-r--r--   0     1001      127    12674 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/export.rs
+-rw-r--r--   0     1001      127     2687 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/knn.rs
+-rw-r--r--   0     1001      127      117 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/lib.rs
+-rw-r--r--   0     1001      127    10767 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/motif.rs
+-rw-r--r--   0     1001      127     2765 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/network.rs
+-rw-r--r--   0     1001      127    19895 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
+-rw-r--r--   0     1001      127     5504 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/bam.rs
+-rw-r--r--   0     1001      127    18667 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/coverage.rs
+-rw-r--r--   0     1001      127    31384 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/genome.rs
+-rw-r--r--   0     1001      127     9610 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/import.rs
+-rw-r--r--   0     1001      127     7967 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/matrix.rs
+-rw-r--r--   0     1001      127     6990 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data.rs
+-rw-r--r--   0     1001      127      427 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/mod.rs
+-rw-r--r--   0     1001      127    13044 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/preprocessing/qc.rs
+-rw-r--r--   0     1001      127    13427 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/utils/similarity.rs
+-rw-r--r--   0     1001      127     5168 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-core/src/utils.rs
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 snapatac2-2.6.2/snapatac2-python/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/LICENSE
+-rw-r--r--   0     1001      127       85 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/README.md
+-rw-r--r--   0     1001      127      655 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127     2616 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127     3767 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127    11895 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127     7376 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127     6145 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7358 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127    11034 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127    16396 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127     2911 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127      204 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127    37676 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3509 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     3031 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127     6030 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127     5005 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127    14260 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127      324 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127     8737 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127    11325 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127     9283 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127    19537 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127     1251 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127    11022 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127     4509 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127    19618 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127     2078 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127    13935 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/call_peaks.rs
+-rw-r--r--   0     1001      127    15184 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/embedding.rs
+-rw-r--r--   0     1001      127     3156 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/export.rs
+-rw-r--r--   0     1001      127      748 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/knn.rs
+-rw-r--r--   0     1001      127     3451 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/lib.rs
+-rw-r--r--   0     1001      127     4759 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/motif.rs
+-rw-r--r--   0     1001      127     1195 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/network.rs
+-rw-r--r--   0     1001      127    11952 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/preprocessing.rs
+-rw-r--r--   0     1001      127     8499 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/utils/anndata.rs
+-rw-r--r--   0     1001      127    10859 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/src/utils.rs
+-rw-r--r--   0     1001      127     2015 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_func.py
+-rw-r--r--   0     1001      127     2195 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_pipeline.py
+-rw-r--r--   0     1001      127     4262 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_similarity.py
+-rw-r--r--   0     1001      127      132 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_tools/test.bam
+-rw-r--r--   0     1001      127      130 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_tools/test.bed.gz
+-rw-r--r--   0     1001      127      131 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_tools/test_clean.tsv.gz
+-rw-r--r--   0     1001      127     4668 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/tests/test_tools.py
+-rw-r--r--   0     1001      127    98049 2024-05-09 10:34:36.000000 snapatac2-2.6.2/snapatac2-python/Cargo.lock
+-rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 snapatac2-2.6.2/pyproject.toml
+-rw-r--r--   0     1001      127    11325 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127     1251 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127     8737 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127     4509 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127     9283 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127     2078 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127    19537 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127      324 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127    19618 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127    11022 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127    16396 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127    11034 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127     2911 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127    11895 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127     7358 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127     2616 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127      655 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127    14260 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127     6030 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127      204 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127     5005 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127     3509 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     3031 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127    37676 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3767 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127     6145 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7376 2024-05-09 10:34:36.000000 snapatac2-2.6.2/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127       85 2024-05-09 10:34:36.000000 snapatac2-2.6.2/README.md
+-rw-r--r--   0     1001      127     1080 2024-05-09 10:34:36.000000 snapatac2-2.6.2/LICENSE
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 snapatac2-2.6.2/PKG-INFO
```

### Comparing `snapatac2-2.6.1/snapatac2-core/Cargo.toml` & `snapatac2-2.6.2/snapatac2-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 keywords = ["single-cell", "biology"]
 
 [dependencies]
 anndata = "0.3.3"
 anyhow = "1.0"
 bigtools = { version = "0.4", features = ["read", "write"] }
 bincode = "1.3"
-bed-utils = "0.2"
-extsort = "0.4"
+bed-utils = "0.3"
+extsort = "0.5"
 flate2 = "1.0"
 tokio = "1.34"
 hora = "0.1"
 kdtree = "0.7"
 itertools = "0.12"
 indexmap = "2.2"
 indicatif = {version = "0.17", features = ["rayon"] }
@@ -32,8 +32,8 @@
 polars = { version = "0.39", features = ["ndarray", "dtype-categorical"] }
 rayon = "1.10"
 regex = "1.6"
 serde = "1.0"
 statrs = "0.16"
 smallvec = "1.13"
 tempfile = "3.3"
-zstd = { version = "0.13", features = ["zstdmt"] }
+zstd = { version = "0.13", features = ["zstdmt"] }
```

### Comparing `snapatac2-2.6.1/snapatac2-core/LICENSE` & `snapatac2-2.6.2/snapatac2-core/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/embedding.rs` & `snapatac2-2.6.2/snapatac2-core/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/export.rs` & `snapatac2-2.6.2/snapatac2-core/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/knn.rs` & `snapatac2-2.6.2/snapatac2-core/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/motif.rs` & `snapatac2-2.6.2/snapatac2-core/src/motif.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/network.rs` & `snapatac2-2.6.2/snapatac2-core/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         alignment::record::{Cigar, Flags, data::field::{Tag, Value}, cigar::op::Kind},
         Header,
     },
 };
 use bed_utils::bed::{BEDLike, Strand};
 use std::collections::HashMap;
 use itertools::Itertools;
-use extsort::{sorter::Sortable, ExternalSorter};
+use extsort::{Sortable, ExternalSorter};
 use bincode;
 use log::warn;
 use rayon::prelude::ParallelSliceMut;
 use serde::{Serialize, Deserialize};
 use anyhow::{Result, bail, anyhow, Context};
 use regex::Regex;
 
@@ -161,20 +161,24 @@
         } else {
             self.alignment_start
         }
     }
 }
 
 impl Sortable for AlignmentInfo {
-    fn encode<W: std::io::Write>(&self, writer: &mut W) {
-        bincode::serialize_into(writer, self).unwrap();
+    fn encode<W: std::io::Write>(&self, writer: &mut W) -> std::io::Result<()> {
+        bincode::serialize_into(writer, self).map_err(|e|
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 
-    fn decode<R: std::io::Read>(reader: &mut R) -> Option<Self> {
-        bincode::deserialize_from(reader).ok()
+    fn decode<R: std::io::Read>(reader: &mut R) -> std::io::Result<Self> {
+        bincode::deserialize_from(reader).map_err(|e|
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 }
 
 
 /// Reads are considered duplicates if and only if they have the same fingerprint.
 #[derive(Eq, PartialEq, Debug, Hash)]
 pub enum FingerPrint {
@@ -416,14 +420,15 @@
             .with_segment_size(chunk)
             .with_sort_dir(tmp_dir)
             .with_parallel_sort()
             .sort_by(reads, |a, b| a.barcode.cmp(&b.barcode)
                 .then_with(|| a.unclipped_start.cmp(&b.unclipped_start))
                 .then_with(|| a.unclipped_end.cmp(&b.unclipped_end))
             ).unwrap()
+            .map(|x| x.unwrap())
     }
 
     RecordGroups {
         is_paired,
         groups: sort_rec(
             reads.map(move |x| AlignmentInfo::new(&x, barcode_loc, umi_loc).unwrap())
                 .filter(|x| x.barcode.is_some()),
```

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/bam.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/coverage.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/coverage.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/genome.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/genome.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/import.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/import.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/matrix.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data/matrix.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/count_data.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/preprocessing/qc.rs` & `snapatac2-2.6.2/snapatac2-core/src/preprocessing/qc.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::{io::{Read, BufRead, BufReader}, ops::Div, collections::{HashMap, HashSet}};
 use anndata::data::CsrNonCanonical;
 use bed_utils::bed::{GenomicRange, BEDLike, tree::BedTree, ParseError, Strand};
 use anyhow::Result;
 use serde::{Serialize, Deserialize};
-use extsort::sorter::Sortable;
+use extsort::Sortable;
 use bincode;
 use smallvec::{SmallVec, smallvec};
 
 pub type CellBarcode = String;
 
 /// Fragments from single-cell ATAC-seq experiment. Each fragment is represented
 /// by a genomic coordinate, cell barcode and a integer value.
@@ -18,21 +18,24 @@
     pub end: u64,
     pub barcode: Option<CellBarcode>,
     pub count: u32,
     pub strand: Option<Strand>,
 }
 
 impl Sortable for Fragment {
-    fn encode<W: std::io::Write>(&self, writer: &mut W) {
-        bincode::serialize_into(writer, self)
-            .unwrap_or_else(|e| panic!("Failed to serialize fragment: {}", e));
+    fn encode<W: std::io::Write>(&self, writer: &mut W) -> std::io::Result<()> {
+        bincode::serialize_into(writer, self).map_err(|e| 
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 
-    fn decode<R: std::io::Read>(reader: &mut R) -> Option<Self> {
-        bincode::deserialize_from(reader).ok()
+    fn decode<R: std::io::Read>(reader: &mut R) -> std::io::Result<Self> {
+        bincode::deserialize_from(reader).map_err(|e|
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 }
 
 impl Fragment {
     pub fn to_insertions(&self) -> SmallVec<[GenomicRange; 2]> {
         match self.strand {
             None => smallvec![
@@ -137,21 +140,24 @@
     pub chrom2: String,
     pub start2: u64,
     pub barcode: CellBarcode,
     pub count: u32,
 }
 
 impl Sortable for Contact {
-    fn encode<W: std::io::Write>(&self, writer: &mut W) {
-        bincode::serialize_into(writer, self)
-            .unwrap_or_else(|e| panic!("Failed to serialize fragment: {}", e));
+    fn encode<W: std::io::Write>(&self, writer: &mut W) -> std::io::Result<()> {
+        bincode::serialize_into(writer, self).map_err(|e|
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 
-    fn decode<R: std::io::Read>(reader: &mut R) -> Option<Self> {
-        bincode::deserialize_from(reader).ok()
+    fn decode<R: std::io::Read>(reader: &mut R) -> std::io::Result<Self> {
+        bincode::deserialize_from(reader).map_err(|e|
+            std::io::Error::new(std::io::ErrorKind::Other, e.to_string())
+        )
     }
 }
 
 impl std::str::FromStr for Contact {
     type Err = ParseError;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
```

### Comparing `snapatac2-2.6.1/snapatac2-core/src/utils/similarity.rs` & `snapatac2-2.6.2/snapatac2-core/src/utils/similarity.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-core/src/utils.rs` & `snapatac2-2.6.2/snapatac2-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/Cargo.toml` & `snapatac2-2.6.2/snapatac2-python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [package]
 name = "snapatac2"
-version = "2.6.1"
+version = "2.6.2"
 edition = "2021"
 authors = ["Kai Zhang <kai@kzhang.org>"]
 description = "Rust APIs"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
 snapatac2-core = { path = "../snapatac2-core" }
 anndata = "0.3.3"
 anndata-hdf5 = "0.2"
 pyanndata = "0.3.3"
-extsort = "0.4"
+extsort = "0.5"
 anyhow = "1.0"
-bed-utils = "0.2"
+bed-utils = "0.3"
 flate2 = "1.0"
 itertools = "0.12"
 indicatif = "0.17"
 linreg = "0.2"
 log = "0.4"
 linfa = "0.6"
 linfa-clustering = "0.6"
```

### Comparing `snapatac2-2.6.1/snapatac2-python/LICENSE` & `snapatac2-2.6.2/snapatac2-python/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/__init__.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/_io.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/_utils.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/datasets.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/export/__init__.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/genome.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/genome.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/metrics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import snapatac2._snapatac2 as internal
 from snapatac2.genome import Genome
 
 def tsse(
     adata: internal.AnnData | list[internal.AnnData],
     gene_anno: Genome | Path,
     *,
+    exclude_chroms: list[str] | str | None = ["chrM", "M"],
     inplace: bool = True,
     n_jobs: int = 8,
 ) -> np.ndarray | list[np.ndarray] | None:
     """ Compute the TSS enrichment score (TSSe) for each cell.
 
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
@@ -23,14 +24,16 @@
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
         `adata` could also be a list of AnnData objects.
         In this case, the function will be applied to each AnnData object in parallel.
     gene_anno
         A :class:`~snapatac2.Genome` object or a GTF/GFF file containing the gene annotation.
+    exclude_chroms
+        A list of chromosomes to exclude.
     inplace
         Whether to add the results to `adata.obs` or return it as a dictionary.
     n_jobs
         Number of jobs to run in parallel when `adata` is a list.
         If `n_jobs=-1`, all CPUs will be used.
 
     Returns
@@ -53,19 +56,19 @@
     Name: tsse, dtype: float64
     """
     gene_anno = gene_anno.annotation if isinstance(gene_anno, Genome) else gene_anno
  
     if isinstance(adata, list):
         result = snapatac2._utils.anndata_par(
             adata,
-            lambda x: tsse(x, gene_anno, inplace=inplace),
+            lambda x: tsse(x, gene_anno, exclude_chroms=exclude_chroms, inplace=inplace),
             n_jobs=n_jobs,
         )
     else:
-        result = np.array(internal.tss_enrichment(adata, gene_anno))
+        result = np.array(internal.tss_enrichment(adata, gene_anno, exclude_chroms))
         if inplace:
             adata.obs["tsse"] = result
     if inplace:
         return None
     else:
         return result
```

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_basic.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_embedding.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_network.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.2/snapatac2-python/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/call_peaks.rs` & `snapatac2-2.6.2/snapatac2-python/src/call_peaks.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/embedding.rs` & `snapatac2-2.6.2/snapatac2-python/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/export.rs` & `snapatac2-2.6.2/snapatac2-python/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/knn.rs` & `snapatac2-2.6.2/snapatac2-python/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/lib.rs` & `snapatac2-2.6.2/snapatac2-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/motif.rs` & `snapatac2-2.6.2/snapatac2-python/src/motif.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/network.rs` & `snapatac2-2.6.2/snapatac2-python/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/preprocessing.rs` & `snapatac2-2.6.2/snapatac2-python/src/preprocessing.rs`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     let fragments = bed::io::Reader::new(utils::open_file_for_read(&fragment_file), Some("#".to_string()))
         .into_records::<Fragment>().map(|x| {
             let mut f = x.unwrap();
             shift_fragment(&mut f, shift_left, shift_right);
             f
     });
     let sorted_fragments: Box<dyn Iterator<Item = Fragment>> = if !fragment_is_sorted_by_name {
-        Box::new(bed::sort_bed_by_key(fragments, |x| x.barcode.clone(), tempdir))
+        Box::new(bed::sort_bed_by_key(fragments, |x| x.barcode.clone(), tempdir).map(|x| x.unwrap()))
     } else {
         Box::new(fragments)
     };
 
     macro_rules! run {
         ($data:expr) => {
             preprocessing::import_fragments(
@@ -160,14 +160,15 @@
             tempfile::tempdir()
         }.expect("failed to create tmperorary directory");
         Box::new(extsort::ExternalSorter::new()
             .with_segment_size(50000000)
             .with_sort_dir(tmp.path().to_path_buf())
             .with_parallel_sort()
             .sort_by_key(contacts, |x| x.barcode.clone()).unwrap()
+            .map(|x| x.unwrap())
         )
     } else {
         Box::new(contacts)
     };
 
     macro_rules! run {
         ($data:expr) => {
@@ -323,17 +324,24 @@
 
 /// QC metrics
 
 #[pyfunction]
 pub(crate) fn tss_enrichment(
     anndata: AnnDataLike,
     gtf_file: PathBuf,
+    exclude_chroms: Option<Vec<String>>,
 ) -> Result<Vec<f64>>
 {
-    let tss = preprocessing::read_tss(utils::open_file_for_read(gtf_file)).unique();
+    let exclude_chroms = match exclude_chroms {
+        Some(chrs) => chrs.into_iter().collect(),
+        None => HashSet::new(), 
+    };
+    let tss = preprocessing::read_tss(utils::open_file_for_read(gtf_file))
+        .unique()
+        .filter(|(chr, _, _)| !exclude_chroms.contains(chr));
     let promoters = preprocessing::make_promoter_map(tss);
 
     macro_rules! run {
         ($data:expr) => {
             $data.tss_enrichment(&promoters)
         }
     }
@@ -373,8 +381,8 @@
     macro_rules! run {
         ($data:expr) => {
             $data.fragment_size_distribution(max_recorded_size)
         }
     }
 
     crate::with_anndata!(&anndata, run)
-}
+}
```

### Comparing `snapatac2-2.6.1/snapatac2-python/src/utils/anndata.rs` & `snapatac2-2.6.2/snapatac2-python/src/utils/anndata.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/src/utils.rs` & `snapatac2-2.6.2/snapatac2-python/src/utils.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/tests/test_func.py` & `snapatac2-2.6.2/snapatac2-python/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/tests/test_pipeline.py` & `snapatac2-2.6.2/snapatac2-python/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/tests/test_similarity.py` & `snapatac2-2.6.2/snapatac2-python/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/tests/test_tools.py` & `snapatac2-2.6.2/snapatac2-python/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/snapatac2-python/Cargo.lock` & `snapatac2-2.6.2/snapatac2-python/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -249,23 +249,23 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bed-utils"
-version = "0.2.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c43420179bf4e3f57335f50092361dcc4229b8ccb79cb7c7bfe71aa1f5b8c105"
+checksum = "f55747ca3b14034422f4a0fb4741ebb21d94c8a383f95fa44d138c1c1b05ae76"
 dependencies = [
  "bincode",
  "bio",
  "extsort",
  "indexmap 2.2.3",
- "itertools 0.8.2",
+ "itertools 0.12.1",
  "lexical",
  "num",
  "num-traits",
  "serde",
  "tempfile",
 ]
 
@@ -302,30 +302,29 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bio"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25dccfc5babf5a4f505ab5bdda0e18d4b5fc1600c222677c54992203632cbdf5"
+checksum = "7a72cb93babf08c85b375c2938ac678cc637936b3ebb72266d433cec2577f6c2"
 dependencies = [
  "anyhow",
  "approx 0.5.1",
  "bio-types",
  "bit-set",
  "bv",
  "bytecount",
  "csv",
  "custom_derive",
  "editdistancek",
  "enum-map",
  "fxhash",
- "getset",
  "itertools 0.11.0",
  "itertools-num",
  "lazy_static",
  "multimap",
  "ndarray",
  "newtype_derive",
  "num-integer",
@@ -853,17 +852,17 @@
 name = "ethnum"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
 
 [[package]]
 name = "extsort"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffc5bb6fbca3c5ce6a51f6857eab8c35c898b2fbcb62ff1b728243dd19ec0c9f"
+checksum = "b55aeea941ed0cc991b26e54270a58fa2611708804d4b4f8a3f4c974ad161b2a"
 dependencies = [
  "rayon",
  "skeptic",
  "tempfile",
 ]
 
 [[package]]
@@ -1037,26 +1036,14 @@
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "getset"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e45727250e75cc04ff2846a66397da8ef2b3db8e40e0cef4df67950a07621eb9"
-dependencies = [
- "proc-macro-error",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "glob"
@@ -1289,23 +1276,14 @@
 name = "inventory"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "itertools"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f56a2d0bc861f9165be4eb3442afd3c236d8a98afd426f65d92324ae1091a484"
-dependencies = [
- "either",
-]
-
-[[package]]
-name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
@@ -2617,38 +2595,14 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "proc-macro-error"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
-dependencies = [
- "proc-macro-error-attr",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
- "version_check",
-]
-
-[[package]]
-name = "proc-macro-error-attr"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
-dependencies = [
- "proc-macro2",
- "quote",
- "version_check",
-]
-
-[[package]]
 name = "proc-macro2"
 version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
@@ -3262,15 +3216,15 @@
  "autocfg",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "snapatac2"
-version = "2.6.1"
+version = "2.6.2"
 dependencies = [
  "anndata",
  "anndata-hdf5",
  "anyhow",
  "bed-utils",
  "extsort",
  "flate2",
```

### Comparing `snapatac2-2.6.1/pyproject.toml` & `snapatac2-2.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.2/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.2/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.2/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.2/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.2/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.2/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.2/python/snapatac2/tools/_embedding.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_network.py` & `snapatac2-2.6.2/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.2/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.2/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.2/python/snapatac2/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.2/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/datasets.py` & `snapatac2-2.6.2/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.2/python/snapatac2/metrics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import snapatac2._snapatac2 as internal
 from snapatac2.genome import Genome
 
 def tsse(
     adata: internal.AnnData | list[internal.AnnData],
     gene_anno: Genome | Path,
     *,
+    exclude_chroms: list[str] | str | None = ["chrM", "M"],
     inplace: bool = True,
     n_jobs: int = 8,
 ) -> np.ndarray | list[np.ndarray] | None:
     """ Compute the TSS enrichment score (TSSe) for each cell.
 
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
@@ -23,14 +24,16 @@
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
         `adata` could also be a list of AnnData objects.
         In this case, the function will be applied to each AnnData object in parallel.
     gene_anno
         A :class:`~snapatac2.Genome` object or a GTF/GFF file containing the gene annotation.
+    exclude_chroms
+        A list of chromosomes to exclude.
     inplace
         Whether to add the results to `adata.obs` or return it as a dictionary.
     n_jobs
         Number of jobs to run in parallel when `adata` is a list.
         If `n_jobs=-1`, all CPUs will be used.
 
     Returns
@@ -53,19 +56,19 @@
     Name: tsse, dtype: float64
     """
     gene_anno = gene_anno.annotation if isinstance(gene_anno, Genome) else gene_anno
  
     if isinstance(adata, list):
         result = snapatac2._utils.anndata_par(
             adata,
-            lambda x: tsse(x, gene_anno, inplace=inplace),
+            lambda x: tsse(x, gene_anno, exclude_chroms=exclude_chroms, inplace=inplace),
             n_jobs=n_jobs,
         )
     else:
-        result = np.array(internal.tss_enrichment(adata, gene_anno))
+        result = np.array(internal.tss_enrichment(adata, gene_anno, exclude_chroms))
         if inplace:
             adata.obs["tsse"] = result
     if inplace:
         return None
     else:
         return result
```

### Comparing `snapatac2-2.6.1/python/snapatac2/_io.py` & `snapatac2-2.6.2/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/__init__.py` & `snapatac2-2.6.2/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_scrublet.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.2/python/snapatac2/preprocessing/_basic.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/_utils.py` & `snapatac2-2.6.2/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/genome.py` & `snapatac2-2.6.2/python/snapatac2/genome.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/python/snapatac2/export/__init__.py` & `snapatac2-2.6.2/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/LICENSE` & `snapatac2-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.1/PKG-INFO` & `snapatac2-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapatac2
-Version: 2.6.1
+Version: 2.6.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: anndata >=0.8.0, <0.11.0
 Requires-Dist: kaleido
 Requires-Dist: multiprocess
```

