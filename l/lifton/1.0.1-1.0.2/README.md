# Comparing `tmp/lifton-1.0.1.tar.gz` & `tmp/lifton-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifton-1.0.1.tar", last modified: Mon May  6 01:24:29 2024, max compression
+gzip compressed data, was "lifton-1.0.2.tar", last modified: Wed May  8 22:06:44 2024, max compression
```

## Comparing `lifton-1.0.1.tar` & `lifton-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.460955 lifton-1.0.1/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-1.0.1/LICENSE
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-05-06 01:24:29.449955 lifton-1.0.1/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27543 2024-05-06 01:23:28.000000 lifton-1.0.1/README.md
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:28.146952 lifton-1.0.1/lifton/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-05-06 01:22:29.000000 lifton-1.0.1/lifton/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-1.0.1/lifton/align.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-25 19:14:34.000000 lifton-1.0.1/lifton/annotation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-21 18:41:09.000000 lifton-1.0.1/lifton/extract_sequence.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-21 18:41:11.000000 lifton-1.0.1/lifton/get_id_fraction.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-1.0.1/lifton/intervals.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.253954 lifton-1.0.1/lifton/liftoff/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-1.0.1/lifton/liftoff/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/align_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/aligned_seg.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/extract_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/feature_hierarchy.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/find_best_mapping.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/fix_overlapping_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/lift_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-1.0.1/lifton/liftoff/liftoff_main.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/liftoff_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/liftover_types.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/merge_lifted_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/new_feature.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/polish.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:29.394955 lifton-1.0.1/lifton/liftoff/tests/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/tests/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-1.0.1/lifton/liftoff/tests/test_advanced.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-1.0.1/lifton/liftoff/tests/test_basic.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-1.0.1/lifton/liftoff/write_new_gff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20403 2024-05-06 01:23:50.000000 lifton-1.0.1/lifton/lifton.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34486 2024-05-06 01:21:50.000000 lifton-1.0.1/lifton/lifton_class.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20597 2024-04-24 11:32:28.000000 lifton-1.0.1/lifton/lifton_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-1.0.1/lifton/logger.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-05-04 23:05:47.000000 lifton-1.0.1/lifton/protein_maximization.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5764 2024-04-21 23:00:23.000000 lifton-1.0.1/lifton/run_evaluation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9031 2024-05-06 01:01:57.000000 lifton-1.0.1/lifton/run_liftoff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6350 2024-05-05 21:10:16.000000 lifton-1.0.1/lifton/run_miniprot.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 21:25:50.000000 lifton-1.0.1/lifton/stats.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4191 2024-04-21 22:07:42.000000 lifton-1.0.1/lifton/variants.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-05-06 01:24:28.384953 lifton-1.0.1/lifton.egg-info/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/SOURCES.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/dependency_links.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/entry_points.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/requires.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-05-06 01:24:26.000000 lifton-1.0.1/lifton.egg-info/top_level.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-05-06 01:24:29.470955 lifton-1.0.1/setup.cfg
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      865 2024-05-06 01:22:42.000000 lifton-1.0.1/setup.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752896 lifton-1.0.2/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34599 2024-01-03 16:41:07.000000 lifton-1.0.2/LICENSE
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752298 lifton-1.0.2/Lifton.egg-info/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29602 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/PKG-INFO
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1336 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/SOURCES.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/dependency_links.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       46 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/entry_points.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      168 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/requires.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        7 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/top_level.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29602 2024-05-08 22:06:44.752620 lifton-1.0.2/PKG-INFO
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    28941 2024-05-08 21:36:41.000000 lifton-1.0.2/README.md
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.745715 lifton-1.0.2/lifton/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       23 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     8659 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/align.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6640 2024-04-25 20:36:02.000000 lifton-1.0.2/lifton/annotation.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2620 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/extract_sequence.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1823 2024-04-24 16:55:38.000000 lifton-1.0.2/lifton/get_id_fraction.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      578 2024-01-17 14:20:47.000000 lifton-1.0.2/lifton/intervals.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.751541 lifton-1.0.2/lifton/liftoff/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        0 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    13175 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/align_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      597 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/aligned_seg.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    10276 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/extract_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      190 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/feature_hierarchy.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    19044 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/find_best_mapping.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9361 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/fix_overlapping_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5664 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/lift_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    15486 2024-04-24 10:49:54.000000 lifton-1.0.2/lifton/liftoff/liftoff_main.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4032 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/liftoff_utils.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5206 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/liftover_types.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     3945 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/merge_lifted_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      372 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/new_feature.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    14008 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/polish.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752090 lifton-1.0.2/lifton/liftoff/tests/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2058 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/test_advanced.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1895 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/test_basic.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5428 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/write_new_gff.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20403 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34486 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton_class.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20759 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton_utils.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      233 2024-01-22 16:32:54.000000 lifton-1.0.2/lifton/logger.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     7585 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/protein_maximization.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5764 2024-04-23 23:08:43.000000 lifton-1.0.2/lifton/run_evaluation.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9031 2024-04-24 10:52:31.000000 lifton-1.0.2/lifton/run_liftoff.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6350 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/run_miniprot.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5595 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/stats.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4191 2024-04-23 23:08:43.000000 lifton-1.0.2/lifton/variants.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       38 2024-05-08 22:06:44.752955 lifton-1.0.2/setup.cfg
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      865 2024-05-08 21:36:41.000000 lifton-1.0.2/setup.py
```

### Comparing `lifton-1.0.1/LICENSE` & `lifton-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/PKG-INFO` & `lifton-1.0.2/Lifton.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,76 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.1
+Version: 1.0.2
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: biopython>=1.76
+Requires-Dist: cigar>=0.1.3
+Requires-Dist: parasail>=1.2.4
+Requires-Dist: intervaltree>=3.1.0
+Requires-Dist: interlap>=0.2.6
+Requires-Dist: networkx>=2.4
+Requires-Dist: pyfaidx>=0.5.8
+Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1
+Requires-Dist: ujson>=3.2.0
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/LiftOn/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 <a class="reference external image-reference" href="https://img.shields.io/badge/License-GPLv3-yellow.svg"><img alt="https://img.shields.io/badge/License-GPLv3-yellow.svg" src="https://img.shields.io/badge/License-GPLv3-yellow.svg"></a>
-<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.0.0.1-blue"></a>
+<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.1.0.0-blue"></a>
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
 
 LiftOn is a homology-based lift-over tool using both DNA-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true" target="_blank">Liftoff</a>, credits to <a href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en" target="_blank">Dr. Alaina Shumate</a>) and protein-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621" target="_blank">miniprot</a>, credits to <a href="http://liheng.org" target="_blank">Dr. Heng Li</a>) to accurately map annotations between genome assemblies of the same or different species. LiftOn employs a two-step <a href="https://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm">protein maximization algorithm</a> to improve the annotation of protein-coding genes in the T2T-CHM13 <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz" target="_blank">JHU RefSeqv110 + Liftoff v5.1</a> annotation.
