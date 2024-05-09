# Comparing `tmp/imodelsx-1.0.5.tar.gz` & `tmp/imodelsx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodelsx-1.0.5.tar", last modified: Wed May  8 13:22:01 2024, max compression
+gzip compressed data, was "imodelsx-1.0.6.tar", last modified: Wed May  8 13:27:51 2024, max compression
```

## Comparing `imodelsx-1.0.5.tar` & `imodelsx-1.0.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.449416 imodelsx-1.0.5/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:22:01.445417 imodelsx-1.0.5/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.389415 imodelsx-1.0.5/imodelsx/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      653 2024-05-06 13:13:22.000000 imodelsx-1.0.5/imodelsx/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.421416 imodelsx-1.0.5/imodelsx/auglinear/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.5/imodelsx/auglinear/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.5/imodelsx/auglinear/auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.5/imodelsx/auglinear/embed.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.437416 imodelsx-1.0.5/imodelsx/augtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.5/imodelsx/augtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.5/imodelsx/augtree/augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.5/imodelsx/augtree/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.5/imodelsx/augtree/embed.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.5/imodelsx/augtree/ensemble.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.5/imodelsx/augtree/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.5/imodelsx/augtree/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.5/imodelsx/augtree/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.5/imodelsx/cache_save_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/d3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.5/imodelsx/d3/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.5/imodelsx/d3/d3.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.5/imodelsx/d3/step1_get_extreme.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.5/imodelsx/d3/step2_proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.5/imodelsx/d3/step3_verifier.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.5/imodelsx/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.5/imodelsx/dummy_script.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.5/imodelsx/embeddings.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/iprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/autoprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.5/imodelsx/iprompt/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/gumbel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.5/imodelsx/iprompt/hotflip.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/ipromptx.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.5/imodelsx/iprompt/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/prompt_tune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.5/imodelsx/iprompt/utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/kan/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 12:53:34.000000 imodelsx-1.0.5/imodelsx/kan/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12031 2024-05-06 13:10:10.000000 imodelsx-1.0.5/imodelsx/kan/kan_modules.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6580 2024-05-08 13:19:10.000000 imodelsx-1.0.5/imodelsx/kan/kan_sklearn.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.5/imodelsx/linear_finetune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.5/imodelsx/linear_ngram.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.5/imodelsx/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.5/imodelsx/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.5/imodelsx/process_results.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/imodelsx/sasc/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.5/imodelsx/sasc/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.5/imodelsx/sasc/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.5/imodelsx/sasc/m1_ngrams.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.5/imodelsx/sasc/m2_summarize.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.5/imodelsx/sasc/m3_generate.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14932 2024-05-07 20:58:56.000000 imodelsx-1.0.5/imodelsx/submit_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/imodelsx/treeprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.5/imodelsx/treeprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.5/imodelsx/treeprompt/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.5/imodelsx/treeprompt/treeprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.5/imodelsx/util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.5/imodelsx/viz.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.409415 imodelsx-1.0.5/imodelsx.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1643 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-08 13:22:01.449416 imodelsx-1.0.5/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-08 13:11:33.000000 imodelsx-1.0.5/setup.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/tests/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.5/tests/test_auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.5/tests/test_auglinear_pipeline.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.5/tests/test_augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.5/tests/test_iprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.5/tests/test_llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.5/tests/test_ngram_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.5/tests/test_sasc.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.248340 imodelsx-1.0.6/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:27:51.248340 imodelsx-1.0.6/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.236339 imodelsx-1.0.6/imodelsx/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      653 2024-05-06 13:13:22.000000 imodelsx-1.0.6/imodelsx/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.240340 imodelsx-1.0.6/imodelsx/auglinear/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.6/imodelsx/auglinear/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.6/imodelsx/auglinear/auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.6/imodelsx/auglinear/embed.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.240340 imodelsx-1.0.6/imodelsx/augtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.6/imodelsx/augtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.6/imodelsx/augtree/augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.6/imodelsx/augtree/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.6/imodelsx/augtree/embed.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.6/imodelsx/augtree/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.6/imodelsx/augtree/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.6/imodelsx/augtree/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.6/imodelsx/augtree/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.6/imodelsx/cache_save_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.240340 imodelsx-1.0.6/imodelsx/d3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.6/imodelsx/d3/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.6/imodelsx/d3/d3.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.6/imodelsx/d3/step1_get_extreme.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.6/imodelsx/d3/step2_proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.6/imodelsx/d3/step3_verifier.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.6/imodelsx/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.6/imodelsx/dummy_script.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.6/imodelsx/embeddings.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.244340 imodelsx-1.0.6/imodelsx/iprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.6/imodelsx/iprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.6/imodelsx/iprompt/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.6/imodelsx/iprompt/autoprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.6/imodelsx/iprompt/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.6/imodelsx/iprompt/gumbel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.6/imodelsx/iprompt/hotflip.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.6/imodelsx/iprompt/ipromptx.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.6/imodelsx/iprompt/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.6/imodelsx/iprompt/prompt_tune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.6/imodelsx/iprompt/utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.244340 imodelsx-1.0.6/imodelsx/kan/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 12:53:34.000000 imodelsx-1.0.6/imodelsx/kan/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12031 2024-05-06 13:10:10.000000 imodelsx-1.0.6/imodelsx/kan/kan_modules.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6580 2024-05-08 13:19:10.000000 imodelsx-1.0.6/imodelsx/kan/kan_sklearn.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.6/imodelsx/linear_finetune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.6/imodelsx/linear_ngram.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.6/imodelsx/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.6/imodelsx/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.6/imodelsx/process_results.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.244340 imodelsx-1.0.6/imodelsx/sasc/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.6/imodelsx/sasc/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.6/imodelsx/sasc/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.6/imodelsx/sasc/m1_ngrams.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.6/imodelsx/sasc/m2_summarize.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.6/imodelsx/sasc/m3_generate.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14932 2024-05-07 20:58:56.000000 imodelsx-1.0.6/imodelsx/submit_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.248340 imodelsx-1.0.6/imodelsx/treeprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.6/imodelsx/treeprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.6/imodelsx/treeprompt/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.6/imodelsx/treeprompt/treeprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.6/imodelsx/util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.6/imodelsx/viz.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.240340 imodelsx-1.0.6/imodelsx.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:27:51.000000 imodelsx-1.0.6/imodelsx.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1643 2024-05-08 13:27:51.000000 imodelsx-1.0.6/imodelsx.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-08 13:27:51.000000 imodelsx-1.0.6/imodelsx.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-08 13:27:51.000000 imodelsx-1.0.6/imodelsx.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-08 13:27:51.000000 imodelsx-1.0.6/imodelsx.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-08 13:27:51.248340 imodelsx-1.0.6/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-08 13:27:12.000000 imodelsx-1.0.6/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:27:51.248340 imodelsx-1.0.6/tests/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.6/tests/test_auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.6/tests/test_auglinear_pipeline.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.6/tests/test_augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.6/tests/test_iprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.6/tests/test_llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.6/tests/test_ngram_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.6/tests/test_sasc.py
```

### Comparing `imodelsx-1.0.5/PKG-INFO` & `imodelsx-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.5 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.6 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.5/imodelsx/__init__.py` & `imodelsx-1.0.6/imodelsx/__init__.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/auglinear/auglinear.py` & `imodelsx-1.0.6/imodelsx/auglinear/auglinear.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/auglinear/embed.py` & `imodelsx-1.0.6/imodelsx/auglinear/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/augtree.py` & `imodelsx-1.0.6/imodelsx/augtree/augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/data.py` & `imodelsx-1.0.6/imodelsx/augtree/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/embed.py` & `imodelsx-1.0.6/imodelsx/augtree/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/ensemble.py` & `imodelsx-1.0.6/imodelsx/augtree/ensemble.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/llm.py` & `imodelsx-1.0.6/imodelsx/augtree/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/stump.py` & `imodelsx-1.0.6/imodelsx/augtree/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/augtree/utils.py` & `imodelsx-1.0.6/imodelsx/augtree/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/cache_save_utils.py` & `imodelsx-1.0.6/imodelsx/cache_save_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/d3/d3.py` & `imodelsx-1.0.6/imodelsx/d3/d3.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/d3/step1_get_extreme.py` & `imodelsx-1.0.6/imodelsx/d3/step1_get_extreme.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/d3/step2_proposer.py` & `imodelsx-1.0.6/imodelsx/d3/step2_proposer.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/d3/step3_verifier.py` & `imodelsx-1.0.6/imodelsx/d3/step3_verifier.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/data.py` & `imodelsx-1.0.6/imodelsx/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/embeddings.py` & `imodelsx-1.0.6/imodelsx/embeddings.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/api.py` & `imodelsx-1.0.6/imodelsx/iprompt/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/autoprompt.py` & `imodelsx-1.0.6/imodelsx/iprompt/autoprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/data.py` & `imodelsx-1.0.6/imodelsx/iprompt/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/gumbel.py` & `imodelsx-1.0.6/imodelsx/iprompt/gumbel.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/hotflip.py` & `imodelsx-1.0.6/imodelsx/iprompt/hotflip.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/ipromptx.py` & `imodelsx-1.0.6/imodelsx/iprompt/ipromptx.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/llm.py` & `imodelsx-1.0.6/imodelsx/iprompt/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/prompt_tune.py` & `imodelsx-1.0.6/imodelsx/iprompt/prompt_tune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/iprompt/utils.py` & `imodelsx-1.0.6/imodelsx/iprompt/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/kan/kan_modules.py` & `imodelsx-1.0.6/imodelsx/kan/kan_modules.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/kan/kan_sklearn.py` & `imodelsx-1.0.6/imodelsx/kan/kan_sklearn.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/linear_finetune.py` & `imodelsx-1.0.6/imodelsx/linear_finetune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/linear_ngram.py` & `imodelsx-1.0.6/imodelsx/linear_ngram.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/llm.py` & `imodelsx-1.0.6/imodelsx/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/metrics.py` & `imodelsx-1.0.6/imodelsx/metrics.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/process_results.py` & `imodelsx-1.0.6/imodelsx/process_results.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/sasc/api.py` & `imodelsx-1.0.6/imodelsx/sasc/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/sasc/m1_ngrams.py` & `imodelsx-1.0.6/imodelsx/sasc/m1_ngrams.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/sasc/m2_summarize.py` & `imodelsx-1.0.6/imodelsx/sasc/m2_summarize.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/sasc/m3_generate.py` & `imodelsx-1.0.6/imodelsx/sasc/m3_generate.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/submit_utils.py` & `imodelsx-1.0.6/imodelsx/submit_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/treeprompt/stump.py` & `imodelsx-1.0.6/imodelsx/treeprompt/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/treeprompt/treeprompt.py` & `imodelsx-1.0.6/imodelsx/treeprompt/treeprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/util.py` & `imodelsx-1.0.6/imodelsx/util.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx/viz.py` & `imodelsx-1.0.6/imodelsx/viz.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/imodelsx.egg-info/PKG-INFO` & `imodelsx-1.0.6/imodelsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.5 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.6 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
```

### Comparing `imodelsx-1.0.5/imodelsx.egg-info/SOURCES.txt` & `imodelsx-1.0.6/imodelsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/setup.py` & `imodelsx-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'InstructorEmbedding', # embeddings for emb_diff_module
     # 'sentence-transformers', # embeddings for emb_diff_module
     # pdoc3 # for generating docs
 ]
 
 setuptools.setup(
     name="imodelsx",
-    version="1.0.5",
+    version="1.0.6",
     author="Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng",
     author_email="chansingh@microsoft.com",
     description="Library to explain a dataset in natural language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodelsX",
     packages=setuptools.find_packages(
```

### Comparing `imodelsx-1.0.5/tests/test_auglinear_pipeline.py` & `imodelsx-1.0.6/tests/test_auglinear_pipeline.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/tests/test_augtree.py` & `imodelsx-1.0.6/tests/test_augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/tests/test_iprompt.py` & `imodelsx-1.0.6/tests/test_iprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/tests/test_llm.py` & `imodelsx-1.0.6/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/tests/test_ngram_list.py` & `imodelsx-1.0.6/tests/test_ngram_list.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.5/tests/test_sasc.py` & `imodelsx-1.0.6/tests/test_sasc.py`

 * *Files identical despite different names*

