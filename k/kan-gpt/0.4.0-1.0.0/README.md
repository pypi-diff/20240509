# Comparing `tmp/kan_gpt-0.4.0.tar.gz` & `tmp/kan_gpt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.4.0.tar", last modified: Wed May  8 17:43:45 2024, max compression
+gzip compressed data, was "kan_gpt-1.0.0.tar", last modified: Thu May  9 02:35:47 2024, max compression
```

## Comparing `kan_gpt-0.4.0.tar` & `kan_gpt-1.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.176074 kan_gpt-0.4.0/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/download_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.176074 kan_gpt-0.4.0/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/efficient_kan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_dataset_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.746924 kan_gpt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-09 02:35:47.746924 kan_gpt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.738924 kan_gpt-1.0.0/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/download_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.738924 kan_gpt-1.0.0/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/efficient_kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.738924 kan_gpt-1.0.0/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.742924 kan_gpt-1.0.0/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.742924 kan_gpt-1.0.0/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.742924 kan_gpt-1.0.0/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 02:35:47.000000 kan_gpt-1.0.0/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 02:35:47.746924 kan_gpt-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:47.742924 kan_gpt-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 02:35:39.000000 kan_gpt-1.0.0/tests/test_train.py
```

### Comparing `kan_gpt-0.4.0/HISTORY.md` & `kan_gpt-1.0.0/HISTORY.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
 - Version increment. [Aditya NG]
+- Merge pull request #11 from wektorz/fix_missing_dataset_dowload.
+  [Aditya]
+
+  add missing dataset dowload to setup that caused train to fail in jupyter notebook
+- Update KAN_GPT.ipynb. [Wiktor Zdrojewski]
+
+  add missing dowload that caused train to fail
+- Docs(mkdocs): results added. [Aditya NG]
+- Docs(README,media): results and metrics. [Aditya NG]
+- Feat(train.py): metrics added. [Aditya NG]
+- Release: version 0.4.0 🚀 [Aditya NG]
+
+
+0.4.0 (2024-05-08)
+------------------
+- Release: version 0.4.0 🚀 [Aditya NG]
+- Version increment. [Aditya NG]
 - Fix(kan_gpt/efficient_kan/__init__.py): missing init file. [Aditya NG]
 - Feat(README.md): results added. [Aditya NG]
 - Docs(mkdocs): documentation for mkdocs. [Aditya NG]
 - Feat(sweep): slower learning rate. [Aditya NG]
 - Fix(sweep): max_iters. [Aditya NG]
 - Fix(sweep): cuda device. [Aditya NG]
 - Ci(main): disabled wandb in ci. [Aditya NG]
```

### Comparing `kan_gpt-0.4.0/LICENSE` & `kan_gpt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/PKG-INFO` & `kan_gpt-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.4.0
+Version: 1.0.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -118,15 +118,18 @@
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
 ## Results
 
 We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
 
-<img src="media/results.png">
+
+| Metrics |   |   |
+|---------|---------|---------|
+| ![results_loss](media/results_loss.png) | ![results_cross_entropy](media/results_cross_entropy.png) | ![results_perplexity](media/results_perplexity.png) |
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.4.0/README.md` & `kan_gpt-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -85,15 +85,18 @@
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
 ## Results
 
 We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
 
-<img src="media/results.png">
+
+| Metrics |   |   |
+|---------|---------|---------|
+| ![results_loss](media/results_loss.png) | ![results_cross_entropy](media/results_cross_entropy.png) | ![results_perplexity](media/results_perplexity.png) |
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.4.0/kan_gpt/cli.py` & `kan_gpt-1.0.0/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/dataset.py` & `kan_gpt-1.0.0/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/download_dataset.py` & `kan_gpt-1.0.0/kan_gpt/download_dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/efficient_kan/model.py` & `kan_gpt-1.0.0/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/KAN.py` & `kan_gpt-1.0.0/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/KANLayer.py` & `kan_gpt-1.0.0/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/LBFGS.py` & `kan_gpt-1.0.0/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-1.0.0/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-1.0.0/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/spline.py` & `kan_gpt-1.0.0/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/kan/utils.py` & `kan_gpt-1.0.0/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/mingpt/bpe.py` & `kan_gpt-1.0.0/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/mingpt/model.py` & `kan_gpt-1.0.0/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/mingpt/trainer.py` & `kan_gpt-1.0.0/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/mingpt/utils.py` & `kan_gpt-1.0.0/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/model.py` & `kan_gpt-1.0.0/kan_gpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/prompt.py` & `kan_gpt-1.0.0/kan_gpt/prompt.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt/sweep.py` & `kan_gpt-1.0.0/kan_gpt/sweep.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-1.0.0/kan_gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.4.0
+Version: 1.0.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -118,15 +118,18 @@
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
 ## Results
 
 We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
 
-<img src="media/results.png">
+
+| Metrics |   |   |
+|---------|---------|---------|
+| ![results_loss](media/results_loss.png) | ![results_cross_entropy](media/results_cross_entropy.png) | ![results_perplexity](media/results_perplexity.png) |
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-0.4.0/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-1.0.0/kan_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/setup.py` & `kan_gpt-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_dataset_download.py` & `kan_gpt-1.0.0/tests/test_dataset_download.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_efficient_kan.py` & `kan_gpt-1.0.0/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_gpt_kan.py` & `kan_gpt-1.0.0/tests/test_gpt_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_gpt_mlp.py` & `kan_gpt-1.0.0/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_kan.py` & `kan_gpt-1.0.0/tests/test_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.4.0/tests/test_train.py` & `kan_gpt-1.0.0/tests/test_train.py`

 * *Files identical despite different names*