-The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.<section id="why-lifton" class="">
+The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.
+
+<section id="installation-wrap" class="">
+<h2>Installation<a class="headerlink" href="#installation-wrap" title="Permalink to this heading">#</a></h2>
+
+<section id="install-through-pip">
+<span id="id2"></span><h3>Install through pip<a class="headerlink" href="#install-through-pip" title="Permalink to this heading">#</a></h3>
+<p>LiftOn is on <a class="reference external" href="https://pypi.org/project/lifton/">PyPi</a> now. Check out all the releases <a class="reference external" href="https://pypi.org/manage/project/lifton/releases/">here</a>. Pip automatically resolves and installs any dependencies required by LiftOn.</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ pip install lifton
+</pre></div>
+</div>
+<div class="line-block">
+</div>
+</section>
+
+<section id="install-from-source">
+<span id="id4"></span><h3>Install from source<a class="headerlink" href="#install-from-source" title="Permalink to this heading">#</a></h3>
+<p>You can also install LiftOn from source. Check out the <a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn">latest version </a>
+!</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+</pre></div>
+</div>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
+</section>
+
+
+<section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, there are 30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429 viruses listed on NCBI (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/browse/#!/overview/">NCBI genome browser</a>). However, genome annotation is lagging behind. As more high-quality assemblies are generated, we need an accurate lift-over tool to annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> tool maps genes based on DNA alignments alone. <a class="reference external" href="https://github.com/lh3/miniprot">Miniprot</a> maps genes based on protein alignments but, without gene structure information, may not be as accurate on their own (See <a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html#why-lifton-qa"><span class="std std-ref">FAQ Common mistakes of Liftoff and miniprot</span></a>). LiftOn combines both DNA-to-genome and protein-to-genome alignments and produces better gene mapping results! LiftOn improves upon the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distantly related species lift-over</strong>: A key limitation of DNA-based lift-over tools is that they do not perform well when the reference and target genomes have significantly diverged. With the help of protein alignments and the protein maximization algorithm, LiftOn improves the lift-over process between distantly related species. See "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_mouse_2_rat.html#distant-species-liftover-mouse-to-rat"><span class="std std-ref">Mouse to Rat</span></a>" and "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_drosophila_erecta.html#distant-species-liftover-drosophila-melanogaster-2-erecta"><span class="std std-ref">Drosophila melanogaster to Drosophila erecta</span></a>" result sections.</p></li>
 </ol>
 <p>LiftOn is free, it's open source, it's easy to install , and it's in Python!</p>
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.1 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.2 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE[My Logo]
+markdown License-File: LICENSE Requires-Dist: numpy>=1.22.0 Requires-Dist:
+biopython>=1.76 Requires-Dist: cigar>=0.1.3 Requires-Dist: parasail>=1.2.4
+Requires-Dist: intervaltree>=3.1.0 Requires-Dist: interlap>=0.2.6 Requires-
+Dist: networkx>=2.4 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_o_w_n_l_o_a_d_s_/_K_u_a_n_h_a_o_-_C_h_a_o_/_l_i_f_t_o_n_/
 _t_o_t_a_l_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_g_i_t_h_u_b_&_l_a_b_e_l_=_D_o_w_n_l_o_a_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_p_l_a_t_f_o_r_m_-_m_a_c_O_S___/_L_i_n_u_x_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_l_a_b_._r_e_s_e_a_r_c_h_._g_o_o_g_l_e_._c_o_m_/
 _a_s_s_e_t_s_/_c_o_l_a_b_-_b_a_d_g_e_._s_v_g_]
@@ -17,14 +21,25 @@
 assemblies of the same or different species. LiftOn employs a two-step _p_r_o_t_e_i_n
 _m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m to improve the annotation of protein-coding genes in the
 T2T-CHM13 _J_H_U_ _R_e_f_S_e_q_v_1_1_0_ _+_ _L_i_f_t_o_f_f_ _v_5_._1 annotation. The latest T2T-CHM13
 annotation generated by LiftOn is available as
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_ _(_f_t_p_:_/_/_f_t_p_._c_c_b_._j_h_u_._e_d_u_/_p_u_b_/_d_a_t_a_/_L_i_f_t_O_n_/
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_)
 .
+********** IInnssttaallllaattiioonn_## **********
+******** IInnssttaallll tthhrroouugghh ppiipp_## ********
+LiftOn is on _P_y_P_i now. Check out all the releases _h_e_r_e. Pip automatically
+resolves and installs any dependencies required by LiftOn.
+$ pip install lifton
+******** IInnssttaallll ffrroomm ssoouurrccee_## ********
+You can also install LiftOn from source. Check out the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ !
+$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+
 ********** WWhhyy LLiiffttOOnn?â??_## **********
    1. BBuurrggeeoonniinngg nnuummbbeerr ooff ggeennoommee aasssseemmbblliieess: As of December 2023, there are
       30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429
       viruses listed on NCBI (_N_C_B_I_ _g_e_n_o_m_e_ _b_r_o_w_s_e_r). However, genome annotation
       is lagging behind. As more high-quality assemblies are generated, we need
       an accurate lift-over tool to annotate them.
    2. IImmpprroovveedd pprrootteeiinn--ccooddiinngg ggeennee mmaappppiinngg: The popular _L_i_f_t_o_f_f tool maps genes
```

### Comparing `lifton-1.0.1/README.md` & `lifton-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,54 @@
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/LiftOn/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 <a class="reference external image-reference" href="https://img.shields.io/badge/License-GPLv3-yellow.svg"><img alt="https://img.shields.io/badge/License-GPLv3-yellow.svg" src="https://img.shields.io/badge/License-GPLv3-yellow.svg"></a>
-<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.0.0.1-blue"></a>
+<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.1.0.0-blue"></a>
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
 
 LiftOn is a homology-based lift-over tool using both DNA-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true" target="_blank">Liftoff</a>, credits to <a href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en" target="_blank">Dr. Alaina Shumate</a>) and protein-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621" target="_blank">miniprot</a>, credits to <a href="http://liheng.org" target="_blank">Dr. Heng Li</a>) to accurately map annotations between genome assemblies of the same or different species. LiftOn employs a two-step <a href="https://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm">protein maximization algorithm</a> to improve the annotation of protein-coding genes in the T2T-CHM13 <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz" target="_blank">JHU RefSeqv110 + Liftoff v5.1</a> annotation.
-The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.<section id="why-lifton" class="">
+The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.
+
+<section id="installation-wrap" class="">
+<h2>Installation<a class="headerlink" href="#installation-wrap" title="Permalink to this heading">#</a></h2>
+
+<section id="install-through-pip">
+<span id="id2"></span><h3>Install through pip<a class="headerlink" href="#install-through-pip" title="Permalink to this heading">#</a></h3>
+<p>LiftOn is on <a class="reference external" href="https://pypi.org/project/lifton/">PyPi</a> now. Check out all the releases <a class="reference external" href="https://pypi.org/manage/project/lifton/releases/">here</a>. Pip automatically resolves and installs any dependencies required by LiftOn.</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ pip install lifton
+</pre></div>
+</div>
+<div class="line-block">
+</div>
+</section>
+
+<section id="install-from-source">
+<span id="id4"></span><h3>Install from source<a class="headerlink" href="#install-from-source" title="Permalink to this heading">#</a></h3>
+<p>You can also install LiftOn from source. Check out the <a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn">latest version </a>
+!</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+</pre></div>
+</div>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
+</section>
+
+
+<section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, there are 30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429 viruses listed on NCBI (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/browse/#!/overview/">NCBI genome browser</a>). However, genome annotation is lagging behind. As more high-quality assemblies are generated, we need an accurate lift-over tool to annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> tool maps genes based on DNA alignments alone. <a class="reference external" href="https://github.com/lh3/miniprot">Miniprot</a> maps genes based on protein alignments but, without gene structure information, may not be as accurate on their own (See <a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html#why-lifton-qa"><span class="std std-ref">FAQ Common mistakes of Liftoff and miniprot</span></a>). LiftOn combines both DNA-to-genome and protein-to-genome alignments and produces better gene mapping results! LiftOn improves upon the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distantly related species lift-over</strong>: A key limitation of DNA-based lift-over tools is that they do not perform well when the reference and target genomes have significantly diverged. With the help of protein alignments and the protein maximization algorithm, LiftOn improves the lift-over process between distantly related species. See "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_mouse_2_rat.html#distant-species-liftover-mouse-to-rat"><span class="std std-ref">Mouse to Rat</span></a>" and "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_drosophila_erecta.html#distant-species-liftover-drosophila-melanogaster-2-erecta"><span class="std std-ref">Drosophila melanogaster to Drosophila erecta</span></a>" result sections.</p></li>
 </ol>
 <p>LiftOn is free, it's open source, it's easy to install , and it's in Python!</p>
```

#### html2text {}

```diff
@@ -13,14 +13,25 @@
 assemblies of the same or different species. LiftOn employs a two-step _p_r_o_t_e_i_n
 _m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m to improve the annotation of protein-coding genes in the
 T2T-CHM13 _J_H_U_ _R_e_f_S_e_q_v_1_1_0_ _+_ _L_i_f_t_o_f_f_ _v_5_._1 annotation. The latest T2T-CHM13
 annotation generated by LiftOn is available as
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_ _(_f_t_p_:_/_/_f_t_p_._c_c_b_._j_h_u_._e_d_u_/_p_u_b_/_d_a_t_a_/_L_i_f_t_O_n_/
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_)
 .
+********** IInnssttaallllaattiioonn_## **********
+******** IInnssttaallll tthhrroouugghh ppiipp_## ********
+LiftOn is on _P_y_P_i now. Check out all the releases _h_e_r_e. Pip automatically
+resolves and installs any dependencies required by LiftOn.
+$ pip install lifton
+******** IInnssttaallll ffrroomm ssoouurrccee_## ********
+You can also install LiftOn from source. Check out the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ !
+$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+
 ********** WWhhyy LLiiffttOOnn?â??_## **********
    1. BBuurrggeeoonniinngg nnuummbbeerr ooff ggeennoommee aasssseemmbblliieess: As of December 2023, there are
       30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429
       viruses listed on NCBI (_N_C_B_I_ _g_e_n_o_m_e_ _b_r_o_w_s_e_r). However, genome annotation
       is lagging behind. As more high-quality assemblies are generated, we need
       an accurate lift-over tool to annotate them.
    2. IImmpprroovveedd pprrootteeiinn--ccooddiinngg ggeennee mmaappppiinngg: The popular _L_i_f_t_o_f_f tool maps genes
```

### Comparing `lifton-1.0.1/lifton/align.py` & `lifton-1.0.2/lifton/align.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/annotation.py` & `lifton-1.0.2/lifton/annotation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/extract_sequence.py` & `lifton-1.0.2/lifton/extract_sequence.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/get_id_fraction.py` & `lifton-1.0.2/lifton/get_id_fraction.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/intervals.py` & `lifton-1.0.2/lifton/intervals.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/align_features.py` & `lifton-1.0.2/lifton/liftoff/align_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/aligned_seg.py` & `lifton-1.0.2/lifton/liftoff/aligned_seg.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/extract_features.py` & `lifton-1.0.2/lifton/liftoff/extract_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/find_best_mapping.py` & `lifton-1.0.2/lifton/liftoff/find_best_mapping.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/fix_overlapping_features.py` & `lifton-1.0.2/lifton/liftoff/fix_overlapping_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/lift_features.py` & `lifton-1.0.2/lifton/liftoff/lift_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/liftoff_main.py` & `lifton-1.0.2/lifton/liftoff/liftoff_main.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/liftoff_utils.py` & `lifton-1.0.2/lifton/liftoff/liftoff_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/liftover_types.py` & `lifton-1.0.2/lifton/liftoff/liftover_types.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/merge_lifted_features.py` & `lifton-1.0.2/lifton/liftoff/merge_lifted_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/polish.py` & `lifton-1.0.2/lifton/liftoff/polish.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/tests/test_advanced.py` & `lifton-1.0.2/lifton/liftoff/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/tests/test_basic.py` & `lifton-1.0.2/lifton/liftoff/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/liftoff/write_new_gff.py` & `lifton-1.0.2/lifton/liftoff/write_new_gff.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/lifton.py` & `lifton-1.0.2/lifton/lifton.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/lifton_class.py` & `lifton-1.0.2/lifton/lifton_class.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/lifton_utils.py` & `lifton-1.0.2/lifton/lifton_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,20 +329,24 @@
             # Write out reference gene features IDs
             # Decide if its type
             gene_type_key = ""
             if args.annotation_database.upper() == "REFSEQ":
                 gene_type_key = "gene_biotype"
             elif args.annotation_database.upper() == "GENCODE" or args.annotation_database.upper() == "ENSEMBL" or args.annotation_database.upper() == "CHESS":
                 gene_type_key = "gene_type"
-            if locus.attributes[gene_type_key][0] == "protein_coding" and len(CDS_children) > 0:
-                feature.is_protein_coding = True
-                fw_gene.write(f"{locus.id}\tcoding\n")
-            elif (locus.attributes[gene_type_key][0] == "lncRNA" or locus.attributes[gene_type_key][0] == "ncRNA"):
-                feature.is_non_coding = True
-                fw_gene.write(f"{locus.id}\tnon-coding\n")
+
+            if gene_type_key in locus.attributes.keys():
+                if locus.attributes[gene_type_key][0] == "protein_coding" and len(CDS_children) > 0:
+                    feature.is_protein_coding = True
+                    fw_gene.write(f"{locus.id}\tcoding\n")
+                elif (locus.attributes[gene_type_key][0] == "lncRNA" or locus.attributes[gene_type_key][0] == "ncRNA"):
+                    feature.is_non_coding = True
+                    fw_gene.write(f"{locus.id}\tnon-coding\n")
+                else:
+                    fw_gene.write(f"{locus.id}\tother\n")
             else:
                 fw_gene.write(f"{locus.id}\tother\n")
             exon_children = list(ref_db.db_connection.children(locus, featuretype='exon', level=1, order_by='start'))
             if len(exon_children) > 0:
                 __process_ref_liffover_features(locus, ref_db, None)
             else:
                 transcripts = ref_db.db_connection.children(locus, level=1)
```

### Comparing `lifton-1.0.1/lifton/protein_maximization.py` & `lifton-1.0.2/lifton/protein_maximization.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/run_evaluation.py` & `lifton-1.0.2/lifton/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/run_liftoff.py` & `lifton-1.0.2/lifton/run_liftoff.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/run_miniprot.py` & `lifton-1.0.2/lifton/run_miniprot.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/stats.py` & `lifton-1.0.2/lifton/stats.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton/variants.py` & `lifton-1.0.2/lifton/variants.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.1/lifton.egg-info/PKG-INFO` & `lifton-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,76 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.1
+Version: 1.0.2
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: biopython>=1.76
+Requires-Dist: cigar>=0.1.3
+Requires-Dist: parasail>=1.2.4
+Requires-Dist: intervaltree>=3.1.0
+Requires-Dist: interlap>=0.2.6
+Requires-Dist: networkx>=2.4
+Requires-Dist: pyfaidx>=0.5.8
+Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1
+Requires-Dist: ujson>=3.2.0
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/LiftOn/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 <a class="reference external image-reference" href="https://img.shields.io/badge/License-GPLv3-yellow.svg"><img alt="https://img.shields.io/badge/License-GPLv3-yellow.svg" src="https://img.shields.io/badge/License-GPLv3-yellow.svg"></a>
-<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.0.0.1-blue"></a>
+<a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.1.0.0-blue"></a>
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download" src="https://img.shields.io/github/downloads/Kuanhao-Chao/lifton/total.svg?style=social&amp;logo=github&amp;label=Download"></a>
 <a class="reference external image-reference" href="https://github.com/Kuanhao-Chao/lifton/releases"><img alt="https://img.shields.io/badge/platform-macOS_/Linux-green.svg" src="https://img.shields.io/badge/platform-macOS_/Linux-green.svg"></a>
 <a class="reference external image-reference" href="https://colab.research.google.com/github/Kuanhao-Chao/lifton/blob/main/notebook/lifton_example.ipynb"><img alt="https://colab.research.google.com/assets/colab-badge.svg" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
 
 LiftOn is a homology-based lift-over tool using both DNA-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true" target="_blank">Liftoff</a>, credits to <a href="https://scholar.google.com/citations?user=N3tXk7QAAAAJ&amp;hl=en" target="_blank">Dr. Alaina Shumate</a>) and protein-DNA alignments (from <a href="https://academic.oup.com/bioinformatics/article/39/1/btad014/6989621" target="_blank">miniprot</a>, credits to <a href="http://liheng.org" target="_blank">Dr. Heng Li</a>) to accurately map annotations between genome assemblies of the same or different species. LiftOn employs a two-step <a href="https://ccb.jhu.edu/lifton/content/behind_scenes.html#protein-maximization-algorithm">protein maximization algorithm</a> to improve the annotation of protein-coding genes in the T2T-CHM13 <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz" target="_blank">JHU RefSeqv110 + Liftoff v5.1</a> annotation.
-The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.<section id="why-lifton" class="">
+The latest T2T-CHM13 annotation generated by LiftOn is available as <a href="https://tinyurl.com/4xywtwve" target="_blank">JHU_LiftOn_v1.0_chm13v2.0.gff3 (ftp://ftp.ccb.jhu.edu/pub/data/LiftOn/JHU_LiftOn_v1.0_chm13v2.0.gff3) <i class="fa fa-download"></i></a>.
+
+<section id="installation-wrap" class="">
+<h2>Installation<a class="headerlink" href="#installation-wrap" title="Permalink to this heading">#</a></h2>
+
+<section id="install-through-pip">
+<span id="id2"></span><h3>Install through pip<a class="headerlink" href="#install-through-pip" title="Permalink to this heading">#</a></h3>
+<p>LiftOn is on <a class="reference external" href="https://pypi.org/project/lifton/">PyPi</a> now. Check out all the releases <a class="reference external" href="https://pypi.org/manage/project/lifton/releases/">here</a>. Pip automatically resolves and installs any dependencies required by LiftOn.</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ pip install lifton
+</pre></div>
+</div>
+<div class="line-block">
+</div>
+</section>
+
+<section id="install-from-source">
+<span id="id4"></span><h3>Install from source<a class="headerlink" href="#install-from-source" title="Permalink to this heading">#</a></h3>
+<p>You can also install LiftOn from source. Check out the <a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn">latest version </a>
+!</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+</pre></div>
+</div>
+<div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
+</section>
+
+
+<section id="why-lifton" class="">
 <h2>Why LiftOn❓<a class="headerlink" href="#why-lifton" title="Permalink to this heading">#</a></h2>
 <ol class="arabic simple">
 <li><p><strong>Burgeoning number of genome assemblies</strong>: As of December 2023, there are 30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429 viruses listed on NCBI (<a class="reference external" href="https://www.ncbi.nlm.nih.gov/genome/browse/#!/overview/">NCBI genome browser</a>). However, genome annotation is lagging behind. As more high-quality assemblies are generated, we need an accurate lift-over tool to annotate them.</p></li>
 <li><p><strong>Improved protein-coding gene mapping</strong>: The popular <a class="reference external" href="https://academic.oup.com/bioinformatics/article/37/12/1639/6035128?login=true">Liftoff</a> tool maps genes based on DNA alignments alone. <a class="reference external" href="https://github.com/lh3/miniprot">Miniprot</a> maps genes based on protein alignments but, without gene structure information, may not be as accurate on their own (See <a class="reference internal" href="https://ccb.jhu.edu/lifton/content/how_to_page.html#why-lifton-qa"><span class="std std-ref">FAQ Common mistakes of Liftoff and miniprot</span></a>). LiftOn combines both DNA-to-genome and protein-to-genome alignments and produces better gene mapping results! LiftOn improves upon the current released T2T-CHM13 annotation (<a class="reference external" href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13v2.0_RefSeq_Liftoff_v5.1.gff3.gz">JHU RefSeqv110 + Liftoff v5.1</a>).</p></li>
 <li><p><strong>Improved distantly related species lift-over</strong>: A key limitation of DNA-based lift-over tools is that they do not perform well when the reference and target genomes have significantly diverged. With the help of protein alignments and the protein maximization algorithm, LiftOn improves the lift-over process between distantly related species. See "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_mouse_2_rat.html#distant-species-liftover-mouse-to-rat"><span class="std std-ref">Mouse to Rat</span></a>" and "<a class="reference internal" href="https://ccb.jhu.edu/lifton/content/distant_species_liftover/liftover_drosophila_erecta.html#distant-species-liftover-drosophila-melanogaster-2-erecta"><span class="std std-ref">Drosophila melanogaster to Drosophila erecta</span></a>" result sections.</p></li>
 </ol>
 <p>LiftOn is free, it's open source, it's easy to install , and it's in Python!</p>
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.1 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.2 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE[My Logo]
+markdown License-File: LICENSE Requires-Dist: numpy>=1.22.0 Requires-Dist:
+biopython>=1.76 Requires-Dist: cigar>=0.1.3 Requires-Dist: parasail>=1.2.4
+Requires-Dist: intervaltree>=3.1.0 Requires-Dist: interlap>=0.2.6 Requires-
+Dist: networkx>=2.4 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_o_w_n_l_o_a_d_s_/_K_u_a_n_h_a_o_-_C_h_a_o_/_l_i_f_t_o_n_/
 _t_o_t_a_l_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_g_i_t_h_u_b_&_l_a_b_e_l_=_D_o_w_n_l_o_a_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_p_l_a_t_f_o_r_m_-_m_a_c_O_S___/_L_i_n_u_x_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_l_a_b_._r_e_s_e_a_r_c_h_._g_o_o_g_l_e_._c_o_m_/
 _a_s_s_e_t_s_/_c_o_l_a_b_-_b_a_d_g_e_._s_v_g_]
@@ -17,14 +21,25 @@
 assemblies of the same or different species. LiftOn employs a two-step _p_r_o_t_e_i_n
 _m_a_x_i_m_i_z_a_t_i_o_n_ _a_l_g_o_r_i_t_h_m to improve the annotation of protein-coding genes in the
 T2T-CHM13 _J_H_U_ _R_e_f_S_e_q_v_1_1_0_ _+_ _L_i_f_t_o_f_f_ _v_5_._1 annotation. The latest T2T-CHM13
 annotation generated by LiftOn is available as
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_ _(_f_t_p_:_/_/_f_t_p_._c_c_b_._j_h_u_._e_d_u_/_p_u_b_/_d_a_t_a_/_L_i_f_t_O_n_/
 _J_H_U___L_i_f_t_O_n___v_1_._0___c_h_m_1_3_v_2_._0_._g_f_f_3_)
 .
+********** IInnssttaallllaattiioonn_## **********
+******** IInnssttaallll tthhrroouugghh ppiipp_## ********
+LiftOn is on _P_y_P_i now. Check out all the releases _h_e_r_e. Pip automatically
+resolves and installs any dependencies required by LiftOn.
+$ pip install lifton
+******** IInnssttaallll ffrroomm ssoouurrccee_## ********
+You can also install LiftOn from source. Check out the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ !
+$ git clone https://github.com/Kuanhao-Chao/LiftOn
+
+$ python setup.py install
+
 ********** WWhhyy LLiiffttOOnn?â??_## **********
    1. BBuurrggeeoonniinngg nnuummbbeerr ooff ggeennoommee aasssseemmbblliieess: As of December 2023, there are
       30,530 eukaryotic genomes, 567,228 prokaryotic genomes, and 66,429
       viruses listed on NCBI (_N_C_B_I_ _g_e_n_o_m_e_ _b_r_o_w_s_e_r). However, genome annotation
       is lagging behind. As more high-quality assemblies are generated, we need
       an accurate lift-over tool to annotate them.
    2. IImmpprroovveedd pprrootteeiinn--ccooddiinngg ggeennee mmaappppiinngg: The popular _L_i_f_t_o_f_f tool maps genes
```

### Comparing `lifton-1.0.1/setup.py` & `lifton-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).resolve().parent
 long_description = (this_directory / "./README.md").read_text()
 setuptools.setup(
 	name="lifton",
-	version="1.0.1",
+	version="1.0.2",
 	author="Kuan-Hao Chao",
 	author_email="kh.chao@cs.jhu.edu",
 	description="Combining DNA and protein alignments to improve genome annotation with LiftOn",
 	url="https://github.com/Kuanhao-Chao/Lifton",
 	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=2.4', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0'],
 	python_requires='>=3.6',
 	packages=setuptools.find_packages(),
```

