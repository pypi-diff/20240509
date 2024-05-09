# Comparing `tmp/pyfmtools-0.81.tar.gz` & `tmp/pyfmtools-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmtools-0.81.tar", last modified: Tue Apr 11 01:52:08 2023, max compression
+gzip compressed data, was "pyfmtools-5.1.tar", last modified: Thu May  9 01:15:28 2024, max compression
```

## Comparing `pyfmtools-0.81.tar` & `pyfmtools-5.1.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.689706 pyfmtools-0.81/
--rw-r--r--   0 nhenseler   (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-0.81/LICENSE.txt
--rw-rw-r--   0 nhenseler   (501) staff       (20)      211 2022-06-27 07:31:35.000000 pyfmtools-0.81/MANIFEST.in
--rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-04-11 01:52:08.689284 pyfmtools-0.81/PKG-INFO
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-0.81/README.md
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.423642 pyfmtools-0.81/dist/
--rw-r--r--   0 nhenseler   (501) staff       (20)   436101 2023-04-11 01:52:07.000000 pyfmtools-0.81/dist/pyfmtools-0.81-cp39-cp39-macosx_10_9_x86_64.whl
--rw-r--r--   0 nhenseler   (501) staff       (20)       38 2023-04-11 01:52:08.689870 pyfmtools-0.81/setup.cfg
--rw-r--r--   0 nhenseler   (501) staff       (20)      946 2023-04-11 01:47:13.000000 pyfmtools-0.81/setup.py
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.681332 pyfmtools-0.81/src/
--rw-------   0 nhenseler   (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-0.81/src/binarylattice.h
--rw-r--r--   0 nhenseler   (501) staff       (20)    10148 2022-05-23 02:31:18.000000 pyfmtools-0.81/src/buildPyfmtools.py
--rw-------   0 nhenseler   (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-0.81/src/colamd.c
--rw-------   0 nhenseler   (501) staff       (20)     9804 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/colamd.h
--rw-------   0 nhenseler   (501) staff       (20)    19373 2020-04-28 01:07:53.000000 pyfmtools-0.81/src/commonlib.c
--rw-------   0 nhenseler   (501) staff       (20)     8894 2020-04-28 01:28:51.000000 pyfmtools-0.81/src/commonlib.h
--rw-------   0 nhenseler   (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/declare.h
--rw-------   0 nhenseler   (501) staff       (20)    26583 2021-02-16 05:37:08.000000 pyfmtools-0.81/src/fmrandom.cpp
--rw-------   0 nhenseler   (501) staff       (20)     6042 2021-02-15 23:08:21.000000 pyfmtools-0.81/src/fmrandom.h
--rw-------   0 nhenseler   (501) staff       (20)     7326 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/fortify.h
--rw-------   0 nhenseler   (501) staff       (20)    42931 2021-06-26 11:56:42.000000 pyfmtools-0.81/src/fuzzymeasurefit.cpp
--rw-------   0 nhenseler   (501) staff       (20)    10458 2020-09-15 03:02:02.000000 pyfmtools-0.81/src/fuzzymeasurefit.h
--rw-------   0 nhenseler   (501) staff       (20)    46580 2021-02-12 00:35:43.000000 pyfmtools-0.81/src/fuzzymeasurefit3.cpp
--rw-------   0 nhenseler   (501) staff       (20)    53584 2022-03-23 22:37:43.000000 pyfmtools-0.81/src/fuzzymeasuretools.bak.cpp
--rw-------   0 nhenseler   (501) staff       (20)    19772 2022-05-19 03:16:38.000000 pyfmtools-0.81/src/fuzzymeasuretools.bak.h
--rw-------   0 nhenseler   (501) staff       (20)    53591 2023-04-11 01:38:11.000000 pyfmtools-0.81/src/fuzzymeasuretools.cpp
--rw-------   0 nhenseler   (501) staff       (20)    19220 2023-04-11 01:38:11.000000 pyfmtools-0.81/src/fuzzymeasuretools.h
--rw-------   0 nhenseler   (501) staff       (20)      750 2022-04-13 06:22:25.000000 pyfmtools-0.81/src/generaldefs.h
--rw-------   0 nhenseler   (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-0.81/src/hbio.h
--rw-------   0 nhenseler   (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-0.81/src/ini.c
--rw-------   0 nhenseler   (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/ini.h
--rw-------   0 nhenseler   (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-0.81/src/isfixedvar.c
--rw-------   0 nhenseler   (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_BFP.h
--rw-------   0 nhenseler   (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_BFP1.h
--rw-------   0 nhenseler   (501) staff       (20)     4444 2021-02-16 05:56:16.000000 pyfmtools-0.81/src/lp_BFP2.h
--rw-------   0 nhenseler   (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_Hash.c
--rw-------   0 nhenseler   (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_Hash.h
--rw-------   0 nhenseler   (501) staff       (20)    23763 2020-09-15 01:45:42.000000 pyfmtools-0.81/src/lp_LUSOL.c
--rw-------   0 nhenseler   (501) staff       (20)     2818 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_LUSOL.h
--rw-------   0 nhenseler   (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MDO.c
--rw-------   0 nhenseler   (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MDO.h
--rw-------   0 nhenseler   (501) staff       (20)    53842 2021-02-16 06:53:34.000000 pyfmtools-0.81/src/lp_MPS.c
--rw-------   0 nhenseler   (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MPS.h
--rw-------   0 nhenseler   (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_SOS.c
--rw-------   0 nhenseler   (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_SOS.h
--rw-------   0 nhenseler   (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_crash.c
--rw-------   0 nhenseler   (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_crash.h
--rw-------   0 nhenseler   (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-0.81/src/lp_etaPFI.h
--rw-------   0 nhenseler   (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_explicit.h
--rw-------   0 nhenseler   (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_fortify.h
--rw-------   0 nhenseler   (501) staff       (20)   286090 2022-05-23 02:33:29.000000 pyfmtools-0.81/src/lp_lib.c
--rw-------   0 nhenseler   (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-0.81/src/lp_lib.h
--rw-------   0 nhenseler   (501) staff       (20)    96546 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_matrix.c
--rw-------   0 nhenseler   (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_matrix.h
--rw-------   0 nhenseler   (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-0.81/src/lp_mipbb.c
--rw-------   0 nhenseler   (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_mipbb.h
--rw-------   0 nhenseler   (501) staff       (20)    23491 2021-02-12 00:36:06.000000 pyfmtools-0.81/src/lp_params.c
--rw-------   0 nhenseler   (501) staff       (20)   184143 2021-07-24 00:59:10.000000 pyfmtools-0.81/src/lp_presolve.c
--rw-------   0 nhenseler   (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_presolve.h
--rw-------   0 nhenseler   (501) staff       (20)    68918 2020-09-24 08:24:57.000000 pyfmtools-0.81/src/lp_price.c
--rw-------   0 nhenseler   (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_price.h
--rw-------   0 nhenseler   (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_pricePSE.c
--rw-------   0 nhenseler   (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_pricePSE.h
--rw-------   0 nhenseler   (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-0.81/src/lp_report.c
--rw-------   0 nhenseler   (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_report.h
--rw-------   0 nhenseler   (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-0.81/src/lp_rlp.h
--rw-------   0 nhenseler   (501) staff       (20)    29508 2017-12-15 12:16:42.000000 pyfmtools-0.81/src/lp_scale.c
--rw-------   0 nhenseler   (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_scale.h
--rw-------   0 nhenseler   (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_simplex.c
--rw-------   0 nhenseler   (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_simplex.h
--rw-------   0 nhenseler   (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-0.81/src/lp_types.h
--rw-------   0 nhenseler   (501) staff       (20)    26914 2020-09-24 08:01:30.000000 pyfmtools-0.81/src/lp_utils.c
--rw-------   0 nhenseler   (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_utils.h
--rw-------   0 nhenseler   (501) staff       (20)    11210 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/lp_wlp.c
--rw-------   0 nhenseler   (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_wlp.h
--rw-------   0 nhenseler   (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-0.81/src/lpkit.h
--rw-------   0 nhenseler   (501) staff       (20)    21870 2020-09-24 08:24:40.000000 pyfmtools-0.81/src/lpslink56.c
--rw-------   0 nhenseler   (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lpsolve.h
--rw-------   0 nhenseler   (501) staff       (20)    24934 2020-04-28 01:21:09.000000 pyfmtools-0.81/src/lusol.c
--rw-------   0 nhenseler   (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol.h
--rw-------   0 nhenseler   (501) staff       (20)   135944 2017-12-15 11:57:34.000000 pyfmtools-0.81/src/lusol1.h
--rw-------   0 nhenseler   (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol2.h
--rw-------   0 nhenseler   (501) staff       (20)    28424 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6a.h
--rw-------   0 nhenseler   (501) staff       (20)     4498 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6l0.h
--rw-------   0 nhenseler   (501) staff       (20)     4899 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6u.h
--rw-------   0 nhenseler   (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol7a.h
--rw-------   0 nhenseler   (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol8a.h
--rw-------   0 nhenseler   (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/lusolio.c
--rw-------   0 nhenseler   (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusolio.h
--rw-------   0 nhenseler   (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-0.81/src/minimalsplus.h
--rw-------   0 nhenseler   (501) staff       (20)    13025 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/mmio.c
--rw-------   0 nhenseler   (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/mmio.h
--rw-------   0 nhenseler   (501) staff       (20)    19312 2020-04-28 01:22:16.000000 pyfmtools-0.81/src/myblas.c
--rw-------   0 nhenseler   (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-0.81/src/myblas.h
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.685625 pyfmtools-0.81/src/pyfmtools.egg-info/
--rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/PKG-INFO
--rw-r--r--   0 nhenseler   (501) staff       (20)     1776 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/SOURCES.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)        1 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/dependency_links.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       12 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/requires.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       21 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/top_level.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)    48236 2023-03-27 07:08:40.000000 pyfmtools-0.81/src/pyfmtools.py
--rw-------   0 nhenseler   (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-0.81/src/sparselib.c
--rw-------   0 nhenseler   (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/sparselib.h
--rw-------   0 nhenseler   (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-0.81/src/stdafx.h
--rw-------   0 nhenseler   (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/ufortify.h
--rw-------   0 nhenseler   (501) staff       (20)    87216 2022-05-23 02:18:42.000000 pyfmtools-0.81/src/wrapperpy.cpp
--rw-------   0 nhenseler   (501) staff       (20)    14390 2022-05-20 09:48:18.000000 pyfmtools-0.81/src/wrapperpy.h
--rw-------   0 nhenseler   (501) staff       (20)    28266 2020-09-24 07:46:24.000000 pyfmtools-0.81/src/yacc_read.c
--rw-------   0 nhenseler   (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-0.81/src/yacc_read.h
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.688521 pyfmtools-0.81/tests/
--rw-------   0 nhenseler   (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-0.81/tests/test_no_wrapper.py
--rw-r--r--   0 nhenseler   (501) staff       (20)    27771 2022-06-28 04:36:04.000000 pyfmtools-0.81/tests/test_wrapper.py
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-09 01:15:28.080225 pyfmtools-5.1/
+-rw-r--r--   0 gleb       (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-5.1/LICENSE.txt
+-rw-rw-r--   0 gleb       (501) staff       (20)      239 2024-05-08 11:29:16.000000 pyfmtools-5.1/MANIFEST.in
+-rw-r--r--   0 gleb       (501) staff       (20)     5355 2024-05-09 01:15:28.080153 pyfmtools-5.1/PKG-INFO
+-rw-rw-r--   0 gleb       (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-5.1/README.md
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-09 01:15:28.057909 pyfmtools-5.1/dist/
+-rw-r--r--   0 gleb       (501) staff       (20)   497054 2024-05-09 01:14:54.000000 pyfmtools-5.1/dist/pyfmtools-5.1-cp312-cp312-macosx_14_0_arm64.whl
+-rw-r--r--   0 gleb       (501) staff       (20)       38 2024-05-09 01:15:28.080599 pyfmtools-5.1/setup.cfg
+-rw-r--r--   0 gleb       (501) staff       (20)      947 2024-04-21 05:18:21.000000 pyfmtools-5.1/setup.py
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-09 01:15:28.078382 pyfmtools-5.1/src/
+-rw-------   0 gleb       (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-5.1/src/binarylattice.h
+-rw-r--r--   0 gleb       (501) staff       (20)    12359 2024-05-05 06:50:55.000000 pyfmtools-5.1/src/buildPyfmtools.py
+-rw-------   0 gleb       (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-5.1/src/colamd.c
+-rw-r--r--   0 gleb       (501) staff       (20)     9805 2024-04-14 06:20:55.000000 pyfmtools-5.1/src/colamd.h
+-rw-r--r--   0 gleb       (501) staff       (20)    19333 2024-04-14 05:56:20.000000 pyfmtools-5.1/src/commonlib.c
+-rw-r--r--   0 gleb       (501) staff       (20)     8898 2023-11-18 13:55:16.000000 pyfmtools-5.1/src/commonlib.h
+-rw-------   0 gleb       (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/declare.h
+-rw-r--r--   0 gleb       (501) staff       (20)    26878 2024-04-25 03:30:44.000000 pyfmtools-5.1/src/fmrandom.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)     9046 2024-04-25 05:08:55.000000 pyfmtools-5.1/src/fmrandom.h
+-rw-r--r--   0 gleb       (501) staff       (20)    53034 2024-05-08 10:01:08.000000 pyfmtools-5.1/src/fmrandomsort.inc
+-rw-r--r--   0 gleb       (501) staff       (20)     7328 2023-11-18 13:41:34.000000 pyfmtools-5.1/src/fortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)    45535 2024-04-25 07:04:40.000000 pyfmtools-5.1/src/fuzzymeasurefit.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    10737 2024-04-26 08:00:42.000000 pyfmtools-5.1/src/fuzzymeasurefit.h
+-rw-r--r--   0 gleb       (501) staff       (20)    57669 2024-05-08 11:02:45.000000 pyfmtools-5.1/src/fuzzymeasurefit3.cpp
+-rw-------   0 gleb       (501) staff       (20)    53584 2022-03-23 22:37:43.000000 pyfmtools-5.1/src/fuzzymeasuretools.bak.cpp
+-rw-------   0 gleb       (501) staff       (20)    19772 2022-05-19 03:16:38.000000 pyfmtools-5.1/src/fuzzymeasuretools.bak.h
+-rw-r--r--   0 gleb       (501) staff       (20)    53752 2024-05-02 11:03:22.000000 pyfmtools-5.1/src/fuzzymeasuretools.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    18169 2024-05-02 11:02:46.000000 pyfmtools-5.1/src/fuzzymeasuretools.h
+-rw-r--r--   0 gleb       (501) staff       (20)      500 2024-04-25 09:14:22.000000 pyfmtools-5.1/src/gbrealloc.c
+-rw-r--r--   0 gleb       (501) staff       (20)     1030 2024-04-30 06:46:32.000000 pyfmtools-5.1/src/generaldefs.h
+-rw-------   0 gleb       (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-5.1/src/hbio.h
+-rw-------   0 gleb       (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-5.1/src/ini.c
+-rw-------   0 gleb       (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/ini.h
+-rw-------   0 gleb       (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-5.1/src/isfixedvar.c
+-rw-------   0 gleb       (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_BFP.h
+-rw-------   0 gleb       (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_BFP1.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4420 2024-04-14 05:45:40.000000 pyfmtools-5.1/src/lp_BFP2.h
+-rw-------   0 gleb       (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-5.1/src/lp_Hash.c
+-rw-------   0 gleb       (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_Hash.h
+-rw-r--r--   0 gleb       (501) staff       (20)    23763 2024-03-24 08:42:10.000000 pyfmtools-5.1/src/lp_LUSOL.c
+-rw-r--r--   0 gleb       (501) staff       (20)     2818 2024-03-24 08:42:23.000000 pyfmtools-5.1/src/lp_LUSOL.h
+-rw-------   0 gleb       (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_MDO.c
+-rw-------   0 gleb       (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_MDO.h
+-rw-r--r--   0 gleb       (501) staff       (20)    54130 2024-03-24 08:48:14.000000 pyfmtools-5.1/src/lp_MPS.c
+-rw-------   0 gleb       (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_MPS.h
+-rw-------   0 gleb       (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-5.1/src/lp_SOS.c
+-rw-------   0 gleb       (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_SOS.h
+-rw-------   0 gleb       (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_crash.c
+-rw-------   0 gleb       (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_crash.h
+-rw-------   0 gleb       (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-5.1/src/lp_etaPFI.h
+-rw-------   0 gleb       (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_explicit.h
+-rw-------   0 gleb       (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_fortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)   286192 2024-04-14 11:30:55.000000 pyfmtools-5.1/src/lp_lib.c
+-rw-------   0 gleb       (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-5.1/src/lp_lib.h
+-rw-r--r--   0 gleb       (501) staff       (20)    96482 2024-04-14 05:46:59.000000 pyfmtools-5.1/src/lp_matrix.c
+-rw-------   0 gleb       (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_matrix.h
+-rw-------   0 gleb       (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-5.1/src/lp_mipbb.c
+-rw-------   0 gleb       (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_mipbb.h
+-rw-r--r--   0 gleb       (501) staff       (20)    23636 2023-02-01 11:29:49.000000 pyfmtools-5.1/src/lp_params.c
+-rw-r--r--   0 gleb       (501) staff       (20)   184288 2023-02-01 11:29:56.000000 pyfmtools-5.1/src/lp_presolve.c
+-rw-------   0 gleb       (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_presolve.h
+-rw-r--r--   0 gleb       (501) staff       (20)    68814 2024-04-14 05:47:56.000000 pyfmtools-5.1/src/lp_price.c
+-rw-------   0 gleb       (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_price.h
+-rw-------   0 gleb       (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_pricePSE.c
+-rw-------   0 gleb       (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_pricePSE.h
+-rw-------   0 gleb       (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-5.1/src/lp_report.c
+-rw-------   0 gleb       (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_report.h
+-rw-------   0 gleb       (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-5.1/src/lp_rlp.h
+-rw-r--r--   0 gleb       (501) staff       (20)    29500 2024-04-14 05:49:01.000000 pyfmtools-5.1/src/lp_scale.c
+-rw-------   0 gleb       (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_scale.h
+-rw-------   0 gleb       (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-5.1/src/lp_simplex.c
+-rw-------   0 gleb       (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_simplex.h
+-rw-------   0 gleb       (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-5.1/src/lp_types.h
+-rw-r--r--   0 gleb       (501) staff       (20)    26898 2024-04-14 05:50:17.000000 pyfmtools-5.1/src/lp_utils.c
+-rw-------   0 gleb       (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_utils.h
+-rw-r--r--   0 gleb       (501) staff       (20)    11305 2024-03-24 08:48:01.000000 pyfmtools-5.1/src/lp_wlp.c
+-rw-------   0 gleb       (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lp_wlp.h
+-rw-------   0 gleb       (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-5.1/src/lpkit.h
+-rw-r--r--   0 gleb       (501) staff       (20)    21901 2024-04-14 05:51:50.000000 pyfmtools-5.1/src/lpslink56.c
+-rw-------   0 gleb       (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lpsolve.h
+-rw-r--r--   0 gleb       (501) staff       (20)    25092 2023-02-01 11:24:58.000000 pyfmtools-5.1/src/lusol.c
+-rw-------   0 gleb       (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lusol.h
+-rw-r--r--   0 gleb       (501) staff       (20)   135888 2024-04-14 06:11:02.000000 pyfmtools-5.1/src/lusol1.h
+-rw-------   0 gleb       (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lusol2.h
+-rw-r--r--   0 gleb       (501) staff       (20)    28376 2024-04-14 06:10:22.000000 pyfmtools-5.1/src/lusol6a.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4490 2024-04-14 06:09:47.000000 pyfmtools-5.1/src/lusol6l0.h
+-rw-r--r--   0 gleb       (501) staff       (20)     4891 2024-04-14 06:11:21.000000 pyfmtools-5.1/src/lusol6u.h
+-rw-------   0 gleb       (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lusol7a.h
+-rw-------   0 gleb       (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lusol8a.h
+-rw-------   0 gleb       (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-5.1/src/lusolio.c
+-rw-------   0 gleb       (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/lusolio.h
+-rw-------   0 gleb       (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-5.1/src/minimalsplus.h
+-rw-r--r--   0 gleb       (501) staff       (20)    13168 2023-02-01 11:25:41.000000 pyfmtools-5.1/src/mmio.c
+-rw-------   0 gleb       (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/mmio.h
+-rw-r--r--   0 gleb       (501) staff       (20)    19256 2024-04-14 05:52:37.000000 pyfmtools-5.1/src/myblas.c
+-rw-------   0 gleb       (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-5.1/src/myblas.h
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-09 01:15:28.079852 pyfmtools-5.1/src/pyfmtools.egg-info/
+-rw-r--r--   0 gleb       (501) staff       (20)     5355 2024-05-09 01:15:28.000000 pyfmtools-5.1/src/pyfmtools.egg-info/PKG-INFO
+-rw-r--r--   0 gleb       (501) staff       (20)     1823 2024-05-09 01:15:28.000000 pyfmtools-5.1/src/pyfmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 gleb       (501) staff       (20)        1 2024-05-09 01:15:28.000000 pyfmtools-5.1/src/pyfmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 gleb       (501) staff       (20)       12 2024-05-09 01:15:28.000000 pyfmtools-5.1/src/pyfmtools.egg-info/requires.txt
+-rw-r--r--   0 gleb       (501) staff       (20)       21 2024-05-09 01:15:28.000000 pyfmtools-5.1/src/pyfmtools.egg-info/top_level.txt
+-rw-r--r--   0 gleb       (501) staff       (20)    57619 2024-05-09 01:05:40.000000 pyfmtools-5.1/src/pyfmtools.py
+-rw-------   0 gleb       (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-5.1/src/sparselib.c
+-rw-------   0 gleb       (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/sparselib.h
+-rw-------   0 gleb       (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-5.1/src/stdafx.h
+-rw-------   0 gleb       (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-5.1/src/ufortify.h
+-rw-r--r--   0 gleb       (501) staff       (20)    95125 2024-05-09 01:10:56.000000 pyfmtools-5.1/src/wrapperpy.cpp
+-rw-r--r--   0 gleb       (501) staff       (20)    16290 2024-05-05 06:50:06.000000 pyfmtools-5.1/src/wrapperpy.h
+-rw-r--r--   0 gleb       (501) staff       (20)    28420 2023-02-01 11:30:06.000000 pyfmtools-5.1/src/yacc_read.c
+-rw-------   0 gleb       (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-5.1/src/yacc_read.h
+drwxr-xr-x   0 gleb       (501) staff       (20)        0 2024-05-09 01:15:28.079574 pyfmtools-5.1/tests/
+-rw-------   0 gleb       (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-5.1/tests/test_no_wrapper.py
+-rw-r--r--   0 gleb       (501) staff       (20)    32976 2024-05-09 01:12:08.000000 pyfmtools-5.1/tests/test_wrapper.py
```

### Comparing `pyfmtools-0.81/LICENSE.txt` & `pyfmtools-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/PKG-INFO` & `pyfmtools-5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 0.81
+Version: 5.1
 Summary: Library for handling and fitting fuzzy measures
-Home-page: UNKNOWN
+Home-page: 
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: cffi>=1.0.0
 
 # Pyfmtools    
 Pyfmtools provides various tools for handling fuzzy measures, calculating various indices, Choquet and Sugeno integrals, as well as fitting fuzzy measures to empirical data. This package is designed for Python , but it also includes the C++ source files and a user manual.
 Chapter 2 of the user manual provides some background on fuzzy measures. A more detailed overview can be found in [4, 5, 12, 16] and references therein. Chapter 3 of the user manual outlines computational methods used to fit fuzzy measures to empirical data. The description of the programming library pyfmtools is given in Chapter 4. Examples of its usage are provided in Section 4.6.
 To cite pyfmtools package, use references [2–6,21–24]. 
 ### New in version 4
 Random generation of fuzzy measures of different types, including k-additive, k-interactive, supermodular and submodular, sparse representation of k- additive fuzzy measures.<br>
@@ -149,8 +148,7 @@
 
 
 ### Test
 To unit test type:
 ```python
 $ test/test_no_wrapper.py
 ```
-
```

### Comparing `pyfmtools-0.81/README.md` & `pyfmtools-5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/setup.py` & `pyfmtools-5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup( 
     name="pyfmtools",
-    version="0.81",
+    version="5.01",
     description="Library for handling and fitting fuzzy measures",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="",
     author='Gleb Beliakov, Norbert Henseler',
     author_email='gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au',
     license_file='LICENSE.txt',
@@ -24,8 +24,8 @@
     setup_requires=['cffi>=1.0.0'],
     cffi_modules=['./src/buildPyfmtools.py:ffibuilder'],
     include_package_data=True,
     package_data={'':['tests/test_wrapper.py', 'test/test_no_wrapper.py']},
 )
 
     
-    
+
```

### Comparing `pyfmtools-0.81/src/binarylattice.h` & `pyfmtools-5.1/src/binarylattice.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/buildPyfmtools.py` & `pyfmtools-5.1/src/buildPyfmtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from cffi import FFI
 import os
 
 ffibuilder = FFI()
 PATH = os.path.dirname(__file__)
 
 ffibuilder.cdef(r"""
+    extern "Python" int(py_user_defined_measurecheck)(int*, double *);
     typedef unsigned long long int_64;
     struct  fm_env {
 	int n;
 	int m;
 	int* card;
 	int* cardpos;
 	double* bit2card;
 	double* card2bit;
 	double* factorials;};
     struct  fm_env_sparse { 
-	int xx[40];};
+	int xx[44];};
     double py_min_subset(double* x, int n, int_64 S);
     double py_max_subset(double* x, int n, int_64 S);
     void py_ConvertCard2Bit(double* dest, double* src,  struct fm_env* env);
     double py_min_subsetC(double* x, int n, int_64 S, struct fm_env* env);
     double py_max_subsetNegC(double* x, int n, int_64 S, struct fm_env* env);
     int py_SizeArraykinteractive(int n, int k, struct fm_env* env);
     int py_IsSubsetC(int i, int j, struct fm_env* env); 
@@ -55,15 +56,15 @@
     void py_fittingWAM(int datanum, struct fm_env* env, double* v, double* dataset);
     void py_Interaction(double* Mob, double* v, struct fm_env* env);
     void py_InteractionB(double* Mob, double* v, struct fm_env* env);
     void py_InteractionMob(double* Mob, double* v, struct fm_env* env);
     void py_InteractionBMob(double* Mob, double* v, struct fm_env* env);
     void py_BipartitionShapleyIndex(double* v, double* w, struct fm_env* env);
     void py_BipartitionBanzhafIndex(double* v, double* w, struct fm_env* env);
-    void py_BNonadditivityIndexMob(double* Mob, double* w, struct fm_env* env);
+    void py_NonadditivityIndexMob(double* Mob, double* w, struct fm_env* env);
     void py_NonadditivityIndex(double* v, double* w, struct fm_env* env);
 	void py_NonmodularityIndex(double* v, double* w, struct fm_env* env);
 	void py_NonmodularityIndexMob(double* Mob, double* w, struct fm_env* env);	
 	void py_NonmodularityIndexKinteractive(double* v, double* w, int kint,  struct fm_env* env);
     void py_NonmodularityIndexMobkadditive(double* Mob, double* w, int k,  struct fm_env* env);
    	void py_ShowCoalitions(int* coalition, struct fm_env* env);
 	void py_ShowCoalitionsCard(int* coalition, struct fm_env* env);
@@ -92,14 +93,15 @@
     double py_WAM(double* x, double* v, struct fm_env* env);
     void py_Zeta(double* Mob, double* v, struct fm_env* env);
 	void py_dualMobKadd(int m, int length, int k, double* src, double* dest, struct fm_env* env);
 	void py_Shapley2addMob(double* v, double* x, int n);
 	void py_Banzhaf2addMob(double* v, double* x, int n);
     double py_Choquet2addMob(double*x, double* Mob, int n);
 	int py_fm_arraysize(int n, int kint, struct fm_env* env);
+    int py_fm_arraysize_kadd(int n, int kint, struct fm_env* env);
 	int py_generate_fm_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
 	int py_generate_fmconvex_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
 	int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
 	int py_generate_fm_2additive_convex(int num, int n,  double * vv);
 	int py_generate_fm_2additive_concave(int num, int n, double * vv);
     int py_generate_fm_2additive_convex_withsomeindependent(int num, int n, double * vv);
     void py_export_maximal_chains(int n, double* v, double* mc, struct fm_env* env);
@@ -123,22 +125,41 @@
     void py_expand_sparse_full(double* v, struct fm_env_sparse* env);
 	void py_sparse_get_singletons(int n, double* v, struct fm_env_sparse* env);
 	int py_sparse_get_pairs(int* pairs, double* v, struct fm_env_sparse* env);
 	int py_sparse_get_tuples(int* tuples, double* v, struct fm_env_sparse* env);
     int   py_generate_fm_2additive_convex_sparse(int n, struct fm_env_sparse* env);
     int   py_generate_fm_kadditive_convex_sparse(int n, int k, int nonzero, struct fm_env_sparse* env);
     void py_Nonmodularityindex_sparse(double* w, int n, struct fm_env_sparse* env);
+     void py_generate_fm_sorting(int num, int n, int markov, int option, double * vv, struct fm_env* env);
+ int py_CheckMonotonicitySortMerge(double * vv, double* indices, struct fm_env* env);
+ int py_CheckMonotonicitySortInsert(double * vv, double* indices, struct fm_env* env);
+ int py_CheckMonotonicitySimple(double * vv,struct fm_env* env);
+ void py_GenerateAntibuoyant( double * vv, struct fm_env* env);
+ int py_generate_fm_belief(int num, int n, int kadd, double * vv, struct fm_env* env);
+ int py_generate_fm_balanced(int num, int n,  double * vv, struct fm_env* env);
+ int py_generate_fm_2additive(int num, int n,  double * vv);
+ int py_CheckMonMob2additive2(double * vv, int n, int length, double* temp);
+ int py_CheckMonotonicityMob(double * vv, int len, struct fm_env* env);
+ int py_CheckConvexityMonMob(double * vv, int len, struct fm_env* env);
+ void py_ConvertCoMob2KinterCall(int n, int kint, int len, double* mu, double * vv, int fullmu, struct fm_env* env);
+ double py_ChoquetCoMobKInter(double* x, double* Mob, int kadd, int len, struct fm_env* env);
+ void py_fitting2additive(int datanum, int n, int len,  double* v, double* dataset, int  options, double* indexlow, double* indexhi, int option1, double* orness);
+ int py_generate_fm_randomwalk(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+ int py_generate_fm_kinteractivedualconvex(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+ int py_generate_fm_kinteractivedualconcave(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+ int py_generate_fm_2additive_randomwalk2(int num, int n, int markov, int option, double step,  double * vv, void* extrachecks);
     """, override=True)
 
 pyfmtools_src=['src/colamd.c','src/lp_lib.c','src/lp_params.c','src/lp_simplex.c','src/lusolio.c','src/commonlib.c','src/lp_LUSOL.c','src/lp_presolve.c','src/lpslink56.c','src/mmio.c',
 	'src/ini.c','src/lp_matrix.c','src/lp_price.c','src/lp_SOS.c','src/myblas.c','src/isfixedvar.c','src/lp_MDO.c','src/lp_pricePSE.c','src/lp_utils.c','src/sparselib.c',
-	'src/lp_crash.c','src/lp_mipbb.c','src/lp_report.c','src/lp_wlp.c','src/yacc_read.c','src/lp_Hash.c','src/lp_MPS.c','src/lp_scale.c','src/lusol.c',
+	'src/lp_crash.c','src/lp_mipbb.c','src/lp_report.c','src/lp_wlp.c','src/yacc_read.c','src/lp_Hash.c','src/lp_MPS.c','src/lp_scale.c','src/lusol.c','src/gbrealloc.c',
 	'src/fmrandom.cpp','src/fuzzymeasurefit.cpp','src/wrapperpy.cpp','src/fuzzymeasurefit3.cpp','src/fuzzymeasuretools.cpp']
 
 ffibuilder.set_source("_pyfmtools",r""" #include "wrapperpy.h" """,  
     sources=pyfmtools_src,
+            extra_compile_args=["-Wno-c++11-extensions","-Wno-c++11-long-long","-Wno-unused-but-set-variable","-Wno-sign-compare","-Wno-c++11-extra-semi","-Wno-unreachable-code","-Wno-parentheses-equality","-Wno-empty-body"],
     include_dirs=[PATH],
     )
     
 
 if __name__ == "__main__":
     ffibuilder.compile(verbose=True)
```

### Comparing `pyfmtools-0.81/src/colamd.c` & `pyfmtools-5.1/src/colamd.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/colamd.h` & `pyfmtools-5.1/src/colamd.h`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 #ifdef __cplusplus
   #define __EXTERN_C extern "C"
 #else
   #define __EXTERN_C
 #endif
 */
 
+
 #ifndef __BORLANDC__
 
   #ifdef __cplusplus
     #define __EXTERN_C extern "C"
   #else
     #define __EXTERN_C
   #endif
@@ -273,14 +274,14 @@
 ) ;
 
 void symamd_report
 (
     int stats [COLAMD_STATS]
 ) ;
 
-#endif /* COLAMD_H */
+
 
 
 #ifdef __cplusplus
 }
 #endif
-
+#endif /* COLAMD_H */
```

### Comparing `pyfmtools-0.81/src/commonlib.c` & `pyfmtools-5.1/src/commonlib.c`

 * *Files 1% similar despite different names*

```diff
@@ -343,16 +343,16 @@
 
 /* Heap sort function (procedurally based on the Numerical Recipes version,
    but expanded and generalized to hande any object with the use of
    qsort-style comparison operator).  An expanded version is also implemented,
    where interchanges are reflected in a caller-initialized integer "tags" list. */
 void hpsort(void *attributes, int count, int offset, int recsize, MYBOOL descending, findCompare_func findCompare)
 {
-  register int  i, j, k, ir, order;
-  register char *hold, *base;
+   int  i, j, k, ir, order;
+   char *hold, *base;
   char          *save;
 
   if(count < 2)
     return;
   offset -= 1;
   attributes = CMP_ATTRIBUTES(offset);
   base = CMP_ATTRIBUTES(1);
@@ -405,16 +405,16 @@
   if(count < 2)
     return;
   if(tags == NULL) {
     hpsort(attributes, count, offset, recsize, descending, findCompare);
     return;
   }
   else {
-    register int  i, j, k, ir, order;
-    register char *hold, *base;
+     int  i, j, k, ir, order;
+     char *hold, *base;
     char          *save;
     int           savetag;
 
     offset -= 1;
     attributes = CMP_ATTRIBUTES(offset);
     tags += offset;
     base = CMP_ATTRIBUTES(1);
@@ -511,15 +511,15 @@
 void QS_delete(UNIONTYPE QSORTrec a[], int ipos, int epos)
 {
   for(; epos > ipos; epos--)
     a[epos] = a[epos-1];
 }
 int QS_sort(UNIONTYPE QSORTrec a[], int l, int r, findCompare_func findCompare)
 {
-  register int i, j, nmove = 0;
+   int i, j, nmove = 0;
   UNIONTYPE QSORTrec v;
 
   /* Perform the a fast QuickSort */
   if((r-l) > QS_IS_switch) {
     i = (r+l)/2;
 
     /* Tri-Median Method */
```

### Comparing `pyfmtools-0.81/src/commonlib.h` & `pyfmtools-5.1/src/commonlib.h`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,18 @@
   #define my_LoadLibrary(name)              dlopen(name, RTLD_LAZY)
   #define my_GetProcAddress(handle, name)   dlsym(handle, name)
   #define my_FreeLibrary(handle)            dlclose(handle); \
                                             handle = NULL
 #endif
 
 
+
+
+
+
 /* ************************************************************************ */
 /* Define sizes of standard number types                                    */
 /* ************************************************************************ */
 #ifndef LLONG
   #if defined __BORLANDC__
     #define LLONG __int64
   #elif !defined _MSC_VER || _MSC_VER >= 1310
```

### Comparing `pyfmtools-0.81/src/fmrandom.cpp` & `pyfmtools-5.1/src/fmrandom.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,37 @@
 
 #define NO_R
 
 using namespace std;
 
 
 
+#ifndef NO_R
+unif_R_class<double> distribution(0.0, 1.0);
+#else
+std::uniform_real_distribution<> distribution(0.0, 1.0);
+#endif
+
+
 
-std::uniform_real_distribution<double> distribution(0.0, 1.0);
 
 
 
 random_device rd;
 mt19937 rng(rd());    // random-number engine used (Mersenne-Twister in this case)
 
 
-
+/*
 template <class T> struct prec : binary_function <T, T, bool> {
 	bool operator() (const T& x, const T& y) const { return x < y; }
 };
 template <class T> struct succ : binary_function <T, T, bool> {
 	bool operator() (const T& x, const T& y) const { return x < y; }
 };
+*/
 // These definitions can be changed to support other data types. They sin in the .h file
 
 //typedef uint16_t myint;
 //typedef unsigned int myint;
 //typedef int_64 myint;
 //typedef unsigned int uint;
 //typedef float  myfloat;
@@ -409,14 +416,23 @@
 	// count the number of items as the sum of Cin
 	int r = 1; // for emptyset
 	for (int i = 1;i <= k; i++)
 		r += (int)(choose(i, n));
 	return r;
 }
 
+
+int fm_arraysize_2add(int n)
+{
+	// calculates the number of parameers needed in cardinal representation for 2-additive capacity
+	// no 0 included !!!
+	return (int)(choose(2, n)) + n;
+}
+
+
 myfloat fm_delta(int m, int kint, myfloat K)
 {  // delta is the fixed marginal contribution in the k-interactive fuzzy measures
 //	if (m == (kint + 1)) return (myfloat)(1.0 - K);
 	if (m <= kint + 1) return 0;
 	return (myfloat)(1.0 - K) / (m - kint - 1);
 }
 
@@ -650,15 +666,15 @@
 	vector<myint>  v1, v2, v0(length);
 
 	string s5, s6;
 
 	std::vector<BYTE> decodedData1;
 
 
-	int NN = 0;
+    int NN=0;
 	myint i, j1, j;
 	double Wei, WeiS, p, u;
 	Edge E;
 	vector<Edge> edges;
 
 	for (i = 0;i < length;i++) v1.push_back((myint)card2bit[i + 1]);
 
@@ -830,15 +846,15 @@
 	if (opt1 == 1 && length*num < 20 * 200000) dorejection = 1;
 
 	vector<myint>  v1, v2, v0(length);
 
 	string s5, s6;
 	std::vector<BYTE> decodedData1;
 	
-	int NN = 0;
+    int NN=0;
 	myint i, j1, j;
 	double Wei, WeiS, p, u;
 	Edge E;
 	vector<Edge> edges;
 
 	for (i = 0;i < length;i++) v1.push_back((myint)card2bit[i + 1]);
 
@@ -1037,7 +1053,13 @@
 		}
 		// reshuffle
 		// is it guaranteed no repeats?
 		//std::shuffle(std::begin(temp), std::end(temp), rng);
 		std::next_permutation(temp.begin(), temp.end());
 	}
 }
+
+
+
+
+
+#include "fmrandomsort.inc"
```

### Comparing `pyfmtools-0.81/src/fortify.h` & `pyfmtools-5.1/src/fortify.h`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # define signed
 #endif
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
+
+
 #ifdef FORTIFY
 
 typedef void (*OutputFuncPtr) __OF((char *));
 
 extern char *_Fortify_file;
 extern int _Fortify_line;
```

### Comparing `pyfmtools-0.81/src/fuzzymeasurefit.cpp` & `pyfmtools-5.1/src/fuzzymeasurefit.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -40,29 +40,31 @@
 
 
 
 #include <cstdio>
 #include <cstdlib>
 #include <iostream>
 #include <fstream>
-using namespace std;
+
 #include <cmath>
 #include <algorithm>
 
 
 
 
-using namespace std;
+
 //#include <R.h>
 // note that programs using this code should be linked against lp_solve library,
 // which should be downloaded and installed separatly. These references are only
 // to the readers of that library.
-
-#include "fuzzymeasuretools.h"
 #include "lp_lib.h"
+#include "fuzzymeasuretools.h"
+
+
+
 
 struct Less_than {
 	int operator()(const valindex& a, const valindex& b) { return a.v < b.v; }
 };
 struct Greater_than {
 	int operator()(const valindex& a, const valindex& b) { return a.v > b.v; }
 };
@@ -76,15 +78,15 @@
 			double* indexlow, double* indexhigh, int option1, double* orness )
 // K for data, Kadd for k-additive f.m.
 // indexlow, indexhigh are 0-based for Shapley values (contain only singletos
 // but are 1-based and in cardinality ordering (like the f.m. themselves, the first element = emptyset) 
 // when they contain all  m values of all interaction indices
 {
 
-	  int counter = 0;
+  int counter = 0;
   int i,j,k,k1,res,i1;
   int result;
   int_64 A, B, C;
   lprec		*MyLP;
   int RowsR,RowsC, RowsC1;
 
   valindex *tempyk;
@@ -1706,10 +1708,146 @@
 
 	free(sol);
 	delete_lp(MyLP);
 //	fclose(on);
 	return result;
 }
 
+#define Infty 10e20
+
+int	LinearFunctionFitLP(int n,  int K, double *v, double* XYData, int options)
+// simple linear function with positive coefs and constant term unrestricted
+
+{
+  int i,k,res;
+  int result;
+
+  lprec		*MyLP;
+  int RowsR,RowsC, RowsC1;
+
+  //valindex *tempyk;
+  //double temp;
+
+
+
+// calculate how many rows/columns we need
+
+  RowsC1	= 1; // this is vertical shift term
+  RowsR=K*2; RowsC = n + RowsC1*2;
+
+//cout<<"inside fmtools"<<endl;
+//cout<< RowsR<<" "<<RowsC<<endl;
+
+  MyLP = make_lp( RowsR+RowsC, 0);
+  
+//cout<<"inside fmtools lpsolve "<<endl;
 
+  MyLP->do_presolve=FALSE;   
+  set_verbose(MyLP,3);
+  int itemp = RowsC+2 +1; // just the max number of entries per column
+
+
+
+  double *row;
+  int	 *rowno;
+  row=new double[itemp];
+  rowno=new int[itemp];
+//  int re;
+
+// the first K columns
+  rowno[0]=0;
+  for(k=0;k<K; k++) { 
+	    //rowno[0] is the obj. function
+	    row[0] = XYData [k*(n+1)+n ];//y[k]; //
+		rowno[1]=k+1;  // 1-based
+		rowno[2]=k+1+ K;
+		row[1]=-1; 
+		row[2]= 1;
+// now the vales of h_A
+
+		for(i=0;i<n;i++) { (tempxi[i]).v=XYData[k*(n+1)+i]; (tempxi[i]).i=i;}
+		
+			for(i=0;i<n;i++) {// singletons
+				row[2+i+1]=    tempxi[i].v;
+				rowno[2+i+1] = RowsR +i +1;
+			}
+
+// two more (plus and minus)
+        row[2+n+1]=1;
+        rowno[2+n+1] =RowsR +n +1;
+        row[2+n+1+1]=-1;
+        rowno[2+n+1+1] =RowsR +n +1+1;
+        
+                
+		add_columnex(MyLP, itemp, row, rowno);
+
+// now repeat everything, just change the sign
+		for(i=0;i<itemp;i++) row[i]=-row[i];
+
+		add_columnex(MyLP, itemp, row, rowno);
+  }
+
+
+	int RR=get_Nrows(MyLP);
+	int CC=get_Ncolumns(MyLP);
+	for(i=1;i<=RR;i++) {
+		set_rh(MyLP,i, 0 ); 
+		set_constr_type(MyLP,i,LE);
+
+	}
+	for(i=1;i<=CC;i++) {
+		set_bounds(MyLP, i, 0.0, Infty);
+	}
+
+	for(i=1;i<=RowsR;i++) {
+		set_rh(MyLP,i, Infty ); 
+	}
+
+	set_maxim(MyLP); // well, we always do that
+
+
+
+	double *sol=(double*)malloc(sizeof(double)*(1 + RR + CC));
+
+//	 write_lp(MyLP, "model.lp");
+//	cout<<"finished building LP "<< RR<< " " <<CC<<endl;
+//	set_outputfile(MyLP, "log.txt");
+//	print_lp(MyLP);
+
+  set_verbose(MyLP,0);
+
+	res=solve(MyLP);
+//	double minval,rp,rm;
+
+	if(res==OPTIMAL) {
+//		temp=0;
+		get_dual_solution(MyLP, sol);
+
+		//minval = get_objective(MyLP) ;  // minimum
+
+		for(i=1;i<=K;i++)
+		{
+		//	rp= sol[i]; // residuals
+		//	rm= sol[i+K];
+//			temp += (rp+rm);
+		}
+//cout<<" min value "<<minval<<" "<<temp<<endl;
+
+
+		for(i=1; i<=n + 1; i++)
+		{
+			v[i-1]= sol[i+RowsR]; // singletons and shift
+		}
+		v[n]-=sol[n+2+RowsR];// negative part
+		
+		result=1;
+	} // no optimal
+	else result=0;
+
+	delete[] row;
+	delete[] rowno;
+	free (sol);
+	delete_lp(MyLP);
+	return result;
+}
 
 //#include "fuzzymeasurefit3.cpp"
```

### Comparing `pyfmtools-0.81/src/fuzzymeasurefit.h` & `pyfmtools-5.1/src/fuzzymeasurefit.h`

 * *Files 2% similar despite different names*

```diff
@@ -198,7 +198,13 @@
 LIBDLL_API int	FuzzyMeasureFitLPKinteractiveMarginalMaxChain(int n, int_64 m, int K, int Kadd, double *v, double* XYData, int options,
 	double* indexlow, double* indexhigh, int option1, double* orness, double KConst);
 
 LIBDLL_API int	FuzzyMeasureFitLPKinteractiveAutoK(int n, int_64 m, int K, int Kadd, double *v, double* XYData, int options,
 	double* indexlow, double* indexhigh, int option1, double* orness, double* KConst, int maxiter);
 
 LIBDLL_API int testmap(int n, int m);
+
+LIBDLL_API int FuzzyMeasureFit2additive(int n, int datanum, int length,
+	int options, double* indexlow, double* indexhigh, int option1, double* orness, double* Mob, double* XYData);
+	
+LIBDLL_API 	int	LinearFunctionFitLP(int n,  int K, double *v, double* XYData, int options);
+
```

### Comparing `pyfmtools-0.81/src/fuzzymeasurefit3.cpp` & `pyfmtools-5.1/src/fuzzymeasurefit3.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
 
 
 #include <cstdio>
 #include <cstdlib>
 #include <iostream>
 #include <fstream>
-using namespace std;
+
 #include <cmath>
 #include <algorithm>
 
 
 
 #include <map>
 #include <set>
 #include <unordered_set>
 #include <iterator>
 #include<vector>
 
-using namespace std;
+
 //#include <R.h>
 // note that programs using this code should be linked against lp_solve library,
 // which should be downloaded and installed separatly. These references are only
 // to the readers of that library.
-
+#include "lp_lib.h"
 #include "fuzzymeasuretools.h"
 #include "fuzzymeasurefit.h"
-#include "lp_lib.h"
 
 
+using namespace std;
 template <class ForwardIterator, class T>
 void myiota(ForwardIterator first, ForwardIterator last, T val)
 {
 	while (first != last) {
 		*first = val;
 		++first;
 		++val;
@@ -51,48 +51,48 @@
 
 
 #define mtokey(a,b)( (a)|(int_64(b)<<56))
 #define setfromkey(a) ((a)& 0x00FFFFFFFFFFFFFF)
 #define varfromkey(a) (((a)>>56)& 0xFF)
 
 
-#ifndef byte
-typedef unsigned char  byte;
+#ifndef mybyte
+typedef unsigned char  mybyte;
 #endif
 
 struct arrayindex {
-	byte* v;
+	mybyte* v;
 };
 
 
 class greaterindex {
 public:
-	const  byte* container;
+	const  mybyte* container;
 	  int  N=0;
 
-	  greaterindex(const byte* incontainer, const int n) { container = incontainer; N = n; };
+	  greaterindex(const mybyte* incontainer, const int n) { container = incontainer; N = n; };
 	  bool operator() (const int& a, const int& b);
 
 };
 bool greaterindex:: operator() (const int& a, const int& b) {
 	for (int i = 0; i < N; i++)
 	if (container[a + i] == container[b + i]);
 	else if (container[a + i] > container[b + i])
 		return 1; else return 0;
 	return 0;
 }
 
 typedef map<int_64, int> Mymap;
 //typedef set<int, greaterindex <int*> > Myset;
 
-byte string2number(string& s, byte i) { return (byte)s[i] - 1; }
-void number2string(string& s, byte i, byte n) { s[i] = n + 1; }
+mybyte string2number(string& s, mybyte i) { return (mybyte)s[i] - 1; }
+void number2string(string& s, mybyte i, mybyte n) { s[i] = n + 1; }
 
-void Setinsert(int_64& S, string St, byte pos){ AddToSet(&S, string2number(St, pos)); }
-void Setremove(int_64& S, string St, byte pos){ RemoveFromSet(&S, string2number(St, pos)); }
+void Setinsert(int_64& S, string St, mybyte pos){ AddToSet(&S, string2number(St, pos)); }
+void Setremove(int_64& S, string St, mybyte pos){ RemoveFromSet(&S, string2number(St, pos)); }
 void CodeMaxChain(int* chain, string & S, int n){
 	for (int i = 0; i < n; i++)
 		number2string(S, i, chain[i]);
 }
 
 
 
@@ -1825,10 +1825,437 @@
 	free(sol);
 	delete_lp(MyLP);
 	delete_lp(MyLPSave);
 	return result;
 }
 
 
+struct Less_than0 {
+	int operator()(const valindex& a, const valindex& b) { return a.v < b.v; }
+};
+Less_than0 less_than0;
+
+LIBDLL_API int FuzzyMeasureFit2additive(int n, int datanum, int length, 
+	int options, double* indexlow, double* indexhigh, int option1, double* orness, double* Mob, double* XYData)
+{
+	//	int	FuzzyMeasureFitLP(int n, int_64 m, int K, int Kadd, double* v, double* XYData, int options,
+	//		double* indexlow, double* indexhigh, int option1, double* orness)
+			// K for data, Kadd for k-additive f.m.
+			// indexlow, indexhigh are 0-based for Shapley values (contain only singletos
+			// but are 1-based and in cardinality ordering (like the f.m. themselves, the first element = emptyset) 
+			// when they contain all  m values of all interaction indices
+
+
+	int counter = 0;
+	int i, j, k, res, i1;
+	int result;
+
+	lprec* MyLP;
+	int RowsR, RowsC, RowsC1;
+
+	valindex* tempyk;
+	// double temp;
+
+   // calculate how many rows/columns we need
+	int K = datanum;
+	RowsC1 = length - n; //how many non-singletons
+	RowsR = K * 2; RowsC = n + RowsC1 * 2;
+	//+ve and -ve
+
+
+	MyLP = make_lp(0, RowsR + RowsC);
+	set_add_rowmode(MyLP, TRUE);
+
+	//MyLP = make_lp(RowsR + RowsC+1, 0);
+	//  MyLP->do_presolve=FALSE;   
+	set_verbose(MyLP, 3);
+
+	int itemp = RowsR + RowsC + 1; // just the max number of entries per row
+
+	double* row;
+	int* rowno;
+	row = new double[itemp];
+	rowno = new int[itemp];
+
+
+	for (i = 1; i <= RowsR; i++) {
+		set_obj(MyLP, i, 1.0);
+	}
+
+	for (k = 0; k < ( int)K; k++) {
+		rowno[1] = k + 1;  // 1-based
+		rowno[2] = k + 1 + K;
+		row[1] = -1; //+
+		row[2] = 1;  //-
+		row[0] = XYData[k * (n + 1) + n]; // rhs
+        
+		// singletons
+
+		for (i = 0; i < n; i++) {// singletons
+			row[2 + i + 1] = XYData[k * (n + 1) + i];
+			rowno[2 + i + 1] = RowsR + i + 1;
+            
+		}
+        
+		// pairs
+		int t = 2 + n;
+		for (i = 0; i < n; i++)
+			for (j = i + 1; j < n; j++) {
+				rowno[t  + 1] = RowsR + t - 1;  // rowsR+n+1+index
+				row[t  + 1] = min(XYData[k * (n + 1) + i], XYData[k * (n + 1) + j]);
+
+				rowno[t  + 1 + RowsC1] = RowsR + t - 1 + RowsC1;  // rowsR+n+1+index
+				row[t  + 1 + RowsC1] = -row[t + 1];
+				t++;
+			}
+
+		add_constraintex(MyLP, RowsC + 2, row + 1, rowno + 1, EQ, row[0]);
+
+
+		counter += RowsC + 2;
+	}
+	// finished data
+
+	// monotonicity
+	row[0] = 0;
+	for (i = 0; i < n; i++) {
+		row[1] = 1;
+		rowno[1] = RowsR + i + 1;
+		int t = 1;
+		int s = 1;
+		for (k = 0; k < n; k++) // pair k,j
+			for (j = k + 1; j < n; j++) {
+				if (k == i || j == i) {
+                    s++;
+					row[s] = 1;
+					rowno[s] = t + n + RowsC1 + RowsR;  // negative pair in order
+				}
+				t++;
+			}
+		// I have s entries now
+		add_constraintex(MyLP, s, row + 1, rowno + 1, GE, row[0]);
+	}
+
+	// last one all values  add to one 
+	for (i = 0; i < RowsC; i++) {
+		row[i + 1] = 1;
+		rowno[i + 1] = i + RowsR + 1;
+	}
+	row[0] = 1;
+	add_constraintex(MyLP, RowsC, row + 1, rowno + 1, EQ, row[0]);
+
+
+
+
+
+	// add interaction indices if needed
+
+	switch (options) {
+	case 0: break; // no indices supplied
+	case 3: // both shapley bounds supplied
+	case 1: // shapley lower bounds supplied 
+		if (indexlow != NULL)
+			for (i = 0; i < n; i++) if (indexlow[i] > 0) {
+				row[0] = indexlow[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = RowsR + i + 1; // singleton
+
+
+				int t = 1;
+				int s = 1;
+				for (k = 0; k < n; k++) // pair k,j
+					for (j = k + 1; j < n; j++) {
+						if (k == i || j == i) {
+							row[s + 1] = 0.5;
+							rowno[s + 1] = t + n + RowsR;  // positive pair in order
+							s++;
+							row[s + 1] = -0.5;
+							rowno[s + 1] = t + n + RowsC1 + RowsR;  // negative pair in order
+							s++;
+						}
+						t++;
+					}
+				// I have s entries now
+				add_constraintex(MyLP, s, row + 1, rowno + 1, GE, row[0]);
+			}
+
+		if (options == 1) break;
+	case 2: // shapley upper bounds supplied // almost the same as above, but change of sign
+		if (indexhigh != NULL)
+			for (i = 0; i < n; i++) if (indexhigh[i] < 1) {
+				row[0] = indexhigh[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = RowsR + i + 1; // singleton
+
+				int t = 1;
+				int s = 1;
+				for (k = 0; k < n; k++) // pair k,j
+					for (j = k + 1; j < n; j++) {
+						if (k == i || j == i) {
+							row[s + 1] = 0.5;
+							rowno[s + 1] = t + n + RowsR;  // positive pair in order
+							s++;
+							row[s + 1] = -0.5;
+							rowno[s + 1] = t + n + RowsC1 + RowsR;  // negative pair in order
+							s++;
+						}
+						t++;
+					}
+				// I have s entries now
+				add_constraintex(MyLP, s, row + 1, rowno + 1, LE, row[0]);
+			}
+
+		break;
+
+	case 6: // all  bounds on interaction indices 
+	case 4: // all lower bounds on interaction indices 
+		if (indexlow != NULL) {
+
+			// singletons
+			for (i = 0; i < n; i++) if (indexlow[i] > 0) {
+				row[0] = indexlow[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = RowsR + i + 1; // singleton
+
+
+				int t = 1;
+				int s = 1;
+				for (k = 0; k < n; k++) // pair k,j
+					for (j = k + 1; j < n; j++) {
+						if (k == i || j == i) {
+							row[s + 1] = 0.5;
+							rowno[s + 1] = t + n + RowsR;  // positive pair in order
+							s++;
+							row[s + 1] = -0.5;
+							rowno[s + 1] = t + n + RowsC1 + RowsR;  // negative pair in order
+							s++;
+						}
+						t++;
+					}
+				// I have s entries now
+				add_constraintex(MyLP, s, row + 1, rowno + 1, GE, row[0]);
+			}
+			// pairs
+
+			for (i = n; i < RowsC1; i++) if (indexlow[i] > 0) {
+				row[0] = indexlow[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = 1 + n + RowsR;
+				row[2] = -1;
+				rowno[2] = 1 + n + RowsR + RowsC1;
+
+				// I have 2 entries now
+				add_constraintex(MyLP, 2, row + 1, rowno + 1, GE, row[0]);
+			}
+		}
+
+		if (options == 4) break;
+	case 5: // all upper bounds on interaction indices  // almost the same as above 
+		if (indexhigh != NULL)
+		{ // singletons
+			for (i = 0; i < n; i++) if (indexhigh[i] < 1) {
+				row[0] = indexhigh[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = RowsR + i + 1; // singleton
+
+				int t = 1;
+				int s = 1;
+				for (k = 0; k < n; k++) // pair k,j
+					for (j = k + 1; j < n; j++) {
+						if (k == i || j == i) {
+							row[s + 1] = 0.5;
+							rowno[s + 1] = t + n + RowsR;  // positive pair in order
+							s++;
+							row[s + 1] = -0.5;
+							rowno[s + 1] = t + n + RowsC1 + RowsR;  // negative pair in order
+							s++;
+						}
+						t++;
+					}
+				// I have s entries now
+				add_constraintex(MyLP, s, row + 1, rowno + 1, LE, row[0]);
+			}
+
+			for (i = n; i < RowsC1; i++) if (indexhigh[i] < 1) {
+				row[0] = indexhigh[i];
+				rowno[0] = 0;
+				row[1] = 1;
+				rowno[1] = 1 + n + RowsR;
+				row[2] = -1;
+				rowno[2] = 1 + n + RowsR + RowsC1;
+
+				// I have 2 entries now
+				add_constraintex(MyLP, 2, row + 1, rowno + 1, LE, row[0]);
+			}
+		}
+
+		break;
+	}
+
+	// additional options:
+	// bit 1 = specified orness value
+	// bit 2 = add condition that f.m. is balanced
+	// bit 3 = add condition of preservation of output orderings
+	double wei = 1.;
+	if ((option1 & 0x1) == 0x1) { // orness specified orness[0]=lower bound, orness[1]=upper bound
+		if (orness[0] > 0) {
+			row[0] = orness[0] * wei; rowno[0] = 0; k = 1;
+
+			for (i = 0; i < n; i++) {// singletons
+				row[i + 1] = wei / 2.;
+				rowno[i + 1] = RowsR + i + 1;
+			}
+			int t = n + 1;
+			for (i = 0; i < n; i++)
+				for (j = i + 1; j < n; j++) {
+					rowno[t] = RowsR + t;  // rowsR+n+1+index
+					row[t] = wei * (n - 2.) / 3. / (n - 1.);
+
+					rowno[t + RowsC1] = RowsR + t + RowsC1;  // rowsR+n+1+index
+					row[t + RowsC1] = -row[t];
+                    t++;
+				}
+
+			add_constraintex(MyLP, RowsC, row + 1, rowno + 1, GE, row[0]);
+
+		}
+
+		// upper bound
+		if (orness[1] < 1) {
+			row[0] = orness[1] * wei; rowno[0] = 0; k = 1;
+
+			for (i = 0; i < n; i++) {// singletons
+				row[i + 1] = wei / 2.;
+				rowno[i + 1] = RowsR + i + 1;
+			}
+			int t = n + 1;
+			for (i = 0; i < n; i++)
+				for (j = i + 1; j < n; j++) {
+					rowno[t] = RowsR + t;  // rowsR+n+1+index
+					row[t] = wei * (n - 2.) / 3. / (n - 1.);
+
+					rowno[t + RowsC1] = RowsR + t + RowsC1;  // rowsR+n+1+index
+					row[t + RowsC1] = -row[t];
+                    t++;
+				}
+
+			add_constraintex(MyLP, RowsC, row + 1, rowno + 1, LE, row[0]);
+		}
+	} // orness
+
+	if ((option1 & 0x2) == 0x2) { // balanced. Means there plenty of conditions of the same type as monotonicity constraints, but more of those
+		// this is not yet implemented, reserved for future use
+	}
+	if ((option1 & 0x4) == 0x4) { // presevation of output orderings. to reduce the number of conditions, sort the outputs in increasing order
+		tempyk = new valindex[K];
+
+		for (k = 0; k < K; k++) { (tempyk[k]).v = XYData[k * (n + 1) + n]; (tempyk[k]).i = k; }
+		sort(&(tempyk[0]), &(tempyk[K]), less_than0); // sorted in increasing order
+
+
+		for (int ii = 0; ii < K - 1; ii++) {
+			i = (tempyk[ii]).i;
+			j = (tempyk[ii + 1]).i;// so the constraint involves j-th and i-th data
+			rowno[0] = 0; row[0] = 0; k = 1;
+
+			for (int k1 = 0; k1 < n; k1++) {// singletons
+				row[k] = XYData[j * (n + 1) + k1] - XYData[i * (n + 1) + k1];
+				rowno[k] = RowsR + k;
+				k++;
+			}
+			// pairs
+
+			for (i1 = 0; i1 < n; i1++)
+				for (int j1 = i1 + 1; j1 < n; j1++) {
+					rowno[k] = RowsR + k;  // rowsR+n+1+index
+					row[k] = min(XYData[j * (n + 1) + i1], XYData[j * (n + 1) + j1]) - min(XYData[i * (n + 1) + i1], XYData[i * (n + 1) + j1]);
+
+					rowno[k + RowsC1] = rowno[k] + RowsC1;  // rowsR+n+1+index
+					row[k + RowsC1] = -row[k];
+					k++;
+				}
+
+			add_constraintex(MyLP, k + RowsC1, row + 1, rowno + 1, GE, row[0]);
+
+		}
+		delete[] tempyk;
+	}
+
+	set_add_rowmode(MyLP, FALSE);// why?
+	int RR = get_Nrows(MyLP);
+	int CC = get_Ncolumns(MyLP);
+    
+    
+    // here in fact we can only use singletons as bound constraints, if this is the variables, so can be residuals and singletons but not pairs. todo: experiment with speed
+	for (i = 1; i <= CC; i++) {
+		set_bounds(MyLP, i, 0.0, 1.0);
+	}
+	// including the residuals on the chosen interval of values
+
+	set_minim(MyLP); // well, we always do that
+
+
+   // cout<<"before LP"<<RR<<" "<<CC<<endl;
+
+	double* sol = (double*)malloc(sizeof(double) * (1 + RR + CC));
+
+	//	 write_lp(MyLP, "model.lp");
+	//	cout<<"finished building LP "<< RR<< " " <<CC<<endl;
+	//	set_outputfile(MyLP, "log.txt");
+	//	print_lp(MyLP);
+	//	cout << n << "\t" << K << "\t" << Kadd << "\t" << RR << "\t" << CC  << "\t"<<counter<<endl;
+
+	set_verbose(MyLP, 0);
+
+
+	res = solve(MyLP);
+	double minval = 10e10;
+ 
+	if (res == OPTIMAL) {
+		//		temp=0;
+		get_primal_solution(MyLP, sol); // dual???
+
+		minval = get_objective(MyLP);  // minimum
+
+		for (i = 1; i <= K; i++)
+		{
+			//rp= sol[i]; // residuals
+			//rm= sol[i+K];
+//			//temp += (rp+rm);
+		}
+		//cout<<" min value "<<minval<<" "<<temp<<endl;
+
+
+
+		for (i = 1; i <= n; i++)
+		{
+			Mob[i - 1] = sol[i + RowsR + RR]; // singletons
+		}
+		for (i = 0; i < RowsC1; i++)
+		{
+			Mob[i + n] = sol[n + RowsR + RR + 1 + i] - sol[n + RowsR + RR + 1 + RowsC1 + i]; //pairs, in m+-m-
+		}
+
+		result = 1;
+	} // no optimal
+	else result = 0;
+
+	// just to cheat the compiler
+	minval = minval + 1;
+	delete[] row;
+	delete[] rowno;
+
+
+	free(sol);
+	delete_lp(MyLP);
+   // std::cout<<result<<std::endl;
+	return result;
+
+}
```

### Comparing `pyfmtools-0.81/src/fuzzymeasuretools.bak.cpp` & `pyfmtools-5.1/src/fuzzymeasuretools.bak.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/fuzzymeasuretools.bak.h` & `pyfmtools-5.1/src/fuzzymeasuretools.bak.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/fuzzymeasuretools.cpp` & `pyfmtools-5.1/src/fuzzymeasuretools.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,14 @@
 #include <fstream>
 #include <cmath>
 #include <algorithm>
 #include <ctime>
 #include<random>
 #include <numeric>
 
-#define MEMCHK
-// GB: this makes extra checks for sparse structures, not to go out of bounds, but at the cost of some losses in speed
-// comment out if certain not to go out of bounds and speed is an issue
 
 clock_t clockS, clockF;
 double TotalTime;
 void   ResetTime() { TotalTime = 0; clockS = clock(); }
 
 double ElapsedTime()
 {
@@ -122,14 +119,18 @@
  int_64 choose(int i, int n)
 {
 	if (i == 1) return n;
 	if (i == 2) return (int_64)(n*(n - 1)) / 2;
 	if (i == 3) return (int_64)(n*(n - 1)*(n - 2)) / 6;
 	if (i == 4) return (int_64)(n*(n - 1)*(n - 2)*(n-3)) / 24;
 	if (i == 5) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n-4)) / 120;
+	if (i == 6) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n-5)) / 120/6;
+	if (i == 7) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n-5)*(n-6)) / 120/42;
+	if (i == 8) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)*(n - 6)*(n-7)) / 120/42/8;
+	if (i == 9) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)*(n - 6)*(n - 7)*(n-8)) / 120/42/72;
 
 	return (int_64)(m_factorials[n] / m_factorials[i] / m_factorials[n - i]);
 }
 
 double ChooseInverse(int n, int a, int b) { return m_factorials[b] * m_factorials[n - a - b] / m_factorials[n - a]; }
 
 double minf(double a, double b) {if (a<b) return a; else return b;}
@@ -165,58 +166,54 @@
 #  define __builtin_popcountl  __popcnt  //_mm_popcnt_u64
 inline unsigned int bitweight(int_64 i) {
 	return __builtin_popcountl((uint32_t)(i >> 32)) + __builtin_popcountl((uint32_t)i);
 }
 #endif
 
 #else 
-//#ifndef CHAR_BIT
-//#define CHAR_BIT 8
-//#endif	
-
 uint bitweight(int_64 v) {
 	v = v - ((v >> 1) & (int_64)~(int_64)0 / 3);                           // temp
 	v = (v & (int_64)~(int_64)0 / 15 * 3) + ((v >> 2) & (int_64)~(int_64)0 / 15 * 3);      // temp
 	v = (v + (v >> 4)) & (int_64)~(int_64)0 / 255 * 15;                      // temp
-	unsigned int c = (int_64)(v * ((int_64)~(int_64)0 / 255)) >> (sizeof(int_64) - 1) * 8 ; // count  CHAR_BIT
+	unsigned int c = (int_64)(v * ((int_64)~(int_64)0 / 255)) >> (sizeof(int_64) - 1) * CHAR_BIT; // count
 	return (unsigned int)c;
 }
 //#endif
 /*
 unsigned int bitweight(unsigned int i)
 {
 	 i = i - ((i >> 1) & 0x55555555);
 	 i = (i & 0x33333333) + ((i >> 2) & 0x33333333);
 	 return (((i + (i >> 4)) & 0x0F0F0F0F) * 0x01010101) >> 24;
 }*/
 #endif
 
-int_64 UnivSetTable[20] = { 0, 1, 3, 7, 15, 31, 63, 127, 255,511,1023,2047,4095,8191,16383,32767,65535,131071,262143, 524287};
+int_64 UnivSetTable[20] = { 0, 1, 3, 7, 15, 31, 63, 127, 255,511,1023,2047,4095,8191,16383,32767,65535,131071,262143 };
 //int_64 UnivSetTable[7] = { 0, 1, 3, 7, 15, 31, 63};
 
 
 double xlogx(double t) { if(t<GBtolerance) return 0; else return t*log(t);} 
 
 void RemoveFromSet(int_64* A, int i) { *A &= (~(int_64(1) << i)); }
 void AddToSet(int_64* A, int i) { *A |= (int_64(1) << i); }
-int  IsInSet(int_64 A, int i) { return int((A >> i) & 0x1); }  // 0-based i
+int  IsInSet(int_64 A, int i) { return int((A >> i) & 0x1); }
 int  IsSubset(int_64 A, int_64 B) { return ((A & B) == B); } //
 int_64 Setunion(int_64 A, int_64 B) { return (A | B); }
 int_64 Setintersection(int_64 A, int_64 B) { return (A & B); }
 int_64 Setdiff(int_64 A, int_64 B) { return (A & ~(A & B)); }
 
 int Removei_th_bitFromSet(int_64* A, int i) { int_64 B = (*A) & (~(int_64(1) << i)); 
                           if (B == *A) return 1; else *A = B; return 0; 
 }
 
 int_64 UniversalSet(int n) {
 	int_64 A = UnivSetTable[min(n, 19)];
 	while (n > 19)  {AddToSet(&A, --n);}
 	return A;
-}
+};
 
 // Additions to version 4
 int_64 remove1bit(int_64 a, int i)
 // counting fom 0
 {
 	int_64 b = 1;
 	b = b << i;
@@ -1407,22 +1404,31 @@
 
 double Choquet2add(double*x, double* Mob, int n)
 /* This is a calculation of the Choquet integral from the Moebius transform for 2-additive capacities.
 */
 {
 	double val = 0;
 	// the formula is singleton + all pairs/2
-	int start = n;
 	for (int i = 0;i < n; i++) {
 		val+= Mob[i]*x[i];  // singleton
-		for (int j = i + 1;j < n;j++) {
-			val += Mob[start] * minf(x[i], x[j]) ;  // pair
-			start++;
-		}
 
+		int start = n; int step = n; int row = 0;
+		start += (i - 1); if (start < n) start = n; // special case i==0
+		if (i > 0) step = n - 1;
+		for (int j = 1;j < n;j++) {
+			val  +=  Mob[start] * minf(x[i], x[j]) *0.5;  // pair
+//			cout << start << " ";
+			if (row < i) {
+				step -= 1;  row++; if (row == i) start++;
+			}// row not reached
+			else {
+				step = 1;  row++;
+			}// rest of the row
+			start += step;
+		}
 	}
 	return val;
 }
 /* ====================== Sparse FM in Mobius representation ==================================*/
 
 //#define FM_SPARSE
 #ifdef FM_SPARSE
@@ -1449,102 +1455,102 @@
 	vector<uint16_t> m_tuple_content;  // for any j such that m_tules[j] is the value, m_tuple_content[m_tuple_start[j]] is the cardinality
 };
 */
 // just the preparation, no content yet
 // takes as the argument the list of indices with cardinalities, (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
 void Prepare_FM_sparse(int n, int tupsize, int* tuples, struct SparseFM* cap)
 {
-	cap->n=n;
-	cap->m_singletons.resize(n);
-	cap->m_pairs.reserve(10);
-	cap->m_pair_index.reserve(10);
-	cap->m_tuple_content.reserve(10);
-	cap->m_tuple_start.reserve(10);
-	cap->m_tuples.reserve(10);
-
-	int i = 0;
-	while (i < tupsize)
-	{
-		int card = tuples[i];
-		if (card == 2)//pair, make them ordered
-		{
-			cap->m_pairs.push_back(0.0);
-			i++;
-			int t1 = tuples[i];
-			i++;
-			int t2 = tuples[i];
-			i++;
-			cap->m_pair_index.push_back(min(t1, t2));
-			cap->m_pair_index.push_back(max(t1, t2));
-		}
-		else // card>2
-		{
-			cap->m_tuple_content.push_back(card);
-			cap->m_tuples.push_back(0.0);
-//			cap->m_tuple_content.push_back(card);
-			cap->m_tuple_start.push_back((int) cap->m_tuple_content.size() - 1);
-			i++;
-			for (int j = 0;j < card;j++) {
-				cap->m_tuple_content.push_back(tuples[i]);
-				i++;
-			}
+    cap->n=n;
+    cap->m_singletons.resize(n);
+    cap->m_pairs.reserve(10);
+    cap->m_pair_index.reserve(10);
+    cap->m_tuple_content.reserve(10);
+    cap->m_tuple_start.reserve(10);
+    cap->m_tuples.reserve(10);
+
+    int i = 0;
+    while (i < tupsize)
+    {
+        int card = tuples[i];
+        if (card == 2)//pair, make them ordered
+        {
+            cap->m_pairs.push_back(0.0);
+            i++;
+            int t1 = tuples[i];
+            i++;
+            int t2 = tuples[i];
+            i++;
+            cap->m_pair_index.push_back(min(t1, t2));
+            cap->m_pair_index.push_back(max(t1, t2));
+        }
+        else // card>2
+        {
+            cap->m_tuple_content.push_back(card);
+            cap->m_tuples.push_back(0.0);
+//            cap->m_tuple_content.push_back(card);
+            cap->m_tuple_start.push_back((int) cap->m_tuple_content.size() - 1);
+            i++;
+            for (int j = 0;j < card;j++) {
+                cap->m_tuple_content.push_back(tuples[i]);
+                i++;
+            }
 
-		}
-	}
+        }
+    }
 }
 
 // with content
 // takes as the argument the list of indices with cardinalities, (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
 void Prepare_FM_sparse(int n, int tupsize, double *tups, int* tuples, struct SparseFM* cap)
 {
-	cap->n=n;
-	cap->m_singletons.resize(n);
-	cap->m_pairs.reserve(10);
-	cap->m_pair_index.reserve(10);
-	cap->m_tuple_content.reserve(10);
-	cap->m_tuple_start.reserve(10);
-	cap->m_tuples.reserve(10);
-
-	int i = 0, j=0;
-	while (i < tupsize)
-	{
-		int card = tuples[i];
-		if (card == 2)//pair, make them ordered
-		{
-			(tups==NULL? cap->m_pairs.push_back(0.0): cap->m_pairs.push_back(tups[j]));
-			j++;
-			
-			i++;
-			int t1 = tuples[i];
-			i++;
-			int t2 = tuples[i];
-			i++;
-			cap->m_pair_index.push_back(min(t1, t2));
-			cap->m_pair_index.push_back(max(t1, t2));
-		}
-		else // card>2
-		{
-			cap->m_tuple_content.push_back(card);
-			(tups==NULL? cap->m_tuples.push_back(0.0): cap->m_tuples.push_back(tups[j])); j++;
-		//	cap->m_tuples.push_back(tups[i]);
-	//		cap->m_tuple_content.push_back(card);
-			cap->m_tuple_start.push_back((int) cap->m_tuple_content.size() - 1);
-			i++;
-			for (int j = 0;j < card;j++) {
-				cap->m_tuple_content.push_back(tuples[i]);
-				i++;
-			}
+    cap->n=n;
+    cap->m_singletons.resize(n);
+    cap->m_pairs.reserve(10);
+    cap->m_pair_index.reserve(10);
+    cap->m_tuple_content.reserve(10);
+    cap->m_tuple_start.reserve(10);
+    cap->m_tuples.reserve(10);
+
+    int i = 0, j=0;
+    while (i < tupsize)
+    {
+        int card = tuples[i];
+        if (card == 2)//pair, make them ordered
+        {
+            (tups==NULL? cap->m_pairs.push_back(0.0): cap->m_pairs.push_back(tups[j]));
+            j++;
+            
+            i++;
+            int t1 = tuples[i];
+            i++;
+            int t2 = tuples[i];
+            i++;
+            cap->m_pair_index.push_back(min(t1, t2));
+            cap->m_pair_index.push_back(max(t1, t2));
+        }
+        else // card>2
+        {
+            cap->m_tuple_content.push_back(card);
+            (tups==NULL? cap->m_tuples.push_back(0.0): cap->m_tuples.push_back(tups[j])); j++;
+        //    cap->m_tuples.push_back(tups[i]);
+    //        cap->m_tuple_content.push_back(card);
+            cap->m_tuple_start.push_back((int) cap->m_tuple_content.size() - 1);
+            i++;
+            for (int j = 0;j < card;j++) {
+                cap->m_tuple_content.push_back(tuples[i]);
+                i++;
+            }
 
-		}
-	}
+        }
+    }
 }
 
 void Prepare_FM_sparse0(int n, int tupsize,int* tuples, struct SparseFM* cap)
 {
-	Prepare_FM_sparse(n,tupsize,NULL,tuples, cap);
+    Prepare_FM_sparse(n,tupsize,NULL,tuples, cap);
 }
 
 void Free_FM_sparse(struct SparseFM* cap)
 {
 	if (cap->n > 0) {
 		cap->m_singletons.resize(0);
 		cap->m_pairs.resize(0);
@@ -1554,17 +1560,14 @@
 		cap->m_tuples.resize(0);
 		cap->n = 0;
 	}
 }
 
 int TupleCardinalitySparse(int i, struct SparseFM* cap) // only for tuples
 {
-#ifdef	MEMCHK
-	if(cap->m_tuple_start.size()<=i) return 0; else
-#endif
 	return cap->m_tuple_content[cap->m_tuple_start[i]];
 }
 
 int  GetSizeArrayTuples(struct SparseFM* cap)
 {
 	return (int) cap->m_tuple_content.size();
 }
@@ -1574,27 +1577,16 @@
 	return (int) cap->m_tuples.size();
 }
 
 // now sets are indexed by A = the position of the element in the respective array (singletons, tuples or pairs)
 int             IsInSetSparse(int A, int card, int i, struct SparseFM* cap)                 // does i belong to set A?
 {
 	if (card == 1) return (A == i);
-
-	
-	if (card == 2)  {	
-#ifdef	MEMCHK	
-		if(2*A >= cap->m_pair_index.size()) return 0; // out of bounds
-#endif		
-		return((cap->m_pair_index[2 * A] == (uint16_t)i) || (cap->m_pair_index[2 * A + 1] == (uint16_t)i));
-	}
+	if (card == 2) return((cap->m_pair_index[2 * A] == (uint16_t)i) || (cap->m_pair_index[2 * A + 1] == (uint16_t)i));
 	// else process tuple
-#ifdef	MEMCHK	
-	if(A >= cap->m_tuple_start.size()) return 0; // out of bounds
-#endif	
-	
 	for (int j = 1;j <= cap->m_tuple_content[cap->m_tuple_start[A]]; j++)
 		if (cap->m_tuple_content[cap->m_tuple_start[A] + j] == i) return 1;
 
 	return 0;
 }
 
 int             IsSubsetSparse(int A, int cardA, int B, int cardB, struct SparseFM* cap)       // is B subset of A ?  careful, will not work if B has repeated entries by mistake
@@ -1603,72 +1595,50 @@
 	if (cardB == 1)
 	{
 		return IsInSetSparse(A, cardA, B, cap);
 	}
 	if (cardB == 2) {
 		if (cardA == 1) return 0;
 		if (cardA == 2) return (A == B);
-#ifdef	MEMCHK	
-		if(2*B >= cap->m_pair_index.size()) return 0; // out of bounds
-#endif			
-		
 		return (IsInSetSparse(A, cardA, cap->m_pair_index[2 * B], cap) && IsInSetSparse(A, cardA, cap->m_pair_index[2 * B + 1], cap));
 	}
 
-#ifdef	MEMCHK
-	if(B >= cap->m_tuple_start.size()) return 0; // out of bounds
-#endif		
-	
 	for (int j = 1;j <= cap->m_tuple_content[cap->m_tuple_start[B]]; j++) {
 		if (!IsInSetSparse(A, cardA, cap->m_tuple_content[cap->m_tuple_start[B] + j], cap)) return 0;
 	}
 	return 1;
 }
 
 
 
 double min_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap) // returns minimum of x_i, such that i belongs to set S
 {
 	if (cardS == 1) return x[S];
 	if (cardS == 2)
 	{
-#ifdef	MEMCHK		
-		if(2*S >= cap->m_pair_index.size()) return 0; // out of bounds
-#endif			
 		double t1 = x[cap->m_pair_index[2 * S] -1];
 		double t2 = x[cap->m_pair_index[2 * S + 1]  -1];
 		return min(t1, t2);
 	}
 	double t = 10e10;
-#ifdef	MEMCHK	
-	if(S >= cap->m_tuple_start.size()) return 0; // out of bounds
-#endif		
-	
 	for (int j = 1;j <= cap->m_tuple_content[cap->m_tuple_start[S]]; j++)
 		t = min(t, x[cap->m_tuple_content[cap->m_tuple_start[S] + j]  -1]);
 
 	return t;
 }
 double max_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap) // returns maximum of x_i, such that i belongs to set S
 {
 	if (cardS == 1) return x[S];
 	if (cardS == 2)
 	{
-#ifdef	MEMCHK		
-		if(2*S >= cap->m_pair_index.size()) return 0; // out of bounds
-#endif		
 		double t1 = x[cap->m_pair_index[2 * S]  -1];
 		double t2 = x[cap->m_pair_index[2 * S + 1]  -1];
 		return max(t1, t2);
 	}
 	double t = -10e10;
-	
-#ifdef	MEMCHK	
-	if(S >= cap->m_tuple_start.size()) return 0; // out of bounds
-#endif		
 	for (int j = 1;j <= cap->m_tuple_content[cap->m_tuple_start[S]]; j++)
 		t = max(t, x[cap->m_tuple_content[cap->m_tuple_start[S] + j]  -1]);
 
 	return t;
 }
 
 double ChoquetMobSparse(double*x, int n, struct SparseFM* cap)
@@ -1700,15 +1670,15 @@
 	}
 
 	// tuples
 	for (size_t  j = 0;j < cap->m_tuples.size(); j++) {
 		double r = 1. / cap->m_tuple_content[cap->m_tuple_start[j]]; // cardinality
 
 		for (int k = 1;k <= cap->m_tuple_content[cap->m_tuple_start[j]]; k++)
-			v[cap->m_tuple_content[cap->m_tuple_start[j] + k] -1 ] += cap->m_tuples[j] * r;
+			v[cap->m_tuple_content[cap->m_tuple_start[j] + k]-1] += cap->m_tuples[j] * r;
 
 	}
 }
 
 void BanzhafMobSparse(double* v, int n, struct SparseFM* cap)
 {
 	for (int i = 0;i < n; i++)
@@ -1721,99 +1691,98 @@
 	}
 
 	// tuples
 	for (size_t  j = 0;j < cap->m_tuples.size(); j++) {
 		double r = 1. / ( 1<< (cap->m_tuple_content[cap->m_tuple_start[j]] -1) ); // 2^(cardinality-1)
 
 		for (int k = 1;k <= cap->m_tuple_content[cap->m_tuple_start[j]]; k++)
-			v[cap->m_tuple_content[cap->m_tuple_start[j] + k] -1  ] += cap->m_tuples[j] * r;
+			v[cap->m_tuple_content[cap->m_tuple_start[j] + k]-1] += cap->m_tuples[j] * r;
 
 	}
 }
 
 
 
 void NonmodularityIndexMobSparse(double* w, int n, int_64 m, struct SparseFM* cap) // calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform of 
 //a k-additive FM in cardinality ordering (of length 2^n=m), using sparse representation
 {
 	int_64 id, A;
 	w[0] = 0;
-	for (int_64 i = (int_64)0; i < m; i++) w[i] = 0;	
-	
-	for (id = (int_64)1; id < m; id++)
+	for (int i = 0;i < n; i++)
+		w[i] = cap->m_singletons[i];  // singleton
+
+	for (int_64 i = (int_64)n; i < m; i++) w[i] = 0;
+
+	for (id = (int_64)n; id < m; id++)
 	{
-		if(Cardinality(id)==1) {
-			for( int i=0;i<n;i++) if(IsInSet(id,i))
-				{w[id]=cap->m_singletons[i];break;}
-		} else {
-			for (size_t j = 0;j < cap->m_pairs.size(); j++)
-			{
-				A = 0;
-				AddToSet(&A, (cap->m_pair_index[2 * j] - 1)); // 1based to 0-based
-				AddToSet(&A, (cap->m_pair_index[2 * j + 1] - 1));
-				if (IsSubset(id, A))
-					w[id] += 2 * cap->m_pairs[j];
-			}
+		for (size_t j = 0;j < cap->m_pairs.size(); j++)
+		{
+			A = 0;
+			AddToSet(&A, (cap->m_pair_index[2 * j] - 1)); // 1based to 0-based
+			AddToSet(&A, (cap->m_pair_index[2 * j + 1] - 1));
+			if (IsSubset(id, A))
+				w[id] += 2 * cap->m_pairs[j];
+		}
 
-			for (size_t  i = 0; i < cap->m_tuples.size();i++) {
-				A = 0;
-				for (int  j = 1;j <= cap->m_tuple_start[i];j++)
-					AddToSet(&A, (cap->m_tuple_content[cap->m_tuple_start[i] + j] - 1));
-				if (IsSubset(id, A))
-					w[id] += cap->m_tuples[i] * cap->m_tuple_content[cap->m_tuple_start[i]];  // cardinality
-			}
-		
-			w[id] /= Cardinality(id);
+		for (size_t  i = 0; i < cap->m_tuples.size();i++) {
+			A = 0;
+			for (int  j = 1;j <= cap->m_tuple_start[i];j++)
+				AddToSet(&A, (cap->m_tuple_content[cap->m_tuple_start[i] + j] - 1));
+			if (IsSubset(id, A))
+				w[id] += cap->m_tuples[i] * cap->m_tuple_content[cap->m_tuple_start[i]];  // cardinality
 		}
+		w[id] /= card[card2bit[id]];
 	}
 }
 
 
 void PopulateFM2Add_Sparse(double* singletons, int numpairs, double* pairs, int* indicesp1, int* indicesp2 , struct SparseFM* cap)
 { //FM is already prepared, just add singletons and pairs
 	
 	for (int i = 0;i < cap->n;i++) cap->m_singletons[i] = singletons[i];
 
 	for (int i = 0;i < numpairs; i++) {
-		cap->m_pairs[i] = pairs[i];
-		cap->m_pair_index[2 * i] = indicesp1[ i];
-		cap->m_pair_index[2 * i+1] = indicesp2[i];
+		cap->m_pairs.push_back(pairs[i]);
+		cap->m_pair_index.push_back(uint16_t(indicesp1[ i]));
+		cap->m_pair_index.push_back(uint16_t(indicesp2[i]));
 	}
 }
 
 
 void AddPairSparse(int i, int j, double* v, struct SparseFM* cap)
 {
 	cap->m_pairs.push_back(*v);
-	cap->m_pair_index.push_back(min(i, j));
-	cap->m_pair_index.push_back(max(i, j));
+	cap->m_pair_index.push_back(uint16_t(min(i, j)));
+	cap->m_pair_index.push_back(uint16_t(max(i, j)));
 }
 void AddTupleSparse(int tupsize, int* tuple, double* v, struct SparseFM* cap)
 {
 	cap->m_tuples.push_back(*v);
 	cap->m_tuple_start.push_back((int) cap->m_tuple_content.size());
 
 	cap->m_tuple_content.push_back(tupsize);
 
 	for (int j = 0;j < tupsize;j++) {
-		cap->m_tuple_content.push_back(tuple[j]);
+		cap->m_tuple_content.push_back((uint16_t)(tuple[j]));
 	}
 }
 
 void PopulateFM2Add_Sparse_from2add(int n, double * v, struct SparseFM* cap)
 {
 	Prepare_FM_sparse(n, 0, NULL, cap);
 	for (int i = 0;i < n;i++) cap->m_singletons[i] = v[i];
 	
 	//int len = n*(n - 1) / 2;
 	int i = n;
 	for(int k=0;k <n-1; k++)
 		for (int j = k + 1;j < n;j++) {
-			if (v[i] != 0) AddPairSparse(k+1, j+1, &(v[i]), cap);
-			i++;
+			if (v[i] != 0) 
+				AddPairSparse(k + 1, j + 1, &(v[i]), cap);
+//			printf("add %f %d %d\n", v[i], k + 1, j + 1);
+			i++;	
 		}
 }
 
 void Expand2AddFull(double* v, struct SparseFM* cap)
 {
 	// array v needs to be n+choose(n,2) in size at least, not checked
 	for (int i = 0;i < cap->n;i++) v[i] = cap->m_singletons[i];
@@ -1846,16 +1815,17 @@
 		AddToSet(&A, (cap->m_pair_index[2*i]-1 ));
 		AddToSet(&A, (cap->m_pair_index[2 * i+1]-1));
 		v[A]= cap->m_pairs[i];
 	}
 
 	for (size_t  i = 0; i < cap->m_tuples.size();i++) {
 		A = 0;
-		for(int  j=1;j<=cap->m_tuple_start[i];j++)
+		for(int  j=1;j<=cap->m_tuple_content[cap->m_tuple_start[i]];j++){
 			AddToSet(&A, (cap->m_tuple_content[cap->m_tuple_start[i]+j]  -1) );
+		}
 		v[A] = cap->m_tuples[i];
 	}
 }
 
 void ExportSparseSingletons(int n, double *v, struct SparseFM* cap)
 {
 	for (int i = 0;i < n;i++) v[i] = cap->m_singletons[i];
```

### Comparing `pyfmtools-0.81/src/fuzzymeasuretools.h` & `pyfmtools-5.1/src/fuzzymeasuretools.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,439 +1,386 @@
-/********************* Fuzzy measure toolkit ******************************************
-
-This is a set of useful routines for manipulations with fuzzy measures 
-(and other set functions). They include binary encoding of a discrete set 
-(as  integers (up to 32 elements in a set)), simple set operations: 
-intersection, union, inclusion, difference, etc. various representations of 
-fuzzy measures (standard, Moebius), orderings of their values, conversions, 
-calculations of Shapley, Banzhaf and other interaction indices, orness, entropy, etc.
-Calculation of Choquet and Sugeno integrals for a given input x.
-
---------------------------------------------------------------------------------------
- *
- *      begin                : May 10 2007
- *		end					 : September 3 2020
- *              version                          : 4.0 
- *              copyright            : (C) 2007-2020 by Gleb Beliakov
- *              email                : gleb@deakin.edu.au
- *
- * 
- * This program is free software; you can redistribute it and/or modify
- * it under the terms of the Lesser GNU General Public License as published by
- * the Free Software Foundation; either version 2 of the License, or (at
- * your option) any later version.
- * 
- * This program is distributed in the hope that it will be useful, but
- * WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
- * Lesser General Public License for more details.
- * 
- * You should have received a copy of the GNU Lesser General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
-**************************************************************************************/
-
-
-/*
-Notes: The bitwise operations (sets, subsets, element of the set, etc.) are 0-based, ie element 1 corresponds to the 0th element of set A. 
-
-Sparse representation: 1-based , ie pair (1,2) corresponds to the bitwise set A=11b =3
-
-Geberal capacities start with 0 (emptyset) and go to 2^n elements
-// in binary ordering the subsets are ordered as
-// 0 1 2 12 3 13 23 123 4 14 24 124 34 134 234 1234,...
-// (which corresponds to the order 0,1,2,3,... in binary form)
-// in cardinality ordering they are ordered as
-// 0 1 2 3 4 5 6 12 13 14 15 16 23 24 25 26 34 35 36 45 46 56 123 124,...
-// (empty, singletons, pairs,triples, etc.)
-
-2-additive capacities are coded as an array of singletons (starting from 0, hence no empty set) and pairs without repetitions that is pairs (1,2), (1,3)...(2,3), (2,4)...(3,4)...
-Always in cardinality ordering
-
-Sparse representation is the structure SparseFM - contains arrays of singletons, nonzero pairs and their indices (1-based) tuples and their cardinalities and indices
-Sparse is meaningful for Mobius/interaction or nonmodularity representations
-
-
-2-additive and sparse methods canbe called without Preparations_FM
-
-*/
-
-#include "generaldefs.h"
-
-#define FM_SPARSE
-
-#define GBtolerance 0.00001
-
-double ElapsedTime();
-void   ResetTime();
-
-struct valindex {
-        double v;
-        int i;
-} ;
-
-
-//#define int_64 unsigned long long
-typedef unsigned long long int_64;
-
-typedef unsigned short uint16_t;
-
-//typedef int_64 myint;
-typedef unsigned int myint;
-
-//typedef uint16_t myint;
-// any of the above, for m<16 use uint_16
-
-typedef unsigned int uint;
-
-// float or double
-//typedef float  myfloat;
-typedef double  myfloat;
-
-/* Global arrays*/
-extern valindex tempxi[100];
-
-LIBDLL_API extern double   *m_factorials;  // keeps factorials  n! up to n
-LIBDLL_API extern int      *card;                  // array to keep set cardinalities in binary ordering
-LIBDLL_API extern int *cardpos;   // array to store the indices of elements of different cardinalities in the cardinality ordering
-
-LIBDLL_API extern int_64 *bit2card; // arrays to transform from one ordering to another
-LIBDLL_API extern int_64 *card2bit;
-
-LIBDLL_API extern int *cardposm;   // array to store the indices of elements of different cardinalities in the cardinality ordering
-
-LIBDLL_API extern int_64 *bit2cardm; // arrays to transform from one ordering to another
-LIBDLL_API extern int_64 *card2bitm;
-
-#include<cstdlib>
-#include <vector>
-using namespace std;
-
-
-#ifdef FM_SPARSE
-
-
-/*
-template <class T>
-class vectorWrapper : public std::vector<T>
-{   
-public:
-  vectorWrapper() {
-    this->_M_impl _M_start = this->_M_impl _M_finish = this->_M_impl _M_end_of_storage = NULL;
-  }   
-
-  vectorWrapper(T* sourceArray, int arraySize)
-  {   
-    this->_M_impl _M_start = sourceArray;
-    this->_M_impl _M_finish = this->_M_impl _M_end_of_storage = sourceArray + arraySize;
-  }   
-
-  ~vectorWrapper() {
-    this->_M_impl _M_start = this->_M_impl _M_finish = this->_M_impl _M_end_of_storage = NULL;
-  }   
-
-  void wrapArray(T* sourceArray, int arraySize)
-  {   
-    this->_M_impl _M_start = sourceArray;
-    this->_M_impl _M_finish = this->_M_impl _M_end_of_storage = sourceArray + arraySize;
-  }   
-};*/
-
-#ifdef R_cpp11
-//#include "cpp11.hpp"
-
-//#define m_singletons (*p_singletons)
-//#define m_pairs (*p_pairs)
-//#define m_tuples (*p_tuples)
-//#define m_pair_index (*p_pair_index)
-//#define m_tuple_start (*p_tuple_start)
-//#define m_tuple_content (*p_tuple_content)
-
-
-
-
-struct SparseFM {
-	int n;
-
-	vector<double>  m_singletons;
-	vector<double>  m_pairs;
-	vector<double>  m_tuples;
-
-	vector<int> m_pair_index;// goes in pairs, hence  m_pair_index[2i],m_pair_index[2i+1] corresponds to m_pairs[i];
-
-	vector<int> m_tuple_start; // pints to cardinality, list of elements, stored  in m_tuple_content
-	vector<int> m_tuple_content;  // for any j such that m_tules[j] is the value, m_tuple_content[m_tuple_start[j]] is the cardinality
-};	
-#else
-struct SparseFM {
-	int n;
-
-	vector<double>  m_singletons;
-	vector<double>  m_pairs;
-	vector<double>  m_tuples;
-
-	vector<uint16_t> m_pair_index;// goes in pairs, hence  m_pair_index[2i],m_pair_index[2i+1] corresponds to m_pairs[i];
-
-	vector<int> m_tuple_start; // pints to cardinality, list of elements, stored  in m_tuple_content
-	vector<uint16_t> m_tuple_content;  // for any j such that m_tules[j] is the value, m_tuple_content[m_tuple_start[j]] is the cardinality
-};	
-#endif
-#endif
-
-LIBDLL_API int_64 Bit2Card(int_64 c);
-LIBDLL_API int_64 Card2Bit(int_64 c);
-
-// this routine should be called first to prepare all the arrays for small FM (up to n=15, may be 24 (sizes are 2^n)), otherwise the arrays become too big
-LIBDLL_API void Preparations_FM(int n, int_64 *m);
-
-LIBDLL_API void Preparations_fm_marginal(int n, int_64 *m, int Kinter);
-
-LIBDLL_API void ConvertCard2Bit(double* dest, double* src,  int_64 m);
-
-LIBDLL_API int_64 Bit2card(int_64 id, int n, int kint, int arraysize);
-
-// this routine should be called last to clean all the arrays
-LIBDLL_API void Cleanup_FM();
-
-
-/* useful routines */
-extern double   minf(double a, double b); 
-double  maxf(double a, double b);
-int             sign(int i);   // sign of i
-int             IsOdd(int i);  // is i odd ?
-
-
-LIBDLL_API unsigned int bitweight(int_64 i);
-
-LIBDLL_API unsigned int cardf(int_64 i); // count how many bits in i are set
-LIBDLL_API double xlogx(double t);         // x log x (but takes care of x close to 0, using tolerance parameter
-
-
-/* Set manipulations. A set is represented by an unsigned int (32 bits) */
-LIBDLL_API void    RemoveFromSet(int_64* A, int i);  // remove a from set i
-LIBDLL_API void    AddToSet(int_64* A, int i);               // add a to set i
-LIBDLL_API int             IsInSet(int_64 A, int i);                 // does a belong to set i?
-LIBDLL_API int             IsSubset(int_64 A, int_64 B);       // is B subset of A ?
-LIBDLL_API int_64  Setunion(int_64 A, int_64 B); // returns the  union of sets A and B
-LIBDLL_API int_64  Setintersection(int_64 A, int_64 B); // returns the  intersection of sets i and j
-LIBDLL_API int_64  Setdiff(int_64 A, int_64 B);                  // returns set difference  i \ j
-LIBDLL_API double min_subset(double* x, int n, int_64 S); // returns minimum of x_i, such that i belongs to set S
-LIBDLL_API double max_subset(double* x, int n, int_64 S); // returns maximum of x_i, such that i belongs to set S
-LIBDLL_API int_64 UniversalSet(int n);
-LIBDLL_API int Removei_th_bitFromSet(int_64* A, int i);
-
-LIBDLL_API  int_64 choose(int i, int n);
-
-
-
-
-LIBDLL_API int_64 remove1bit(int_64 a, int i);
-// counting fom 0
-
-
-LIBDLL_API int_64 RemoveHighestBit(int_64 a, int K);
-
-LIBDLL_API inline int HasBitsAboveK(int_64 a, int K) { // K counting from 1
-	return(a >= (int_64)1 << K);
-}
-
-LIBDLL_API inline int TopElement(int_64 a) {
-	// return true is a= 11111...
-	return (bitweight(a + 1) == 1);
-}
-
-
-
-#include "fmrandom.h"
-
-
-
-
-
-
-LIBDLL_API void ExpandKinteractive2Bit(double* dest, double* src, int n, int_64 m, int kint, int arraysize);
-LIBDLL_API void ExpandKinteractive2Bit_m(double* dest, double* src, int n, int_64 m, int kint, int arraysize, double* VVC);
-// converts compact k-interactive representation to full length binary ordering. The second call required working memory of size m.
-
-LIBDLL_API unsigned int ShowValue(int_64 s); // shows the elements of a subset as a decimal string (up to 10 elements)
-
-LIBDLL_API double Choquet(double*x, double* v, int n, int_64 m);
-/* Calculates the value of a descrete Choquet integral of x, wrt fuzzy measure v. 
-   Parameters: x array[n] ,v array[m], n, m=2^n 
-   This proceduce requires sorting the array of pairs (v[i],i) in non-decreasing order
-   (perfored by standard STL sort function, and RemoveFromSet() function, to remove
-   an indicated bit from a set (in its binary representation). 
-*/
-
-LIBDLL_API double ChoquetKinter(double*x, double* v, int n, int_64 m, int kint);
-/* As above, but for kinteractive f.m. using compact representation of v  (in cardinality ordering! */
-
-LIBDLL_API double ChoquetMob(double*x, double* Mob, int n, int_64 m);
-/* This is an alternative calculation of the Choquet integral from the Moebius transform v. 
-   It is not as efficient as Choquet(). Provided for testing purposes.
-*/
-
-LIBDLL_API double Sugeno(double*x, double* v, int n, int_64 m);
-/* Calculates the value of a descrete Sugeno integral of x, wrt fuzzy measure v 
-Parameters: x array[n] ,v array[m], n, m=2^n 
-This proceduce requires sorting the array of pairs (v[i],i) in non-decreasing order
-(perfored by standard STL sort function, and RemoveFromSet() function, to remove
-an indicated bit from a set (in its binary representation)
-Also requires maxf and minf functions.
-*/
-
-LIBDLL_API double OWA(double*x, double* v, int n );
-/* Calculates the value of OWA */
-
-LIBDLL_API double WAM(double*x, double* v, int n );
-/* Calculates the value of WAM */
-
-LIBDLL_API void ConstructLambdaMeasure(double *singletons, double *lambda, double *v, int n, int_64 m);
-/* Given the values of the fuzzy measure at singletons, finds the appropriate
-lambda, and constructs the rest of the fuzzy measure. Returns lambda and v at the output
-*/
-
-/* ---------------Operations on fuzzy measures -------------------------*/
-
-LIBDLL_API double Orness(double* Mob, int n, int_64 m); // calculates orness value of a fuzzy measure
-
-LIBDLL_API double Entropy(double* v, int n, int_64 m);// calculates Entropy of a fuzzy measure
-
-LIBDLL_API double OrnessOWA(double* w, int n); // calculates orness value of a fuzzy measure
-
-LIBDLL_API void Mobius(double* v, double* Mob, int n, int_64 m); // calculates Moebius representation of v
-/* the output array w should have the same size 2^n=m as v */
-
-LIBDLL_API void Zeta(double* Mob, double* v, int n, int_64 m);// calculates inverse Moebius transform
-
-LIBDLL_API void Shapley(double* v, double* x, int n, int_64 m); // calculates the array x of Shapley values
-LIBDLL_API void Banzhaf(double* v, double* x, int n, int_64 m);// calculates the array x of Banzhaf indices
-
-LIBDLL_API void ShapleyMob(double* Mob, double* w, int n, int_64 m);
-LIBDLL_API void BanzhafMob(double* Mob, double* w, int n, int_64 m);
-
-LIBDLL_API void InteractionMob(double* Mob, double* w, int_64 m); // calculates all 2^n interaction indices (returned in w)
-LIBDLL_API void InteractionBMob(double* Mob, double* w, int_64 m); // calculates all 2^n Banzhaf interaction indices (returned in w)
-
-LIBDLL_API void NonadditivityIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n nonadditivity indices (returned in w)
-LIBDLL_API void NonadditivityIndexMob(double* Mob, double* w, int n, int_64 m); // calculates  all 2^n nonadditivity indices (returned in w) using Mobius transform
-
-
-LIBDLL_API void NonmodularityIndex(double* v, double* w, int n, int_64 m);
-// calculates  all 2^n nonmodularity indices (returned in w)
-
-LIBDLL_API void NonmodularityIndexMob(double* Mob, double* w, int n, int_64 m);
-// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform
-
-LIBDLL_API void NonmodularityIndexMobkadditive(double* Mob, double* w, int n, int k, int_64 m);
-// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform of 
-//a k-additive FM in cardinality ordering (of length 2^n=m)
-
-LIBDLL_API void NonmodularityIndexKinteractive(double* v, double* w, int n, int kint,int_64 m, int length );
-// the same for k-interactive FM. Requires the length = arraysize of the k-interactive FM. Can be optimised by not calculating many zeros, todo.
-
-LIBDLL_API void BipartitionShapleyIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n bipartition Shapley indices (returned in w)
-LIBDLL_API void BipartitionBanzhafIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n bipartition Banzhaf indices (returned in w)
-
-LIBDLL_API void dualm(double* v, double* w, int n, int_64 m); // calculates the dual fuzzy measure, returns it in w
-LIBDLL_API void dualMob(myfloat* src, myfloat* dest, int_64 m);  // same using Mobius
-
-// Various queries about a fuzzy measure. All performed with a given tolerance. 
-LIBDLL_API int IsMeasureAdditive(double* v, int n, int_64 m);
-LIBDLL_API int IsMeasureBalanced(double* v, int_64 m);
-LIBDLL_API int IsMeasureSelfdual(double* v, int_64 m);
-LIBDLL_API int IsMeasureSubadditive(double* v, int_64 m);
-LIBDLL_API int IsMeasureSubmodular(double* v, int_64 m);
-LIBDLL_API int IsMeasureSuperadditive(double* v, int_64 m);
-LIBDLL_API int IsMeasureSupermodular(double* v, int_64 m);
-LIBDLL_API int IsMeasureSymmetric(double* v, int n, int_64 m);
-LIBDLL_API int IsMeasureKMaxitive(double* v, int n, int_64 m);
-
-
-
-
-LIBDLL_API void dualMobKadd( myfloat* src, myfloat* dest, int m, int length, int k);
-
-LIBDLL_API void Shapley2addMob(double* v, double* x, int n);
-// calculates the array x of Shapley values for 2 additive fm in compact representation (cardinality based)
-LIBDLL_API void Banzhaf2addMob(double* v, double* x, int n);
-// calculates the array x of Banzhaf indices for 2 additive fm in compact representation (cardinality based)
-
-LIBDLL_API double Choquet2add(double*x, double* Mob, int n);
-// calculates the Choquet integal of x  for 2 additive fm in compact Mobius representation (cardinality based)
-
-LIBDLL_API void random_coefficients(int n, vector<myfloat> & c);
-
-#ifdef FM_SPARSE
-
-/*
-Sparse representation of k-additive capacities. Thre representation is in the form of singletons, pairs and tuples with nonzero values, stored and indexed in the respective 
-arrays (see above in this file)
-
- Prepares an empty structure, given the list of cardinalities of the nonzero tuples (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
-
- It is used to allocate storage and later populate these values
-*/
-LIBDLL_API void Prepare_FM_sparse0(int n, int tupsize,  int* tuples, struct SparseFM* cap);
-LIBDLL_API void Prepare_FM_sparse(int n, int tupsize, double *tups, int* tuples, struct SparseFM* cap);
-LIBDLL_API void Free_FM_sparse(struct SparseFM* cap);
-
-/*  Returns the cardinality of the tuple numbered i in the list of tuples */
-LIBDLL_API int TupleCardinalitySparse(int i, struct SparseFM* cap);
-
-LIBDLL_API int  GetNumTuples(struct SparseFM* cap);
-LIBDLL_API int  GetSizeArrayTuples(struct SparseFM* cap);
-
-
-/* checks if element i (1-based!!!) belongs to the tuple indexed A (whose cardinality can be 1,2, other (automatically determined) */
-LIBDLL_API int             IsInSetSparse(int A, int card, int i, struct SparseFM* cap);
-
-/* checks if tuple B is a subset of A */
-LIBDLL_API int             IsSubsetSparse(int A, int cardA, int B, int cardB, struct SparseFM* cap);
-
-/* calculates minimum (maximum) of (x_i) with the indices belonging to tuple indexed as S (its cardinality cardS can be 1,2, other( put 3, will be determined automatically)
-note that x is 0-based, tuples are 1-based */
-LIBDLL_API double min_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap);
-LIBDLL_API double max_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap);
-
-/* calculates the Choquet integral in Mobius representation */
-LIBDLL_API double ChoquetMobSparse(double*x, int n, struct SparseFM* cap);
-
-/* Shapley and Banzhaf values vector of a capacity */
-LIBDLL_API void ShapleyMobSparse(double* v, int n, struct SparseFM* cap);
-LIBDLL_API void BanzhafMobSparse(double* v, int n, struct SparseFM* cap);
-
-LIBDLL_API void NonmodularityIndexMobSparse(double* w, int n, int_64 m, struct SparseFM* cap);
-// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform of 
-//a k-additive FM in cardinality ordering (of length 2^n=m), using sparse representation
-
-/* populates 2-additive sparse capacity with nonzero values using the singletons and two arrays of indices (of size numpairs) . Indices need to be 1-based. Singletons 0-based */
-LIBDLL_API void PopulateFM2Add_Sparse(double* singletons, int numpairs, double* pairs, int* indicesp1, int* indicesp2, struct SparseFM* cap);
-
-/* for populating capacities. Add pair (v_ij) to the structure. indices are 1-based */
-LIBDLL_API void AddPairSparse(int i, int j, double* v, struct SparseFM* cap);
-/* for populating capacities, adds a tuple of size tupsize whose 1-based indices are in tuple */
-LIBDLL_API void AddTupleSparse(int tupsize, int* tuple, double* v, struct SparseFM* cap);
-
-/* Given 2-additive capacity singletons=pairs in one array v , selects nonzero pairs */
-LIBDLL_API void PopulateFM2Add_Sparse_from2add(int n, double * v, struct SparseFM* cap);
-
-/* from sparse to full representaiotn of 2-additive capacity (singletons and paits, augmented with 0 ) Vector v has to be allocated, size is n+ n(n-1)/2 */
-LIBDLL_API void Expand2AddFull(double* v, struct SparseFM* cap);
-
-/* from sparse to full capacity (vector v, size 2^n has to be preallocated) */
-LIBDLL_API void ExpandSparseFull(double* v, struct SparseFM* cap);
-
-LIBDLL_API void ExportSparseSingletons(int n, double *v, struct SparseFM* cap);
-LIBDLL_API int ExportSparsePairs(int* pairs, double *v, struct SparseFM* cap);
-LIBDLL_API int ExportSparseTuples(int* tuples, double *v, struct SparseFM* cap);
-
-
-/* random generation of  sparse supermodular capacities */
-LIBDLL_API int generate_fm_2additive_convex_sparse(int n, struct SparseFM* cap);
-
-/* this is actually a total monotone, Belief measure */
-LIBDLL_API int generate_fm_kadditive_convex_sparse(int n, int k, int nonzero, struct SparseFM* cap);
-
-
-
-#endif
+/********************* Fuzzy measure toolkit ******************************************
+
+This is a set of useful routines for manipulations with fuzzy measures 
+(and other set functions). They include binary encoding of a discrete set 
+(as  integers (up to 32 elements in a set)), simple set operations: 
+intersection, union, inclusion, difference, etc. various representations of 
+fuzzy measures (standard, Moebius), orderings of their values, conversions, 
+calculations of Shapley, Banzhaf and other interaction indices, orness, entropy, etc.
+Calculation of Choquet and Sugeno integrals for a given input x.
+
+--------------------------------------------------------------------------------------
+ *
+ *      begin                : May 10 2007
+ *		end					 : September 3 2020
+ *              version                          : 4.0 
+ *              copyright            : (C) 2007-2020 by Gleb Beliakov
+ *              email                : gleb@deakin.edu.au
+ *
+ * 
+ * This program is free software; you can redistribute it and/or modify
+ * it under the terms of the Lesser GNU General Public License as published by
+ * the Free Software Foundation; either version 2 of the License, or (at
+ * your option) any later version.
+ * 
+ * This program is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+ * Lesser General Public License for more details.
+ * 
+ * You should have received a copy of the GNU Lesser General Public License
+ * along with this program; if not, write to the Free Software
+ * Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
+**************************************************************************************/
+
+
+/*
+Notes: The bitwise operations (sets, subsets, element of the set, etc.) are 0-based, ie element 1 corresponds to the 0th element of set A. 
+
+Sparse representation: 1-based , ie pair (1,2) corresponds to the bitwise set A=11b =3
+
+Geberal capacities start with 0 (emptyset) and go to 2^n elements
+// in binary ordering the subsets are ordered as
+// 0 1 2 12 3 13 23 123 4 14 24 124 34 134 234 1234,...
+// (which corresponds to the order 0,1,2,3,... in binary form)
+// in cardinality ordering they are ordered as
+// 0 1 2 3 4 5 6 12 13 14 15 16 23 24 25 26 34 35 36 45 46 56 123 124,...
+// (empty, singletons, pairs,triples, etc.)
+
+2-additive capacities are coded as an array of singletons (starting from 0, hence no empty set) and pairs without repetitions that is pairs (1,2), (1,3)...(2,3), (2,4)...(3,4)...
+Always in cardinality ordering
+
+Sparse representation is the structure SparseFM - contains arrays of singletons, nonzero pairs and their indices (1-based) tuples and their cardinalities and indices
+Sparse is meaningful for Mobius/interaction or nonmodularity representations
+
+
+2-additive and sparse methods canbe called without Preparations_FM
+
+*/
+
+#include "generaldefs.h"
+
+#define FM_SPARSE
+
+#define GBtolerance 0.00001
+
+double ElapsedTime();
+void   ResetTime();
+
+struct valindex {
+        double v;
+        int i;
+} ;
+
+
+//#define int_64 unsigned long long
+typedef unsigned long long int_64;
+
+typedef unsigned short uint16_t;
+
+//typedef int_64 myint;
+//typedef unsigned int myint;
+
+typedef uint16_t myint;
+// any of the above, for m<16 use uint_16
+
+typedef unsigned int uint;
+
+// float or double
+//typedef float  myfloat;
+typedef double  myfloat;
+
+/* Global arrays*/
+extern valindex tempxi[100];
+
+LIBDLL_API extern double   *m_factorials;  // keeps factorials  n! up to n
+LIBDLL_API extern int      *card;                  // array to keep set cardinalities in binary ordering
+LIBDLL_API extern int *cardpos;   // array to store the indices of elements of different cardinalities in the cardinality ordering
+
+LIBDLL_API extern int_64 *bit2card; // arrays to transform from one ordering to another
+LIBDLL_API extern int_64 *card2bit;
+
+LIBDLL_API extern int *cardposm;   // array to store the indices of elements of different cardinalities in the cardinality ordering
+
+LIBDLL_API extern int_64 *bit2cardm; // arrays to transform from one ordering to another
+LIBDLL_API extern int_64 *card2bitm;
+
+#include<cstdlib>
+#include <vector>
+using namespace std;
+
+#ifdef FM_SPARSE
+
+
+
+struct SparseFM {
+	int n;
+
+	vector<double>  m_singletons;
+	vector<double>  m_pairs;
+	vector<double>  m_tuples;
+
+	vector<int> m_pair_index;// goes in pairs, hence  m_pair_index[2i],m_pair_index[2i+1] corresponds to m_pairs[i]; // was uint_16 - incompatibility
+
+	vector<int> m_tuple_start; // pints to cardinality, list of elements, stored  in m_tuple_content
+	vector<int> m_tuple_content;  // for any j such that m_tules[j] is the value, m_tuple_content[m_tuple_start[j]] is the cardinality
+};
+#endif
+
+LIBDLL_API int_64 Bit2Card(int_64 c);
+LIBDLL_API int_64 Card2Bit(int_64 c);
+
+// this routine should be called first to prepare all the arrays for small FM (up to n=15, may be 24 (sizes are 2^n)), otherwise the arrays become too big
+LIBDLL_API void Preparations_FM(int n, int_64 *m);
+
+LIBDLL_API void Preparations_fm_marginal(int n, int_64 *m, int Kinter);
+
+LIBDLL_API void ConvertCard2Bit(double* dest, double* src,  int_64 m);
+
+LIBDLL_API int_64 Bit2card(int_64 id, int n, int kint, int arraysize);
+
+// this routine should be called last to clean all the arrays
+LIBDLL_API void Cleanup_FM();
+
+
+/* useful routines */
+extern double   minf(double a, double b); 
+double  maxf(double a, double b);
+int             sign(int i);   // sign of i
+int             IsOdd(int i);  // is i odd ?
+
+
+LIBDLL_API unsigned int bitweight(int_64 i);
+
+LIBDLL_API unsigned int cardf(int_64 i); // count how many bits in i are set
+LIBDLL_API double xlogx(double t);         // x log x (but takes care of x close to 0, using tolerance parameter
+
+
+/* Set manipulations. A set is represented by an unsigned int (32 bits) */
+LIBDLL_API void    RemoveFromSet(int_64* A, int i);  // remove a from set i
+LIBDLL_API void    AddToSet(int_64* A, int i);               // add a to set i
+LIBDLL_API int             IsInSet(int_64 A, int i);                 // does a belong to set i?
+LIBDLL_API int             IsSubset(int_64 A, int_64 B);       // is B subset of A ?
+LIBDLL_API int_64  Setunion(int_64 A, int_64 B); // returns the  union of sets A and B
+LIBDLL_API int_64  Setintersection(int_64 A, int_64 B); // returns the  intersection of sets i and j
+LIBDLL_API int_64  Setdiff(int_64 A, int_64 B);                  // returns set difference  i \ j
+LIBDLL_API double min_subset(double* x, int n, int_64 S); // returns minimum of x_i, such that i belongs to set S
+LIBDLL_API double max_subset(double* x, int n, int_64 S); // returns maximum of x_i, such that i belongs to set S
+LIBDLL_API int_64 UniversalSet(int n);
+LIBDLL_API int Removei_th_bitFromSet(int_64* A, int i);
+
+LIBDLL_API  int_64 choose(int i, int n);
+
+
+
+
+LIBDLL_API int_64 remove1bit(int_64 a, int i);
+// counting fom 0
+
+
+LIBDLL_API int_64 RemoveHighestBit(int_64 a, int K);
+
+LIBDLL_API inline int HasBitsAboveK(int_64 a, int K) { // K counting from 1
+	return(a >= (int_64)1 << K);
+}
+
+LIBDLL_API inline int TopElement(int_64 a) {
+	// return true is a= 11111...
+	return (bitweight(a + 1) == 1);
+}
+
+
+
+#include "fmrandom.h"
+
+
+
+
+
+
+LIBDLL_API void ExpandKinteractive2Bit(double* dest, double* src, int n, int_64 m, int kint, int arraysize);
+LIBDLL_API void ExpandKinteractive2Bit_m(double* dest, double* src, int n, int_64 m, int kint, int arraysize, double* VVC);
+// converts compact k-interactive representation to full length binary ordering. The second call required working memory of size m.
+
+LIBDLL_API unsigned int ShowValue(int_64 s); // shows the elements of a subset as a decimal string (up to 10 elements)
+
+LIBDLL_API double Choquet(double*x, double* v, int n, int_64 m);
+/* Calculates the value of a descrete Choquet integral of x, wrt fuzzy measure v. 
+   Parameters: x array[n] ,v array[m], n, m=2^n 
+   This proceduce requires sorting the array of pairs (v[i],i) in non-decreasing order
+   (perfored by standard STL sort function, and RemoveFromSet() function, to remove
+   an indicated bit from a set (in its binary representation). 
+*/
+
+LIBDLL_API double ChoquetKinter(double*x, double* v, int n, int_64 m, int kint);
+/* As above, but for kinteractive f.m. using compact representation of v  (in cardinality ordering! */
+
+LIBDLL_API double ChoquetMob(double*x, double* Mob, int n, int_64 m);
+/* This is an alternative calculation of the Choquet integral from the Moebius transform v. 
+   It is not as efficient as Choquet(). Provided for testing purposes.
+*/
+
+LIBDLL_API double Sugeno(double*x, double* v, int n, int_64 m);
+/* Calculates the value of a descrete Sugeno integral of x, wrt fuzzy measure v 
+Parameters: x array[n] ,v array[m], n, m=2^n 
+This proceduce requires sorting the array of pairs (v[i],i) in non-decreasing order
+(perfored by standard STL sort function, and RemoveFromSet() function, to remove
+an indicated bit from a set (in its binary representation)
+Also requires maxf and minf functions.
+*/
+
+LIBDLL_API double OWA(double*x, double* v, int n );
+/* Calculates the value of OWA */
+
+LIBDLL_API double WAM(double*x, double* v, int n );
+/* Calculates the value of WAM */
+
+LIBDLL_API void ConstructLambdaMeasure(double *singletons, double *lambda, double *v, int n, int_64 m);
+/* Given the values of the fuzzy measure at singletons, finds the appropriate
+lambda, and constructs the rest of the fuzzy measure. Returns lambda and v at the output
+*/
+
+/* ---------------Operations on fuzzy measures -------------------------*/
+
+LIBDLL_API double Orness(double* Mob, int n, int_64 m); // calculates orness value of a fuzzy measure
+
+LIBDLL_API double Entropy(double* v, int n, int_64 m);// calculates Entropy of a fuzzy measure
+
+LIBDLL_API double OrnessOWA(double* w, int n); // calculates orness value of a fuzzy measure
+
+LIBDLL_API void Mobius(double* v, double* Mob, int n, int_64 m); // calculates Moebius representation of v
+/* the output array w should have the same size 2^n=m as v */
+
+LIBDLL_API void Zeta(double* Mob, double* v, int n, int_64 m);// calculates inverse Moebius transform
+
+LIBDLL_API void Shapley(double* v, double* x, int n, int_64 m); // calculates the array x of Shapley values
+LIBDLL_API void Banzhaf(double* v, double* x, int n, int_64 m);// calculates the array x of Banzhaf indices
+
+LIBDLL_API void ShapleyMob(double* Mob, double* w, int n, int_64 m);
+LIBDLL_API void BanzhafMob(double* Mob, double* w, int n, int_64 m);
+
+LIBDLL_API void InteractionMob(double* Mob, double* w, int_64 m); // calculates all 2^n interaction indices (returned in w)
+LIBDLL_API void InteractionBMob(double* Mob, double* w, int_64 m); // calculates all 2^n Banzhaf interaction indices (returned in w)
+
+LIBDLL_API void NonadditivityIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n nonadditivity indices (returned in w)
+LIBDLL_API void NonadditivityIndexMob(double* Mob, double* w, int n, int_64 m); // calculates  all 2^n nonadditivity indices (returned in w) using Mobius transform
+
+
+LIBDLL_API void NonmodularityIndex(double* v, double* w, int n, int_64 m);
+// calculates  all 2^n nonmodularity indices (returned in w)
+
+LIBDLL_API void NonmodularityIndexMob(double* Mob, double* w, int n, int_64 m);
+// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform
+
+LIBDLL_API void NonmodularityIndexMobkadditive(double* Mob, double* w, int n, int k, int_64 m);
+// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform of 
+//a k-additive FM in cardinality ordering (of length 2^n=m)
+
+LIBDLL_API void NonmodularityIndexKinteractive(double* v, double* w, int n, int kint,int_64 m, int length );
+// the same for k-interactive FM. Requires the length = arraysize of the k-interactive FM. Can be optimised by not calculating many zeros, todo.
+
+LIBDLL_API void BipartitionShapleyIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n bipartition Shapley indices (returned in w)
+LIBDLL_API void BipartitionBanzhafIndex(double* v, double* w, int n, int_64 m); // calculates  all 2^n bipartition Banzhaf indices (returned in w)
+
+LIBDLL_API void dualm(double* v, double* w, int n, int_64 m); // calculates the dual fuzzy measure, returns it in w
+LIBDLL_API void dualMob(myfloat* src, myfloat* dest, int_64 m);  // same using Mobius
+
+// Various queries about a fuzzy measure. All performed with a given tolerance. 
+LIBDLL_API int IsMeasureAdditive(double* v, int n, int_64 m);
+LIBDLL_API int IsMeasureBalanced(double* v, int_64 m);
+LIBDLL_API int IsMeasureSelfdual(double* v, int_64 m);
+LIBDLL_API int IsMeasureSubadditive(double* v, int_64 m);
+LIBDLL_API int IsMeasureSubmodular(double* v, int_64 m);
+LIBDLL_API int IsMeasureSuperadditive(double* v, int_64 m);
+LIBDLL_API int IsMeasureSupermodular(double* v, int_64 m);
+LIBDLL_API int IsMeasureSymmetric(double* v, int n, int_64 m);
+LIBDLL_API int IsMeasureKMaxitive(double* v, int n, int_64 m);
+
+
+
+
+LIBDLL_API void dualMobKadd( myfloat* src, myfloat* dest, int m, int length, int k);
+
+LIBDLL_API void Shapley2addMob(double* v, double* x, int n);
+// calculates the array x of Shapley values for 2 additive fm in compact representation (cardinality based)
+LIBDLL_API void Banzhaf2addMob(double* v, double* x, int n);
+// calculates the array x of Banzhaf indices for 2 additive fm in compact representation (cardinality based)
+
+LIBDLL_API double Choquet2add(double*x, double* Mob, int n);
+// calculates the Choquet integal of x  for 2 additive fm in compact Mobius representation (cardinality based)
+
+LIBDLL_API void random_coefficients(int n, vector<myfloat> & c);
+
+#ifdef FM_SPARSE
+
+/*
+Sparse representation of k-additive capacities. Thre representation is in the form of singletons, pairs and tuples with nonzero values, stored and indexed in the respective 
+arrays (see above in this file)
+
+ Prepares an empty structure, given the list of cardinalities of the nonzero tuples (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
+
+ It is used to allocate storage and later populate these values
+*/
+LIBDLL_API void Prepare_FM_sparse0(int n, int tupsize,  int* tuples, struct SparseFM* cap);
+LIBDLL_API void Prepare_FM_sparse(int n, int tupsize, double *tups, int* tuples, struct SparseFM* cap);
+LIBDLL_API void Free_FM_sparse(struct SparseFM* cap);
+
+/*  Returns the cardinality of the tuple numbered i in the list of tuples */
+LIBDLL_API int TupleCardinalitySparse(int i, struct SparseFM* cap);
+
+LIBDLL_API int  GetNumTuples(struct SparseFM* cap);
+LIBDLL_API int  GetSizeArrayTuples(struct SparseFM* cap);
+
+
+/* checks if element i (1-based!!!) belongs to the tuple indexed A (whose cardinality can be 1,2, other (automatically determined) */
+LIBDLL_API int             IsInSetSparse(int A, int card, int i, struct SparseFM* cap);
+
+/* checks if tuple B is a subset of A */
+LIBDLL_API int             IsSubsetSparse(int A, int cardA, int B, int cardB, struct SparseFM* cap);
+
+/* calculates minimum (maximum) of (x_i) with the indices belonging to tuple indexed as S (its cardinality cardS can be 1,2, other( put 3, will be determined automatically)
+note that x is 0-based, tuples are 1-based */
+LIBDLL_API double min_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap);
+LIBDLL_API double max_subsetSparse(double* x, int n, int S, int cardS, struct SparseFM* cap);
+
+/* calculates the Choquet integral in Mobius representation */
+LIBDLL_API double ChoquetMobSparse(double*x, int n, struct SparseFM* cap);
+
+/* Shapley and Banzhaf values vector of a capacity */
+LIBDLL_API void ShapleyMobSparse(double* v, int n, struct SparseFM* cap);
+LIBDLL_API void BanzhafMobSparse(double* v, int n, struct SparseFM* cap);
+
+LIBDLL_API void NonmodularityIndexMobSparse(double* w, int n, int_64 m, struct SparseFM* cap);
+// calculates  all 2^n nonmodularity indices (returned in w) using Mobius transform of 
+//a k-additive FM in cardinality ordering (of length 2^n=m), using sparse representation
+
+/* populates 2-additive sparse capacity with nonzero values using the singletons and two arrays of indices (of size numpairs) . Indices need to be 1-based. Singletons 0-based */
+LIBDLL_API void PopulateFM2Add_Sparse(double* singletons, int numpairs, double* pairs, int* indicesp1, int* indicesp2, struct SparseFM* cap);
+
+/* for populating capacities. Add pair (v_ij) to the structure. indices are 1-based */
+LIBDLL_API void AddPairSparse(int i, int j, double* v, struct SparseFM* cap);
+/* for populating capacities, adds a tuple of size tupsize whose 1-based indices are in tuple */
+LIBDLL_API void AddTupleSparse(int tupsize, int* tuple, double* v, struct SparseFM* cap);
+
+/* Given 2-additive capacity singletons=pairs in one array v , selects nonzero pairs */
+LIBDLL_API void PopulateFM2Add_Sparse_from2add(int n, double * v, struct SparseFM* cap);
+
+/* from sparse to full representaiotn of 2-additive capacity (singletons and paits, augmented with 0 ) Vector v has to be allocated, size is n+ n(n-1)/2 */
+LIBDLL_API void Expand2AddFull(double* v, struct SparseFM* cap);
+
+/* from sparse to full capacity (vector v, size 2^n has to be preallocated) */
+LIBDLL_API void ExpandSparseFull(double* v, struct SparseFM* cap);
+
+LIBDLL_API void ExportSparseSingletons(int n, double *v, struct SparseFM* cap);
+LIBDLL_API int ExportSparsePairs(int* pairs, double *v, struct SparseFM* cap);
+LIBDLL_API int ExportSparseTuples(int* tuples, double *v, struct SparseFM* cap);
+
+
+/* random generation of  sparse supermodular capacities */
+LIBDLL_API int generate_fm_2additive_convex_sparse(int n, struct SparseFM* cap);
+
+/* this is actually a total monotone, Belief measure */
+LIBDLL_API int generate_fm_kadditive_convex_sparse(int n, int k, int nonzero, struct SparseFM* cap);
+
+
+
+#endif
```

### Comparing `pyfmtools-0.81/src/generaldefs.h` & `pyfmtools-5.1/src/generaldefs.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+#include <stdlib.h>
 #ifndef NO_R
 #define NO_R
 #endif
 #define _CRT_SECURE_NO_WARNINGS
 
 #if defined  (_WIN32)
 #define LIBEXP 	__declspec(dllexport)  
@@ -23,14 +23,36 @@
 
 #if defined (_WIN32)
 #define mystrncpy(a,b,c) strcpy_s(a,c,b)
 #define strdup _strdup
 #else 
 #define mystrncpy(a,b,c) memcpy(a,b,c)
 #endif
+
+
+//#if defined realloc
+//# undef realloc
+//#endif
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+void * GB_realloc(void *ptr,size_t new_size);
+
+#ifdef __cplusplus
+}
+#endif
+
+#ifndef __cplusplus
+#define realloc(ptr,new_size)        GB_realloc(ptr, new_size)
+#endif
+
+
+
 //strncpy(a,c,b)
 
 //typedef int_64 myint;
 //typedef unsigned int myint;
 //typedef uint16_t myint;
 // any of the above, for m<16 use uint_16
```

### Comparing `pyfmtools-0.81/src/hbio.h` & `pyfmtools-5.1/src/hbio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/ini.c` & `pyfmtools-5.1/src/ini.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_BFP.h` & `pyfmtools-5.1/src/lp_BFP.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_BFP1.h` & `pyfmtools-5.1/src/lp_BFP1.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_BFP2.h` & `pyfmtools-5.1/src/lp_BFP2.h`

 * *Files 2% similar despite different names*

```diff
@@ -144,17 +144,17 @@
 
   lu = lp->invB;
 
   if(pcol == NULL)
     pcol = lu->pcol;
 
   if(theta != 0) {
-    register int    i, n = lp->rows;
-    register LREAL  roundzero = lp->epsvalue;
-    register LREAL  *rhs = lp->rhs, rhsmax = 0;
+     int    i, n = lp->rows;
+     LREAL  roundzero = lp->epsvalue;
+     LREAL  *rhs = lp->rhs, rhsmax = 0;
 
     for(i = 0; i <= n; i++, rhs++, pcol++) {
       (*rhs) -= theta * (*pcol);
       my_roundzero(*rhs, roundzero);
       SETMAX(rhsmax, fabs(*rhs));
     }
     lp->rhsmax = rhsmax;
```

### Comparing `pyfmtools-0.81/src/lp_Hash.c` & `pyfmtools-5.1/src/lp_Hash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_Hash.h` & `pyfmtools-5.1/src/lp_Hash.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_LUSOL.c` & `pyfmtools-5.1/src/lp_LUSOL.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_LUSOL.h` & `pyfmtools-5.1/src/lp_LUSOL.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_MDO.c` & `pyfmtools-5.1/src/lp_MDO.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_MPS.c` & `pyfmtools-5.1/src/lp_MPS.c`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,28 @@
 #include "lp_report.h"
 #include "lp_MPS.h"
 
 #ifdef FORTIFY
 # include "lp_fortify.h"
 #endif
 
+#ifndef mysprintf1_M
+int mysprintf1(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+#define mysprintf1_M
+#endif
+
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf1
+
+
 /* Define buffer-size controled function mapping */
 # if defined _MSC_VER
 #  define vsnprintf _vsnprintf
 # endif
 
 /* MPS file input and output routines for lp_solve                           */
 /* ------------------------------------------------------------------------- */
@@ -1156,25 +1170,28 @@
 STATIC char *MPSnameFREE(char *name)
 {
   if(strlen(name) < 8)
     return(MPSnameFIXED(name));
   else
     return(name);
 }
-
+#ifndef WRITEDATA
+#define WRITEDATA
 static void write_data(void *userhandle, write_modeldata_func write_modeldata, char *format, ...)
 {
   char buff[DEF_STRBUFSIZE+1];
   va_list ap;
 
   va_start(ap, format);
   vsnprintf(buff, DEF_STRBUFSIZE, format, ap);
   write_modeldata(userhandle, buff);
   va_end(ap);
 }
+#endif
+
 
 MYBOOL MPS_writefileex(lprec *lp, int typeMPS, void *userhandle, write_modeldata_func write_modeldata)
 {
   int    i, j, jj, je, k, marker, putheader, ChangeSignObj = FALSE, *idx, *idx1;
   MYBOOL ok = TRUE, names_used;
   REAL   a, *val, *val1;
 /* "Output" not defined. Excluded April 19 2006 SEB. */
@@ -1441,19 +1458,22 @@
   write_data(userhandle, write_modeldata, "ENDATA\n");
 
   lp->names_used = names_used;
 
   return(ok);
 }
 
+#ifndef WRITECOMMENT
+#define WRITECOMMENT
 static int __WINAPI write_lpdata(void *userhandle, char *buf)
 {
   fputs(buf, (FILE *) userhandle);
   return(TRUE);
 }
+#endif
 
 MYBOOL MPS_writefile(lprec *lp, int typeMPS, char *filename)
 {
   FILE *output; /* = stdout; */
   MYBOOL ok;
 
   ok = ((output = fopen(filename, "w")) != NULL);
```

### Comparing `pyfmtools-0.81/src/lp_MPS.h` & `pyfmtools-5.1/src/lp_MPS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_SOS.c` & `pyfmtools-5.1/src/lp_SOS.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_SOS.h` & `pyfmtools-5.1/src/lp_SOS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_crash.c` & `pyfmtools-5.1/src/lp_crash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_etaPFI.h` & `pyfmtools-5.1/src/lp_etaPFI.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_explicit.h` & `pyfmtools-5.1/src/lp_explicit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_lib.c` & `pyfmtools-5.1/src/lp_lib.c`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 /*----------------------------------------------------------------------------------- */
 #include <signal.h>
 #include <string.h>
 #include <float.h>
 #include <math.h>
 
 #if LoadInverseLib == TRUE
-  #if defined _MSC_VER  || _WIN32
+  #ifdef WIN32 
     #include <windows.h>
   #else
     #include <dlfcn.h>
   #endif
 #endif
 
 
@@ -81,15 +81,29 @@
 #include "lp_price.h"
 #include "lp_pricePSE.h"
 
 #ifdef FORTIFY
 # include "lp_fortify.h"
 #endif
 
+int mysprintf2(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+
+
+
 
+
+
+
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf2
 /* ---------------------------------------------------------------------------------- */
 /* Define some globals                                                                */
 /* ---------------------------------------------------------------------------------- */
 int callcount = 0;
 
 /* buttrey remove */
 int buttrey_thing = 0;
@@ -1362,15 +1376,15 @@
 {
   lprec *lp;
 
   callcount++;
   if(rows < 0 || columns < 0)
     return(NULL);
 
-  lp = (lprec*) calloc(1, sizeof(*lp));
+  lp = (lprec*) calloc(1, sizeof(lprec));// GB *lp ??
   if(!lp)
     return(NULL);
 
   set_lp_name(lp, NULL);
   lp->names_used    = FALSE;
   lp->use_row_names = TRUE;
   lp->use_col_names = TRUE;
@@ -5024,15 +5038,15 @@
 
   /* Release the BFP and basis if we are active */
   if(lp->invB != NULL)
     bfp_free(lp);
 
 #if LoadInverseLib == TRUE
   if(lp->hBFP != NULL) {
-  #ifdef _WIN32
+  #ifdef WIN32
     FreeLibrary(lp->hBFP);
   #else
     dlclose(lp->hBFP);
   #endif
     lp->hBFP = NULL;
   }
 #endif
@@ -5075,15 +5089,15 @@
     lp->bfp_refactcount = bfp_refactcount;
     lp->bfp_isSetI = bfp_isSetI;
     lp->bfp_findredundant = bfp_findredundant;
 #endif
   }
   else {
 #if LoadInverseLib == TRUE
-  #ifdef _WIN32
+  #ifdef WIN32
    /* Get a handle to the Windows DLL module. */
     lp->hBFP = LoadLibrary(filename);
 
    /* If the handle is valid, try to get the function addresses. */
     if(lp->hBFP != NULL) {
       lp->bfp_compatible           = (BFPbool_lpintintint *)
                                       GetProcAddress(lp->hBFP, "bfp_compatible");
@@ -5380,15 +5394,15 @@
 MYBOOL __WINAPI set_XLI(lprec *lp, char *filename)
 /* (Re)mapping of external language interface variant methods is done here */
 {
   int result = LIB_LOADED;
 
 #if LoadLanguageLib == TRUE
   if(lp->hXLI != NULL) {
-  #ifdef _WIN32
+  #ifdef WIN32
     FreeLibrary(lp->hXLI);
   #else
     dlclose(lp->hXLI);
   #endif
     lp->hXLI = NULL;
   }
 #endif
@@ -5401,15 +5415,15 @@
     lp->xli_compatible = xli_compatible;
     lp->xli_readmodel = xli_readmodel;
     lp->xli_writemodel = xli_writemodel;
 #endif
   }
   else {
 #if LoadLanguageLib == TRUE
-  #ifdef _WIN32
+  #ifdef WIN32
    /* Get a handle to the Windows DLL module. */
     lp->hXLI = LoadLibrary(filename);
 
    /* If the handle is valid, try to get the function addresses. */
     if(lp->hXLI != NULL) {
       lp->xli_compatible           = (XLIbool_lpintintint *)
                                       GetProcAddress(lp->hXLI, "xli_compatible");
@@ -5504,20 +5518,20 @@
 /* Fill vector of basic OF values or subtract incoming values from these.
    This function is called twice during reduced cost updates when the basis
    does not contain the basic OF vector as the top row.  The colno[] array
    is filled with the count of non-zero values and the index to those. */
 {
   int            i, n = lp->rows, nz = 0;
   REAL           *obj = lp->obj;
-  register REAL epsvalue = lp->epsvalue;
+   REAL epsvalue = lp->epsvalue;
 
   /* Compute offset over the specified objective indeces (step 2) */
   if(coltarget != NULL) {
-    register int  ix, m = coltarget[0];
-    register REAL value;
+     int  ix, m = coltarget[0];
+     REAL value;
 
     for(i = 1, coltarget++; i <= m; i++, coltarget++) {
       ix = *coltarget;
       value = -crow[ix];
       if(ix > n)
         value += obj[ix - n];
       crow[ix] = value;
@@ -5528,15 +5542,15 @@
           colno[nz] = ix;
       }
     }
   }
 
   /* Get the basic objective function values (step 1) */
   else {
-    register int *basvar = lp->var_basic;
+     int *basvar = lp->var_basic;
 
     for(i = 1, crow++, basvar++; i <= n;
          i++, crow++, basvar++) {
       if(*basvar <= n)
         *crow = 0;
       else
         *crow = obj[(*basvar) - n];
@@ -7682,15 +7696,15 @@
 }
 
 STATIC int compute_theta(lprec *lp, int rownr, LREAL *theta, int isupbound, REAL HarrisScalar, MYBOOL primal)
 /* The purpose of this routine is to compute the non-basic bound state / value of
    the leaving variable. Note that the incoming theta is "d" in Chvatal-terminology */
 {
   int             colnr = lp->var_basic[rownr];
-  register LREAL x     = lp->rhs[rownr];
+   LREAL x     = lp->rhs[rownr];
   REAL            lb    = 0,  /* Put lower bound here when the fully bounded version is implemented */
                   ub    = lp->upbo[colnr],
                   eps   = lp->epsprimal;  /* Primal feasibility tolerance */
 
   /* Compute theta for the primal simplex */
   HarrisScalar *= eps;
   if(primal) {
```

### Comparing `pyfmtools-0.81/src/lp_lib.h` & `pyfmtools-5.1/src/lp_lib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_matrix.c` & `pyfmtools-5.1/src/lp_matrix.c`

 * *Files 0% similar despite different names*

```diff
@@ -3111,2925 +3111,2921 @@
 0000c260: 7d0a 7d0a 0a53 5441 5449 4320 766f 6964  }.}..STATIC void
 0000c270: 206d 6174 5f6d 756c 7461 6464 284d 4154   mat_multadd(MAT
 0000c280: 7265 6320 2a6d 6174 2c20 5245 414c 202a  rec *mat, REAL *
 0000c290: 6c68 7376 6563 746f 722c 2069 6e74 2076  lhsvector, int v
 0000c2a0: 6172 6e72 2c20 5245 414c 206d 756c 7429  arnr, REAL mult)
 0000c2b0: 0a7b 0a20 2069 6e74 2020 2020 2020 2020  .{.  int        
 0000c2c0: 2020 2020 2020 2063 6f6c 6e72 3b0a 2020         colnr;.  
-0000c2d0: 7265 6769 7374 6572 2069 6e74 2020 2020  register int    
-0000c2e0: 2020 6962 2c20 6965 2c20 2a6d 6174 526f    ib, ie, *matRo
-0000c2f0: 776e 723b 0a20 2072 6567 6973 7465 7220  wnr;.  register 
-0000c300: 5245 414c 2020 2020 202a 6d61 7456 616c  REAL     *matVal
-0000c310: 7565 3b0a 0a20 202f 2a20 4861 6e64 6c65  ue;..  /* Handle
-0000c320: 2063 6173 6520 6f66 2061 2073 6c61 636b   case of a slack
-0000c330: 2076 6172 6961 626c 6520 2a2f 0a20 2069   variable */.  i
-0000c340: 6628 7661 726e 7220 3c3d 206d 6174 2d3e  f(varnr <= mat->
-0000c350: 6c70 2d3e 726f 7773 2920 7b0a 2020 2020  lp->rows) {.    
-0000c360: 6c68 7376 6563 746f 725b 7661 726e 725d  lhsvector[varnr]
-0000c370: 202b 3d20 6d75 6c74 3b0a 2020 2020 7265   += mult;.    re
-0000c380: 7475 726e 3b0a 2020 7d0a 0a20 202f 2a20  turn;.  }..  /* 
-0000c390: 446f 206f 7065 7261 7469 6f6e 206f 6e20  Do operation on 
-0000c3a0: 7468 6520 6f62 6a65 6374 6976 6520 2a2f  the objective */
-0000c3b0: 0a20 2069 6628 6d61 742d 3e6c 702d 3e6d  .  if(mat->lp->m
-0000c3c0: 6174 4120 3d3d 206d 6174 290a 2020 2020  atA == mat).    
-0000c3d0: 6c68 7376 6563 746f 725b 305d 202b 3d20  lhsvector[0] += 
-0000c3e0: 6765 745f 4f46 5f61 6374 6976 6528 6d61  get_OF_active(ma
-0000c3f0: 742d 3e6c 702c 2076 6172 6e72 2c20 6d75  t->lp, varnr, mu
-0000c400: 6c74 293b 0a0a 2020 2f2a 2053 6361 6e20  lt);..  /* Scan 
-0000c410: 7468 6520 636f 6e73 7472 6169 6e74 206d  the constraint m
-0000c420: 6174 7269 7820 7461 7267 6574 2063 6f6c  atrix target col
-0000c430: 756d 6e73 202a 2f0a 2020 636f 6c6e 7220  umns */.  colnr 
-0000c440: 3d20 7661 726e 7220 2d20 6d61 742d 3e6c  = varnr - mat->l
-0000c450: 702d 3e72 6f77 733b 0a20 2069 6220 3d20  p->rows;.  ib = 
-0000c460: 6d61 742d 3e63 6f6c 5f65 6e64 5b63 6f6c  mat->col_end[col
-0000c470: 6e72 202d 2031 5d3b 0a20 2069 6520 3d20  nr - 1];.  ie = 
-0000c480: 6d61 742d 3e63 6f6c 5f65 6e64 5b63 6f6c  mat->col_end[col
-0000c490: 6e72 5d3b 0a20 2069 6628 6962 203c 2069  nr];.  if(ib < i
-0000c4a0: 6529 207b 0a0a 2020 2020 2f2a 2049 6e69  e) {..    /* Ini
-0000c4b0: 7469 616c 697a 6520 706f 696e 7465 7273  tialize pointers
-0000c4c0: 202a 2f0a 2020 2020 6d61 7452 6f77 6e72   */.    matRownr
-0000c4d0: 203d 2026 434f 4c5f 4d41 545f 524f 574e   = &COL_MAT_ROWN
-0000c4e0: 5228 6962 293b 0a20 2020 206d 6174 5661  R(ib);.    matVa
-0000c4f0: 6c75 6520 3d20 2643 4f4c 5f4d 4154 5f56  lue = &COL_MAT_V
-0000c500: 414c 5545 2869 6229 3b0a 0a20 2020 202f  ALUE(ib);..    /
-0000c510: 2a20 5468 656e 206c 6f6f 7020 6f76 6572  * Then loop over
-0000c520: 2061 6c6c 2072 6567 756c 6172 2072 6f77   all regular row
-0000c530: 7320 2a2f 0a20 2020 2066 6f72 283b 2069  s */.    for(; i
-0000c540: 6220 3c20 6965 3b0a 2020 2020 2020 2020  b < ie;.        
-0000c550: 6962 2b2b 2c20 6d61 7456 616c 7565 202b  ib++, matValue +
-0000c560: 3d20 6d61 7456 616c 7565 5374 6570 2c20  = matValueStep, 
-0000c570: 6d61 7452 6f77 6e72 202b 3d20 6d61 7452  matRownr += matR
-0000c580: 6f77 436f 6c53 7465 7029 207b 0a20 2020  owColStep) {.   
-0000c590: 2020 206c 6873 7665 6374 6f72 5b2a 6d61     lhsvector[*ma
-0000c5a0: 7452 6f77 6e72 5d20 2b3d 206d 756c 7420  tRownr] += mult 
-0000c5b0: 2a20 282a 6d61 7456 616c 7565 293b 0a20  * (*matValue);. 
-0000c5c0: 2020 207d 0a20 207d 0a0a 7d0a 0a53 5441     }.  }..}..STA
-0000c5d0: 5449 4320 4d59 424f 4f4c 206d 6174 5f73  TIC MYBOOL mat_s
-0000c5e0: 6574 7661 6c75 6528 4d41 5472 6563 202a  etvalue(MATrec *
-0000c5f0: 6d61 742c 2069 6e74 2052 6f77 2c20 696e  mat, int Row, in
-0000c600: 7420 436f 6c75 6d6e 2c20 5245 414c 2056  t Column, REAL V
-0000c610: 616c 7565 2c20 4d59 424f 4f4c 2064 6f73  alue, MYBOOL dos
-0000c620: 6361 6c65 290a 7b0a 2020 696e 7420 2020  cale).{.  int   
-0000c630: 2065 6c6d 6e72 2c20 6c61 7374 656c 6d2c   elmnr, lastelm,
-0000c640: 2069 2c20 526f 7741 203d 2052 6f77 2c20   i, RowA = Row, 
-0000c650: 436f 6c75 6d6e 4120 3d20 436f 6c75 6d6e  ColumnA = Column
-0000c660: 3b0a 2020 4d59 424f 4f4c 2069 7341 3b0a  ;.  MYBOOL isA;.
-0000c670: 0a20 202f 2a20 5468 6973 2066 756e 6374  .  /* This funct
-0000c680: 696f 6e20 6973 2069 6e65 6666 6963 6965  ion is inefficie
-0000c690: 6e74 2069 6620 7573 6564 2074 6f20 6164  nt if used to ad
-0000c6a0: 6420 6e65 7720 6d61 7472 6978 2065 6e74  d new matrix ent
-0000c6b0: 7269 6573 2069 6e0a 2020 2020 206f 7468  ries in.     oth
-0000c6c0: 6572 2070 6c61 6365 7320 7468 616e 2061  er places than a
-0000c6d0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
-0000c6e0: 206d 6174 7269 782e 204f 4b20 666f 7220   matrix. OK for 
-0000c6f0: 7265 706c 6163 696e 6720 6578 6973 7469  replacing existi
-0000c700: 6e67 0a20 2020 2020 6120 6e6f 6e2d 7a65  ng.     a non-ze
-0000c710: 726f 2076 616c 7565 2077 6974 6820 616e  ro value with an
-0000c720: 6f74 6865 7220 6e6f 6e2d 7a65 726f 2076  other non-zero v
-0000c730: 616c 7565 202a 2f0a 2020 6973 4120 3d20  alue */.  isA = 
-0000c740: 284d 5942 4f4f 4c29 2028 6d61 7420 3d3d  (MYBOOL) (mat ==
-0000c750: 206d 6174 2d3e 6c70 2d3e 6d61 7441 293b   mat->lp->matA);
-0000c760: 0a20 2069 6628 6d61 742d 3e69 735f 726f  .  if(mat->is_ro
-0000c770: 776f 7264 6572 290a 2020 2020 7377 6170  worder).    swap
-0000c780: 494e 5428 2652 6f77 2c20 2643 6f6c 756d  INT(&Row, &Colum
-0000c790: 6e29 3b0a 0a20 202f 2a20 5365 7420 736d  n);..  /* Set sm
-0000c7a0: 616c 6c20 6e75 6d62 6572 7320 746f 207a  all numbers to z
-0000c7b0: 6572 6f20 2a2f 0a20 2069 6628 6661 6273  ero */.  if(fabs
-0000c7c0: 2856 616c 7565 2920 3c20 6d61 742d 3e65  (Value) < mat->e
-0000c7d0: 7073 7661 6c75 6529 0a20 2020 2056 616c  psvalue).    Val
-0000c7e0: 7565 203d 2030 3b0a 2369 6664 6566 2044  ue = 0;.#ifdef D
-0000c7f0: 6f4d 6174 7269 7852 6f75 6e64 696e 670a  oMatrixRounding.
-0000c800: 2020 656c 7365 0a20 2020 2056 616c 7565    else.    Value
-0000c810: 203d 2072 6f75 6e64 546f 5072 6563 6973   = roundToPrecis
-0000c820: 696f 6e28 5661 6c75 652c 206d 6174 2d3e  ion(Value, mat->
-0000c830: 6570 7376 616c 7565 293b 0a23 656e 6469  epsvalue);.#endi
-0000c840: 660a 0a20 202f 2a20 4368 6563 6b20 6966  f..  /* Check if
-0000c850: 2077 6520 6e65 6564 2074 6f20 7570 6461   we need to upda
-0000c860: 7465 2063 6f6c 756d 6e20 7370 6163 6520  te column space 
-0000c870: 2a2f 0a20 2069 6628 436f 6c75 6d6e 203e  */.  if(Column >
-0000c880: 206d 6174 2d3e 636f 6c75 6d6e 7329 207b   mat->columns) {
-0000c890: 0a20 2020 2069 6628 6973 4129 0a20 2020  .    if(isA).   
-0000c8a0: 2020 2069 6e63 5f63 6f6c 5f73 7061 6365     inc_col_space
-0000c8b0: 286d 6174 2d3e 6c70 2c20 436f 6c75 6d6e  (mat->lp, Column
-0000c8c0: 4120 2d20 6d61 742d 3e63 6f6c 756d 6e73  A - mat->columns
-0000c8d0: 293b 0a20 2020 2065 6c73 650a 2020 2020  );.    else.    
-0000c8e0: 2020 696e 635f 6d61 7463 6f6c 5f73 7061    inc_matcol_spa
-0000c8f0: 6365 286d 6174 2c20 436f 6c75 6d6e 202d  ce(mat, Column -
-0000c900: 206d 6174 2d3e 636f 6c75 6d6e 7329 3b0a   mat->columns);.
-0000c910: 2020 7d0a 0a20 202f 2a20 4669 6e64 206f    }..  /* Find o
-0000c920: 7574 2069 6620 7765 2061 6c72 6561 6479  ut if we already
-0000c930: 2068 6176 6520 7375 6368 2061 6e20 656e   have such an en
-0000c940: 7472 792c 206f 7220 7265 7475 726e 2069  try, or return i
-0000c950: 6e73 6572 7469 6f6e 2070 6f69 6e74 202a  nsertion point *
-0000c960: 2f0a 2020 6920 3d20 6d61 745f 6669 6e64  /.  i = mat_find
-0000c970: 696e 7328 6d61 742c 2052 6f77 2c20 436f  ins(mat, Row, Co
-0000c980: 6c75 6d6e 2c20 2665 6c6d 6e72 2c20 4641  lumn, &elmnr, FA
-0000c990: 4c53 4529 3b0a 2020 6966 2869 203d 3d20  LSE);.  if(i == 
-0000c9a0: 2d31 290a 2020 2020 7265 7475 726e 2846  -1).    return(F
-0000c9b0: 414c 5345 293b 0a0a 2020 6966 2869 7341  ALSE);..  if(isA
-0000c9c0: 290a 2020 2020 7365 745f 6163 7469 6f6e  ).    set_action
-0000c9d0: 2826 6d61 742d 3e6c 702d 3e73 7078 5f61  (&mat->lp->spx_a
-0000c9e0: 6374 696f 6e2c 2041 4354 494f 4e5f 5245  ction, ACTION_RE
-0000c9f0: 4241 5345 207c 2041 4354 494f 4e5f 5245  BASE | ACTION_RE
-0000ca00: 434f 4d50 5554 4520 7c20 4143 5449 4f4e  COMPUTE | ACTION
-0000ca10: 5f52 4549 4e56 4552 5429 3b0a 0a20 2069  _REINVERT);..  i
-0000ca20: 6628 6920 3e3d 2030 2920 7b0a 2020 2020  f(i >= 0) {.    
-0000ca30: 2f2a 2074 6865 7265 2069 7320 616e 2065  /* there is an e
-0000ca40: 7869 7374 696e 6720 656e 7472 7920 2a2f  xisting entry */
-0000ca50: 0a20 2020 2069 6628 6661 6273 2856 616c  .    if(fabs(Val
-0000ca60: 7565 2920 3e20 6d61 742d 3e65 7073 7661  ue) > mat->epsva
-0000ca70: 6c75 6529 207b 202f 2a20 7765 2072 6570  lue) { /* we rep
-0000ca80: 6c61 6365 2069 7420 6279 2073 6f6d 6574  lace it by somet
-0000ca90: 6869 6e67 206e 6f6e 2d7a 6572 6f20 2a2f  hing non-zero */
-0000caa0: 0a20 2020 2020 2069 6628 6973 4129 207b  .      if(isA) {
-0000cab0: 0a20 2020 2020 2020 2056 616c 7565 203d  .        Value =
-0000cac0: 206d 795f 6368 7369 676e 2869 735f 6368   my_chsign(is_ch
-0000cad0: 7369 676e 286d 6174 2d3e 6c70 2c20 526f  sign(mat->lp, Ro
-0000cae0: 7741 292c 2056 616c 7565 293b 0a20 2020  wA), Value);.   
-0000caf0: 2020 2020 2069 6628 646f 7363 616c 6520       if(doscale 
-0000cb00: 2626 206d 6174 2d3e 6c70 2d3e 7363 616c  && mat->lp->scal
-0000cb10: 696e 675f 7573 6564 290a 2020 2020 2020  ing_used).      
-0000cb20: 2020 2020 5661 6c75 6520 3d20 7363 616c      Value = scal
-0000cb30: 6564 5f6d 6174 286d 6174 2d3e 6c70 2c20  ed_mat(mat->lp, 
-0000cb40: 5661 6c75 652c 2052 6f77 412c 2043 6f6c  Value, RowA, Col
-0000cb50: 756d 6e41 293b 0a20 2020 2020 207d 0a20  umnA);.      }. 
-0000cb60: 2020 2020 2043 4f4c 5f4d 4154 5f56 414c       COL_MAT_VAL
-0000cb70: 5545 2865 6c6d 6e72 2920 3d20 5661 6c75  UE(elmnr) = Valu
-0000cb80: 653b 0a20 2020 207d 0a20 2020 2065 6c73  e;.    }.    els
-0000cb90: 6520 7b20 2f2a 2073 6574 7469 6e67 2065  e { /* setting e
-0000cba0: 7869 7374 696e 6720 6e6f 6e2d 7a65 726f  xisting non-zero
-0000cbb0: 2065 6e74 7279 2074 6f20 7a65 726f 2e20   entry to zero. 
-0000cbc0: 5265 6d6f 7665 2074 6865 2065 6e74 7279  Remove the entry
-0000cbd0: 202a 2f0a 2020 2020 2020 2f2a 2054 6869   */.      /* Thi
-0000cbe0: 7320 6d69 6768 7420 7265 6d6f 7665 2061  s might remove a
-0000cbf0: 6e20 656e 7469 7265 2063 6f6c 756d 6e2c  n entire column,
-0000cc00: 206f 7220 6c65 6176 6520 6a75 7374 2061   or leave just a
-0000cc10: 2062 6f75 6e64 2e20 4e6f 0a20 2020 2020   bound. No.     
-0000cc20: 2020 2020 206e 6963 6520 736f 6c75 7469       nice soluti
-0000cc30: 6f6e 2066 6f72 2074 6861 7420 7965 7420  on for that yet 
-0000cc40: 2a2f 0a0a 2020 2020 2020 2f2a 2053 6869  */..      /* Shi
-0000cc50: 6674 2075 7020 7461 696c 2065 6e64 206f  ft up tail end o
-0000cc60: 6620 7468 6520 6d61 7472 6978 202a 2f0a  f the matrix */.
-0000cc70: 2020 2020 2020 6c61 7374 656c 6d20 3d20        lastelm = 
-0000cc80: 6d61 745f 6e6f 6e7a 6572 6f73 286d 6174  mat_nonzeros(mat
-0000cc90: 293b 0a23 6966 2030 0a20 2020 2020 2066  );.#if 0.      f
-0000cca0: 6f72 2869 203d 2065 6c6d 6e72 3b20 6920  or(i = elmnr; i 
-0000ccb0: 3c20 6c61 7374 656c 6d20 3b20 692b 2b29  < lastelm ; i++)
-0000ccc0: 207b 0a20 2020 2020 2020 2043 4f4c 5f4d   {.        COL_M
-0000ccd0: 4154 5f43 4f50 5928 692c 2069 202b 2031  AT_COPY(i, i + 1
-0000cce0: 293b 0a20 2020 2020 207d 0a23 656c 7365  );.      }.#else
-0000ccf0: 0a20 2020 2020 206c 6173 7465 6c6d 202d  .      lastelm -
-0000cd00: 3d20 656c 6d6e 723b 0a20 2020 2020 2043  = elmnr;.      C
-0000cd10: 4f4c 5f4d 4154 5f4d 4f56 4528 656c 6d6e  OL_MAT_MOVE(elmn
-0000cd20: 722c 2065 6c6d 6e72 202b 2031 2c20 6c61  r, elmnr + 1, la
-0000cd30: 7374 656c 6d29 3b0a 2365 6e64 6966 0a20  stelm);.#endif. 
-0000cd40: 2020 2020 2066 6f72 2869 203d 2043 6f6c       for(i = Col
-0000cd50: 756d 6e3b 2069 203c 3d20 6d61 742d 3e63  umn; i <= mat->c
-0000cd60: 6f6c 756d 6e73 3b20 692b 2b29 0a20 2020  olumns; i++).   
-0000cd70: 2020 2020 206d 6174 2d3e 636f 6c5f 656e       mat->col_en
-0000cd80: 645b 695d 2d2d 3b0a 0a20 2020 2020 206d  d[i]--;..      m
-0000cd90: 6174 2d3e 726f 775f 656e 645f 7661 6c69  at->row_end_vali
-0000cda0: 6420 3d20 4641 4c53 453b 0a20 2020 207d  d = FALSE;.    }
-0000cdb0: 0a20 207d 0a20 2065 6c73 6520 6966 2866  .  }.  else if(f
-0000cdc0: 6162 7328 5661 6c75 6529 203e 206d 6174  abs(Value) > mat
-0000cdd0: 2d3e 6570 7376 616c 7565 2920 7b0a 2020  ->epsvalue) {.  
-0000cde0: 2020 2f2a 206e 6f20 6578 6973 7469 6e67    /* no existing
-0000cdf0: 2065 6e74 7279 2e20 6d61 6b65 206e 6577   entry. make new
-0000ce00: 206f 6e65 206f 6e6c 7920 6966 206e 6f74   one only if not
-0000ce10: 206e 6561 726c 7920 7a65 726f 202a 2f0a   nearly zero */.
-0000ce20: 2020 2020 2f2a 2063 6865 636b 2069 6620      /* check if 
-0000ce30: 6d6f 7265 2073 7061 6365 2069 7320 6e65  more space is ne
-0000ce40: 6564 6564 2066 6f72 206d 6174 7269 7820  eded for matrix 
-0000ce50: 2a2f 0a20 2020 2069 6628 2169 6e63 5f6d  */.    if(!inc_m
-0000ce60: 6174 5f73 7061 6365 286d 6174 2c20 3129  at_space(mat, 1)
-0000ce70: 290a 2020 2020 2020 7265 7475 726e 2846  ).      return(F
-0000ce80: 414c 5345 293b 0a0a 2020 2020 6966 2843  ALSE);..    if(C
-0000ce90: 6f6c 756d 6e20 3e20 6d61 742d 3e63 6f6c  olumn > mat->col
-0000cea0: 756d 6e73 2920 7b0a 2020 2020 2020 6920  umns) {.      i 
-0000ceb0: 3d20 6d61 742d 3e63 6f6c 756d 6e73 202b  = mat->columns +
-0000cec0: 2031 3b0a 2020 2020 2020 6966 2869 7341   1;.      if(isA
-0000ced0: 290a 2020 2020 2020 2020 7368 6966 745f  ).        shift_
-0000cee0: 636f 6c64 6174 6128 6d61 742d 3e6c 702c  coldata(mat->lp,
-0000cef0: 2069 2c20 436f 6c75 6d6e 4120 2d20 6d61   i, ColumnA - ma
-0000cf00: 742d 3e63 6f6c 756d 6e73 2c20 4e55 4c4c  t->columns, NULL
-0000cf10: 293b 0a20 2020 2020 2065 6c73 650a 2020  );.      else.  
-0000cf20: 2020 2020 2020 6d61 745f 7368 6966 7463        mat_shiftc
-0000cf30: 6f6c 7328 6d61 742c 2026 692c 2043 6f6c  ols(mat, &i, Col
-0000cf40: 756d 6e20 2d20 6d61 742d 3e63 6f6c 756d  umn - mat->colum
-0000cf50: 6e73 2c20 4e55 4c4c 293b 0a20 2020 207d  ns, NULL);.    }
-0000cf60: 0a0a 2020 2020 2f2a 2053 6869 6674 2064  ..    /* Shift d
-0000cf70: 6f77 6e20 7461 696c 2065 6e64 206f 6620  own tail end of 
-0000cf80: 7468 6520 6d61 7472 6978 2062 7920 6f6e  the matrix by on
-0000cf90: 6520 2a2f 0a20 2020 206c 6173 7465 6c6d  e */.    lastelm
-0000cfa0: 203d 206d 6174 5f6e 6f6e 7a65 726f 7328   = mat_nonzeros(
-0000cfb0: 6d61 7429 3b0a 2369 6620 3120 2f2a 2044  mat);.#if 1 /* D
-0000cfc0: 6f65 7320 636f 6d70 696c 6572 206f 7074  oes compiler opt
-0000cfd0: 696d 697a 6174 696f 6e20 776f 726b 2062  imization work b
-0000cfe0: 6574 7465 7220 6865 7265 3f20 2a2f 0a20  etter here? */. 
-0000cff0: 2020 2066 6f72 2869 203d 206c 6173 7465     for(i = laste
-0000d000: 6c6d 3b20 6920 3e20 656c 6d6e 7220 3b20  lm; i > elmnr ; 
-0000d010: 692d 2d29 207b 0a20 2020 2020 2043 4f4c  i--) {.      COL
-0000d020: 5f4d 4154 5f43 4f50 5928 692c 2069 202d  _MAT_COPY(i, i -
-0000d030: 2031 293b 0a20 2020 207d 0a23 656c 7365   1);.    }.#else
-0000d040: 0a20 2020 206c 6173 7465 6c6d 202d 3d20  .    lastelm -= 
-0000d050: 656c 6d6e 7220 2d20 313b 0a20 2020 2043  elmnr - 1;.    C
-0000d060: 4f4c 5f4d 4154 5f4d 4f56 4528 656c 6d6e  OL_MAT_MOVE(elmn
-0000d070: 7220 2b20 312c 2065 6c6d 6e72 2c20 6c61  r + 1, elmnr, la
-0000d080: 7374 656c 6d29 3b0a 2365 6e64 6966 0a0a  stelm);.#endif..
-0000d090: 2020 2020 2f2a 2053 6574 206e 6577 2065      /* Set new e
-0000d0a0: 6c65 6d65 6e74 202a 2f0a 2020 2020 6966  lement */.    if
-0000d0b0: 2869 7341 2920 7b0a 2020 2020 2020 5661  (isA) {.      Va
-0000d0c0: 6c75 6520 3d20 6d79 5f63 6873 6967 6e28  lue = my_chsign(
-0000d0d0: 6973 5f63 6873 6967 6e28 6d61 742d 3e6c  is_chsign(mat->l
-0000d0e0: 702c 2052 6f77 4129 2c20 5661 6c75 6529  p, RowA), Value)
-0000d0f0: 3b0a 2020 2020 2020 6966 2864 6f73 6361  ;.      if(dosca
-0000d100: 6c65 290a 2020 2020 2020 2020 5661 6c75  le).        Valu
-0000d110: 6520 3d20 7363 616c 6564 5f6d 6174 286d  e = scaled_mat(m
-0000d120: 6174 2d3e 6c70 2c20 5661 6c75 652c 2052  at->lp, Value, R
-0000d130: 6f77 412c 2043 6f6c 756d 6e41 293b 0a20  owA, ColumnA);. 
-0000d140: 2020 207d 0a20 2020 2053 4554 5f4d 4154     }.    SET_MAT
-0000d150: 5f69 6a41 2865 6c6d 6e72 2c20 526f 772c  _ijA(elmnr, Row,
-0000d160: 2043 6f6c 756d 6e2c 2056 616c 7565 293b   Column, Value);
-0000d170: 0a0a 2020 2020 2f2a 2055 7064 6174 6520  ..    /* Update 
-0000d180: 636f 6c75 6d6e 2069 6e64 6578 6573 202a  column indexes *
-0000d190: 2f0a 2020 2020 666f 7228 6920 3d20 436f  /.    for(i = Co
-0000d1a0: 6c75 6d6e 3b20 6920 3c3d 206d 6174 2d3e  lumn; i <= mat->
-0000d1b0: 636f 6c75 6d6e 733b 2069 2b2b 290a 2020  columns; i++).  
-0000d1c0: 2020 2020 6d61 742d 3e63 6f6c 5f65 6e64      mat->col_end
-0000d1d0: 5b69 5d2b 2b3b 0a0a 2020 2020 6d61 742d  [i]++;..    mat-
-0000d1e0: 3e72 6f77 5f65 6e64 5f76 616c 6964 203d  >row_end_valid =
-0000d1f0: 2046 414c 5345 3b0a 2020 7d0a 0a20 2069   FALSE;.  }..  i
-0000d200: 6628 6973 4120 2626 2028 6d61 742d 3e6c  f(isA && (mat->l
-0000d210: 702d 3e76 6172 5f69 735f 6672 6565 2021  p->var_is_free !
-0000d220: 3d20 4e55 4c4c 2920 2626 2028 6d61 742d  = NULL) && (mat-
-0000d230: 3e6c 702d 3e76 6172 5f69 735f 6672 6565  >lp->var_is_free
-0000d240: 5b43 6f6c 756d 6e41 5d20 3e20 3029 290a  [ColumnA] > 0)).
-0000d250: 2020 2020 7265 7475 726e 2820 6d61 745f      return( mat_
-0000d260: 7365 7476 616c 7565 286d 6174 2c20 526f  setvalue(mat, Ro
-0000d270: 7741 2c20 6d61 742d 3e6c 702d 3e76 6172  wA, mat->lp->var
-0000d280: 5f69 735f 6672 6565 5b43 6f6c 756d 6e41  _is_free[ColumnA
-0000d290: 5d2c 202d 5661 6c75 652c 2064 6f73 6361  ], -Value, dosca
-0000d2a0: 6c65 2920 293b 0a20 2072 6574 7572 6e28  le) );.  return(
-0000d2b0: 5452 5545 293b 0a7d 0a0a 5354 4154 4943  TRUE);.}..STATIC
-0000d2c0: 204d 5942 4f4f 4c20 6d61 745f 6170 7065   MYBOOL mat_appe
-0000d2d0: 6e64 7661 6c75 6528 4d41 5472 6563 202a  ndvalue(MATrec *
-0000d2e0: 6d61 742c 2069 6e74 2052 6f77 2c20 5245  mat, int Row, RE
-0000d2f0: 414c 2056 616c 7565 290a 7b0a 2020 696e  AL Value).{.  in
-0000d300: 7420 2a65 6c6d 6e72 2c20 436f 6c75 6d6e  t *elmnr, Column
-0000d310: 203d 206d 6174 2d3e 636f 6c75 6d6e 733b   = mat->columns;
-0000d320: 0a0a 2020 2f2a 2053 6574 2073 6d61 6c6c  ..  /* Set small
-0000d330: 206e 756d 6265 7273 2074 6f20 7a65 726f   numbers to zero
-0000d340: 202a 2f0a 2020 6966 2866 6162 7328 5661   */.  if(fabs(Va
-0000d350: 6c75 6529 203c 206d 6174 2d3e 6570 7376  lue) < mat->epsv
-0000d360: 616c 7565 290a 2020 2020 5661 6c75 6520  alue).    Value 
-0000d370: 3d20 303b 0a23 6966 6465 6620 446f 4d61  = 0;.#ifdef DoMa
-0000d380: 7472 6978 526f 756e 6469 6e67 0a20 2065  trixRounding.  e
-0000d390: 6c73 650a 2020 2020 5661 6c75 6520 3d20  lse.    Value = 
-0000d3a0: 726f 756e 6454 6f50 7265 6369 7369 6f6e  roundToPrecision
-0000d3b0: 2856 616c 7565 2c20 6d61 742d 3e65 7073  (Value, mat->eps
-0000d3c0: 7661 6c75 6529 3b0a 2365 6e64 6966 0a0a  value);.#endif..
-0000d3d0: 2020 2f2a 2043 6865 636b 2069 6620 6d6f    /* Check if mo
-0000d3e0: 7265 2073 7061 6365 2069 7320 6e65 6564  re space is need
-0000d3f0: 6564 2066 6f72 206d 6174 7269 7820 2a2f  ed for matrix */
-0000d400: 0a20 2069 6628 2169 6e63 5f6d 6174 5f73  .  if(!inc_mat_s
-0000d410: 7061 6365 286d 6174 2c20 3129 290a 2020  pace(mat, 1)).  
-0000d420: 2020 7265 7475 726e 2846 414c 5345 293b    return(FALSE);
-0000d430: 0a0a 2369 6664 6566 2050 6172 616e 6f69  ..#ifdef Paranoi
-0000d440: 610a 2020 2f2a 2043 6865 636b 2076 616c  a.  /* Check val
-0000d450: 6964 2069 6e64 6563 6573 202a 2f0a 2020  id indeces */.  
-0000d460: 6966 2828 526f 7720 3c20 3029 207c 7c20  if((Row < 0) || 
-0000d470: 2852 6f77 203e 206d 6174 2d3e 726f 7773  (Row > mat->rows
-0000d480: 2929 207b 0a20 2020 2072 6570 6f72 7428  )) {.    report(
-0000d490: 6d61 742d 3e6c 702c 2053 4556 4552 452c  mat->lp, SEVERE,
-0000d4a0: 2022 6d61 745f 6170 7065 6e64 7661 6c75   "mat_appendvalu
-0000d4b0: 653a 2049 6e76 616c 6964 2072 6f77 2069  e: Invalid row i
-0000d4c0: 6e64 6578 2025 6420 7370 6563 6966 6965  ndex %d specifie
-0000d4d0: 645c 6e22 2c20 526f 7729 3b0a 2020 2020  d\n", Row);.    
-0000d4e0: 7265 7475 726e 2846 414c 5345 293b 0a20  return(FALSE);. 
-0000d4f0: 207d 0a23 656e 6469 660a 0a20 202f 2a20   }.#endif..  /* 
-0000d500: 4765 7420 696e 7365 7274 696f 6e20 706f  Get insertion po
-0000d510: 696e 7420 616e 6420 7365 7420 7661 6c75  int and set valu
-0000d520: 6520 2a2f 0a20 2065 6c6d 6e72 203d 206d  e */.  elmnr = m
-0000d530: 6174 2d3e 636f 6c5f 656e 6420 2b20 436f  at->col_end + Co
-0000d540: 6c75 6d6e 3b0a 2020 5345 545f 4d41 545f  lumn;.  SET_MAT_
-0000d550: 696a 4128 282a 656c 6d6e 7229 2c20 526f  ijA((*elmnr), Ro
-0000d560: 772c 2043 6f6c 756d 6e2c 2056 616c 7565  w, Column, Value
-0000d570: 293b 0a0a 2020 2f2a 2055 7064 6174 6520  );..  /* Update 
-0000d580: 636f 6c75 6d6e 2063 6f75 6e74 202a 2f0a  column count */.
-0000d590: 2020 282a 656c 6d6e 7229 2b2b 3b0a 2020    (*elmnr)++;.  
-0000d5a0: 6d61 742d 3e72 6f77 5f65 6e64 5f76 616c  mat->row_end_val
-0000d5b0: 6964 203d 2046 414c 5345 3b0a 0a20 2072  id = FALSE;..  r
-0000d5c0: 6574 7572 6e28 5452 5545 293b 0a7d 0a0a  eturn(TRUE);.}..
-0000d5d0: 5354 4154 4943 204d 5942 4f4f 4c20 6d61  STATIC MYBOOL ma
-0000d5e0: 745f 6571 7561 6c52 6f77 7328 4d41 5472  t_equalRows(MATr
-0000d5f0: 6563 202a 6d61 742c 2069 6e74 2062 6173  ec *mat, int bas
-0000d600: 6572 6f77 2c20 696e 7420 636f 6d70 726f  erow, int compro
-0000d610: 7729 0a7b 0a20 204d 5942 4f4f 4c20 7374  w).{.  MYBOOL st
-0000d620: 6174 7573 203d 2046 414c 5345 3b0a 0a20  atus = FALSE;.. 
-0000d630: 2069 6628 6d61 745f 7661 6c69 6461 7465   if(mat_validate
-0000d640: 286d 6174 2929 207b 0a20 2020 2069 6e74  (mat)) {.    int
-0000d650: 2062 6a31 203d 2030 2c20 656a 312c 2062   bj1 = 0, ej1, b
-0000d660: 6a32 203d 2030 2c20 656a 323b 0a0a 2020  j2 = 0, ej2;..  
-0000d670: 2020 2f2a 2047 6574 2073 7461 7274 696e    /* Get startin
-0000d680: 6720 616e 6420 656e 6469 6e67 2070 6f73  g and ending pos
-0000d690: 6974 696f 6e73 202a 2f0a 2020 2020 6966  itions */.    if
-0000d6a0: 2862 6173 6572 6f77 203e 3d20 3029 0a20  (baserow >= 0). 
-0000d6b0: 2020 2020 2062 6a31 203d 206d 6174 2d3e       bj1 = mat->
-0000d6c0: 726f 775f 656e 645b 6261 7365 726f 772d  row_end[baserow-
-0000d6d0: 315d 3b0a 2020 2020 656a 3120 3d20 6d61  1];.    ej1 = ma
-0000d6e0: 742d 3e72 6f77 5f65 6e64 5b62 6173 6572  t->row_end[baser
-0000d6f0: 6f77 5d3b 0a20 2020 2069 6628 636f 6d70  ow];.    if(comp
-0000d700: 726f 7720 3e3d 2030 290a 2020 2020 2020  row >= 0).      
-0000d710: 626a 3220 3d20 6d61 742d 3e72 6f77 5f65  bj2 = mat->row_e
-0000d720: 6e64 5b63 6f6d 7072 6f77 2d31 5d3b 0a20  nd[comprow-1];. 
-0000d730: 2020 2065 6a32 203d 206d 6174 2d3e 726f     ej2 = mat->ro
-0000d740: 775f 656e 645b 636f 6d70 726f 775d 3b0a  w_end[comprow];.
-0000d750: 2020 2020 2f2a 2046 6169 6c20 6966 2072      /* Fail if r
-0000d760: 6f77 206c 656e 6774 6873 2061 7265 2075  ow lengths are u
-0000d770: 6e65 7175 616c 202a 2f0a 2020 2020 6966  nequal */.    if
-0000d780: 2828 656a 312d 626a 3129 2021 3d20 2865  ((ej1-bj1) != (e
-0000d790: 6a32 2d62 6a32 2929 0a20 2020 2020 2072  j2-bj2)).      r
-0000d7a0: 6574 7572 6e28 2073 7461 7475 7320 293b  eturn( status );
-0000d7b0: 0a0a 2020 2020 2f2a 2043 6f6d 7061 7265  ..    /* Compare
-0000d7c0: 2063 6f6c 756d 6e20 696e 6465 7820 616e   column index an
-0000d7d0: 6420 7661 6c75 652c 2065 6c65 6d65 6e74  d value, element
-0000d7e0: 2062 7920 656c 656d 656e 7420 2a2f 0a20   by element */. 
-0000d7f0: 2020 2066 6f72 283b 2062 6a31 203c 2065     for(; bj1 < e
-0000d800: 6a31 3b20 626a 312b 2b2c 2062 6a32 2b2b  j1; bj1++, bj2++
-0000d810: 2920 7b0a 2020 2020 2020 6966 2843 4f4c  ) {.      if(COL
-0000d820: 5f4d 4154 5f43 4f4c 4e52 2862 6a31 2920  _MAT_COLNR(bj1) 
-0000d830: 213d 2043 4f4c 5f4d 4154 5f43 4f4c 4e52  != COL_MAT_COLNR
-0000d840: 2862 6a32 2929 0a20 2020 2020 2020 2062  (bj2)).        b
-0000d850: 7265 616b 3b0a 2369 6620 310a 2020 2020  reak;.#if 1.    
-0000d860: 2020 6966 2866 6162 7328 6765 745f 6d61    if(fabs(get_ma
-0000d870: 745f 6279 696e 6465 7828 6d61 742d 3e6c  t_byindex(mat->l
-0000d880: 702c 2062 6a31 2c20 5452 5545 2c20 4641  p, bj1, TRUE, FA
-0000d890: 4c53 4529 2d67 6574 5f6d 6174 5f62 7969  LSE)-get_mat_byi
-0000d8a0: 6e64 6578 286d 6174 2d3e 6c70 2c20 626a  ndex(mat->lp, bj
-0000d8b0: 322c 2054 5255 452c 2046 414c 5345 2929  2, TRUE, FALSE))
-0000d8c0: 203e 206d 6174 2d3e 6c70 2d3e 6570 7370   > mat->lp->epsp
-0000d8d0: 7269 6d61 6c29 0a23 656c 7365 0a20 2020  rimal).#else.   
-0000d8e0: 2020 2069 6628 6661 6273 2843 4f4c 5f4d     if(fabs(COL_M
-0000d8f0: 4154 5f56 414c 5545 2862 6a31 292d 434f  AT_VALUE(bj1)-CO
-0000d900: 4c5f 4d41 545f 5641 4c55 4528 626a 3229  L_MAT_VALUE(bj2)
-0000d910: 2920 3e20 6d61 742d 3e6c 702d 3e65 7073  ) > mat->lp->eps
-0000d920: 7072 696d 616c 290a 2365 6e64 6966 0a20  primal).#endif. 
-0000d930: 2020 2020 2020 2062 7265 616b 3b0a 2020         break;.  
-0000d940: 2020 7d0a 2020 2020 7374 6174 7573 203d    }.    status =
-0000d950: 2028 4d59 424f 4f4c 2920 2862 6a31 203d   (MYBOOL) (bj1 =
-0000d960: 3d20 656a 3129 3b0a 2020 7d0a 2020 7265  = ej1);.  }.  re
-0000d970: 7475 726e 2820 7374 6174 7573 2029 3b0a  turn( status );.
-0000d980: 7d0a 0a53 5441 5449 4320 696e 7420 6d61  }..STATIC int ma
-0000d990: 745f 6669 6e64 636f 6c75 6d6e 284d 4154  t_findcolumn(MAT
-0000d9a0: 7265 6320 2a6d 6174 2c20 696e 7420 6d61  rec *mat, int ma
-0000d9b0: 7469 6e64 6578 290a 7b0a 2020 696e 7420  tindex).{.  int 
-0000d9c0: 6a3b 0a0a 2020 666f 7228 6a20 3d20 313b  j;..  for(j = 1;
-0000d9d0: 206a 203c 3d20 6d61 742d 3e63 6f6c 756d   j <= mat->colum
-0000d9e0: 6e73 3b20 6a2b 2b29 207b 0a20 2020 2069  ns; j++) {.    i
-0000d9f0: 6628 6d61 7469 6e64 6578 203c 206d 6174  f(matindex < mat
-0000da00: 2d3e 636f 6c5f 656e 645b 6a5d 290a 2020  ->col_end[j]).  
-0000da10: 2020 2020 6272 6561 6b3b 0a20 207d 0a20      break;.  }. 
-0000da20: 2072 6574 7572 6e28 6a29 3b0a 7d0a 0a53   return(j);.}..S
-0000da30: 5441 5449 4320 696e 7420 6d61 745f 6578  TATIC int mat_ex
-0000da40: 7061 6e64 636f 6c75 6d6e 284d 4154 7265  pandcolumn(MATre
-0000da50: 6320 2a6d 6174 2c20 696e 7420 636f 6c6e  c *mat, int coln
-0000da60: 722c 2052 4541 4c20 2a63 6f6c 756d 6e2c  r, REAL *column,
-0000da70: 2069 6e74 202a 6e7a 6c69 7374 2c20 4d59   int *nzlist, MY
-0000da80: 424f 4f4c 2073 6967 6e65 6441 290a 7b0a  BOOL signedA).{.
-0000da90: 2020 4d59 424f 4f4c 2020 6973 4120 3d20    MYBOOL  isA = 
-0000daa0: 284d 5942 4f4f 4c29 2028 6d61 742d 3e6c  (MYBOOL) (mat->l
-0000dab0: 702d 3e6d 6174 4120 3d3d 206d 6174 293b  p->matA == mat);
-0000dac0: 0a20 2069 6e74 2020 2020 2069 2c20 6965  .  int     i, ie
-0000dad0: 2c20 6a2c 206e 7a63 6f75 6e74 203d 2030  , j, nzcount = 0
-0000dae0: 3b0a 2020 5245 414c 2020 2020 2a6d 6174  ;.  REAL    *mat
-0000daf0: 5661 6c75 653b 0a20 2069 6e74 2020 2020  Value;.  int    
-0000db00: 202a 6d61 7452 6f77 6e72 3b0a 0a20 2073   *matRownr;..  s
-0000db10: 6967 6e65 6441 2026 3d20 6973 413b 0a0a  ignedA &= isA;..
-0000db20: 2020 2f2a 2052 6574 7269 6576 6520 6120    /* Retrieve a 
-0000db30: 636f 6c75 6d6e 2066 726f 6d20 7468 6520  column from the 
-0000db40: 7573 6572 2064 6174 6120 6d61 7472 6978  user data matrix
-0000db50: 2041 202a 2f0a 2020 4d45 4d43 4c45 4152   A */.  MEMCLEAR
-0000db60: 2863 6f6c 756d 6e2c 206d 6174 2d3e 726f  (column, mat->ro
-0000db70: 7773 202b 2031 293b 0a20 2069 6628 6973  ws + 1);.  if(is
-0000db80: 4129 207b 0a20 2020 2063 6f6c 756d 6e5b  A) {.    column[
-0000db90: 305d 203d 206d 6174 2d3e 6c70 2d3e 6f72  0] = mat->lp->or
-0000dba0: 6967 5f6f 626a 5b63 6f6c 6e72 5d3b 0a20  ig_obj[colnr];. 
-0000dbb0: 2020 2069 6628 7369 676e 6564 4120 2626     if(signedA &&
-0000dbc0: 2069 735f 6368 7369 676e 286d 6174 2d3e   is_chsign(mat->
-0000dbd0: 6c70 2c20 3029 290a 2020 2020 2020 636f  lp, 0)).      co
-0000dbe0: 6c75 6d6e 5b30 5d20 3d20 2d63 6f6c 756d  lumn[0] = -colum
-0000dbf0: 6e5b 305d 3b0a 2020 7d0a 0a20 2069 203d  n[0];.  }..  i =
-0000dc00: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
-0000dc10: 6c6e 7220 2d20 315d 3b0a 2020 6965 203d  lnr - 1];.  ie =
-0000dc20: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
-0000dc30: 6c6e 725d 3b0a 2020 6d61 7452 6f77 6e72  lnr];.  matRownr
-0000dc40: 203d 2026 434f 4c5f 4d41 545f 524f 574e   = &COL_MAT_ROWN
-0000dc50: 5228 6929 3b0a 2020 6d61 7456 616c 7565  R(i);.  matValue
-0000dc60: 203d 2026 434f 4c5f 4d41 545f 5641 4c55   = &COL_MAT_VALU
-0000dc70: 4528 6929 3b0a 2020 666f 7228 3b20 6920  E(i);.  for(; i 
-0000dc80: 3c20 6965 3b0a 2020 2020 2020 692b 2b2c  < ie;.      i++,
-0000dc90: 206d 6174 526f 776e 7220 2b3d 206d 6174   matRownr += mat
-0000dca0: 526f 7743 6f6c 5374 6570 2c20 6d61 7456  RowColStep, matV
-0000dcb0: 616c 7565 202b 3d20 6d61 7456 616c 7565  alue += matValue
-0000dcc0: 5374 6570 2920 7b0a 2020 2020 6a20 3d20  Step) {.    j = 
-0000dcd0: 2a6d 6174 526f 776e 723b 0a20 2020 2063  *matRownr;.    c
-0000dce0: 6f6c 756d 6e5b 6a5d 203d 202a 6d61 7456  olumn[j] = *matV
-0000dcf0: 616c 7565 3b0a 2020 2020 6966 2873 6967  alue;.    if(sig
-0000dd00: 6e65 6441 2026 2620 6973 5f63 6873 6967  nedA && is_chsig
-0000dd10: 6e28 6d61 742d 3e6c 702c 206a 2929 0a20  n(mat->lp, j)). 
-0000dd20: 2020 2020 2063 6f6c 756d 6e5b 6a5d 203d       column[j] =
-0000dd30: 202d 636f 6c75 6d6e 5b6a 5d3b 0a20 2020   -column[j];.   
-0000dd40: 206e 7a63 6f75 6e74 2b2b 3b0a 2020 2020   nzcount++;.    
-0000dd50: 6966 286e 7a6c 6973 7420 213d 204e 554c  if(nzlist != NUL
-0000dd60: 4c29 0a20 2020 2020 206e 7a6c 6973 745b  L).      nzlist[
-0000dd70: 6e7a 636f 756e 745d 203d 206a 3b0a 2020  nzcount] = j;.  
-0000dd80: 7d0a 2020 6966 286e 7a6c 6973 7420 213d  }.  if(nzlist !=
-0000dd90: 204e 554c 4c29 0a20 2020 206e 7a6c 6973   NULL).    nzlis
-0000dda0: 745b 305d 203d 206e 7a63 6f75 6e74 3b0a  t[0] = nzcount;.
-0000ddb0: 2020 7265 7475 726e 2820 6e7a 636f 756e    return( nzcoun
-0000ddc0: 7420 293b 0a7d 0a0a 5354 4154 4943 204d  t );.}..STATIC M
-0000ddd0: 5942 4f4f 4c20 6d61 745f 636f 6d70 7574  YBOOL mat_comput
-0000dde0: 656d 6178 284d 4154 7265 6320 2a6d 6174  emax(MATrec *mat
-0000ddf0: 290a 7b0a 2020 696e 7420 202a 726f 776e  ).{.  int  *rown
-0000de00: 7220 3d20 2643 4f4c 5f4d 4154 5f52 4f57  r = &COL_MAT_ROW
-0000de10: 4e52 2830 292c 0a20 2020 2020 2020 2a63  NR(0),.       *c
-0000de20: 6f6c 6e72 203d 2026 434f 4c5f 4d41 545f  olnr = &COL_MAT_
-0000de30: 434f 4c4e 5228 3029 2c0a 2020 2020 2020  COLNR(0),.      
-0000de40: 2069 203d 2030 2c20 6965 203d 206d 6174   i = 0, ie = mat
-0000de50: 2d3e 636f 6c5f 656e 645b 6d61 742d 3e63  ->col_end[mat->c
-0000de60: 6f6c 756d 6e73 5d2c 2065 7a20 3d20 303b  olumns], ez = 0;
-0000de70: 0a20 2052 4541 4c20 2a76 616c 7565 203d  .  REAL *value =
-0000de80: 2026 434f 4c5f 4d41 545f 5641 4c55 4528   &COL_MAT_VALUE(
-0000de90: 3029 2c20 6570 736d 6163 6869 6e65 203d  0), epsmachine =
-0000dea0: 206d 6174 2d3e 6c70 2d3e 6570 736d 6163   mat->lp->epsmac
-0000deb0: 6869 6e65 2c20 6162 7376 616c 7565 3b0a  hine, absvalue;.
-0000dec0: 0a20 202f 2a20 5072 6570 6172 6520 6172  .  /* Prepare ar
-0000ded0: 7261 7973 202a 2f0a 2020 6966 2821 616c  rays */.  if(!al
-0000dee0: 6c6f 6352 4541 4c28 6d61 742d 3e6c 702c  locREAL(mat->lp,
-0000def0: 2026 6d61 742d 3e63 6f6c 6d61 782c 206d   &mat->colmax, m
-0000df00: 6174 2d3e 636f 6c75 6d6e 735f 616c 6c6f  at->columns_allo
-0000df10: 632b 312c 2041 5554 4f4d 4154 4943 2920  c+1, AUTOMATIC) 
-0000df20: 7c7c 0a20 2020 2020 2161 6c6c 6f63 5245  ||.     !allocRE
-0000df30: 414c 286d 6174 2d3e 6c70 2c20 266d 6174  AL(mat->lp, &mat
-0000df40: 2d3e 726f 776d 6178 2c20 6d61 742d 3e72  ->rowmax, mat->r
-0000df50: 6f77 735f 616c 6c6f 632b 312c 2041 5554  ows_alloc+1, AUT
-0000df60: 4f4d 4154 4943 2929 0a20 2020 2020 7265  OMATIC)).     re
-0000df70: 7475 726e 2820 4641 4c53 4520 293b 0a20  turn( FALSE );. 
-0000df80: 204d 454d 434c 4541 5228 6d61 742d 3e63   MEMCLEAR(mat->c
-0000df90: 6f6c 6d61 782c 206d 6174 2d3e 636f 6c75  olmax, mat->colu
-0000dfa0: 6d6e 732b 3129 3b0a 2020 4d45 4d43 4c45  mns+1);.  MEMCLE
-0000dfb0: 4152 286d 6174 2d3e 726f 776d 6178 2c20  AR(mat->rowmax, 
-0000dfc0: 6d61 742d 3e72 6f77 732b 3129 3b0a 0a20  mat->rows+1);.. 
-0000dfd0: 202f 2a20 4f62 7461 696e 2074 6865 2072   /* Obtain the r
-0000dfe0: 6f77 2061 6e64 2063 6f6c 756d 6e20 6d61  ow and column ma
-0000dff0: 7869 6d61 2069 6e20 6f6e 6520 7377 6565  xima in one swee
-0000e000: 7020 2a2f 0a20 206d 6174 2d3e 6479 6e72  p */.  mat->dynr
-0000e010: 616e 6765 203d 206d 6174 2d3e 6c70 2d3e  ange = mat->lp->
-0000e020: 696e 6669 6e69 7465 3b0a 2020 666f 7228  infinite;.  for(
-0000e030: 3b20 6920 3c20 6965 3b0a 2020 2020 2020  ; i < ie;.      
-0000e040: 692b 2b2c 2072 6f77 6e72 202b 3d20 6d61  i++, rownr += ma
-0000e050: 7452 6f77 436f 6c53 7465 702c 2063 6f6c  tRowColStep, col
-0000e060: 6e72 202b 3d20 6d61 7452 6f77 436f 6c53  nr += matRowColS
-0000e070: 7465 702c 2076 616c 7565 202b 3d20 6d61  tep, value += ma
-0000e080: 7456 616c 7565 5374 6570 2920 7b0a 2020  tValueStep) {.  
-0000e090: 2020 6162 7376 616c 7565 203d 2066 6162    absvalue = fab
-0000e0a0: 7328 2a76 616c 7565 293b 0a20 2020 2053  s(*value);.    S
-0000e0b0: 4554 4d41 5828 6d61 742d 3e63 6f6c 6d61  ETMAX(mat->colma
-0000e0c0: 785b 2a63 6f6c 6e72 5d2c 2061 6273 7661  x[*colnr], absva
-0000e0d0: 6c75 6529 3b0a 2020 2020 5345 544d 4158  lue);.    SETMAX
-0000e0e0: 286d 6174 2d3e 726f 776d 6178 5b2a 726f  (mat->rowmax[*ro
-0000e0f0: 776e 725d 2c20 6162 7376 616c 7565 293b  wnr], absvalue);
-0000e100: 0a20 2020 2053 4554 4d49 4e28 6d61 742d  .    SETMIN(mat-
-0000e110: 3e64 796e 7261 6e67 652c 2061 6273 7661  >dynrange, absva
-0000e120: 6c75 6529 3b0a 2020 2020 6966 2861 6273  lue);.    if(abs
-0000e130: 7661 6c75 6520 3c20 6570 736d 6163 6869  value < epsmachi
-0000e140: 6e65 290a 2020 2020 2020 657a 2b2b 3b0a  ne).      ez++;.
-0000e150: 2020 7d0a 0a20 202f 2a20 4c61 7374 6c79    }..  /* Lastly
-0000e160: 2c20 636f 6d70 7574 6520 7468 6520 676c  , compute the gl
-0000e170: 6f62 616c 206d 6178 696d 756d 2061 6e64  obal maximum and
-0000e180: 2067 6574 2074 6865 2064 796e 616d 6963   get the dynamic
-0000e190: 2072 616e 6765 202a 2f0a 2020 666f 7228   range */.  for(
-0000e1a0: 6920 3d20 313b 2069 203c 3d20 6d61 742d  i = 1; i <= mat-
-0000e1b0: 3e72 6f77 733b 2069 2b2b 290a 2020 2020  >rows; i++).    
-0000e1c0: 5345 544d 4158 286d 6174 2d3e 726f 776d  SETMAX(mat->rowm
-0000e1d0: 6178 5b30 5d2c 206d 6174 2d3e 726f 776d  ax[0], mat->rowm
-0000e1e0: 6178 5b69 5d29 3b0a 2020 6d61 742d 3e69  ax[i]);.  mat->i
-0000e1f0: 6e66 6e6f 726d 203d 206d 6174 2d3e 636f  nfnorm = mat->co
-0000e200: 6c6d 6178 5b30 5d20 3d20 6d61 742d 3e72  lmax[0] = mat->r
-0000e210: 6f77 6d61 785b 305d 3b0a 2020 6966 286d  owmax[0];.  if(m
-0000e220: 6174 2d3e 6479 6e72 616e 6765 203d 3d20  at->dynrange == 
-0000e230: 3029 207b 0a20 2020 2072 6570 6f72 7428  0) {.    report(
-0000e240: 6d61 742d 3e6c 702c 2053 4556 4552 452c  mat->lp, SEVERE,
-0000e250: 2022 2564 206d 6174 7269 7820 636f 6e74   "%d matrix cont
-0000e260: 6169 6e73 207a 6572 6f2d 7661 6c75 6564  ains zero-valued
-0000e270: 2063 6f65 6666 6963 6965 6e74 732e 5c6e   coefficients.\n
-0000e280: 222c 2065 7a29 3b0a 2020 2020 6d61 742d  ", ez);.    mat-
-0000e290: 3e64 796e 7261 6e67 6520 3d20 6d61 742d  >dynrange = mat-
-0000e2a0: 3e6c 702d 3e69 6e66 696e 6974 653b 0a20  >lp->infinite;. 
-0000e2b0: 207d 0a20 2065 6c73 6520 7b0a 2020 2020   }.  else {.    
-0000e2c0: 6d61 742d 3e64 796e 7261 6e67 6520 3d20  mat->dynrange = 
-0000e2d0: 6d61 742d 3e69 6e66 6e6f 726d 202f 206d  mat->infnorm / m
-0000e2e0: 6174 2d3e 6479 6e72 616e 6765 3b0a 2020  at->dynrange;.  
-0000e2f0: 2020 6966 2865 7a20 3e20 3029 0a20 2020    if(ez > 0).   
-0000e300: 2020 2072 6570 6f72 7428 6d61 742d 3e6c     report(mat->l
-0000e310: 702c 2049 4d50 4f52 5441 4e54 2c20 2225  p, IMPORTANT, "%
-0000e320: 6420 6d61 7472 6978 2063 6f65 6666 6963  d matrix coeffic
-0000e330: 6965 6e74 7320 6265 6c6f 7720 6d61 6368  ients below mach
-0000e340: 696e 6520 7072 6563 6973 696f 6e20 7765  ine precision we
-0000e350: 7265 2066 6f75 6e64 2e5c 6e22 2c20 657a  re found.\n", ez
-0000e360: 293b 0a20 207d 0a0a 2020 7265 7475 726e  );.  }..  return
-0000e370: 2820 5452 5545 2029 3b0a 7d0a 0a53 5441  ( TRUE );.}..STA
-0000e380: 5449 4320 4d59 424f 4f4c 206d 6174 5f74  TIC MYBOOL mat_t
-0000e390: 7261 6e73 706f 7365 284d 4154 7265 6320  ranspose(MATrec 
-0000e3a0: 2a6d 6174 290a 7b0a 2020 696e 7420 2020  *mat).{.  int   
-0000e3b0: 2020 692c 206a 2c20 6e7a 2c20 6b3b 0a20    i, j, nz, k;. 
-0000e3c0: 204d 5942 4f4f 4c20 2073 7461 7475 733b   MYBOOL  status;
-0000e3d0: 0a0a 2020 7374 6174 7573 203d 206d 6174  ..  status = mat
-0000e3e0: 5f76 616c 6964 6174 6528 6d61 7429 3b0a  _validate(mat);.
-0000e3f0: 2020 6966 2873 7461 7475 7329 207b 0a0a    if(status) {..
-0000e400: 2020 2020 2f2a 2043 7265 6174 6520 6120      /* Create a 
-0000e410: 636f 6c75 6d6e 2d6f 7264 6572 6564 2073  column-ordered s
-0000e420: 7061 7273 6520 656c 656d 656e 7420 6c69  parse element li
-0000e430: 7374 3b20 2263 6f6c 756d 6e22 2069 6e64  st; "column" ind
-0000e440: 6578 206d 7573 7420 6265 2073 6869 6674  ex must be shift
-0000e450: 6564 202a 2f0a 2020 2020 6e7a 203d 206d  ed */.    nz = m
-0000e460: 6174 5f6e 6f6e 7a65 726f 7328 6d61 7429  at_nonzeros(mat)
-0000e470: 3b0a 2020 2020 6966 286e 7a20 3e20 3029  ;.    if(nz > 0)
-0000e480: 207b 0a23 6966 204d 6174 7269 7843 6f6c   {.#if MatrixCol
-0000e490: 4163 6365 7373 3d3d 4341 4d5f 5265 636f  Access==CAM_Reco
-0000e4a0: 7264 0a20 2020 2020 204d 4154 6974 656d  rd.      MATitem
-0000e4b0: 202a 6e65 776d 6174 3b0a 2020 2020 2020   *newmat;.      
-0000e4c0: 6e65 776d 6174 203d 2028 4d41 5469 7465  newmat = (MATite
-0000e4d0: 6d20 2a29 206d 616c 6c6f 6328 286d 6174  m *) malloc((mat
-0000e4e0: 2d3e 6d61 745f 616c 6c6f 6329 202a 2073  ->mat_alloc) * s
-0000e4f0: 697a 656f 6628 2a28 6d61 742d 3e63 6f6c  izeof(*(mat->col
-0000e500: 5f6d 6174 2929 293b 0a20 2020 2020 206a  _mat)));.      j
-0000e510: 203d 206d 6174 2d3e 726f 775f 656e 645b   = mat->row_end[
-0000e520: 305d 3b0a 2020 2020 2020 666f 7228 6920  0];.      for(i 
-0000e530: 3d20 6e7a 2d31 3b20 6920 3e3d 206a 203b  = nz-1; i >= j ;
-0000e540: 2069 2d2d 2920 7b0a 2020 2020 2020 2020   i--) {.        
-0000e550: 6b20 3d20 692d 6a3b 0a20 2020 2020 2020  k = i-j;.       
-0000e560: 206e 6577 6d61 745b 6b5d 203d 206d 6174   newmat[k] = mat
-0000e570: 2d3e 636f 6c5f 6d61 745b 6d61 742d 3e72  ->col_mat[mat->r
-0000e580: 6f77 5f6d 6174 5b69 5d5d 3b0a 2020 2020  ow_mat[i]];.    
-0000e590: 2020 2020 6e65 776d 6174 5b6b 5d2e 726f      newmat[k].ro
-0000e5a0: 775f 6e72 203d 206e 6577 6d61 745b 6b5d  w_nr = newmat[k]
-0000e5b0: 2e63 6f6c 5f6e 723b 0a20 2020 2020 207d  .col_nr;.      }
-0000e5c0: 0a20 2020 2020 2066 6f72 2869 203d 206a  .      for(i = j
-0000e5d0: 2d31 3b20 6920 3e3d 2030 203b 2069 2d2d  -1; i >= 0 ; i--
-0000e5e0: 2920 7b0a 2020 2020 2020 2020 6b20 3d20  ) {.        k = 
-0000e5f0: 6e7a 2d6a 2b69 3b0a 2020 2020 2020 2020  nz-j+i;.        
-0000e600: 6e65 776d 6174 5b6b 5d20 3d20 6d61 742d  newmat[k] = mat-
-0000e610: 3e63 6f6c 5f6d 6174 5b6d 6174 2d3e 726f  >col_mat[mat->ro
-0000e620: 775f 6d61 745b 695d 5d3b 0a20 2020 2020  w_mat[i]];.     
-0000e630: 2020 206e 6577 6d61 745b 6b5d 2e72 6f77     newmat[k].row
-0000e640: 5f6e 7220 3d20 6e65 776d 6174 5b6b 5d2e  _nr = newmat[k].
-0000e650: 636f 6c5f 6e72 3b0a 2020 2020 2020 7d0a  col_nr;.      }.
-0000e660: 2020 2020 2020 7377 6170 5054 5228 2876        swapPTR((v
-0000e670: 6f69 6420 2a2a 2920 266d 6174 2d3e 636f  oid **) &mat->co
-0000e680: 6c5f 6d61 742c 2028 766f 6964 202a 2a29  l_mat, (void **)
-0000e690: 2026 6e65 776d 6174 293b 0a20 2020 2020   &newmat);.     
-0000e6a0: 2046 5245 4528 6e65 776d 6174 293b 0a23   FREE(newmat);.#
-0000e6b0: 656c 7365 202f 2a69 6620 4d61 7472 6978  else /*if Matrix
-0000e6c0: 436f 6c41 6363 6573 733d 3d43 414d 5f56  ColAccess==CAM_V
-0000e6d0: 6563 746f 722a 2f0a 2020 2020 2020 5245  ector*/.      RE
-0000e6e0: 414c 202a 6e65 7756 616c 7565 203d 204e  AL *newValue = N
-0000e6f0: 554c 4c3b 0a20 2020 2020 2069 6e74 2020  ULL;.      int  
-0000e700: 2a6e 6577 526f 776e 7220 3d20 4e55 4c4c  *newRownr = NULL
-0000e710: 3b0a 2020 2020 2020 616c 6c6f 6352 4541  ;.      allocREA
-0000e720: 4c28 6d61 742d 3e6c 702c 2026 6e65 7756  L(mat->lp, &newV
-0000e730: 616c 7565 2c20 6d61 742d 3e6d 6174 5f61  alue, mat->mat_a
-0000e740: 6c6c 6f63 2c20 4641 4c53 4529 3b0a 2020  lloc, FALSE);.  
-0000e750: 2020 2020 616c 6c6f 6349 4e54 286d 6174      allocINT(mat
-0000e760: 2d3e 6c70 2c20 266e 6577 526f 776e 722c  ->lp, &newRownr,
-0000e770: 206d 6174 2d3e 6d61 745f 616c 6c6f 632c   mat->mat_alloc,
-0000e780: 2046 414c 5345 293b 0a0a 2020 2020 2020   FALSE);..      
-0000e790: 6a20 3d20 6d61 742d 3e72 6f77 5f65 6e64  j = mat->row_end
-0000e7a0: 5b30 5d3b 0a20 2020 2020 2066 6f72 2869  [0];.      for(i
-0000e7b0: 203d 206e 7a2d 313b 2069 203e 3d20 6a20   = nz-1; i >= j 
-0000e7c0: 3b20 692d 2d29 207b 0a20 2020 2020 2020  ; i--) {.       
-0000e7d0: 206b 203d 2069 2d6a 3b0a 2020 2020 2020   k = i-j;.      
-0000e7e0: 2020 6e65 7756 616c 7565 5b6b 5d20 3d20    newValue[k] = 
-0000e7f0: 524f 575f 4d41 545f 5641 4c55 4528 6929  ROW_MAT_VALUE(i)
-0000e800: 3b0a 2020 2020 2020 2020 6e65 7752 6f77  ;.        newRow
-0000e810: 6e72 5b6b 5d20 3d20 524f 575f 4d41 545f  nr[k] = ROW_MAT_
-0000e820: 434f 4c4e 5228 6929 3b0a 2020 2020 2020  COLNR(i);.      
-0000e830: 7d0a 2020 2020 2020 666f 7228 6920 3d20  }.      for(i = 
-0000e840: 6a2d 313b 2069 203e 3d20 3020 3b20 692d  j-1; i >= 0 ; i-
-0000e850: 2d29 207b 0a20 2020 2020 2020 206b 203d  -) {.        k =
-0000e860: 206e 7a2d 6a2b 693b 0a20 2020 2020 2020   nz-j+i;.       
-0000e870: 206e 6577 5661 6c75 655b 6b5d 203d 2052   newValue[k] = R
-0000e880: 4f57 5f4d 4154 5f56 414c 5545 2869 293b  OW_MAT_VALUE(i);
-0000e890: 0a20 2020 2020 2020 206e 6577 526f 776e  .        newRown
-0000e8a0: 725b 6b5d 203d 2052 4f57 5f4d 4154 5f43  r[k] = ROW_MAT_C
-0000e8b0: 4f4c 4e52 2869 293b 0a20 2020 2020 207d  OLNR(i);.      }
-0000e8c0: 0a0a 2020 2020 2020 7377 6170 5054 5228  ..      swapPTR(
-0000e8d0: 2876 6f69 6420 2a2a 2920 266d 6174 2d3e  (void **) &mat->
-0000e8e0: 636f 6c5f 6d61 745f 726f 776e 722c 2028  col_mat_rownr, (
-0000e8f0: 766f 6964 202a 2a29 2026 6e65 7752 6f77  void **) &newRow
-0000e900: 6e72 293b 0a20 2020 2020 2073 7761 7050  nr);.      swapP
-0000e910: 5452 2828 766f 6964 202a 2a29 2026 6d61  TR((void **) &ma
-0000e920: 742d 3e63 6f6c 5f6d 6174 5f76 616c 7565  t->col_mat_value
-0000e930: 2c20 2876 6f69 6420 2a2a 2920 266e 6577  , (void **) &new
-0000e940: 5661 6c75 6529 3b0a 2020 2020 2020 4652  Value);.      FR
-0000e950: 4545 286e 6577 5661 6c75 6529 3b0a 2020  EE(newValue);.  
-0000e960: 2020 2020 4652 4545 286e 6577 526f 776e      FREE(newRown
-0000e970: 7229 3b0a 2365 6e64 6966 0a20 2020 207d  r);.#endif.    }
-0000e980: 0a0a 2020 2020 2f2a 2054 7261 6e73 6665  ..    /* Transfe
-0000e990: 7220 726f 7720 7374 6172 7420 746f 2063  r row start to c
-0000e9a0: 6f6c 756d 6e20 7374 6172 7420 706f 7369  olumn start posi
-0000e9b0: 7469 6f6e 3b20 6d75 7374 2061 646a 7573  tion; must adjus
-0000e9c0: 7420 666f 7220 6469 6666 6572 656e 7420  t for different 
-0000e9d0: 6f66 6673 6574 7320 2a2f 0a20 2020 2069  offsets */.    i
-0000e9e0: 6628 6d61 742d 3e72 6f77 7320 3d3d 206d  f(mat->rows == m
-0000e9f0: 6174 2d3e 726f 7773 5f61 6c6c 6f63 290a  at->rows_alloc).
-0000ea00: 2020 2020 2020 696e 635f 6d61 7463 6f6c        inc_matcol
-0000ea10: 5f73 7061 6365 286d 6174 2c20 3129 3b0a  _space(mat, 1);.
-0000ea20: 2020 2020 6a20 3d20 6d61 742d 3e72 6f77      j = mat->row
-0000ea30: 5f65 6e64 5b30 5d3b 0a20 2020 2066 6f72  _end[0];.    for
-0000ea40: 2869 203d 206d 6174 2d3e 726f 7773 3b20  (i = mat->rows; 
-0000ea50: 6920 3e3d 2031 3b20 692d 2d29 0a20 2020  i >= 1; i--).   
-0000ea60: 2020 206d 6174 2d3e 726f 775f 656e 645b     mat->row_end[
-0000ea70: 695d 202d 3d20 6a3b 0a20 2020 206d 6174  i] -= j;.    mat
-0000ea80: 2d3e 726f 775f 656e 645b 6d61 742d 3e72  ->row_end[mat->r
-0000ea90: 6f77 735d 203d 206e 7a3b 0a20 2020 2073  ows] = nz;.    s
-0000eaa0: 7761 7050 5452 2828 766f 6964 202a 2a29  wapPTR((void **)
-0000eab0: 2026 6d61 742d 3e72 6f77 5f65 6e64 2c20   &mat->row_end, 
-0000eac0: 2876 6f69 6420 2a2a 2920 266d 6174 2d3e  (void **) &mat->
-0000ead0: 636f 6c5f 656e 6429 3b0a 0a20 2020 202f  col_end);..    /
-0000eae0: 2a20 5377 6170 2061 7272 6179 7320 6f66  * Swap arrays of
-0000eaf0: 206d 6178 696d 756d 2076 616c 7565 7320   maximum values 
-0000eb00: 2a2f 0a20 2020 2073 7761 7050 5452 2828  */.    swapPTR((
-0000eb10: 766f 6964 202a 2a29 2026 6d61 742d 3e72  void **) &mat->r
-0000eb20: 6f77 6d61 782c 2028 766f 6964 202a 2a29  owmax, (void **)
-0000eb30: 2026 6d61 742d 3e63 6f6c 6d61 7829 3b0a   &mat->colmax);.
-0000eb40: 0a20 2020 202f 2a20 5377 6170 2061 7272  .    /* Swap arr
-0000eb50: 6179 2073 697a 6573 202a 2f0a 2020 2020  ay sizes */.    
-0000eb60: 7377 6170 494e 5428 266d 6174 2d3e 726f  swapINT(&mat->ro
-0000eb70: 7773 2c20 266d 6174 2d3e 636f 6c75 6d6e  ws, &mat->column
-0000eb80: 7329 3b0a 2020 2020 7377 6170 494e 5428  s);.    swapINT(
-0000eb90: 266d 6174 2d3e 726f 7773 5f61 6c6c 6f63  &mat->rows_alloc
-0000eba0: 2c20 266d 6174 2d3e 636f 6c75 6d6e 735f  , &mat->columns_
-0000ebb0: 616c 6c6f 6329 3b0a 0a20 2020 202f 2a20  alloc);..    /* 
-0000ebc0: 4669 6e61 6c6c 7920 7365 7420 6375 7272  Finally set curr
-0000ebd0: 656e 7420 7374 6f72 6167 6520 6d6f 6465  ent storage mode
-0000ebe0: 202a 2f0a 2020 2020 6d61 742d 3e69 735f   */.    mat->is_
-0000ebf0: 726f 776f 7264 6572 203d 2028 4d59 424f  roworder = (MYBO
-0000ec00: 4f4c 2920 216d 6174 2d3e 6973 5f72 6f77  OL) !mat->is_row
-0000ec10: 6f72 6465 723b 0a20 2020 206d 6174 2d3e  order;.    mat->
-0000ec20: 726f 775f 656e 645f 7661 6c69 6420 3d20  row_end_valid = 
-0000ec30: 4641 4c53 453b 0a20 207d 0a20 2072 6574  FALSE;.  }.  ret
-0000ec40: 7572 6e28 7374 6174 7573 293b 0a7d 0a0a  urn(status);.}..
-0000ec50: 0a2f 2a20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ./* ------------
+0000c2d0: 2069 6e74 2020 2020 2020 6962 2c20 6965   int      ib, ie
+0000c2e0: 2c20 2a6d 6174 526f 776e 723b 0a20 2020  , *matRownr;.   
+0000c2f0: 5245 414c 2020 2020 202a 6d61 7456 616c  REAL     *matVal
+0000c300: 7565 3b0a 0a20 202f 2a20 4861 6e64 6c65  ue;..  /* Handle
+0000c310: 2063 6173 6520 6f66 2061 2073 6c61 636b   case of a slack
+0000c320: 2076 6172 6961 626c 6520 2a2f 0a20 2069   variable */.  i
+0000c330: 6628 7661 726e 7220 3c3d 206d 6174 2d3e  f(varnr <= mat->
+0000c340: 6c70 2d3e 726f 7773 2920 7b0a 2020 2020  lp->rows) {.    
+0000c350: 6c68 7376 6563 746f 725b 7661 726e 725d  lhsvector[varnr]
+0000c360: 202b 3d20 6d75 6c74 3b0a 2020 2020 7265   += mult;.    re
+0000c370: 7475 726e 3b0a 2020 7d0a 0a20 202f 2a20  turn;.  }..  /* 
+0000c380: 446f 206f 7065 7261 7469 6f6e 206f 6e20  Do operation on 
+0000c390: 7468 6520 6f62 6a65 6374 6976 6520 2a2f  the objective */
+0000c3a0: 0a20 2069 6628 6d61 742d 3e6c 702d 3e6d  .  if(mat->lp->m
+0000c3b0: 6174 4120 3d3d 206d 6174 290a 2020 2020  atA == mat).    
+0000c3c0: 6c68 7376 6563 746f 725b 305d 202b 3d20  lhsvector[0] += 
+0000c3d0: 6765 745f 4f46 5f61 6374 6976 6528 6d61  get_OF_active(ma
+0000c3e0: 742d 3e6c 702c 2076 6172 6e72 2c20 6d75  t->lp, varnr, mu
+0000c3f0: 6c74 293b 0a0a 2020 2f2a 2053 6361 6e20  lt);..  /* Scan 
+0000c400: 7468 6520 636f 6e73 7472 6169 6e74 206d  the constraint m
+0000c410: 6174 7269 7820 7461 7267 6574 2063 6f6c  atrix target col
+0000c420: 756d 6e73 202a 2f0a 2020 636f 6c6e 7220  umns */.  colnr 
+0000c430: 3d20 7661 726e 7220 2d20 6d61 742d 3e6c  = varnr - mat->l
+0000c440: 702d 3e72 6f77 733b 0a20 2069 6220 3d20  p->rows;.  ib = 
+0000c450: 6d61 742d 3e63 6f6c 5f65 6e64 5b63 6f6c  mat->col_end[col
+0000c460: 6e72 202d 2031 5d3b 0a20 2069 6520 3d20  nr - 1];.  ie = 
+0000c470: 6d61 742d 3e63 6f6c 5f65 6e64 5b63 6f6c  mat->col_end[col
+0000c480: 6e72 5d3b 0a20 2069 6628 6962 203c 2069  nr];.  if(ib < i
+0000c490: 6529 207b 0a0a 2020 2020 2f2a 2049 6e69  e) {..    /* Ini
+0000c4a0: 7469 616c 697a 6520 706f 696e 7465 7273  tialize pointers
+0000c4b0: 202a 2f0a 2020 2020 6d61 7452 6f77 6e72   */.    matRownr
+0000c4c0: 203d 2026 434f 4c5f 4d41 545f 524f 574e   = &COL_MAT_ROWN
+0000c4d0: 5228 6962 293b 0a20 2020 206d 6174 5661  R(ib);.    matVa
+0000c4e0: 6c75 6520 3d20 2643 4f4c 5f4d 4154 5f56  lue = &COL_MAT_V
+0000c4f0: 414c 5545 2869 6229 3b0a 0a20 2020 202f  ALUE(ib);..    /
+0000c500: 2a20 5468 656e 206c 6f6f 7020 6f76 6572  * Then loop over
+0000c510: 2061 6c6c 2072 6567 756c 6172 2072 6f77   all regular row
+0000c520: 7320 2a2f 0a20 2020 2066 6f72 283b 2069  s */.    for(; i
+0000c530: 6220 3c20 6965 3b0a 2020 2020 2020 2020  b < ie;.        
+0000c540: 6962 2b2b 2c20 6d61 7456 616c 7565 202b  ib++, matValue +
+0000c550: 3d20 6d61 7456 616c 7565 5374 6570 2c20  = matValueStep, 
+0000c560: 6d61 7452 6f77 6e72 202b 3d20 6d61 7452  matRownr += matR
+0000c570: 6f77 436f 6c53 7465 7029 207b 0a20 2020  owColStep) {.   
+0000c580: 2020 206c 6873 7665 6374 6f72 5b2a 6d61     lhsvector[*ma
+0000c590: 7452 6f77 6e72 5d20 2b3d 206d 756c 7420  tRownr] += mult 
+0000c5a0: 2a20 282a 6d61 7456 616c 7565 293b 0a20  * (*matValue);. 
+0000c5b0: 2020 207d 0a20 207d 0a0a 7d0a 0a53 5441     }.  }..}..STA
+0000c5c0: 5449 4320 4d59 424f 4f4c 206d 6174 5f73  TIC MYBOOL mat_s
+0000c5d0: 6574 7661 6c75 6528 4d41 5472 6563 202a  etvalue(MATrec *
+0000c5e0: 6d61 742c 2069 6e74 2052 6f77 2c20 696e  mat, int Row, in
+0000c5f0: 7420 436f 6c75 6d6e 2c20 5245 414c 2056  t Column, REAL V
+0000c600: 616c 7565 2c20 4d59 424f 4f4c 2064 6f73  alue, MYBOOL dos
+0000c610: 6361 6c65 290a 7b0a 2020 696e 7420 2020  cale).{.  int   
+0000c620: 2065 6c6d 6e72 2c20 6c61 7374 656c 6d2c   elmnr, lastelm,
+0000c630: 2069 2c20 526f 7741 203d 2052 6f77 2c20   i, RowA = Row, 
+0000c640: 436f 6c75 6d6e 4120 3d20 436f 6c75 6d6e  ColumnA = Column
+0000c650: 3b0a 2020 4d59 424f 4f4c 2069 7341 3b0a  ;.  MYBOOL isA;.
+0000c660: 0a20 202f 2a20 5468 6973 2066 756e 6374  .  /* This funct
+0000c670: 696f 6e20 6973 2069 6e65 6666 6963 6965  ion is inefficie
+0000c680: 6e74 2069 6620 7573 6564 2074 6f20 6164  nt if used to ad
+0000c690: 6420 6e65 7720 6d61 7472 6978 2065 6e74  d new matrix ent
+0000c6a0: 7269 6573 2069 6e0a 2020 2020 206f 7468  ries in.     oth
+0000c6b0: 6572 2070 6c61 6365 7320 7468 616e 2061  er places than a
+0000c6c0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
+0000c6d0: 206d 6174 7269 782e 204f 4b20 666f 7220   matrix. OK for 
+0000c6e0: 7265 706c 6163 696e 6720 6578 6973 7469  replacing existi
+0000c6f0: 6e67 0a20 2020 2020 6120 6e6f 6e2d 7a65  ng.     a non-ze
+0000c700: 726f 2076 616c 7565 2077 6974 6820 616e  ro value with an
+0000c710: 6f74 6865 7220 6e6f 6e2d 7a65 726f 2076  other non-zero v
+0000c720: 616c 7565 202a 2f0a 2020 6973 4120 3d20  alue */.  isA = 
+0000c730: 284d 5942 4f4f 4c29 2028 6d61 7420 3d3d  (MYBOOL) (mat ==
+0000c740: 206d 6174 2d3e 6c70 2d3e 6d61 7441 293b   mat->lp->matA);
+0000c750: 0a20 2069 6628 6d61 742d 3e69 735f 726f  .  if(mat->is_ro
+0000c760: 776f 7264 6572 290a 2020 2020 7377 6170  worder).    swap
+0000c770: 494e 5428 2652 6f77 2c20 2643 6f6c 756d  INT(&Row, &Colum
+0000c780: 6e29 3b0a 0a20 202f 2a20 5365 7420 736d  n);..  /* Set sm
+0000c790: 616c 6c20 6e75 6d62 6572 7320 746f 207a  all numbers to z
+0000c7a0: 6572 6f20 2a2f 0a20 2069 6628 6661 6273  ero */.  if(fabs
+0000c7b0: 2856 616c 7565 2920 3c20 6d61 742d 3e65  (Value) < mat->e
+0000c7c0: 7073 7661 6c75 6529 0a20 2020 2056 616c  psvalue).    Val
+0000c7d0: 7565 203d 2030 3b0a 2369 6664 6566 2044  ue = 0;.#ifdef D
+0000c7e0: 6f4d 6174 7269 7852 6f75 6e64 696e 670a  oMatrixRounding.
+0000c7f0: 2020 656c 7365 0a20 2020 2056 616c 7565    else.    Value
+0000c800: 203d 2072 6f75 6e64 546f 5072 6563 6973   = roundToPrecis
+0000c810: 696f 6e28 5661 6c75 652c 206d 6174 2d3e  ion(Value, mat->
+0000c820: 6570 7376 616c 7565 293b 0a23 656e 6469  epsvalue);.#endi
+0000c830: 660a 0a20 202f 2a20 4368 6563 6b20 6966  f..  /* Check if
+0000c840: 2077 6520 6e65 6564 2074 6f20 7570 6461   we need to upda
+0000c850: 7465 2063 6f6c 756d 6e20 7370 6163 6520  te column space 
+0000c860: 2a2f 0a20 2069 6628 436f 6c75 6d6e 203e  */.  if(Column >
+0000c870: 206d 6174 2d3e 636f 6c75 6d6e 7329 207b   mat->columns) {
+0000c880: 0a20 2020 2069 6628 6973 4129 0a20 2020  .    if(isA).   
+0000c890: 2020 2069 6e63 5f63 6f6c 5f73 7061 6365     inc_col_space
+0000c8a0: 286d 6174 2d3e 6c70 2c20 436f 6c75 6d6e  (mat->lp, Column
+0000c8b0: 4120 2d20 6d61 742d 3e63 6f6c 756d 6e73  A - mat->columns
+0000c8c0: 293b 0a20 2020 2065 6c73 650a 2020 2020  );.    else.    
+0000c8d0: 2020 696e 635f 6d61 7463 6f6c 5f73 7061    inc_matcol_spa
+0000c8e0: 6365 286d 6174 2c20 436f 6c75 6d6e 202d  ce(mat, Column -
+0000c8f0: 206d 6174 2d3e 636f 6c75 6d6e 7329 3b0a   mat->columns);.
+0000c900: 2020 7d0a 0a20 202f 2a20 4669 6e64 206f    }..  /* Find o
+0000c910: 7574 2069 6620 7765 2061 6c72 6561 6479  ut if we already
+0000c920: 2068 6176 6520 7375 6368 2061 6e20 656e   have such an en
+0000c930: 7472 792c 206f 7220 7265 7475 726e 2069  try, or return i
+0000c940: 6e73 6572 7469 6f6e 2070 6f69 6e74 202a  nsertion point *
+0000c950: 2f0a 2020 6920 3d20 6d61 745f 6669 6e64  /.  i = mat_find
+0000c960: 696e 7328 6d61 742c 2052 6f77 2c20 436f  ins(mat, Row, Co
+0000c970: 6c75 6d6e 2c20 2665 6c6d 6e72 2c20 4641  lumn, &elmnr, FA
+0000c980: 4c53 4529 3b0a 2020 6966 2869 203d 3d20  LSE);.  if(i == 
+0000c990: 2d31 290a 2020 2020 7265 7475 726e 2846  -1).    return(F
+0000c9a0: 414c 5345 293b 0a0a 2020 6966 2869 7341  ALSE);..  if(isA
+0000c9b0: 290a 2020 2020 7365 745f 6163 7469 6f6e  ).    set_action
+0000c9c0: 2826 6d61 742d 3e6c 702d 3e73 7078 5f61  (&mat->lp->spx_a
+0000c9d0: 6374 696f 6e2c 2041 4354 494f 4e5f 5245  ction, ACTION_RE
+0000c9e0: 4241 5345 207c 2041 4354 494f 4e5f 5245  BASE | ACTION_RE
+0000c9f0: 434f 4d50 5554 4520 7c20 4143 5449 4f4e  COMPUTE | ACTION
+0000ca00: 5f52 4549 4e56 4552 5429 3b0a 0a20 2069  _REINVERT);..  i
+0000ca10: 6628 6920 3e3d 2030 2920 7b0a 2020 2020  f(i >= 0) {.    
+0000ca20: 2f2a 2074 6865 7265 2069 7320 616e 2065  /* there is an e
+0000ca30: 7869 7374 696e 6720 656e 7472 7920 2a2f  xisting entry */
+0000ca40: 0a20 2020 2069 6628 6661 6273 2856 616c  .    if(fabs(Val
+0000ca50: 7565 2920 3e20 6d61 742d 3e65 7073 7661  ue) > mat->epsva
+0000ca60: 6c75 6529 207b 202f 2a20 7765 2072 6570  lue) { /* we rep
+0000ca70: 6c61 6365 2069 7420 6279 2073 6f6d 6574  lace it by somet
+0000ca80: 6869 6e67 206e 6f6e 2d7a 6572 6f20 2a2f  hing non-zero */
+0000ca90: 0a20 2020 2020 2069 6628 6973 4129 207b  .      if(isA) {
+0000caa0: 0a20 2020 2020 2020 2056 616c 7565 203d  .        Value =
+0000cab0: 206d 795f 6368 7369 676e 2869 735f 6368   my_chsign(is_ch
+0000cac0: 7369 676e 286d 6174 2d3e 6c70 2c20 526f  sign(mat->lp, Ro
+0000cad0: 7741 292c 2056 616c 7565 293b 0a20 2020  wA), Value);.   
+0000cae0: 2020 2020 2069 6628 646f 7363 616c 6520       if(doscale 
+0000caf0: 2626 206d 6174 2d3e 6c70 2d3e 7363 616c  && mat->lp->scal
+0000cb00: 696e 675f 7573 6564 290a 2020 2020 2020  ing_used).      
+0000cb10: 2020 2020 5661 6c75 6520 3d20 7363 616c      Value = scal
+0000cb20: 6564 5f6d 6174 286d 6174 2d3e 6c70 2c20  ed_mat(mat->lp, 
+0000cb30: 5661 6c75 652c 2052 6f77 412c 2043 6f6c  Value, RowA, Col
+0000cb40: 756d 6e41 293b 0a20 2020 2020 207d 0a20  umnA);.      }. 
+0000cb50: 2020 2020 2043 4f4c 5f4d 4154 5f56 414c       COL_MAT_VAL
+0000cb60: 5545 2865 6c6d 6e72 2920 3d20 5661 6c75  UE(elmnr) = Valu
+0000cb70: 653b 0a20 2020 207d 0a20 2020 2065 6c73  e;.    }.    els
+0000cb80: 6520 7b20 2f2a 2073 6574 7469 6e67 2065  e { /* setting e
+0000cb90: 7869 7374 696e 6720 6e6f 6e2d 7a65 726f  xisting non-zero
+0000cba0: 2065 6e74 7279 2074 6f20 7a65 726f 2e20   entry to zero. 
+0000cbb0: 5265 6d6f 7665 2074 6865 2065 6e74 7279  Remove the entry
+0000cbc0: 202a 2f0a 2020 2020 2020 2f2a 2054 6869   */.      /* Thi
+0000cbd0: 7320 6d69 6768 7420 7265 6d6f 7665 2061  s might remove a
+0000cbe0: 6e20 656e 7469 7265 2063 6f6c 756d 6e2c  n entire column,
+0000cbf0: 206f 7220 6c65 6176 6520 6a75 7374 2061   or leave just a
+0000cc00: 2062 6f75 6e64 2e20 4e6f 0a20 2020 2020   bound. No.     
+0000cc10: 2020 2020 206e 6963 6520 736f 6c75 7469       nice soluti
+0000cc20: 6f6e 2066 6f72 2074 6861 7420 7965 7420  on for that yet 
+0000cc30: 2a2f 0a0a 2020 2020 2020 2f2a 2053 6869  */..      /* Shi
+0000cc40: 6674 2075 7020 7461 696c 2065 6e64 206f  ft up tail end o
+0000cc50: 6620 7468 6520 6d61 7472 6978 202a 2f0a  f the matrix */.
+0000cc60: 2020 2020 2020 6c61 7374 656c 6d20 3d20        lastelm = 
+0000cc70: 6d61 745f 6e6f 6e7a 6572 6f73 286d 6174  mat_nonzeros(mat
+0000cc80: 293b 0a23 6966 2030 0a20 2020 2020 2066  );.#if 0.      f
+0000cc90: 6f72 2869 203d 2065 6c6d 6e72 3b20 6920  or(i = elmnr; i 
+0000cca0: 3c20 6c61 7374 656c 6d20 3b20 692b 2b29  < lastelm ; i++)
+0000ccb0: 207b 0a20 2020 2020 2020 2043 4f4c 5f4d   {.        COL_M
+0000ccc0: 4154 5f43 4f50 5928 692c 2069 202b 2031  AT_COPY(i, i + 1
+0000ccd0: 293b 0a20 2020 2020 207d 0a23 656c 7365  );.      }.#else
+0000cce0: 0a20 2020 2020 206c 6173 7465 6c6d 202d  .      lastelm -
+0000ccf0: 3d20 656c 6d6e 723b 0a20 2020 2020 2043  = elmnr;.      C
+0000cd00: 4f4c 5f4d 4154 5f4d 4f56 4528 656c 6d6e  OL_MAT_MOVE(elmn
+0000cd10: 722c 2065 6c6d 6e72 202b 2031 2c20 6c61  r, elmnr + 1, la
+0000cd20: 7374 656c 6d29 3b0a 2365 6e64 6966 0a20  stelm);.#endif. 
+0000cd30: 2020 2020 2066 6f72 2869 203d 2043 6f6c       for(i = Col
+0000cd40: 756d 6e3b 2069 203c 3d20 6d61 742d 3e63  umn; i <= mat->c
+0000cd50: 6f6c 756d 6e73 3b20 692b 2b29 0a20 2020  olumns; i++).   
+0000cd60: 2020 2020 206d 6174 2d3e 636f 6c5f 656e       mat->col_en
+0000cd70: 645b 695d 2d2d 3b0a 0a20 2020 2020 206d  d[i]--;..      m
+0000cd80: 6174 2d3e 726f 775f 656e 645f 7661 6c69  at->row_end_vali
+0000cd90: 6420 3d20 4641 4c53 453b 0a20 2020 207d  d = FALSE;.    }
+0000cda0: 0a20 207d 0a20 2065 6c73 6520 6966 2866  .  }.  else if(f
+0000cdb0: 6162 7328 5661 6c75 6529 203e 206d 6174  abs(Value) > mat
+0000cdc0: 2d3e 6570 7376 616c 7565 2920 7b0a 2020  ->epsvalue) {.  
+0000cdd0: 2020 2f2a 206e 6f20 6578 6973 7469 6e67    /* no existing
+0000cde0: 2065 6e74 7279 2e20 6d61 6b65 206e 6577   entry. make new
+0000cdf0: 206f 6e65 206f 6e6c 7920 6966 206e 6f74   one only if not
+0000ce00: 206e 6561 726c 7920 7a65 726f 202a 2f0a   nearly zero */.
+0000ce10: 2020 2020 2f2a 2063 6865 636b 2069 6620      /* check if 
+0000ce20: 6d6f 7265 2073 7061 6365 2069 7320 6e65  more space is ne
+0000ce30: 6564 6564 2066 6f72 206d 6174 7269 7820  eded for matrix 
+0000ce40: 2a2f 0a20 2020 2069 6628 2169 6e63 5f6d  */.    if(!inc_m
+0000ce50: 6174 5f73 7061 6365 286d 6174 2c20 3129  at_space(mat, 1)
+0000ce60: 290a 2020 2020 2020 7265 7475 726e 2846  ).      return(F
+0000ce70: 414c 5345 293b 0a0a 2020 2020 6966 2843  ALSE);..    if(C
+0000ce80: 6f6c 756d 6e20 3e20 6d61 742d 3e63 6f6c  olumn > mat->col
+0000ce90: 756d 6e73 2920 7b0a 2020 2020 2020 6920  umns) {.      i 
+0000cea0: 3d20 6d61 742d 3e63 6f6c 756d 6e73 202b  = mat->columns +
+0000ceb0: 2031 3b0a 2020 2020 2020 6966 2869 7341   1;.      if(isA
+0000cec0: 290a 2020 2020 2020 2020 7368 6966 745f  ).        shift_
+0000ced0: 636f 6c64 6174 6128 6d61 742d 3e6c 702c  coldata(mat->lp,
+0000cee0: 2069 2c20 436f 6c75 6d6e 4120 2d20 6d61   i, ColumnA - ma
+0000cef0: 742d 3e63 6f6c 756d 6e73 2c20 4e55 4c4c  t->columns, NULL
+0000cf00: 293b 0a20 2020 2020 2065 6c73 650a 2020  );.      else.  
+0000cf10: 2020 2020 2020 6d61 745f 7368 6966 7463        mat_shiftc
+0000cf20: 6f6c 7328 6d61 742c 2026 692c 2043 6f6c  ols(mat, &i, Col
+0000cf30: 756d 6e20 2d20 6d61 742d 3e63 6f6c 756d  umn - mat->colum
+0000cf40: 6e73 2c20 4e55 4c4c 293b 0a20 2020 207d  ns, NULL);.    }
+0000cf50: 0a0a 2020 2020 2f2a 2053 6869 6674 2064  ..    /* Shift d
+0000cf60: 6f77 6e20 7461 696c 2065 6e64 206f 6620  own tail end of 
+0000cf70: 7468 6520 6d61 7472 6978 2062 7920 6f6e  the matrix by on
+0000cf80: 6520 2a2f 0a20 2020 206c 6173 7465 6c6d  e */.    lastelm
+0000cf90: 203d 206d 6174 5f6e 6f6e 7a65 726f 7328   = mat_nonzeros(
+0000cfa0: 6d61 7429 3b0a 2369 6620 3120 2f2a 2044  mat);.#if 1 /* D
+0000cfb0: 6f65 7320 636f 6d70 696c 6572 206f 7074  oes compiler opt
+0000cfc0: 696d 697a 6174 696f 6e20 776f 726b 2062  imization work b
+0000cfd0: 6574 7465 7220 6865 7265 3f20 2a2f 0a20  etter here? */. 
+0000cfe0: 2020 2066 6f72 2869 203d 206c 6173 7465     for(i = laste
+0000cff0: 6c6d 3b20 6920 3e20 656c 6d6e 7220 3b20  lm; i > elmnr ; 
+0000d000: 692d 2d29 207b 0a20 2020 2020 2043 4f4c  i--) {.      COL
+0000d010: 5f4d 4154 5f43 4f50 5928 692c 2069 202d  _MAT_COPY(i, i -
+0000d020: 2031 293b 0a20 2020 207d 0a23 656c 7365   1);.    }.#else
+0000d030: 0a20 2020 206c 6173 7465 6c6d 202d 3d20  .    lastelm -= 
+0000d040: 656c 6d6e 7220 2d20 313b 0a20 2020 2043  elmnr - 1;.    C
+0000d050: 4f4c 5f4d 4154 5f4d 4f56 4528 656c 6d6e  OL_MAT_MOVE(elmn
+0000d060: 7220 2b20 312c 2065 6c6d 6e72 2c20 6c61  r + 1, elmnr, la
+0000d070: 7374 656c 6d29 3b0a 2365 6e64 6966 0a0a  stelm);.#endif..
+0000d080: 2020 2020 2f2a 2053 6574 206e 6577 2065      /* Set new e
+0000d090: 6c65 6d65 6e74 202a 2f0a 2020 2020 6966  lement */.    if
+0000d0a0: 2869 7341 2920 7b0a 2020 2020 2020 5661  (isA) {.      Va
+0000d0b0: 6c75 6520 3d20 6d79 5f63 6873 6967 6e28  lue = my_chsign(
+0000d0c0: 6973 5f63 6873 6967 6e28 6d61 742d 3e6c  is_chsign(mat->l
+0000d0d0: 702c 2052 6f77 4129 2c20 5661 6c75 6529  p, RowA), Value)
+0000d0e0: 3b0a 2020 2020 2020 6966 2864 6f73 6361  ;.      if(dosca
+0000d0f0: 6c65 290a 2020 2020 2020 2020 5661 6c75  le).        Valu
+0000d100: 6520 3d20 7363 616c 6564 5f6d 6174 286d  e = scaled_mat(m
+0000d110: 6174 2d3e 6c70 2c20 5661 6c75 652c 2052  at->lp, Value, R
+0000d120: 6f77 412c 2043 6f6c 756d 6e41 293b 0a20  owA, ColumnA);. 
+0000d130: 2020 207d 0a20 2020 2053 4554 5f4d 4154     }.    SET_MAT
+0000d140: 5f69 6a41 2865 6c6d 6e72 2c20 526f 772c  _ijA(elmnr, Row,
+0000d150: 2043 6f6c 756d 6e2c 2056 616c 7565 293b   Column, Value);
+0000d160: 0a0a 2020 2020 2f2a 2055 7064 6174 6520  ..    /* Update 
+0000d170: 636f 6c75 6d6e 2069 6e64 6578 6573 202a  column indexes *
+0000d180: 2f0a 2020 2020 666f 7228 6920 3d20 436f  /.    for(i = Co
+0000d190: 6c75 6d6e 3b20 6920 3c3d 206d 6174 2d3e  lumn; i <= mat->
+0000d1a0: 636f 6c75 6d6e 733b 2069 2b2b 290a 2020  columns; i++).  
+0000d1b0: 2020 2020 6d61 742d 3e63 6f6c 5f65 6e64      mat->col_end
+0000d1c0: 5b69 5d2b 2b3b 0a0a 2020 2020 6d61 742d  [i]++;..    mat-
+0000d1d0: 3e72 6f77 5f65 6e64 5f76 616c 6964 203d  >row_end_valid =
+0000d1e0: 2046 414c 5345 3b0a 2020 7d0a 0a20 2069   FALSE;.  }..  i
+0000d1f0: 6628 6973 4120 2626 2028 6d61 742d 3e6c  f(isA && (mat->l
+0000d200: 702d 3e76 6172 5f69 735f 6672 6565 2021  p->var_is_free !
+0000d210: 3d20 4e55 4c4c 2920 2626 2028 6d61 742d  = NULL) && (mat-
+0000d220: 3e6c 702d 3e76 6172 5f69 735f 6672 6565  >lp->var_is_free
+0000d230: 5b43 6f6c 756d 6e41 5d20 3e20 3029 290a  [ColumnA] > 0)).
+0000d240: 2020 2020 7265 7475 726e 2820 6d61 745f      return( mat_
+0000d250: 7365 7476 616c 7565 286d 6174 2c20 526f  setvalue(mat, Ro
+0000d260: 7741 2c20 6d61 742d 3e6c 702d 3e76 6172  wA, mat->lp->var
+0000d270: 5f69 735f 6672 6565 5b43 6f6c 756d 6e41  _is_free[ColumnA
+0000d280: 5d2c 202d 5661 6c75 652c 2064 6f73 6361  ], -Value, dosca
+0000d290: 6c65 2920 293b 0a20 2072 6574 7572 6e28  le) );.  return(
+0000d2a0: 5452 5545 293b 0a7d 0a0a 5354 4154 4943  TRUE);.}..STATIC
+0000d2b0: 204d 5942 4f4f 4c20 6d61 745f 6170 7065   MYBOOL mat_appe
+0000d2c0: 6e64 7661 6c75 6528 4d41 5472 6563 202a  ndvalue(MATrec *
+0000d2d0: 6d61 742c 2069 6e74 2052 6f77 2c20 5245  mat, int Row, RE
+0000d2e0: 414c 2056 616c 7565 290a 7b0a 2020 696e  AL Value).{.  in
+0000d2f0: 7420 2a65 6c6d 6e72 2c20 436f 6c75 6d6e  t *elmnr, Column
+0000d300: 203d 206d 6174 2d3e 636f 6c75 6d6e 733b   = mat->columns;
+0000d310: 0a0a 2020 2f2a 2053 6574 2073 6d61 6c6c  ..  /* Set small
+0000d320: 206e 756d 6265 7273 2074 6f20 7a65 726f   numbers to zero
+0000d330: 202a 2f0a 2020 6966 2866 6162 7328 5661   */.  if(fabs(Va
+0000d340: 6c75 6529 203c 206d 6174 2d3e 6570 7376  lue) < mat->epsv
+0000d350: 616c 7565 290a 2020 2020 5661 6c75 6520  alue).    Value 
+0000d360: 3d20 303b 0a23 6966 6465 6620 446f 4d61  = 0;.#ifdef DoMa
+0000d370: 7472 6978 526f 756e 6469 6e67 0a20 2065  trixRounding.  e
+0000d380: 6c73 650a 2020 2020 5661 6c75 6520 3d20  lse.    Value = 
+0000d390: 726f 756e 6454 6f50 7265 6369 7369 6f6e  roundToPrecision
+0000d3a0: 2856 616c 7565 2c20 6d61 742d 3e65 7073  (Value, mat->eps
+0000d3b0: 7661 6c75 6529 3b0a 2365 6e64 6966 0a0a  value);.#endif..
+0000d3c0: 2020 2f2a 2043 6865 636b 2069 6620 6d6f    /* Check if mo
+0000d3d0: 7265 2073 7061 6365 2069 7320 6e65 6564  re space is need
+0000d3e0: 6564 2066 6f72 206d 6174 7269 7820 2a2f  ed for matrix */
+0000d3f0: 0a20 2069 6628 2169 6e63 5f6d 6174 5f73  .  if(!inc_mat_s
+0000d400: 7061 6365 286d 6174 2c20 3129 290a 2020  pace(mat, 1)).  
+0000d410: 2020 7265 7475 726e 2846 414c 5345 293b    return(FALSE);
+0000d420: 0a0a 2369 6664 6566 2050 6172 616e 6f69  ..#ifdef Paranoi
+0000d430: 610a 2020 2f2a 2043 6865 636b 2076 616c  a.  /* Check val
+0000d440: 6964 2069 6e64 6563 6573 202a 2f0a 2020  id indeces */.  
+0000d450: 6966 2828 526f 7720 3c20 3029 207c 7c20  if((Row < 0) || 
+0000d460: 2852 6f77 203e 206d 6174 2d3e 726f 7773  (Row > mat->rows
+0000d470: 2929 207b 0a20 2020 2072 6570 6f72 7428  )) {.    report(
+0000d480: 6d61 742d 3e6c 702c 2053 4556 4552 452c  mat->lp, SEVERE,
+0000d490: 2022 6d61 745f 6170 7065 6e64 7661 6c75   "mat_appendvalu
+0000d4a0: 653a 2049 6e76 616c 6964 2072 6f77 2069  e: Invalid row i
+0000d4b0: 6e64 6578 2025 6420 7370 6563 6966 6965  ndex %d specifie
+0000d4c0: 645c 6e22 2c20 526f 7729 3b0a 2020 2020  d\n", Row);.    
+0000d4d0: 7265 7475 726e 2846 414c 5345 293b 0a20  return(FALSE);. 
+0000d4e0: 207d 0a23 656e 6469 660a 0a20 202f 2a20   }.#endif..  /* 
+0000d4f0: 4765 7420 696e 7365 7274 696f 6e20 706f  Get insertion po
+0000d500: 696e 7420 616e 6420 7365 7420 7661 6c75  int and set valu
+0000d510: 6520 2a2f 0a20 2065 6c6d 6e72 203d 206d  e */.  elmnr = m
+0000d520: 6174 2d3e 636f 6c5f 656e 6420 2b20 436f  at->col_end + Co
+0000d530: 6c75 6d6e 3b0a 2020 5345 545f 4d41 545f  lumn;.  SET_MAT_
+0000d540: 696a 4128 282a 656c 6d6e 7229 2c20 526f  ijA((*elmnr), Ro
+0000d550: 772c 2043 6f6c 756d 6e2c 2056 616c 7565  w, Column, Value
+0000d560: 293b 0a0a 2020 2f2a 2055 7064 6174 6520  );..  /* Update 
+0000d570: 636f 6c75 6d6e 2063 6f75 6e74 202a 2f0a  column count */.
+0000d580: 2020 282a 656c 6d6e 7229 2b2b 3b0a 2020    (*elmnr)++;.  
+0000d590: 6d61 742d 3e72 6f77 5f65 6e64 5f76 616c  mat->row_end_val
+0000d5a0: 6964 203d 2046 414c 5345 3b0a 0a20 2072  id = FALSE;..  r
+0000d5b0: 6574 7572 6e28 5452 5545 293b 0a7d 0a0a  eturn(TRUE);.}..
+0000d5c0: 5354 4154 4943 204d 5942 4f4f 4c20 6d61  STATIC MYBOOL ma
+0000d5d0: 745f 6571 7561 6c52 6f77 7328 4d41 5472  t_equalRows(MATr
+0000d5e0: 6563 202a 6d61 742c 2069 6e74 2062 6173  ec *mat, int bas
+0000d5f0: 6572 6f77 2c20 696e 7420 636f 6d70 726f  erow, int compro
+0000d600: 7729 0a7b 0a20 204d 5942 4f4f 4c20 7374  w).{.  MYBOOL st
+0000d610: 6174 7573 203d 2046 414c 5345 3b0a 0a20  atus = FALSE;.. 
+0000d620: 2069 6628 6d61 745f 7661 6c69 6461 7465   if(mat_validate
+0000d630: 286d 6174 2929 207b 0a20 2020 2069 6e74  (mat)) {.    int
+0000d640: 2062 6a31 203d 2030 2c20 656a 312c 2062   bj1 = 0, ej1, b
+0000d650: 6a32 203d 2030 2c20 656a 323b 0a0a 2020  j2 = 0, ej2;..  
+0000d660: 2020 2f2a 2047 6574 2073 7461 7274 696e    /* Get startin
+0000d670: 6720 616e 6420 656e 6469 6e67 2070 6f73  g and ending pos
+0000d680: 6974 696f 6e73 202a 2f0a 2020 2020 6966  itions */.    if
+0000d690: 2862 6173 6572 6f77 203e 3d20 3029 0a20  (baserow >= 0). 
+0000d6a0: 2020 2020 2062 6a31 203d 206d 6174 2d3e       bj1 = mat->
+0000d6b0: 726f 775f 656e 645b 6261 7365 726f 772d  row_end[baserow-
+0000d6c0: 315d 3b0a 2020 2020 656a 3120 3d20 6d61  1];.    ej1 = ma
+0000d6d0: 742d 3e72 6f77 5f65 6e64 5b62 6173 6572  t->row_end[baser
+0000d6e0: 6f77 5d3b 0a20 2020 2069 6628 636f 6d70  ow];.    if(comp
+0000d6f0: 726f 7720 3e3d 2030 290a 2020 2020 2020  row >= 0).      
+0000d700: 626a 3220 3d20 6d61 742d 3e72 6f77 5f65  bj2 = mat->row_e
+0000d710: 6e64 5b63 6f6d 7072 6f77 2d31 5d3b 0a20  nd[comprow-1];. 
+0000d720: 2020 2065 6a32 203d 206d 6174 2d3e 726f     ej2 = mat->ro
+0000d730: 775f 656e 645b 636f 6d70 726f 775d 3b0a  w_end[comprow];.
+0000d740: 2020 2020 2f2a 2046 6169 6c20 6966 2072      /* Fail if r
+0000d750: 6f77 206c 656e 6774 6873 2061 7265 2075  ow lengths are u
+0000d760: 6e65 7175 616c 202a 2f0a 2020 2020 6966  nequal */.    if
+0000d770: 2828 656a 312d 626a 3129 2021 3d20 2865  ((ej1-bj1) != (e
+0000d780: 6a32 2d62 6a32 2929 0a20 2020 2020 2072  j2-bj2)).      r
+0000d790: 6574 7572 6e28 2073 7461 7475 7320 293b  eturn( status );
+0000d7a0: 0a0a 2020 2020 2f2a 2043 6f6d 7061 7265  ..    /* Compare
+0000d7b0: 2063 6f6c 756d 6e20 696e 6465 7820 616e   column index an
+0000d7c0: 6420 7661 6c75 652c 2065 6c65 6d65 6e74  d value, element
+0000d7d0: 2062 7920 656c 656d 656e 7420 2a2f 0a20   by element */. 
+0000d7e0: 2020 2066 6f72 283b 2062 6a31 203c 2065     for(; bj1 < e
+0000d7f0: 6a31 3b20 626a 312b 2b2c 2062 6a32 2b2b  j1; bj1++, bj2++
+0000d800: 2920 7b0a 2020 2020 2020 6966 2843 4f4c  ) {.      if(COL
+0000d810: 5f4d 4154 5f43 4f4c 4e52 2862 6a31 2920  _MAT_COLNR(bj1) 
+0000d820: 213d 2043 4f4c 5f4d 4154 5f43 4f4c 4e52  != COL_MAT_COLNR
+0000d830: 2862 6a32 2929 0a20 2020 2020 2020 2062  (bj2)).        b
+0000d840: 7265 616b 3b0a 2369 6620 310a 2020 2020  reak;.#if 1.    
+0000d850: 2020 6966 2866 6162 7328 6765 745f 6d61    if(fabs(get_ma
+0000d860: 745f 6279 696e 6465 7828 6d61 742d 3e6c  t_byindex(mat->l
+0000d870: 702c 2062 6a31 2c20 5452 5545 2c20 4641  p, bj1, TRUE, FA
+0000d880: 4c53 4529 2d67 6574 5f6d 6174 5f62 7969  LSE)-get_mat_byi
+0000d890: 6e64 6578 286d 6174 2d3e 6c70 2c20 626a  ndex(mat->lp, bj
+0000d8a0: 322c 2054 5255 452c 2046 414c 5345 2929  2, TRUE, FALSE))
+0000d8b0: 203e 206d 6174 2d3e 6c70 2d3e 6570 7370   > mat->lp->epsp
+0000d8c0: 7269 6d61 6c29 0a23 656c 7365 0a20 2020  rimal).#else.   
+0000d8d0: 2020 2069 6628 6661 6273 2843 4f4c 5f4d     if(fabs(COL_M
+0000d8e0: 4154 5f56 414c 5545 2862 6a31 292d 434f  AT_VALUE(bj1)-CO
+0000d8f0: 4c5f 4d41 545f 5641 4c55 4528 626a 3229  L_MAT_VALUE(bj2)
+0000d900: 2920 3e20 6d61 742d 3e6c 702d 3e65 7073  ) > mat->lp->eps
+0000d910: 7072 696d 616c 290a 2365 6e64 6966 0a20  primal).#endif. 
+0000d920: 2020 2020 2020 2062 7265 616b 3b0a 2020         break;.  
+0000d930: 2020 7d0a 2020 2020 7374 6174 7573 203d    }.    status =
+0000d940: 2028 4d59 424f 4f4c 2920 2862 6a31 203d   (MYBOOL) (bj1 =
+0000d950: 3d20 656a 3129 3b0a 2020 7d0a 2020 7265  = ej1);.  }.  re
+0000d960: 7475 726e 2820 7374 6174 7573 2029 3b0a  turn( status );.
+0000d970: 7d0a 0a53 5441 5449 4320 696e 7420 6d61  }..STATIC int ma
+0000d980: 745f 6669 6e64 636f 6c75 6d6e 284d 4154  t_findcolumn(MAT
+0000d990: 7265 6320 2a6d 6174 2c20 696e 7420 6d61  rec *mat, int ma
+0000d9a0: 7469 6e64 6578 290a 7b0a 2020 696e 7420  tindex).{.  int 
+0000d9b0: 6a3b 0a0a 2020 666f 7228 6a20 3d20 313b  j;..  for(j = 1;
+0000d9c0: 206a 203c 3d20 6d61 742d 3e63 6f6c 756d   j <= mat->colum
+0000d9d0: 6e73 3b20 6a2b 2b29 207b 0a20 2020 2069  ns; j++) {.    i
+0000d9e0: 6628 6d61 7469 6e64 6578 203c 206d 6174  f(matindex < mat
+0000d9f0: 2d3e 636f 6c5f 656e 645b 6a5d 290a 2020  ->col_end[j]).  
+0000da00: 2020 2020 6272 6561 6b3b 0a20 207d 0a20      break;.  }. 
+0000da10: 2072 6574 7572 6e28 6a29 3b0a 7d0a 0a53   return(j);.}..S
+0000da20: 5441 5449 4320 696e 7420 6d61 745f 6578  TATIC int mat_ex
+0000da30: 7061 6e64 636f 6c75 6d6e 284d 4154 7265  pandcolumn(MATre
+0000da40: 6320 2a6d 6174 2c20 696e 7420 636f 6c6e  c *mat, int coln
+0000da50: 722c 2052 4541 4c20 2a63 6f6c 756d 6e2c  r, REAL *column,
+0000da60: 2069 6e74 202a 6e7a 6c69 7374 2c20 4d59   int *nzlist, MY
+0000da70: 424f 4f4c 2073 6967 6e65 6441 290a 7b0a  BOOL signedA).{.
+0000da80: 2020 4d59 424f 4f4c 2020 6973 4120 3d20    MYBOOL  isA = 
+0000da90: 284d 5942 4f4f 4c29 2028 6d61 742d 3e6c  (MYBOOL) (mat->l
+0000daa0: 702d 3e6d 6174 4120 3d3d 206d 6174 293b  p->matA == mat);
+0000dab0: 0a20 2069 6e74 2020 2020 2069 2c20 6965  .  int     i, ie
+0000dac0: 2c20 6a2c 206e 7a63 6f75 6e74 203d 2030  , j, nzcount = 0
+0000dad0: 3b0a 2020 5245 414c 2020 2020 2a6d 6174  ;.  REAL    *mat
+0000dae0: 5661 6c75 653b 0a20 2069 6e74 2020 2020  Value;.  int    
+0000daf0: 202a 6d61 7452 6f77 6e72 3b0a 0a20 2073   *matRownr;..  s
+0000db00: 6967 6e65 6441 2026 3d20 6973 413b 0a0a  ignedA &= isA;..
+0000db10: 2020 2f2a 2052 6574 7269 6576 6520 6120    /* Retrieve a 
+0000db20: 636f 6c75 6d6e 2066 726f 6d20 7468 6520  column from the 
+0000db30: 7573 6572 2064 6174 6120 6d61 7472 6978  user data matrix
+0000db40: 2041 202a 2f0a 2020 4d45 4d43 4c45 4152   A */.  MEMCLEAR
+0000db50: 2863 6f6c 756d 6e2c 206d 6174 2d3e 726f  (column, mat->ro
+0000db60: 7773 202b 2031 293b 0a20 2069 6628 6973  ws + 1);.  if(is
+0000db70: 4129 207b 0a20 2020 2063 6f6c 756d 6e5b  A) {.    column[
+0000db80: 305d 203d 206d 6174 2d3e 6c70 2d3e 6f72  0] = mat->lp->or
+0000db90: 6967 5f6f 626a 5b63 6f6c 6e72 5d3b 0a20  ig_obj[colnr];. 
+0000dba0: 2020 2069 6628 7369 676e 6564 4120 2626     if(signedA &&
+0000dbb0: 2069 735f 6368 7369 676e 286d 6174 2d3e   is_chsign(mat->
+0000dbc0: 6c70 2c20 3029 290a 2020 2020 2020 636f  lp, 0)).      co
+0000dbd0: 6c75 6d6e 5b30 5d20 3d20 2d63 6f6c 756d  lumn[0] = -colum
+0000dbe0: 6e5b 305d 3b0a 2020 7d0a 0a20 2069 203d  n[0];.  }..  i =
+0000dbf0: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
+0000dc00: 6c6e 7220 2d20 315d 3b0a 2020 6965 203d  lnr - 1];.  ie =
+0000dc10: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
+0000dc20: 6c6e 725d 3b0a 2020 6d61 7452 6f77 6e72  lnr];.  matRownr
+0000dc30: 203d 2026 434f 4c5f 4d41 545f 524f 574e   = &COL_MAT_ROWN
+0000dc40: 5228 6929 3b0a 2020 6d61 7456 616c 7565  R(i);.  matValue
+0000dc50: 203d 2026 434f 4c5f 4d41 545f 5641 4c55   = &COL_MAT_VALU
+0000dc60: 4528 6929 3b0a 2020 666f 7228 3b20 6920  E(i);.  for(; i 
+0000dc70: 3c20 6965 3b0a 2020 2020 2020 692b 2b2c  < ie;.      i++,
+0000dc80: 206d 6174 526f 776e 7220 2b3d 206d 6174   matRownr += mat
+0000dc90: 526f 7743 6f6c 5374 6570 2c20 6d61 7456  RowColStep, matV
+0000dca0: 616c 7565 202b 3d20 6d61 7456 616c 7565  alue += matValue
+0000dcb0: 5374 6570 2920 7b0a 2020 2020 6a20 3d20  Step) {.    j = 
+0000dcc0: 2a6d 6174 526f 776e 723b 0a20 2020 2063  *matRownr;.    c
+0000dcd0: 6f6c 756d 6e5b 6a5d 203d 202a 6d61 7456  olumn[j] = *matV
+0000dce0: 616c 7565 3b0a 2020 2020 6966 2873 6967  alue;.    if(sig
+0000dcf0: 6e65 6441 2026 2620 6973 5f63 6873 6967  nedA && is_chsig
+0000dd00: 6e28 6d61 742d 3e6c 702c 206a 2929 0a20  n(mat->lp, j)). 
+0000dd10: 2020 2020 2063 6f6c 756d 6e5b 6a5d 203d       column[j] =
+0000dd20: 202d 636f 6c75 6d6e 5b6a 5d3b 0a20 2020   -column[j];.   
+0000dd30: 206e 7a63 6f75 6e74 2b2b 3b0a 2020 2020   nzcount++;.    
+0000dd40: 6966 286e 7a6c 6973 7420 213d 204e 554c  if(nzlist != NUL
+0000dd50: 4c29 0a20 2020 2020 206e 7a6c 6973 745b  L).      nzlist[
+0000dd60: 6e7a 636f 756e 745d 203d 206a 3b0a 2020  nzcount] = j;.  
+0000dd70: 7d0a 2020 6966 286e 7a6c 6973 7420 213d  }.  if(nzlist !=
+0000dd80: 204e 554c 4c29 0a20 2020 206e 7a6c 6973   NULL).    nzlis
+0000dd90: 745b 305d 203d 206e 7a63 6f75 6e74 3b0a  t[0] = nzcount;.
+0000dda0: 2020 7265 7475 726e 2820 6e7a 636f 756e    return( nzcoun
+0000ddb0: 7420 293b 0a7d 0a0a 5354 4154 4943 204d  t );.}..STATIC M
+0000ddc0: 5942 4f4f 4c20 6d61 745f 636f 6d70 7574  YBOOL mat_comput
+0000ddd0: 656d 6178 284d 4154 7265 6320 2a6d 6174  emax(MATrec *mat
+0000dde0: 290a 7b0a 2020 696e 7420 202a 726f 776e  ).{.  int  *rown
+0000ddf0: 7220 3d20 2643 4f4c 5f4d 4154 5f52 4f57  r = &COL_MAT_ROW
+0000de00: 4e52 2830 292c 0a20 2020 2020 2020 2a63  NR(0),.       *c
+0000de10: 6f6c 6e72 203d 2026 434f 4c5f 4d41 545f  olnr = &COL_MAT_
+0000de20: 434f 4c4e 5228 3029 2c0a 2020 2020 2020  COLNR(0),.      
+0000de30: 2069 203d 2030 2c20 6965 203d 206d 6174   i = 0, ie = mat
+0000de40: 2d3e 636f 6c5f 656e 645b 6d61 742d 3e63  ->col_end[mat->c
+0000de50: 6f6c 756d 6e73 5d2c 2065 7a20 3d20 303b  olumns], ez = 0;
+0000de60: 0a20 2052 4541 4c20 2a76 616c 7565 203d  .  REAL *value =
+0000de70: 2026 434f 4c5f 4d41 545f 5641 4c55 4528   &COL_MAT_VALUE(
+0000de80: 3029 2c20 6570 736d 6163 6869 6e65 203d  0), epsmachine =
+0000de90: 206d 6174 2d3e 6c70 2d3e 6570 736d 6163   mat->lp->epsmac
+0000dea0: 6869 6e65 2c20 6162 7376 616c 7565 3b0a  hine, absvalue;.
+0000deb0: 0a20 202f 2a20 5072 6570 6172 6520 6172  .  /* Prepare ar
+0000dec0: 7261 7973 202a 2f0a 2020 6966 2821 616c  rays */.  if(!al
+0000ded0: 6c6f 6352 4541 4c28 6d61 742d 3e6c 702c  locREAL(mat->lp,
+0000dee0: 2026 6d61 742d 3e63 6f6c 6d61 782c 206d   &mat->colmax, m
+0000def0: 6174 2d3e 636f 6c75 6d6e 735f 616c 6c6f  at->columns_allo
+0000df00: 632b 312c 2041 5554 4f4d 4154 4943 2920  c+1, AUTOMATIC) 
+0000df10: 7c7c 0a20 2020 2020 2161 6c6c 6f63 5245  ||.     !allocRE
+0000df20: 414c 286d 6174 2d3e 6c70 2c20 266d 6174  AL(mat->lp, &mat
+0000df30: 2d3e 726f 776d 6178 2c20 6d61 742d 3e72  ->rowmax, mat->r
+0000df40: 6f77 735f 616c 6c6f 632b 312c 2041 5554  ows_alloc+1, AUT
+0000df50: 4f4d 4154 4943 2929 0a20 2020 2020 7265  OMATIC)).     re
+0000df60: 7475 726e 2820 4641 4c53 4520 293b 0a20  turn( FALSE );. 
+0000df70: 204d 454d 434c 4541 5228 6d61 742d 3e63   MEMCLEAR(mat->c
+0000df80: 6f6c 6d61 782c 206d 6174 2d3e 636f 6c75  olmax, mat->colu
+0000df90: 6d6e 732b 3129 3b0a 2020 4d45 4d43 4c45  mns+1);.  MEMCLE
+0000dfa0: 4152 286d 6174 2d3e 726f 776d 6178 2c20  AR(mat->rowmax, 
+0000dfb0: 6d61 742d 3e72 6f77 732b 3129 3b0a 0a20  mat->rows+1);.. 
+0000dfc0: 202f 2a20 4f62 7461 696e 2074 6865 2072   /* Obtain the r
+0000dfd0: 6f77 2061 6e64 2063 6f6c 756d 6e20 6d61  ow and column ma
+0000dfe0: 7869 6d61 2069 6e20 6f6e 6520 7377 6565  xima in one swee
+0000dff0: 7020 2a2f 0a20 206d 6174 2d3e 6479 6e72  p */.  mat->dynr
+0000e000: 616e 6765 203d 206d 6174 2d3e 6c70 2d3e  ange = mat->lp->
+0000e010: 696e 6669 6e69 7465 3b0a 2020 666f 7228  infinite;.  for(
+0000e020: 3b20 6920 3c20 6965 3b0a 2020 2020 2020  ; i < ie;.      
+0000e030: 692b 2b2c 2072 6f77 6e72 202b 3d20 6d61  i++, rownr += ma
+0000e040: 7452 6f77 436f 6c53 7465 702c 2063 6f6c  tRowColStep, col
+0000e050: 6e72 202b 3d20 6d61 7452 6f77 436f 6c53  nr += matRowColS
+0000e060: 7465 702c 2076 616c 7565 202b 3d20 6d61  tep, value += ma
+0000e070: 7456 616c 7565 5374 6570 2920 7b0a 2020  tValueStep) {.  
+0000e080: 2020 6162 7376 616c 7565 203d 2066 6162    absvalue = fab
+0000e090: 7328 2a76 616c 7565 293b 0a20 2020 2053  s(*value);.    S
+0000e0a0: 4554 4d41 5828 6d61 742d 3e63 6f6c 6d61  ETMAX(mat->colma
+0000e0b0: 785b 2a63 6f6c 6e72 5d2c 2061 6273 7661  x[*colnr], absva
+0000e0c0: 6c75 6529 3b0a 2020 2020 5345 544d 4158  lue);.    SETMAX
+0000e0d0: 286d 6174 2d3e 726f 776d 6178 5b2a 726f  (mat->rowmax[*ro
+0000e0e0: 776e 725d 2c20 6162 7376 616c 7565 293b  wnr], absvalue);
+0000e0f0: 0a20 2020 2053 4554 4d49 4e28 6d61 742d  .    SETMIN(mat-
+0000e100: 3e64 796e 7261 6e67 652c 2061 6273 7661  >dynrange, absva
+0000e110: 6c75 6529 3b0a 2020 2020 6966 2861 6273  lue);.    if(abs
+0000e120: 7661 6c75 6520 3c20 6570 736d 6163 6869  value < epsmachi
+0000e130: 6e65 290a 2020 2020 2020 657a 2b2b 3b0a  ne).      ez++;.
+0000e140: 2020 7d0a 0a20 202f 2a20 4c61 7374 6c79    }..  /* Lastly
+0000e150: 2c20 636f 6d70 7574 6520 7468 6520 676c  , compute the gl
+0000e160: 6f62 616c 206d 6178 696d 756d 2061 6e64  obal maximum and
+0000e170: 2067 6574 2074 6865 2064 796e 616d 6963   get the dynamic
+0000e180: 2072 616e 6765 202a 2f0a 2020 666f 7228   range */.  for(
+0000e190: 6920 3d20 313b 2069 203c 3d20 6d61 742d  i = 1; i <= mat-
+0000e1a0: 3e72 6f77 733b 2069 2b2b 290a 2020 2020  >rows; i++).    
+0000e1b0: 5345 544d 4158 286d 6174 2d3e 726f 776d  SETMAX(mat->rowm
+0000e1c0: 6178 5b30 5d2c 206d 6174 2d3e 726f 776d  ax[0], mat->rowm
+0000e1d0: 6178 5b69 5d29 3b0a 2020 6d61 742d 3e69  ax[i]);.  mat->i
+0000e1e0: 6e66 6e6f 726d 203d 206d 6174 2d3e 636f  nfnorm = mat->co
+0000e1f0: 6c6d 6178 5b30 5d20 3d20 6d61 742d 3e72  lmax[0] = mat->r
+0000e200: 6f77 6d61 785b 305d 3b0a 2020 6966 286d  owmax[0];.  if(m
+0000e210: 6174 2d3e 6479 6e72 616e 6765 203d 3d20  at->dynrange == 
+0000e220: 3029 207b 0a20 2020 2072 6570 6f72 7428  0) {.    report(
+0000e230: 6d61 742d 3e6c 702c 2053 4556 4552 452c  mat->lp, SEVERE,
+0000e240: 2022 2564 206d 6174 7269 7820 636f 6e74   "%d matrix cont
+0000e250: 6169 6e73 207a 6572 6f2d 7661 6c75 6564  ains zero-valued
+0000e260: 2063 6f65 6666 6963 6965 6e74 732e 5c6e   coefficients.\n
+0000e270: 222c 2065 7a29 3b0a 2020 2020 6d61 742d  ", ez);.    mat-
+0000e280: 3e64 796e 7261 6e67 6520 3d20 6d61 742d  >dynrange = mat-
+0000e290: 3e6c 702d 3e69 6e66 696e 6974 653b 0a20  >lp->infinite;. 
+0000e2a0: 207d 0a20 2065 6c73 6520 7b0a 2020 2020   }.  else {.    
+0000e2b0: 6d61 742d 3e64 796e 7261 6e67 6520 3d20  mat->dynrange = 
+0000e2c0: 6d61 742d 3e69 6e66 6e6f 726d 202f 206d  mat->infnorm / m
+0000e2d0: 6174 2d3e 6479 6e72 616e 6765 3b0a 2020  at->dynrange;.  
+0000e2e0: 2020 6966 2865 7a20 3e20 3029 0a20 2020    if(ez > 0).   
+0000e2f0: 2020 2072 6570 6f72 7428 6d61 742d 3e6c     report(mat->l
+0000e300: 702c 2049 4d50 4f52 5441 4e54 2c20 2225  p, IMPORTANT, "%
+0000e310: 6420 6d61 7472 6978 2063 6f65 6666 6963  d matrix coeffic
+0000e320: 6965 6e74 7320 6265 6c6f 7720 6d61 6368  ients below mach
+0000e330: 696e 6520 7072 6563 6973 696f 6e20 7765  ine precision we
+0000e340: 7265 2066 6f75 6e64 2e5c 6e22 2c20 657a  re found.\n", ez
+0000e350: 293b 0a20 207d 0a0a 2020 7265 7475 726e  );.  }..  return
+0000e360: 2820 5452 5545 2029 3b0a 7d0a 0a53 5441  ( TRUE );.}..STA
+0000e370: 5449 4320 4d59 424f 4f4c 206d 6174 5f74  TIC MYBOOL mat_t
+0000e380: 7261 6e73 706f 7365 284d 4154 7265 6320  ranspose(MATrec 
+0000e390: 2a6d 6174 290a 7b0a 2020 696e 7420 2020  *mat).{.  int   
+0000e3a0: 2020 692c 206a 2c20 6e7a 2c20 6b3b 0a20    i, j, nz, k;. 
+0000e3b0: 204d 5942 4f4f 4c20 2073 7461 7475 733b   MYBOOL  status;
+0000e3c0: 0a0a 2020 7374 6174 7573 203d 206d 6174  ..  status = mat
+0000e3d0: 5f76 616c 6964 6174 6528 6d61 7429 3b0a  _validate(mat);.
+0000e3e0: 2020 6966 2873 7461 7475 7329 207b 0a0a    if(status) {..
+0000e3f0: 2020 2020 2f2a 2043 7265 6174 6520 6120      /* Create a 
+0000e400: 636f 6c75 6d6e 2d6f 7264 6572 6564 2073  column-ordered s
+0000e410: 7061 7273 6520 656c 656d 656e 7420 6c69  parse element li
+0000e420: 7374 3b20 2263 6f6c 756d 6e22 2069 6e64  st; "column" ind
+0000e430: 6578 206d 7573 7420 6265 2073 6869 6674  ex must be shift
+0000e440: 6564 202a 2f0a 2020 2020 6e7a 203d 206d  ed */.    nz = m
+0000e450: 6174 5f6e 6f6e 7a65 726f 7328 6d61 7429  at_nonzeros(mat)
+0000e460: 3b0a 2020 2020 6966 286e 7a20 3e20 3029  ;.    if(nz > 0)
+0000e470: 207b 0a23 6966 204d 6174 7269 7843 6f6c   {.#if MatrixCol
+0000e480: 4163 6365 7373 3d3d 4341 4d5f 5265 636f  Access==CAM_Reco
+0000e490: 7264 0a20 2020 2020 204d 4154 6974 656d  rd.      MATitem
+0000e4a0: 202a 6e65 776d 6174 3b0a 2020 2020 2020   *newmat;.      
+0000e4b0: 6e65 776d 6174 203d 2028 4d41 5469 7465  newmat = (MATite
+0000e4c0: 6d20 2a29 206d 616c 6c6f 6328 286d 6174  m *) malloc((mat
+0000e4d0: 2d3e 6d61 745f 616c 6c6f 6329 202a 2073  ->mat_alloc) * s
+0000e4e0: 697a 656f 6628 2a28 6d61 742d 3e63 6f6c  izeof(*(mat->col
+0000e4f0: 5f6d 6174 2929 293b 0a20 2020 2020 206a  _mat)));.      j
+0000e500: 203d 206d 6174 2d3e 726f 775f 656e 645b   = mat->row_end[
+0000e510: 305d 3b0a 2020 2020 2020 666f 7228 6920  0];.      for(i 
+0000e520: 3d20 6e7a 2d31 3b20 6920 3e3d 206a 203b  = nz-1; i >= j ;
+0000e530: 2069 2d2d 2920 7b0a 2020 2020 2020 2020   i--) {.        
+0000e540: 6b20 3d20 692d 6a3b 0a20 2020 2020 2020  k = i-j;.       
+0000e550: 206e 6577 6d61 745b 6b5d 203d 206d 6174   newmat[k] = mat
+0000e560: 2d3e 636f 6c5f 6d61 745b 6d61 742d 3e72  ->col_mat[mat->r
+0000e570: 6f77 5f6d 6174 5b69 5d5d 3b0a 2020 2020  ow_mat[i]];.    
+0000e580: 2020 2020 6e65 776d 6174 5b6b 5d2e 726f      newmat[k].ro
+0000e590: 775f 6e72 203d 206e 6577 6d61 745b 6b5d  w_nr = newmat[k]
+0000e5a0: 2e63 6f6c 5f6e 723b 0a20 2020 2020 207d  .col_nr;.      }
+0000e5b0: 0a20 2020 2020 2066 6f72 2869 203d 206a  .      for(i = j
+0000e5c0: 2d31 3b20 6920 3e3d 2030 203b 2069 2d2d  -1; i >= 0 ; i--
+0000e5d0: 2920 7b0a 2020 2020 2020 2020 6b20 3d20  ) {.        k = 
+0000e5e0: 6e7a 2d6a 2b69 3b0a 2020 2020 2020 2020  nz-j+i;.        
+0000e5f0: 6e65 776d 6174 5b6b 5d20 3d20 6d61 742d  newmat[k] = mat-
+0000e600: 3e63 6f6c 5f6d 6174 5b6d 6174 2d3e 726f  >col_mat[mat->ro
+0000e610: 775f 6d61 745b 695d 5d3b 0a20 2020 2020  w_mat[i]];.     
+0000e620: 2020 206e 6577 6d61 745b 6b5d 2e72 6f77     newmat[k].row
+0000e630: 5f6e 7220 3d20 6e65 776d 6174 5b6b 5d2e  _nr = newmat[k].
+0000e640: 636f 6c5f 6e72 3b0a 2020 2020 2020 7d0a  col_nr;.      }.
+0000e650: 2020 2020 2020 7377 6170 5054 5228 2876        swapPTR((v
+0000e660: 6f69 6420 2a2a 2920 266d 6174 2d3e 636f  oid **) &mat->co
+0000e670: 6c5f 6d61 742c 2028 766f 6964 202a 2a29  l_mat, (void **)
+0000e680: 2026 6e65 776d 6174 293b 0a20 2020 2020   &newmat);.     
+0000e690: 2046 5245 4528 6e65 776d 6174 293b 0a23   FREE(newmat);.#
+0000e6a0: 656c 7365 202f 2a69 6620 4d61 7472 6978  else /*if Matrix
+0000e6b0: 436f 6c41 6363 6573 733d 3d43 414d 5f56  ColAccess==CAM_V
+0000e6c0: 6563 746f 722a 2f0a 2020 2020 2020 5245  ector*/.      RE
+0000e6d0: 414c 202a 6e65 7756 616c 7565 203d 204e  AL *newValue = N
+0000e6e0: 554c 4c3b 0a20 2020 2020 2069 6e74 2020  ULL;.      int  
+0000e6f0: 2a6e 6577 526f 776e 7220 3d20 4e55 4c4c  *newRownr = NULL
+0000e700: 3b0a 2020 2020 2020 616c 6c6f 6352 4541  ;.      allocREA
+0000e710: 4c28 6d61 742d 3e6c 702c 2026 6e65 7756  L(mat->lp, &newV
+0000e720: 616c 7565 2c20 6d61 742d 3e6d 6174 5f61  alue, mat->mat_a
+0000e730: 6c6c 6f63 2c20 4641 4c53 4529 3b0a 2020  lloc, FALSE);.  
+0000e740: 2020 2020 616c 6c6f 6349 4e54 286d 6174      allocINT(mat
+0000e750: 2d3e 6c70 2c20 266e 6577 526f 776e 722c  ->lp, &newRownr,
+0000e760: 206d 6174 2d3e 6d61 745f 616c 6c6f 632c   mat->mat_alloc,
+0000e770: 2046 414c 5345 293b 0a0a 2020 2020 2020   FALSE);..      
+0000e780: 6a20 3d20 6d61 742d 3e72 6f77 5f65 6e64  j = mat->row_end
+0000e790: 5b30 5d3b 0a20 2020 2020 2066 6f72 2869  [0];.      for(i
+0000e7a0: 203d 206e 7a2d 313b 2069 203e 3d20 6a20   = nz-1; i >= j 
+0000e7b0: 3b20 692d 2d29 207b 0a20 2020 2020 2020  ; i--) {.       
+0000e7c0: 206b 203d 2069 2d6a 3b0a 2020 2020 2020   k = i-j;.      
+0000e7d0: 2020 6e65 7756 616c 7565 5b6b 5d20 3d20    newValue[k] = 
+0000e7e0: 524f 575f 4d41 545f 5641 4c55 4528 6929  ROW_MAT_VALUE(i)
+0000e7f0: 3b0a 2020 2020 2020 2020 6e65 7752 6f77  ;.        newRow
+0000e800: 6e72 5b6b 5d20 3d20 524f 575f 4d41 545f  nr[k] = ROW_MAT_
+0000e810: 434f 4c4e 5228 6929 3b0a 2020 2020 2020  COLNR(i);.      
+0000e820: 7d0a 2020 2020 2020 666f 7228 6920 3d20  }.      for(i = 
+0000e830: 6a2d 313b 2069 203e 3d20 3020 3b20 692d  j-1; i >= 0 ; i-
+0000e840: 2d29 207b 0a20 2020 2020 2020 206b 203d  -) {.        k =
+0000e850: 206e 7a2d 6a2b 693b 0a20 2020 2020 2020   nz-j+i;.       
+0000e860: 206e 6577 5661 6c75 655b 6b5d 203d 2052   newValue[k] = R
+0000e870: 4f57 5f4d 4154 5f56 414c 5545 2869 293b  OW_MAT_VALUE(i);
+0000e880: 0a20 2020 2020 2020 206e 6577 526f 776e  .        newRown
+0000e890: 725b 6b5d 203d 2052 4f57 5f4d 4154 5f43  r[k] = ROW_MAT_C
+0000e8a0: 4f4c 4e52 2869 293b 0a20 2020 2020 207d  OLNR(i);.      }
+0000e8b0: 0a0a 2020 2020 2020 7377 6170 5054 5228  ..      swapPTR(
+0000e8c0: 2876 6f69 6420 2a2a 2920 266d 6174 2d3e  (void **) &mat->
+0000e8d0: 636f 6c5f 6d61 745f 726f 776e 722c 2028  col_mat_rownr, (
+0000e8e0: 766f 6964 202a 2a29 2026 6e65 7752 6f77  void **) &newRow
+0000e8f0: 6e72 293b 0a20 2020 2020 2073 7761 7050  nr);.      swapP
+0000e900: 5452 2828 766f 6964 202a 2a29 2026 6d61  TR((void **) &ma
+0000e910: 742d 3e63 6f6c 5f6d 6174 5f76 616c 7565  t->col_mat_value
+0000e920: 2c20 2876 6f69 6420 2a2a 2920 266e 6577  , (void **) &new
+0000e930: 5661 6c75 6529 3b0a 2020 2020 2020 4652  Value);.      FR
+0000e940: 4545 286e 6577 5661 6c75 6529 3b0a 2020  EE(newValue);.  
+0000e950: 2020 2020 4652 4545 286e 6577 526f 776e      FREE(newRown
+0000e960: 7229 3b0a 2365 6e64 6966 0a20 2020 207d  r);.#endif.    }
+0000e970: 0a0a 2020 2020 2f2a 2054 7261 6e73 6665  ..    /* Transfe
+0000e980: 7220 726f 7720 7374 6172 7420 746f 2063  r row start to c
+0000e990: 6f6c 756d 6e20 7374 6172 7420 706f 7369  olumn start posi
+0000e9a0: 7469 6f6e 3b20 6d75 7374 2061 646a 7573  tion; must adjus
+0000e9b0: 7420 666f 7220 6469 6666 6572 656e 7420  t for different 
+0000e9c0: 6f66 6673 6574 7320 2a2f 0a20 2020 2069  offsets */.    i
+0000e9d0: 6628 6d61 742d 3e72 6f77 7320 3d3d 206d  f(mat->rows == m
+0000e9e0: 6174 2d3e 726f 7773 5f61 6c6c 6f63 290a  at->rows_alloc).
+0000e9f0: 2020 2020 2020 696e 635f 6d61 7463 6f6c        inc_matcol
+0000ea00: 5f73 7061 6365 286d 6174 2c20 3129 3b0a  _space(mat, 1);.
+0000ea10: 2020 2020 6a20 3d20 6d61 742d 3e72 6f77      j = mat->row
+0000ea20: 5f65 6e64 5b30 5d3b 0a20 2020 2066 6f72  _end[0];.    for
+0000ea30: 2869 203d 206d 6174 2d3e 726f 7773 3b20  (i = mat->rows; 
+0000ea40: 6920 3e3d 2031 3b20 692d 2d29 0a20 2020  i >= 1; i--).   
+0000ea50: 2020 206d 6174 2d3e 726f 775f 656e 645b     mat->row_end[
+0000ea60: 695d 202d 3d20 6a3b 0a20 2020 206d 6174  i] -= j;.    mat
+0000ea70: 2d3e 726f 775f 656e 645b 6d61 742d 3e72  ->row_end[mat->r
+0000ea80: 6f77 735d 203d 206e 7a3b 0a20 2020 2073  ows] = nz;.    s
+0000ea90: 7761 7050 5452 2828 766f 6964 202a 2a29  wapPTR((void **)
+0000eaa0: 2026 6d61 742d 3e72 6f77 5f65 6e64 2c20   &mat->row_end, 
+0000eab0: 2876 6f69 6420 2a2a 2920 266d 6174 2d3e  (void **) &mat->
+0000eac0: 636f 6c5f 656e 6429 3b0a 0a20 2020 202f  col_end);..    /
+0000ead0: 2a20 5377 6170 2061 7272 6179 7320 6f66  * Swap arrays of
+0000eae0: 206d 6178 696d 756d 2076 616c 7565 7320   maximum values 
+0000eaf0: 2a2f 0a20 2020 2073 7761 7050 5452 2828  */.    swapPTR((
+0000eb00: 766f 6964 202a 2a29 2026 6d61 742d 3e72  void **) &mat->r
+0000eb10: 6f77 6d61 782c 2028 766f 6964 202a 2a29  owmax, (void **)
+0000eb20: 2026 6d61 742d 3e63 6f6c 6d61 7829 3b0a   &mat->colmax);.
+0000eb30: 0a20 2020 202f 2a20 5377 6170 2061 7272  .    /* Swap arr
+0000eb40: 6179 2073 697a 6573 202a 2f0a 2020 2020  ay sizes */.    
+0000eb50: 7377 6170 494e 5428 266d 6174 2d3e 726f  swapINT(&mat->ro
+0000eb60: 7773 2c20 266d 6174 2d3e 636f 6c75 6d6e  ws, &mat->column
+0000eb70: 7329 3b0a 2020 2020 7377 6170 494e 5428  s);.    swapINT(
+0000eb80: 266d 6174 2d3e 726f 7773 5f61 6c6c 6f63  &mat->rows_alloc
+0000eb90: 2c20 266d 6174 2d3e 636f 6c75 6d6e 735f  , &mat->columns_
+0000eba0: 616c 6c6f 6329 3b0a 0a20 2020 202f 2a20  alloc);..    /* 
+0000ebb0: 4669 6e61 6c6c 7920 7365 7420 6375 7272  Finally set curr
+0000ebc0: 656e 7420 7374 6f72 6167 6520 6d6f 6465  ent storage mode
+0000ebd0: 202a 2f0a 2020 2020 6d61 742d 3e69 735f   */.    mat->is_
+0000ebe0: 726f 776f 7264 6572 203d 2028 4d59 424f  roworder = (MYBO
+0000ebf0: 4f4c 2920 216d 6174 2d3e 6973 5f72 6f77  OL) !mat->is_row
+0000ec00: 6f72 6465 723b 0a20 2020 206d 6174 2d3e  order;.    mat->
+0000ec10: 726f 775f 656e 645f 7661 6c69 6420 3d20  row_end_valid = 
+0000ec20: 4641 4c53 453b 0a20 207d 0a20 2072 6574  FALSE;.  }.  ret
+0000ec30: 7572 6e28 7374 6174 7573 293b 0a7d 0a0a  urn(status);.}..
+0000ec40: 0a2f 2a20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ./* ------------
+0000ec50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ec60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ec70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ec80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ec90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eca0: 2d2d 2d2d 2d2d 202a 2f0a 2f2a 2043 6861  ------ */./* Cha
-0000ecb0: 6e67 652d 7472 6163 6b69 6e67 2072 6f75  nge-tracking rou
-0000ecc0: 7469 6e65 7320 2020 2020 2020 2020 2020  tines           
+0000ec90: 2d2d 2d2d 2d2d 202a 2f0a 2f2a 2043 6861  ------ */./* Cha
+0000eca0: 6e67 652d 7472 6163 6b69 6e67 2072 6f75  nge-tracking rou
+0000ecb0: 7469 6e65 7320 2020 2020 2020 2020 2020  tines           
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 2a2f 0a2f 2a20 2d2d 2d2d 2d2d 2d2d 2d2d  */./* ----------
+0000ecf0: 2a2f 0a2f 2a20 2d2d 2d2d 2d2d 2d2d 2d2d  */./* ----------
+0000ed00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ed10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ed20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ed30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ed40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ed50: 2d2d 2d2d 2d2d 2d2d 202a 2f0a 5354 4154  -------- */.STAT
-0000ed60: 4943 2044 656c 7461 5672 6563 202a 6372  IC DeltaVrec *cr
-0000ed70: 6561 7465 556e 646f 4c61 6464 6572 286c  eateUndoLadder(l
-0000ed80: 7072 6563 202a 6c70 2c20 696e 7420 6c65  prec *lp, int le
-0000ed90: 7665 6c69 7465 6d73 2c20 696e 7420 6d61  velitems, int ma
-0000eda0: 786c 6576 656c 7329 0a7b 0a20 2044 656c  xlevels).{.  Del
-0000edb0: 7461 5672 6563 202a 686f 6c64 3b0a 0a20  taVrec *hold;.. 
-0000edc0: 2068 6f6c 6420 3d20 2844 656c 7461 5672   hold = (DeltaVr
-0000edd0: 6563 202a 2920 6d61 6c6c 6f63 2873 697a  ec *) malloc(siz
-0000ede0: 656f 6628 2a68 6f6c 6429 293b 0a20 2068  eof(*hold));.  h
-0000edf0: 6f6c 642d 3e6c 7020 3d20 6c70 3b0a 2020  old->lp = lp;.  
-0000ee00: 686f 6c64 2d3e 6163 7469 7665 6c65 7665  hold->activeleve
-0000ee10: 6c20 3d20 303b 0a20 2068 6f6c 642d 3e74  l = 0;.  hold->t
-0000ee20: 7261 636b 6572 203d 206d 6174 5f63 7265  racker = mat_cre
-0000ee30: 6174 6528 6c70 2c20 6c65 7665 6c69 7465  ate(lp, levelite
-0000ee40: 6d73 2c20 302c 2030 2e30 293b 0a20 2069  ms, 0, 0.0);.  i
-0000ee50: 6e63 5f6d 6174 636f 6c5f 7370 6163 6528  nc_matcol_space(
-0000ee60: 686f 6c64 2d3e 7472 6163 6b65 722c 206d  hold->tracker, m
-0000ee70: 6178 6c65 7665 6c73 293b 0a20 2072 6574  axlevels);.  ret
-0000ee80: 7572 6e28 2068 6f6c 6420 293b 0a7d 0a53  urn( hold );.}.S
-0000ee90: 5441 5449 4320 696e 7420 696e 6372 656d  TATIC int increm
-0000eea0: 656e 7455 6e64 6f4c 6164 6465 7228 4465  entUndoLadder(De
-0000eeb0: 6c74 6156 7265 6320 2a44 5629 0a7b 0a20  ltaVrec *DV).{. 
-0000eec0: 2044 562d 3e61 6374 6976 656c 6576 656c   DV->activelevel
-0000eed0: 2b2b 3b0a 2020 696e 635f 6d61 7463 6f6c  ++;.  inc_matcol
-0000eee0: 5f73 7061 6365 2844 562d 3e74 7261 636b  _space(DV->track
-0000eef0: 6572 2c20 3129 3b0a 2020 6d61 745f 7368  er, 1);.  mat_sh
-0000ef00: 6966 7463 6f6c 7328 4456 2d3e 7472 6163  iftcols(DV->trac
-0000ef10: 6b65 722c 2026 2844 562d 3e61 6374 6976  ker, &(DV->activ
-0000ef20: 656c 6576 656c 292c 2031 2c20 4e55 4c4c  elevel), 1, NULL
-0000ef30: 293b 0a20 2044 562d 3e74 7261 636b 6572  );.  DV->tracker
-0000ef40: 2d3e 636f 6c75 6d6e 732b 2b3b 0a20 2072  ->columns++;.  r
-0000ef50: 6574 7572 6e28 4456 2d3e 6163 7469 7665  eturn(DV->active
-0000ef60: 6c65 7665 6c29 3b0a 7d0a 5354 4154 4943  level);.}.STATIC
-0000ef70: 204d 5942 4f4f 4c20 6d6f 6469 6679 556e   MYBOOL modifyUn
-0000ef80: 646f 4c61 6464 6572 2844 656c 7461 5672  doLadder(DeltaVr
-0000ef90: 6563 202a 4456 2c20 696e 7420 6974 656d  ec *DV, int item
-0000efa0: 6e6f 2c20 5245 414c 2074 6172 6765 745b  no, REAL target[
-0000efb0: 5d2c 2052 4541 4c20 6e65 7776 616c 7565  ], REAL newvalue
-0000efc0: 290a 7b0a 2020 4d59 424f 4f4c 2073 7461  ).{.  MYBOOL sta
-0000efd0: 7475 733b 0a20 2069 6e74 2020 2020 7661  tus;.  int    va
-0000efe0: 7269 6e64 6578 203d 2069 7465 6d6e 6f3b  rindex = itemno;
-0000eff0: 0a20 2052 4541 4c20 2020 6f6c 6476 616c  .  REAL   oldval
-0000f000: 7565 203d 2074 6172 6765 745b 6974 656d  ue = target[item
-0000f010: 6e6f 5d3b 0a0a 2369 666e 6465 6620 5573  no];..#ifndef Us
-0000f020: 654d 696c 7053 6c61 636b 7352 4346 2020  eMilpSlacksRCF  
-0000f030: 2f2a 2043 6865 636b 2069 6620 7765 2073  /* Check if we s
-0000f040: 686f 756c 6420 696e 636c 7564 6520 7261  hould include ra
-0000f050: 6e67 6564 2063 6f6e 7374 7261 696e 7473  nged constraints
-0000f060: 202a 2f0a 2020 7661 7269 6e64 6578 202d   */.  varindex -
-0000f070: 3d20 4456 2d3e 6c70 2d3e 726f 7773 3b0a  = DV->lp->rows;.
-0000f080: 2365 6e64 6966 0a20 2073 7461 7475 7320  #endif.  status 
-0000f090: 3d20 6d61 745f 6170 7065 6e64 7661 6c75  = mat_appendvalu
-0000f0a0: 6528 4456 2d3e 7472 6163 6b65 722c 2076  e(DV->tracker, v
-0000f0b0: 6172 696e 6465 782c 206f 6c64 7661 6c75  arindex, oldvalu
-0000f0c0: 6529 3b0a 2020 7461 7267 6574 5b69 7465  e);.  target[ite
-0000f0d0: 6d6e 6f5d 203d 206e 6577 7661 6c75 653b  mno] = newvalue;
-0000f0e0: 0a20 2072 6574 7572 6e28 7374 6174 7573  .  return(status
-0000f0f0: 293b 0a7d 0a53 5441 5449 4320 696e 7420  );.}.STATIC int 
-0000f100: 636f 756e 7473 556e 646f 4c61 6464 6572  countsUndoLadder
-0000f110: 2844 656c 7461 5672 6563 202a 4456 290a  (DeltaVrec *DV).
-0000f120: 7b0a 2020 6966 2844 562d 3e61 6374 6976  {.  if(DV->activ
-0000f130: 656c 6576 656c 203e 2030 290a 2020 2020  elevel > 0).    
-0000f140: 7265 7475 726e 2820 6d61 745f 636f 6c6c  return( mat_coll
-0000f150: 656e 6774 6828 4456 2d3e 7472 6163 6b65  ength(DV->tracke
-0000f160: 722c 2044 562d 3e61 6374 6976 656c 6576  r, DV->activelev
-0000f170: 656c 2920 293b 0a20 2065 6c73 650a 2020  el) );.  else.  
-0000f180: 2020 7265 7475 726e 2820 3020 293b 0a7d    return( 0 );.}
-0000f190: 0a53 5441 5449 4320 696e 7420 7265 7374  .STATIC int rest
-0000f1a0: 6f72 6555 6e64 6f4c 6164 6465 7228 4465  oreUndoLadder(De
-0000f1b0: 6c74 6156 7265 6320 2a44 562c 2052 4541  ltaVrec *DV, REA
-0000f1c0: 4c20 7461 7267 6574 5b5d 290a 7b0a 2020  L target[]).{.  
-0000f1d0: 696e 7420 6944 203d 2030 3b0a 0a20 2069  int iD = 0;..  i
-0000f1e0: 6628 4456 2d3e 6163 7469 7665 6c65 7665  f(DV->activeleve
-0000f1f0: 6c20 3e20 3029 207b 0a20 2020 204d 4154  l > 0) {.    MAT
-0000f200: 7265 6320 2a6d 6174 203d 2044 562d 3e74  rec *mat = DV->t
-0000f210: 7261 636b 6572 3b0a 2020 2020 696e 7420  racker;.    int 
-0000f220: 2020 2069 4220 3d20 6d61 742d 3e63 6f6c     iB = mat->col
-0000f230: 5f65 6e64 5b44 562d 3e61 6374 6976 656c  _end[DV->activel
-0000f240: 6576 656c 2d31 5d2c 0a20 2020 2020 2020  evel-1],.       
-0000f250: 2020 2020 6945 203d 206d 6174 2d3e 636f      iE = mat->co
-0000f260: 6c5f 656e 645b 4456 2d3e 6163 7469 7665  l_end[DV->active
-0000f270: 6c65 7665 6c5d 2c0a 2020 2020 2020 2020  level],.        
-0000f280: 2020 202a 6d61 7452 6f77 6e72 203d 2026     *matRownr = &
-0000f290: 434f 4c5f 4d41 545f 524f 574e 5228 6942  COL_MAT_ROWNR(iB
-0000f2a0: 293b 0a20 2020 2052 4541 4c20 2020 2a6d  );.    REAL   *m
-0000f2b0: 6174 5661 6c75 6520 3d20 2643 4f4c 5f4d  atValue = &COL_M
-0000f2c0: 4154 5f56 414c 5545 2869 4229 2c0a 2020  AT_VALUE(iB),.  
-0000f2d0: 2020 2020 2020 2020 206f 6c64 7661 6c75           oldvalu
-0000f2e0: 653b 0a0a 2020 2020 2f2a 2052 6573 746f  e;..    /* Resto
-0000f2f0: 7265 2074 6865 2076 616c 7565 7320 2a2f  re the values */
-0000f300: 0a20 2020 2069 4420 3d20 6945 2d69 423b  .    iD = iE-iB;
-0000f310: 0a20 2020 2066 6f72 283b 2069 4220 3c20  .    for(; iB < 
-0000f320: 6945 3b20 6942 2b2b 2c20 6d61 7456 616c  iE; iB++, matVal
-0000f330: 7565 202b 3d20 6d61 7456 616c 7565 5374  ue += matValueSt
-0000f340: 6570 2c20 6d61 7452 6f77 6e72 202b 3d20  ep, matRownr += 
-0000f350: 6d61 7452 6f77 436f 6c53 7465 7029 207b  matRowColStep) {
-0000f360: 0a20 2020 2020 206f 6c64 7661 6c75 6520  .      oldvalue 
-0000f370: 3d20 2a6d 6174 5661 6c75 653b 0a23 6966  = *matValue;.#if
-0000f380: 6465 6620 5573 654d 696c 7053 6c61 636b  def UseMilpSlack
-0000f390: 7352 4346 2020 2f2a 2043 6865 636b 2069  sRCF  /* Check i
-0000f3a0: 6620 7765 2073 686f 756c 6420 696e 636c  f we should incl
-0000f3b0: 7564 6520 7261 6e67 6564 2063 6f6e 7374  ude ranged const
-0000f3c0: 7261 696e 7473 202a 2f0a 2020 2020 2020  raints */.      
-0000f3d0: 7461 7267 6574 5b28 2a6d 6174 526f 776e  target[(*matRown
-0000f3e0: 7229 5d20 3d20 6f6c 6476 616c 7565 3b0a  r)] = oldvalue;.
-0000f3f0: 2365 6c73 650a 2020 2020 2020 7461 7267  #else.      targ
-0000f400: 6574 5b44 562d 3e6c 702d 3e72 6f77 732b  et[DV->lp->rows+
-0000f410: 282a 6d61 7452 6f77 6e72 295d 203d 206f  (*matRownr)] = o
-0000f420: 6c64 7661 6c75 653b 0a23 656e 6469 660a  ldvalue;.#endif.
-0000f430: 2020 2020 7d0a 0a20 2020 202f 2a20 4765      }..    /* Ge
-0000f440: 7420 7269 6420 6f66 2074 6865 2063 6861  t rid of the cha
-0000f450: 6e67 6573 202a 2f0a 2020 2020 6d61 745f  nges */.    mat_
-0000f460: 7368 6966 7463 6f6c 7328 4456 2d3e 7472  shiftcols(DV->tr
-0000f470: 6163 6b65 722c 2026 2844 562d 3e61 6374  acker, &(DV->act
-0000f480: 6976 656c 6576 656c 292c 202d 312c 204e  ivelevel), -1, N
-0000f490: 554c 4c29 3b0a 2020 7d0a 0a20 2072 6574  ULL);.  }..  ret
-0000f4a0: 7572 6e28 6944 293b 0a7d 0a53 5441 5449  urn(iD);.}.STATI
-0000f4b0: 4320 696e 7420 6465 6372 656d 656e 7455  C int decrementU
-0000f4c0: 6e64 6f4c 6164 6465 7228 4465 6c74 6156  ndoLadder(DeltaV
-0000f4d0: 7265 6320 2a44 5629 0a7b 0a20 2069 6e74  rec *DV).{.  int
-0000f4e0: 2064 656c 6574 6564 203d 2030 3b0a 0a20   deleted = 0;.. 
-0000f4f0: 2069 6628 4456 2d3e 6163 7469 7665 6c65   if(DV->activele
-0000f500: 7665 6c20 3e20 3029 207b 0a20 2020 2064  vel > 0) {.    d
-0000f510: 656c 6574 6564 203d 206d 6174 5f73 6869  eleted = mat_shi
-0000f520: 6674 636f 6c73 2844 562d 3e74 7261 636b  ftcols(DV->track
-0000f530: 6572 2c20 2628 4456 2d3e 6163 7469 7665  er, &(DV->active
-0000f540: 6c65 7665 6c29 2c20 2d31 2c20 4e55 4c4c  level), -1, NULL
-0000f550: 293b 0a20 2020 2044 562d 3e61 6374 6976  );.    DV->activ
-0000f560: 656c 6576 656c 2d2d 3b0a 2020 2020 4456  elevel--;.    DV
-0000f570: 2d3e 7472 6163 6b65 722d 3e63 6f6c 756d  ->tracker->colum
-0000f580: 6e73 2d2d 3b0a 2020 7d0a 2020 7265 7475  ns--;.  }.  retu
-0000f590: 726e 2864 656c 6574 6564 293b 0a7d 0a53  rn(deleted);.}.S
-0000f5a0: 5441 5449 4320 4d59 424f 4f4c 2066 7265  TATIC MYBOOL fre
-0000f5b0: 6555 6e64 6f4c 6164 6465 7228 4465 6c74  eUndoLadder(Delt
-0000f5c0: 6156 7265 6320 2a2a 4456 290a 7b0a 2020  aVrec **DV).{.  
-0000f5d0: 6966 2828 4456 203d 3d20 4e55 4c4c 2920  if((DV == NULL) 
-0000f5e0: 7c7c 2028 2a44 5620 3d3d 204e 554c 4c29  || (*DV == NULL)
-0000f5f0: 290a 2020 2020 7265 7475 726e 2846 414c  ).    return(FAL
-0000f600: 5345 293b 0a0a 2020 6d61 745f 6672 6565  SE);..  mat_free
-0000f610: 2826 2828 2a44 5629 2d3e 7472 6163 6b65  (&((*DV)->tracke
-0000f620: 7229 293b 0a20 2046 5245 4528 2a44 5629  r));.  FREE(*DV)
-0000f630: 3b0a 2020 7265 7475 726e 2854 5255 4529  ;.  return(TRUE)
-0000f640: 3b0a 7d0a 0a53 5441 5449 4320 4d59 424f  ;.}..STATIC MYBO
-0000f650: 4f4c 2061 7070 656e 6455 6e64 6f50 7265  OL appendUndoPre
-0000f660: 736f 6c76 6528 6c70 7265 6320 2a6c 702c  solve(lprec *lp,
-0000f670: 204d 5942 4f4f 4c20 6973 7072 696d 616c   MYBOOL isprimal
-0000f680: 2c20 5245 414c 2062 6574 612c 2069 6e74  , REAL beta, int
-0000f690: 2063 6f6c 6e72 4465 7029 0a7b 0a20 204d   colnrDep).{.  M
-0000f6a0: 4154 7265 6320 2a6d 6174 3b0a 0a20 202f  ATrec *mat;..  /
-0000f6b0: 2a20 506f 696e 7420 746f 2063 6f72 7265  * Point to corre
-0000f6c0: 6374 2075 6e64 6f20 7374 7275 6374 7572  ct undo structur
-0000f6d0: 6520 2a2f 0a20 2069 6628 6973 7072 696d  e */.  if(isprim
-0000f6e0: 616c 290a 2020 2020 6d61 7420 3d20 6c70  al).    mat = lp
-0000f6f0: 2d3e 7072 6573 6f6c 7665 5f75 6e64 6f2d  ->presolve_undo-
-0000f700: 3e70 7269 6d61 6c75 6e64 6f2d 3e74 7261  >primalundo->tra
-0000f710: 636b 6572 3b0a 2020 656c 7365 0a20 2020  cker;.  else.   
-0000f720: 206d 6174 203d 206c 702d 3e70 7265 736f   mat = lp->preso
-0000f730: 6c76 655f 756e 646f 2d3e 6475 616c 756e  lve_undo->dualun
-0000f740: 646f 2d3e 7472 6163 6b65 723b 0a0a 2020  do->tracker;..  
-0000f750: 2f2a 2041 7070 656e 6420 7468 6520 6461  /* Append the da
-0000f760: 7461 202a 2f0a 2020 6966 2828 636f 6c6e  ta */.  if((coln
-0000f770: 7244 6570 203e 2030 2920 2626 2028 6265  rDep > 0) && (be
-0000f780: 7461 2021 3d20 3029 2026 260a 2020 2020  ta != 0) &&.    
-0000f790: 2028 6d61 7420 213d 204e 554c 4c29 2026   (mat != NULL) &
-0000f7a0: 2620 286d 6174 2d3e 636f 6c5f 7461 675b  & (mat->col_tag[
-0000f7b0: 305d 203e 2030 2929 207b 0a20 2020 2069  0] > 0)) {.    i
-0000f7c0: 6e74 2069 7820 3d20 6d61 742d 3e63 6f6c  nt ix = mat->col
-0000f7d0: 5f74 6167 5b30 5d3b 0a23 6966 2030 0a20  _tag[0];.#if 0. 
-0000f7e0: 2020 2072 6570 6f72 7428 6c70 2c20 4e4f     report(lp, NO
-0000f7f0: 524d 414c 2c20 2261 7070 656e 6455 6e64  RMAL, "appendUnd
-0000f800: 6f50 7265 736f 6c76 653a 2025 7320 2567  oPresolve: %s %g
-0000f810: 202a 2078 2564 5c6e 222c 0a20 2020 2020   * x%d\n",.     
-0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f830: 2020 2820 6265 7461 203c 2030 203f 2022    ( beta < 0 ? "
-0000f840: 2d22 203a 2022 2b22 292c 2066 6162 7328  -" : "+"), fabs(
-0000f850: 6265 7461 292c 2063 6f6c 6e72 4465 7029  beta), colnrDep)
-0000f860: 3b0a 2365 6e64 6966 0a0a 2020 2020 2f2a  ;.#endif..    /*
-0000f870: 2044 6f20 6e6f 726d 616c 2075 7365 7220   Do normal user 
-0000f880: 7661 7269 6162 6c65 2063 6173 6520 2a2f  variable case */
-0000f890: 0a20 2020 2069 6628 636f 6c6e 7244 6570  .    if(colnrDep
-0000f8a0: 203c 3d20 6c70 2d3e 636f 6c75 6d6e 7329   <= lp->columns)
-0000f8b0: 0a20 2020 2020 206d 6174 5f73 6574 7661  .      mat_setva
-0000f8c0: 6c75 6528 6d61 742c 2063 6f6c 6e72 4465  lue(mat, colnrDe
-0000f8d0: 702c 2069 782c 2062 6574 612c 2046 414c  p, ix, beta, FAL
-0000f8e0: 5345 293b 0a0a 2020 2020 2f2a 2048 616e  SE);..    /* Han
-0000f8f0: 646c 6520 6361 7365 2077 6865 7265 2061  dle case where a
-0000f900: 2073 6c61 636b 2076 6172 6961 626c 6520   slack variable 
-0000f910: 6973 2072 6566 6572 656e 6365 6420 2a2f  is referenced */
-0000f920: 0a20 2020 2065 6c73 6520 7b0a 2020 2020  .    else {.    
-0000f930: 2020 696e 7420 6970 6f73 2c20 6a78 203d    int ipos, jx =
-0000f940: 206d 6174 2d3e 636f 6c5f 7461 675b 6978   mat->col_tag[ix
-0000f950: 5d3b 0a20 2020 2020 206d 6174 5f73 6574  ];.      mat_set
-0000f960: 7661 6c75 6528 6d61 742c 206a 782c 2069  value(mat, jx, i
-0000f970: 782c 2062 6574 612c 2046 414c 5345 293b  x, beta, FALSE);
-0000f980: 0a20 2020 2020 206a 7820 3d20 6d61 745f  .      jx = mat_
-0000f990: 6669 6e64 696e 7328 6d61 742c 206a 782c  findins(mat, jx,
-0000f9a0: 2069 782c 2026 6970 6f73 2c20 4641 4c53   ix, &ipos, FALS
-0000f9b0: 4529 3b0a 2020 2020 2020 434f 4c5f 4d41  E);.      COL_MA
-0000f9c0: 545f 524f 574e 5228 6970 6f73 2920 3d20  T_ROWNR(ipos) = 
-0000f9d0: 636f 6c6e 7244 6570 3b0a 2020 2020 7d0a  colnrDep;.    }.
-0000f9e0: 2020 2020 7265 7475 726e 2820 5452 5545      return( TRUE
-0000f9f0: 2029 3b0a 2020 7d0a 2020 656c 7365 0a20   );.  }.  else. 
-0000fa00: 2020 2072 6574 7572 6e28 2046 414c 5345     return( FALSE
-0000fa10: 2029 3b0a 7d0a 5354 4154 4943 204d 5942   );.}.STATIC MYB
-0000fa20: 4f4f 4c20 6164 6455 6e64 6f50 7265 736f  OOL addUndoPreso
-0000fa30: 6c76 6528 6c70 7265 6320 2a6c 702c 204d  lve(lprec *lp, M
-0000fa40: 5942 4f4f 4c20 6973 7072 696d 616c 2c20  YBOOL isprimal, 
-0000fa50: 696e 7420 636f 6c6e 7245 6c69 6d2c 2052  int colnrElim, R
-0000fa60: 4541 4c20 616c 7068 612c 2052 4541 4c20  EAL alpha, REAL 
-0000fa70: 6265 7461 2c20 696e 7420 636f 6c6e 7244  beta, int colnrD
-0000fa80: 6570 290a 7b0a 2020 696e 7420 2020 2020  ep).{.  int     
-0000fa90: 2020 6978 3b0a 2020 4465 6c74 6156 7265    ix;.  DeltaVre
-0000faa0: 6320 2a2a 4456 3b0a 2020 4d41 5472 6563  c **DV;.  MATrec
-0000fab0: 2020 2020 2a6d 6174 3b0a 2020 7072 6573      *mat;.  pres
-0000fac0: 6f6c 7665 756e 646f 7265 6320 2a70 7364  olveundorec *psd
-0000fad0: 6174 6120 3d20 6c70 2d3e 7072 6573 6f6c  ata = lp->presol
-0000fae0: 7665 5f75 6e64 6f3b 0a0a 2020 2f2a 2050  ve_undo;..  /* P
-0000faf0: 6f69 6e74 2074 6f20 616e 6420 696e 6974  oint to and init
-0000fb00: 6961 6c69 7a65 2075 6e64 6f20 7374 7275  ialize undo stru
-0000fb10: 6374 7572 6520 6174 2066 6972 7374 2063  cture at first c
-0000fb20: 616c 6c20 2a2f 0a20 2069 6628 6973 7072  all */.  if(ispr
-0000fb30: 696d 616c 2920 7b0a 2020 2020 4456 203d  imal) {.    DV =
-0000fb40: 2026 2870 7364 6174 612d 3e70 7269 6d61   &(psdata->prima
-0000fb50: 6c75 6e64 6f29 3b0a 2020 2020 6966 282a  lundo);.    if(*
-0000fb60: 4456 203d 3d20 4e55 4c4c 2920 7b0a 2020  DV == NULL) {.  
-0000fb70: 2020 2020 2a44 5620 3d20 6372 6561 7465      *DV = create
-0000fb80: 556e 646f 4c61 6464 6572 286c 702c 206c  UndoLadder(lp, l
-0000fb90: 702d 3e63 6f6c 756d 6e73 2b31 2c20 6c70  p->columns+1, lp
-0000fba0: 2d3e 636f 6c75 6d6e 7329 3b0a 2020 2020  ->columns);.    
-0000fbb0: 2020 6d61 7420 3d20 282a 4456 292d 3e74    mat = (*DV)->t
-0000fbc0: 7261 636b 6572 3b0a 2020 2020 2020 6d61  racker;.      ma
-0000fbd0: 742d 3e65 7073 7661 6c75 6520 3d20 6c70  t->epsvalue = lp
-0000fbe0: 2d3e 6d61 7441 2d3e 6570 7376 616c 7565  ->matA->epsvalue
-0000fbf0: 3b0a 2020 2020 2020 616c 6c6f 6349 4e54  ;.      allocINT
-0000fc00: 286c 702c 2026 286d 6174 2d3e 636f 6c5f  (lp, &(mat->col_
-0000fc10: 7461 6729 2c20 6c70 2d3e 636f 6c75 6d6e  tag), lp->column
-0000fc20: 732b 312c 2046 414c 5345 293b 0a20 2020  s+1, FALSE);.   
-0000fc30: 2020 206d 6174 2d3e 636f 6c5f 7461 675b     mat->col_tag[
-0000fc40: 305d 203d 2030 3b0a 2020 2020 7d0a 2020  0] = 0;.    }.  
-0000fc50: 7d0a 2020 656c 7365 207b 0a20 2020 2044  }.  else {.    D
-0000fc60: 5620 3d20 2628 7073 6461 7461 2d3e 6475  V = &(psdata->du
-0000fc70: 616c 756e 646f 293b 0a20 2020 2069 6628  alundo);.    if(
-0000fc80: 2a44 5620 3d3d 204e 554c 4c29 207b 0a20  *DV == NULL) {. 
-0000fc90: 2020 2020 202a 4456 203d 2063 7265 6174       *DV = creat
-0000fca0: 6555 6e64 6f4c 6164 6465 7228 6c70 2c20  eUndoLadder(lp, 
-0000fcb0: 6c70 2d3e 726f 7773 2b31 2c20 6c70 2d3e  lp->rows+1, lp->
-0000fcc0: 726f 7773 293b 0a20 2020 2020 206d 6174  rows);.      mat
-0000fcd0: 203d 2028 2a44 5629 2d3e 7472 6163 6b65   = (*DV)->tracke
-0000fce0: 723b 0a20 2020 2020 206d 6174 2d3e 6570  r;.      mat->ep
-0000fcf0: 7376 616c 7565 203d 206c 702d 3e6d 6174  svalue = lp->mat
-0000fd00: 412d 3e65 7073 7661 6c75 653b 0a20 2020  A->epsvalue;.   
-0000fd10: 2020 2061 6c6c 6f63 494e 5428 6c70 2c20     allocINT(lp, 
-0000fd20: 2628 6d61 742d 3e63 6f6c 5f74 6167 292c  &(mat->col_tag),
-0000fd30: 206c 702d 3e72 6f77 732b 312c 2046 414c   lp->rows+1, FAL
-0000fd40: 5345 293b 0a20 2020 2020 206d 6174 2d3e  SE);.      mat->
-0000fd50: 636f 6c5f 7461 675b 305d 203d 2030 3b0a  col_tag[0] = 0;.
-0000fd60: 2020 2020 7d0a 2020 7d0a 2020 6d61 7420      }.  }.  mat 
-0000fd70: 3d20 282a 4456 292d 3e74 7261 636b 6572  = (*DV)->tracker
-0000fd80: 3b0a 2369 6620 300a 2020 7265 706f 7274  ;.#if 0.  report
-0000fd90: 286c 702c 204e 4f52 4d41 4c2c 2022 6164  (lp, NORMAL, "ad
-0000fda0: 6455 6e64 6f50 7265 736f 6c76 653a 2078  dUndoPresolve: x
-0000fdb0: 2564 203d 2025 6720 2573 2025 6720 2a20  %d = %g %s %g * 
-0000fdc0: 7825 645c 6e22 2c0a 2020 2020 2020 2020  x%d\n",.        
-0000fdd0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0000fde0: 6e72 456c 696d 2c20 616c 7068 612c 2028  nrElim, alpha, (
-0000fdf0: 2062 6574 6120 3c20 3020 3f20 222d 2220   beta < 0 ? "-" 
-0000fe00: 3a20 222b 2229 2c20 6661 6273 2862 6574  : "+"), fabs(bet
-0000fe10: 6129 2c20 636f 6c6e 7244 6570 293b 0a23  a), colnrDep);.#
-0000fe20: 656e 6469 660a 2020 2f2a 2041 6464 2074  endif.  /* Add t
-0000fe30: 6865 2064 6174 6120 2a2f 0a20 2069 7820  he data */.  ix 
-0000fe40: 3d20 6d61 742d 3e63 6f6c 5f74 6167 5b30  = mat->col_tag[0
-0000fe50: 5d20 3d20 696e 6372 656d 656e 7455 6e64  ] = incrementUnd
-0000fe60: 6f4c 6164 6465 7228 2a44 5629 3b0a 2020  oLadder(*DV);.  
-0000fe70: 6d61 742d 3e63 6f6c 5f74 6167 5b69 785d  mat->col_tag[ix]
-0000fe80: 203d 2063 6f6c 6e72 456c 696d 3b0a 2020   = colnrElim;.  
-0000fe90: 6966 2861 6c70 6861 2021 3d20 3029 0a20  if(alpha != 0). 
-0000fea0: 2020 206d 6174 5f73 6574 7661 6c75 6528     mat_setvalue(
-0000feb0: 6d61 742c 2030 2c20 6978 2c20 616c 7068  mat, 0, ix, alph
-0000fec0: 612c 2046 414c 5345 293b 0a2f 2a20 2020  a, FALSE);./*   
-0000fed0: 206d 6174 5f61 7070 656e 6476 616c 7565   mat_appendvalue
-0000fee0: 282a 6d61 742c 2030 2c20 616c 7068 6129  (*mat, 0, alpha)
-0000fef0: 3b2a 2f0a 2020 6966 2828 636f 6c6e 7244  ;*/.  if((colnrD
-0000ff00: 6570 203e 2030 2920 2626 2028 6265 7461  ep > 0) && (beta
-0000ff10: 2021 3d20 3029 2920 7b0a 2020 2020 6966   != 0)) {.    if
-0000ff20: 2863 6f6c 6e72 4465 7020 3e20 6c70 2d3e  (colnrDep > lp->
-0000ff30: 636f 6c75 6d6e 7329 0a20 2020 2020 2072  columns).      r
-0000ff40: 6574 7572 6e28 2061 7070 656e 6455 6e64  eturn( appendUnd
-0000ff50: 6f50 7265 736f 6c76 6528 6c70 2c20 6973  oPresolve(lp, is
-0000ff60: 7072 696d 616c 2c20 6265 7461 2c20 636f  primal, beta, co
-0000ff70: 6c6e 7244 6570 2920 293b 0a20 2020 2065  lnrDep) );.    e
-0000ff80: 6c73 650a 2020 2020 2020 6d61 745f 7365  lse.      mat_se
-0000ff90: 7476 616c 7565 286d 6174 2c20 636f 6c6e  tvalue(mat, coln
-0000ffa0: 7244 6570 2c20 6978 2c20 6265 7461 2c20  rDep, ix, beta, 
-0000ffb0: 4641 4c53 4529 3b0a 2020 7d0a 0a20 2072  FALSE);.  }..  r
-0000ffc0: 6574 7572 6e28 2054 5255 4520 293b 0a7d  eturn( TRUE );.}
-0000ffd0: 0a0a 0a0a 2f2a 202d 2d2d 2d2d 2d2d 2d2d  ..../* ---------
+0000ed40: 2d2d 2d2d 2d2d 2d2d 202a 2f0a 5354 4154  -------- */.STAT
+0000ed50: 4943 2044 656c 7461 5672 6563 202a 6372  IC DeltaVrec *cr
+0000ed60: 6561 7465 556e 646f 4c61 6464 6572 286c  eateUndoLadder(l
+0000ed70: 7072 6563 202a 6c70 2c20 696e 7420 6c65  prec *lp, int le
+0000ed80: 7665 6c69 7465 6d73 2c20 696e 7420 6d61  velitems, int ma
+0000ed90: 786c 6576 656c 7329 0a7b 0a20 2044 656c  xlevels).{.  Del
+0000eda0: 7461 5672 6563 202a 686f 6c64 3b0a 0a20  taVrec *hold;.. 
+0000edb0: 2068 6f6c 6420 3d20 2844 656c 7461 5672   hold = (DeltaVr
+0000edc0: 6563 202a 2920 6d61 6c6c 6f63 2873 697a  ec *) malloc(siz
+0000edd0: 656f 6628 2a68 6f6c 6429 293b 0a20 2068  eof(*hold));.  h
+0000ede0: 6f6c 642d 3e6c 7020 3d20 6c70 3b0a 2020  old->lp = lp;.  
+0000edf0: 686f 6c64 2d3e 6163 7469 7665 6c65 7665  hold->activeleve
+0000ee00: 6c20 3d20 303b 0a20 2068 6f6c 642d 3e74  l = 0;.  hold->t
+0000ee10: 7261 636b 6572 203d 206d 6174 5f63 7265  racker = mat_cre
+0000ee20: 6174 6528 6c70 2c20 6c65 7665 6c69 7465  ate(lp, levelite
+0000ee30: 6d73 2c20 302c 2030 2e30 293b 0a20 2069  ms, 0, 0.0);.  i
+0000ee40: 6e63 5f6d 6174 636f 6c5f 7370 6163 6528  nc_matcol_space(
+0000ee50: 686f 6c64 2d3e 7472 6163 6b65 722c 206d  hold->tracker, m
+0000ee60: 6178 6c65 7665 6c73 293b 0a20 2072 6574  axlevels);.  ret
+0000ee70: 7572 6e28 2068 6f6c 6420 293b 0a7d 0a53  urn( hold );.}.S
+0000ee80: 5441 5449 4320 696e 7420 696e 6372 656d  TATIC int increm
+0000ee90: 656e 7455 6e64 6f4c 6164 6465 7228 4465  entUndoLadder(De
+0000eea0: 6c74 6156 7265 6320 2a44 5629 0a7b 0a20  ltaVrec *DV).{. 
+0000eeb0: 2044 562d 3e61 6374 6976 656c 6576 656c   DV->activelevel
+0000eec0: 2b2b 3b0a 2020 696e 635f 6d61 7463 6f6c  ++;.  inc_matcol
+0000eed0: 5f73 7061 6365 2844 562d 3e74 7261 636b  _space(DV->track
+0000eee0: 6572 2c20 3129 3b0a 2020 6d61 745f 7368  er, 1);.  mat_sh
+0000eef0: 6966 7463 6f6c 7328 4456 2d3e 7472 6163  iftcols(DV->trac
+0000ef00: 6b65 722c 2026 2844 562d 3e61 6374 6976  ker, &(DV->activ
+0000ef10: 656c 6576 656c 292c 2031 2c20 4e55 4c4c  elevel), 1, NULL
+0000ef20: 293b 0a20 2044 562d 3e74 7261 636b 6572  );.  DV->tracker
+0000ef30: 2d3e 636f 6c75 6d6e 732b 2b3b 0a20 2072  ->columns++;.  r
+0000ef40: 6574 7572 6e28 4456 2d3e 6163 7469 7665  eturn(DV->active
+0000ef50: 6c65 7665 6c29 3b0a 7d0a 5354 4154 4943  level);.}.STATIC
+0000ef60: 204d 5942 4f4f 4c20 6d6f 6469 6679 556e   MYBOOL modifyUn
+0000ef70: 646f 4c61 6464 6572 2844 656c 7461 5672  doLadder(DeltaVr
+0000ef80: 6563 202a 4456 2c20 696e 7420 6974 656d  ec *DV, int item
+0000ef90: 6e6f 2c20 5245 414c 2074 6172 6765 745b  no, REAL target[
+0000efa0: 5d2c 2052 4541 4c20 6e65 7776 616c 7565  ], REAL newvalue
+0000efb0: 290a 7b0a 2020 4d59 424f 4f4c 2073 7461  ).{.  MYBOOL sta
+0000efc0: 7475 733b 0a20 2069 6e74 2020 2020 7661  tus;.  int    va
+0000efd0: 7269 6e64 6578 203d 2069 7465 6d6e 6f3b  rindex = itemno;
+0000efe0: 0a20 2052 4541 4c20 2020 6f6c 6476 616c  .  REAL   oldval
+0000eff0: 7565 203d 2074 6172 6765 745b 6974 656d  ue = target[item
+0000f000: 6e6f 5d3b 0a0a 2369 666e 6465 6620 5573  no];..#ifndef Us
+0000f010: 654d 696c 7053 6c61 636b 7352 4346 2020  eMilpSlacksRCF  
+0000f020: 2f2a 2043 6865 636b 2069 6620 7765 2073  /* Check if we s
+0000f030: 686f 756c 6420 696e 636c 7564 6520 7261  hould include ra
+0000f040: 6e67 6564 2063 6f6e 7374 7261 696e 7473  nged constraints
+0000f050: 202a 2f0a 2020 7661 7269 6e64 6578 202d   */.  varindex -
+0000f060: 3d20 4456 2d3e 6c70 2d3e 726f 7773 3b0a  = DV->lp->rows;.
+0000f070: 2365 6e64 6966 0a20 2073 7461 7475 7320  #endif.  status 
+0000f080: 3d20 6d61 745f 6170 7065 6e64 7661 6c75  = mat_appendvalu
+0000f090: 6528 4456 2d3e 7472 6163 6b65 722c 2076  e(DV->tracker, v
+0000f0a0: 6172 696e 6465 782c 206f 6c64 7661 6c75  arindex, oldvalu
+0000f0b0: 6529 3b0a 2020 7461 7267 6574 5b69 7465  e);.  target[ite
+0000f0c0: 6d6e 6f5d 203d 206e 6577 7661 6c75 653b  mno] = newvalue;
+0000f0d0: 0a20 2072 6574 7572 6e28 7374 6174 7573  .  return(status
+0000f0e0: 293b 0a7d 0a53 5441 5449 4320 696e 7420  );.}.STATIC int 
+0000f0f0: 636f 756e 7473 556e 646f 4c61 6464 6572  countsUndoLadder
+0000f100: 2844 656c 7461 5672 6563 202a 4456 290a  (DeltaVrec *DV).
+0000f110: 7b0a 2020 6966 2844 562d 3e61 6374 6976  {.  if(DV->activ
+0000f120: 656c 6576 656c 203e 2030 290a 2020 2020  elevel > 0).    
+0000f130: 7265 7475 726e 2820 6d61 745f 636f 6c6c  return( mat_coll
+0000f140: 656e 6774 6828 4456 2d3e 7472 6163 6b65  ength(DV->tracke
+0000f150: 722c 2044 562d 3e61 6374 6976 656c 6576  r, DV->activelev
+0000f160: 656c 2920 293b 0a20 2065 6c73 650a 2020  el) );.  else.  
+0000f170: 2020 7265 7475 726e 2820 3020 293b 0a7d    return( 0 );.}
+0000f180: 0a53 5441 5449 4320 696e 7420 7265 7374  .STATIC int rest
+0000f190: 6f72 6555 6e64 6f4c 6164 6465 7228 4465  oreUndoLadder(De
+0000f1a0: 6c74 6156 7265 6320 2a44 562c 2052 4541  ltaVrec *DV, REA
+0000f1b0: 4c20 7461 7267 6574 5b5d 290a 7b0a 2020  L target[]).{.  
+0000f1c0: 696e 7420 6944 203d 2030 3b0a 0a20 2069  int iD = 0;..  i
+0000f1d0: 6628 4456 2d3e 6163 7469 7665 6c65 7665  f(DV->activeleve
+0000f1e0: 6c20 3e20 3029 207b 0a20 2020 204d 4154  l > 0) {.    MAT
+0000f1f0: 7265 6320 2a6d 6174 203d 2044 562d 3e74  rec *mat = DV->t
+0000f200: 7261 636b 6572 3b0a 2020 2020 696e 7420  racker;.    int 
+0000f210: 2020 2069 4220 3d20 6d61 742d 3e63 6f6c     iB = mat->col
+0000f220: 5f65 6e64 5b44 562d 3e61 6374 6976 656c  _end[DV->activel
+0000f230: 6576 656c 2d31 5d2c 0a20 2020 2020 2020  evel-1],.       
+0000f240: 2020 2020 6945 203d 206d 6174 2d3e 636f      iE = mat->co
+0000f250: 6c5f 656e 645b 4456 2d3e 6163 7469 7665  l_end[DV->active
+0000f260: 6c65 7665 6c5d 2c0a 2020 2020 2020 2020  level],.        
+0000f270: 2020 202a 6d61 7452 6f77 6e72 203d 2026     *matRownr = &
+0000f280: 434f 4c5f 4d41 545f 524f 574e 5228 6942  COL_MAT_ROWNR(iB
+0000f290: 293b 0a20 2020 2052 4541 4c20 2020 2a6d  );.    REAL   *m
+0000f2a0: 6174 5661 6c75 6520 3d20 2643 4f4c 5f4d  atValue = &COL_M
+0000f2b0: 4154 5f56 414c 5545 2869 4229 2c0a 2020  AT_VALUE(iB),.  
+0000f2c0: 2020 2020 2020 2020 206f 6c64 7661 6c75           oldvalu
+0000f2d0: 653b 0a0a 2020 2020 2f2a 2052 6573 746f  e;..    /* Resto
+0000f2e0: 7265 2074 6865 2076 616c 7565 7320 2a2f  re the values */
+0000f2f0: 0a20 2020 2069 4420 3d20 6945 2d69 423b  .    iD = iE-iB;
+0000f300: 0a20 2020 2066 6f72 283b 2069 4220 3c20  .    for(; iB < 
+0000f310: 6945 3b20 6942 2b2b 2c20 6d61 7456 616c  iE; iB++, matVal
+0000f320: 7565 202b 3d20 6d61 7456 616c 7565 5374  ue += matValueSt
+0000f330: 6570 2c20 6d61 7452 6f77 6e72 202b 3d20  ep, matRownr += 
+0000f340: 6d61 7452 6f77 436f 6c53 7465 7029 207b  matRowColStep) {
+0000f350: 0a20 2020 2020 206f 6c64 7661 6c75 6520  .      oldvalue 
+0000f360: 3d20 2a6d 6174 5661 6c75 653b 0a23 6966  = *matValue;.#if
+0000f370: 6465 6620 5573 654d 696c 7053 6c61 636b  def UseMilpSlack
+0000f380: 7352 4346 2020 2f2a 2043 6865 636b 2069  sRCF  /* Check i
+0000f390: 6620 7765 2073 686f 756c 6420 696e 636c  f we should incl
+0000f3a0: 7564 6520 7261 6e67 6564 2063 6f6e 7374  ude ranged const
+0000f3b0: 7261 696e 7473 202a 2f0a 2020 2020 2020  raints */.      
+0000f3c0: 7461 7267 6574 5b28 2a6d 6174 526f 776e  target[(*matRown
+0000f3d0: 7229 5d20 3d20 6f6c 6476 616c 7565 3b0a  r)] = oldvalue;.
+0000f3e0: 2365 6c73 650a 2020 2020 2020 7461 7267  #else.      targ
+0000f3f0: 6574 5b44 562d 3e6c 702d 3e72 6f77 732b  et[DV->lp->rows+
+0000f400: 282a 6d61 7452 6f77 6e72 295d 203d 206f  (*matRownr)] = o
+0000f410: 6c64 7661 6c75 653b 0a23 656e 6469 660a  ldvalue;.#endif.
+0000f420: 2020 2020 7d0a 0a20 2020 202f 2a20 4765      }..    /* Ge
+0000f430: 7420 7269 6420 6f66 2074 6865 2063 6861  t rid of the cha
+0000f440: 6e67 6573 202a 2f0a 2020 2020 6d61 745f  nges */.    mat_
+0000f450: 7368 6966 7463 6f6c 7328 4456 2d3e 7472  shiftcols(DV->tr
+0000f460: 6163 6b65 722c 2026 2844 562d 3e61 6374  acker, &(DV->act
+0000f470: 6976 656c 6576 656c 292c 202d 312c 204e  ivelevel), -1, N
+0000f480: 554c 4c29 3b0a 2020 7d0a 0a20 2072 6574  ULL);.  }..  ret
+0000f490: 7572 6e28 6944 293b 0a7d 0a53 5441 5449  urn(iD);.}.STATI
+0000f4a0: 4320 696e 7420 6465 6372 656d 656e 7455  C int decrementU
+0000f4b0: 6e64 6f4c 6164 6465 7228 4465 6c74 6156  ndoLadder(DeltaV
+0000f4c0: 7265 6320 2a44 5629 0a7b 0a20 2069 6e74  rec *DV).{.  int
+0000f4d0: 2064 656c 6574 6564 203d 2030 3b0a 0a20   deleted = 0;.. 
+0000f4e0: 2069 6628 4456 2d3e 6163 7469 7665 6c65   if(DV->activele
+0000f4f0: 7665 6c20 3e20 3029 207b 0a20 2020 2064  vel > 0) {.    d
+0000f500: 656c 6574 6564 203d 206d 6174 5f73 6869  eleted = mat_shi
+0000f510: 6674 636f 6c73 2844 562d 3e74 7261 636b  ftcols(DV->track
+0000f520: 6572 2c20 2628 4456 2d3e 6163 7469 7665  er, &(DV->active
+0000f530: 6c65 7665 6c29 2c20 2d31 2c20 4e55 4c4c  level), -1, NULL
+0000f540: 293b 0a20 2020 2044 562d 3e61 6374 6976  );.    DV->activ
+0000f550: 656c 6576 656c 2d2d 3b0a 2020 2020 4456  elevel--;.    DV
+0000f560: 2d3e 7472 6163 6b65 722d 3e63 6f6c 756d  ->tracker->colum
+0000f570: 6e73 2d2d 3b0a 2020 7d0a 2020 7265 7475  ns--;.  }.  retu
+0000f580: 726e 2864 656c 6574 6564 293b 0a7d 0a53  rn(deleted);.}.S
+0000f590: 5441 5449 4320 4d59 424f 4f4c 2066 7265  TATIC MYBOOL fre
+0000f5a0: 6555 6e64 6f4c 6164 6465 7228 4465 6c74  eUndoLadder(Delt
+0000f5b0: 6156 7265 6320 2a2a 4456 290a 7b0a 2020  aVrec **DV).{.  
+0000f5c0: 6966 2828 4456 203d 3d20 4e55 4c4c 2920  if((DV == NULL) 
+0000f5d0: 7c7c 2028 2a44 5620 3d3d 204e 554c 4c29  || (*DV == NULL)
+0000f5e0: 290a 2020 2020 7265 7475 726e 2846 414c  ).    return(FAL
+0000f5f0: 5345 293b 0a0a 2020 6d61 745f 6672 6565  SE);..  mat_free
+0000f600: 2826 2828 2a44 5629 2d3e 7472 6163 6b65  (&((*DV)->tracke
+0000f610: 7229 293b 0a20 2046 5245 4528 2a44 5629  r));.  FREE(*DV)
+0000f620: 3b0a 2020 7265 7475 726e 2854 5255 4529  ;.  return(TRUE)
+0000f630: 3b0a 7d0a 0a53 5441 5449 4320 4d59 424f  ;.}..STATIC MYBO
+0000f640: 4f4c 2061 7070 656e 6455 6e64 6f50 7265  OL appendUndoPre
+0000f650: 736f 6c76 6528 6c70 7265 6320 2a6c 702c  solve(lprec *lp,
+0000f660: 204d 5942 4f4f 4c20 6973 7072 696d 616c   MYBOOL isprimal
+0000f670: 2c20 5245 414c 2062 6574 612c 2069 6e74  , REAL beta, int
+0000f680: 2063 6f6c 6e72 4465 7029 0a7b 0a20 204d   colnrDep).{.  M
+0000f690: 4154 7265 6320 2a6d 6174 3b0a 0a20 202f  ATrec *mat;..  /
+0000f6a0: 2a20 506f 696e 7420 746f 2063 6f72 7265  * Point to corre
+0000f6b0: 6374 2075 6e64 6f20 7374 7275 6374 7572  ct undo structur
+0000f6c0: 6520 2a2f 0a20 2069 6628 6973 7072 696d  e */.  if(isprim
+0000f6d0: 616c 290a 2020 2020 6d61 7420 3d20 6c70  al).    mat = lp
+0000f6e0: 2d3e 7072 6573 6f6c 7665 5f75 6e64 6f2d  ->presolve_undo-
+0000f6f0: 3e70 7269 6d61 6c75 6e64 6f2d 3e74 7261  >primalundo->tra
+0000f700: 636b 6572 3b0a 2020 656c 7365 0a20 2020  cker;.  else.   
+0000f710: 206d 6174 203d 206c 702d 3e70 7265 736f   mat = lp->preso
+0000f720: 6c76 655f 756e 646f 2d3e 6475 616c 756e  lve_undo->dualun
+0000f730: 646f 2d3e 7472 6163 6b65 723b 0a0a 2020  do->tracker;..  
+0000f740: 2f2a 2041 7070 656e 6420 7468 6520 6461  /* Append the da
+0000f750: 7461 202a 2f0a 2020 6966 2828 636f 6c6e  ta */.  if((coln
+0000f760: 7244 6570 203e 2030 2920 2626 2028 6265  rDep > 0) && (be
+0000f770: 7461 2021 3d20 3029 2026 260a 2020 2020  ta != 0) &&.    
+0000f780: 2028 6d61 7420 213d 204e 554c 4c29 2026   (mat != NULL) &
+0000f790: 2620 286d 6174 2d3e 636f 6c5f 7461 675b  & (mat->col_tag[
+0000f7a0: 305d 203e 2030 2929 207b 0a20 2020 2069  0] > 0)) {.    i
+0000f7b0: 6e74 2069 7820 3d20 6d61 742d 3e63 6f6c  nt ix = mat->col
+0000f7c0: 5f74 6167 5b30 5d3b 0a23 6966 2030 0a20  _tag[0];.#if 0. 
+0000f7d0: 2020 2072 6570 6f72 7428 6c70 2c20 4e4f     report(lp, NO
+0000f7e0: 524d 414c 2c20 2261 7070 656e 6455 6e64  RMAL, "appendUnd
+0000f7f0: 6f50 7265 736f 6c76 653a 2025 7320 2567  oPresolve: %s %g
+0000f800: 202a 2078 2564 5c6e 222c 0a20 2020 2020   * x%d\n",.     
+0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f820: 2020 2820 6265 7461 203c 2030 203f 2022    ( beta < 0 ? "
+0000f830: 2d22 203a 2022 2b22 292c 2066 6162 7328  -" : "+"), fabs(
+0000f840: 6265 7461 292c 2063 6f6c 6e72 4465 7029  beta), colnrDep)
+0000f850: 3b0a 2365 6e64 6966 0a0a 2020 2020 2f2a  ;.#endif..    /*
+0000f860: 2044 6f20 6e6f 726d 616c 2075 7365 7220   Do normal user 
+0000f870: 7661 7269 6162 6c65 2063 6173 6520 2a2f  variable case */
+0000f880: 0a20 2020 2069 6628 636f 6c6e 7244 6570  .    if(colnrDep
+0000f890: 203c 3d20 6c70 2d3e 636f 6c75 6d6e 7329   <= lp->columns)
+0000f8a0: 0a20 2020 2020 206d 6174 5f73 6574 7661  .      mat_setva
+0000f8b0: 6c75 6528 6d61 742c 2063 6f6c 6e72 4465  lue(mat, colnrDe
+0000f8c0: 702c 2069 782c 2062 6574 612c 2046 414c  p, ix, beta, FAL
+0000f8d0: 5345 293b 0a0a 2020 2020 2f2a 2048 616e  SE);..    /* Han
+0000f8e0: 646c 6520 6361 7365 2077 6865 7265 2061  dle case where a
+0000f8f0: 2073 6c61 636b 2076 6172 6961 626c 6520   slack variable 
+0000f900: 6973 2072 6566 6572 656e 6365 6420 2a2f  is referenced */
+0000f910: 0a20 2020 2065 6c73 6520 7b0a 2020 2020  .    else {.    
+0000f920: 2020 696e 7420 6970 6f73 2c20 6a78 203d    int ipos, jx =
+0000f930: 206d 6174 2d3e 636f 6c5f 7461 675b 6978   mat->col_tag[ix
+0000f940: 5d3b 0a20 2020 2020 206d 6174 5f73 6574  ];.      mat_set
+0000f950: 7661 6c75 6528 6d61 742c 206a 782c 2069  value(mat, jx, i
+0000f960: 782c 2062 6574 612c 2046 414c 5345 293b  x, beta, FALSE);
+0000f970: 0a20 2020 2020 206a 7820 3d20 6d61 745f  .      jx = mat_
+0000f980: 6669 6e64 696e 7328 6d61 742c 206a 782c  findins(mat, jx,
+0000f990: 2069 782c 2026 6970 6f73 2c20 4641 4c53   ix, &ipos, FALS
+0000f9a0: 4529 3b0a 2020 2020 2020 434f 4c5f 4d41  E);.      COL_MA
+0000f9b0: 545f 524f 574e 5228 6970 6f73 2920 3d20  T_ROWNR(ipos) = 
+0000f9c0: 636f 6c6e 7244 6570 3b0a 2020 2020 7d0a  colnrDep;.    }.
+0000f9d0: 2020 2020 7265 7475 726e 2820 5452 5545      return( TRUE
+0000f9e0: 2029 3b0a 2020 7d0a 2020 656c 7365 0a20   );.  }.  else. 
+0000f9f0: 2020 2072 6574 7572 6e28 2046 414c 5345     return( FALSE
+0000fa00: 2029 3b0a 7d0a 5354 4154 4943 204d 5942   );.}.STATIC MYB
+0000fa10: 4f4f 4c20 6164 6455 6e64 6f50 7265 736f  OOL addUndoPreso
+0000fa20: 6c76 6528 6c70 7265 6320 2a6c 702c 204d  lve(lprec *lp, M
+0000fa30: 5942 4f4f 4c20 6973 7072 696d 616c 2c20  YBOOL isprimal, 
+0000fa40: 696e 7420 636f 6c6e 7245 6c69 6d2c 2052  int colnrElim, R
+0000fa50: 4541 4c20 616c 7068 612c 2052 4541 4c20  EAL alpha, REAL 
+0000fa60: 6265 7461 2c20 696e 7420 636f 6c6e 7244  beta, int colnrD
+0000fa70: 6570 290a 7b0a 2020 696e 7420 2020 2020  ep).{.  int     
+0000fa80: 2020 6978 3b0a 2020 4465 6c74 6156 7265    ix;.  DeltaVre
+0000fa90: 6320 2a2a 4456 3b0a 2020 4d41 5472 6563  c **DV;.  MATrec
+0000faa0: 2020 2020 2a6d 6174 3b0a 2020 7072 6573      *mat;.  pres
+0000fab0: 6f6c 7665 756e 646f 7265 6320 2a70 7364  olveundorec *psd
+0000fac0: 6174 6120 3d20 6c70 2d3e 7072 6573 6f6c  ata = lp->presol
+0000fad0: 7665 5f75 6e64 6f3b 0a0a 2020 2f2a 2050  ve_undo;..  /* P
+0000fae0: 6f69 6e74 2074 6f20 616e 6420 696e 6974  oint to and init
+0000faf0: 6961 6c69 7a65 2075 6e64 6f20 7374 7275  ialize undo stru
+0000fb00: 6374 7572 6520 6174 2066 6972 7374 2063  cture at first c
+0000fb10: 616c 6c20 2a2f 0a20 2069 6628 6973 7072  all */.  if(ispr
+0000fb20: 696d 616c 2920 7b0a 2020 2020 4456 203d  imal) {.    DV =
+0000fb30: 2026 2870 7364 6174 612d 3e70 7269 6d61   &(psdata->prima
+0000fb40: 6c75 6e64 6f29 3b0a 2020 2020 6966 282a  lundo);.    if(*
+0000fb50: 4456 203d 3d20 4e55 4c4c 2920 7b0a 2020  DV == NULL) {.  
+0000fb60: 2020 2020 2a44 5620 3d20 6372 6561 7465      *DV = create
+0000fb70: 556e 646f 4c61 6464 6572 286c 702c 206c  UndoLadder(lp, l
+0000fb80: 702d 3e63 6f6c 756d 6e73 2b31 2c20 6c70  p->columns+1, lp
+0000fb90: 2d3e 636f 6c75 6d6e 7329 3b0a 2020 2020  ->columns);.    
+0000fba0: 2020 6d61 7420 3d20 282a 4456 292d 3e74    mat = (*DV)->t
+0000fbb0: 7261 636b 6572 3b0a 2020 2020 2020 6d61  racker;.      ma
+0000fbc0: 742d 3e65 7073 7661 6c75 6520 3d20 6c70  t->epsvalue = lp
+0000fbd0: 2d3e 6d61 7441 2d3e 6570 7376 616c 7565  ->matA->epsvalue
+0000fbe0: 3b0a 2020 2020 2020 616c 6c6f 6349 4e54  ;.      allocINT
+0000fbf0: 286c 702c 2026 286d 6174 2d3e 636f 6c5f  (lp, &(mat->col_
+0000fc00: 7461 6729 2c20 6c70 2d3e 636f 6c75 6d6e  tag), lp->column
+0000fc10: 732b 312c 2046 414c 5345 293b 0a20 2020  s+1, FALSE);.   
+0000fc20: 2020 206d 6174 2d3e 636f 6c5f 7461 675b     mat->col_tag[
+0000fc30: 305d 203d 2030 3b0a 2020 2020 7d0a 2020  0] = 0;.    }.  
+0000fc40: 7d0a 2020 656c 7365 207b 0a20 2020 2044  }.  else {.    D
+0000fc50: 5620 3d20 2628 7073 6461 7461 2d3e 6475  V = &(psdata->du
+0000fc60: 616c 756e 646f 293b 0a20 2020 2069 6628  alundo);.    if(
+0000fc70: 2a44 5620 3d3d 204e 554c 4c29 207b 0a20  *DV == NULL) {. 
+0000fc80: 2020 2020 202a 4456 203d 2063 7265 6174       *DV = creat
+0000fc90: 6555 6e64 6f4c 6164 6465 7228 6c70 2c20  eUndoLadder(lp, 
+0000fca0: 6c70 2d3e 726f 7773 2b31 2c20 6c70 2d3e  lp->rows+1, lp->
+0000fcb0: 726f 7773 293b 0a20 2020 2020 206d 6174  rows);.      mat
+0000fcc0: 203d 2028 2a44 5629 2d3e 7472 6163 6b65   = (*DV)->tracke
+0000fcd0: 723b 0a20 2020 2020 206d 6174 2d3e 6570  r;.      mat->ep
+0000fce0: 7376 616c 7565 203d 206c 702d 3e6d 6174  svalue = lp->mat
+0000fcf0: 412d 3e65 7073 7661 6c75 653b 0a20 2020  A->epsvalue;.   
+0000fd00: 2020 2061 6c6c 6f63 494e 5428 6c70 2c20     allocINT(lp, 
+0000fd10: 2628 6d61 742d 3e63 6f6c 5f74 6167 292c  &(mat->col_tag),
+0000fd20: 206c 702d 3e72 6f77 732b 312c 2046 414c   lp->rows+1, FAL
+0000fd30: 5345 293b 0a20 2020 2020 206d 6174 2d3e  SE);.      mat->
+0000fd40: 636f 6c5f 7461 675b 305d 203d 2030 3b0a  col_tag[0] = 0;.
+0000fd50: 2020 2020 7d0a 2020 7d0a 2020 6d61 7420      }.  }.  mat 
+0000fd60: 3d20 282a 4456 292d 3e74 7261 636b 6572  = (*DV)->tracker
+0000fd70: 3b0a 2369 6620 300a 2020 7265 706f 7274  ;.#if 0.  report
+0000fd80: 286c 702c 204e 4f52 4d41 4c2c 2022 6164  (lp, NORMAL, "ad
+0000fd90: 6455 6e64 6f50 7265 736f 6c76 653a 2078  dUndoPresolve: x
+0000fda0: 2564 203d 2025 6720 2573 2025 6720 2a20  %d = %g %s %g * 
+0000fdb0: 7825 645c 6e22 2c0a 2020 2020 2020 2020  x%d\n",.        
+0000fdc0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0000fdd0: 6e72 456c 696d 2c20 616c 7068 612c 2028  nrElim, alpha, (
+0000fde0: 2062 6574 6120 3c20 3020 3f20 222d 2220   beta < 0 ? "-" 
+0000fdf0: 3a20 222b 2229 2c20 6661 6273 2862 6574  : "+"), fabs(bet
+0000fe00: 6129 2c20 636f 6c6e 7244 6570 293b 0a23  a), colnrDep);.#
+0000fe10: 656e 6469 660a 2020 2f2a 2041 6464 2074  endif.  /* Add t
+0000fe20: 6865 2064 6174 6120 2a2f 0a20 2069 7820  he data */.  ix 
+0000fe30: 3d20 6d61 742d 3e63 6f6c 5f74 6167 5b30  = mat->col_tag[0
+0000fe40: 5d20 3d20 696e 6372 656d 656e 7455 6e64  ] = incrementUnd
+0000fe50: 6f4c 6164 6465 7228 2a44 5629 3b0a 2020  oLadder(*DV);.  
+0000fe60: 6d61 742d 3e63 6f6c 5f74 6167 5b69 785d  mat->col_tag[ix]
+0000fe70: 203d 2063 6f6c 6e72 456c 696d 3b0a 2020   = colnrElim;.  
+0000fe80: 6966 2861 6c70 6861 2021 3d20 3029 0a20  if(alpha != 0). 
+0000fe90: 2020 206d 6174 5f73 6574 7661 6c75 6528     mat_setvalue(
+0000fea0: 6d61 742c 2030 2c20 6978 2c20 616c 7068  mat, 0, ix, alph
+0000feb0: 612c 2046 414c 5345 293b 0a2f 2a20 2020  a, FALSE);./*   
+0000fec0: 206d 6174 5f61 7070 656e 6476 616c 7565   mat_appendvalue
+0000fed0: 282a 6d61 742c 2030 2c20 616c 7068 6129  (*mat, 0, alpha)
+0000fee0: 3b2a 2f0a 2020 6966 2828 636f 6c6e 7244  ;*/.  if((colnrD
+0000fef0: 6570 203e 2030 2920 2626 2028 6265 7461  ep > 0) && (beta
+0000ff00: 2021 3d20 3029 2920 7b0a 2020 2020 6966   != 0)) {.    if
+0000ff10: 2863 6f6c 6e72 4465 7020 3e20 6c70 2d3e  (colnrDep > lp->
+0000ff20: 636f 6c75 6d6e 7329 0a20 2020 2020 2072  columns).      r
+0000ff30: 6574 7572 6e28 2061 7070 656e 6455 6e64  eturn( appendUnd
+0000ff40: 6f50 7265 736f 6c76 6528 6c70 2c20 6973  oPresolve(lp, is
+0000ff50: 7072 696d 616c 2c20 6265 7461 2c20 636f  primal, beta, co
+0000ff60: 6c6e 7244 6570 2920 293b 0a20 2020 2065  lnrDep) );.    e
+0000ff70: 6c73 650a 2020 2020 2020 6d61 745f 7365  lse.      mat_se
+0000ff80: 7476 616c 7565 286d 6174 2c20 636f 6c6e  tvalue(mat, coln
+0000ff90: 7244 6570 2c20 6978 2c20 6265 7461 2c20  rDep, ix, beta, 
+0000ffa0: 4641 4c53 4529 3b0a 2020 7d0a 0a20 2072  FALSE);.  }..  r
+0000ffb0: 6574 7572 6e28 2054 5255 4520 293b 0a7d  eturn( TRUE );.}
+0000ffc0: 0a0a 0a0a 2f2a 202d 2d2d 2d2d 2d2d 2d2d  ..../* ---------
+0000ffd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ffe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010020: 2d2d 2d2d 2d2d 2d2d 2d20 2a2f 0a2f 2a20  --------- */./* 
-00010030: 4869 6768 206c 6576 656c 206d 6174 7269  High level matri
-00010040: 7820 696e 7665 7273 6520 616e 6420 7072  x inverse and pr
-00010050: 6f64 7563 7420 726f 7574 696e 6573 2069  oduct routines i
-00010060: 6e20 6c70 5f73 6f6c 7665 2020 2020 2020  n lp_solve      
-00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010080: 2020 202a 2f0a 2f2a 202d 2d2d 2d2d 2d2d     */./* -------
+00010010: 2d2d 2d2d 2d2d 2d2d 2d20 2a2f 0a2f 2a20  --------- */./* 
+00010020: 4869 6768 206c 6576 656c 206d 6174 7269  High level matri
+00010030: 7820 696e 7665 7273 6520 616e 6420 7072  x inverse and pr
+00010040: 6f64 7563 7420 726f 7574 696e 6573 2069  oduct routines i
+00010050: 6e20 6c70 5f73 6f6c 7665 2020 2020 2020  n lp_solve      
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 202a 2f0a 2f2a 202d 2d2d 2d2d 2d2d     */./* -------
+00010080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000100a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000100b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000100c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000100d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 2a2f 0a0a  ----------- */..
-000100e0: 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /* -------------
+000100c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 2a2f 0a0a  ----------- */..
+000100d0: 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /* -------------
+000100e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000100f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010130: 2d2d 2d2d 2d20 2a2f 0a2f 2a20 2020 2041  ----- */./*    A
-00010140: 2062 7269 6566 2064 6573 6372 6970 7469   brief descripti
-00010150: 6f6e 206f 6620 7468 6520 6261 7369 7320  on of the basis 
-00010160: 696e 7665 7273 6520 616e 6420 6661 6374  inverse and fact
-00010170: 6f72 697a 6174 696f 6e20 6c6f 6769 6320  orization logic 
-00010180: 696e 206c 705f 736f 6c76 6520 2020 202a  in lp_solve    *
-00010190: 2f0a 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d  /./* -----------
+00010120: 2d2d 2d2d 2d20 2a2f 0a2f 2a20 2020 2041  ----- */./*    A
+00010130: 2062 7269 6566 2064 6573 6372 6970 7469   brief descripti
+00010140: 6f6e 206f 6620 7468 6520 6261 7369 7320  on of the basis 
+00010150: 696e 7665 7273 6520 616e 6420 6661 6374  inverse and fact
+00010160: 6f72 697a 6174 696f 6e20 6c6f 6769 6320  orization logic 
+00010170: 696e 206c 705f 736f 6c76 6520 2020 202a  in lp_solve    *
+00010180: 2f0a 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d  /./* -----------
+00010190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000101a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000101b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000101c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000101d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000101e0: 2d2d 2d2d 2d2d 2d20 2a2f 0a2f 2a0a 0a20  ------- */./*.. 
-000101f0: 2020 496e 206f 7264 6572 2074 6f20 6265    In order to be
-00010200: 7474 6572 2075 6e64 6572 7374 616e 6420  tter understand 
-00010210: 7468 6520 6c65 6761 6379 2063 6f64 6520  the legacy code 
-00010220: 666f 7220 6f70 6572 6174 696e 6720 7769  for operating wi
-00010230: 7468 2074 6865 0a20 2020 6261 7369 7320  th the.   basis 
-00010240: 616e 6420 6974 7320 6661 6374 6f72 697a  and its factoriz
-00010250: 6174 696f 6e20 696e 206c 705f 736f 6c76  ation in lp_solv
-00010260: 6520 4920 284b 4529 2077 696c 6c20 6272  e I (KE) will br
-00010270: 6965 666c 7920 6578 706c 6169 6e0a 2020  iefly explain.  
-00010280: 2074 6865 2063 6f6e 7665 6e74 696f 6e73   the conventions
-00010290: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
-000102a0: 6d61 7472 6978 2061 6c67 6562 7261 2e20  matrix algebra. 
-000102b0: 204e 6f74 6520 7468 6174 2077 6974 6820   Note that with 
-000102c0: 6c70 5f73 6f6c 7665 0a20 2020 7665 7273  lp_solve.   vers
-000102d0: 696f 6e20 352e 352c 2069 7420 6973 2061  ion 5.5, it is a
-000102e0: 6c73 6f20 706f 7373 6962 6c65 2074 6f20  lso possible to 
-000102f0: 6469 7265 6374 206c 705f 736f 6c76 6520  direct lp_solve 
-00010300: 746f 2075 7365 2074 6865 2074 7261 6469  to use the tradi
-00010310: 7469 6f6e 616c 0a20 2020 2874 6578 7462  tional.   (textb
-00010320: 6f6f 6b29 2066 6f72 6d61 7420 6279 2073  ook) format by s
-00010330: 6574 7469 6e67 2074 6865 206f 626a 5f69  etting the obj_i
-00010340: 6e5f 4220 7061 7261 6d65 7465 7220 746f  n_B parameter to
-00010350: 2046 414c 5345 2e0a 0a20 2020 5468 6520   FALSE...   The 
-00010360: 6d61 7472 6978 2064 6573 6372 6970 7469  matrix descripti
-00010370: 6f6e 206f 6620 6120 6c69 6e65 6172 2070  on of a linear p
-00010380: 726f 6772 616d 2028 6173 2072 6570 7265  rogram (as repre
-00010390: 7365 6e74 6564 2062 7920 6c70 5f73 6f6c  sented by lp_sol
-000103a0: 7665 2920 676f 6573 0a20 2020 6c69 6b65  ve) goes.   like
-000103b0: 2074 6869 733a 0a0a 2020 2020 2020 2020   this:..        
-000103c0: 2020 206d 6178 696d 697a 6520 2020 2020     maximize     
-000103d0: 2020 2020 6327 780a 2020 2020 2020 2020      c'x.        
-000103e0: 2020 2073 7562 6a65 6374 2074 6f20 2072     subject to  r
-000103f0: 203c 3d20 2041 7820 3c3d 2062 0a20 2020   <=  Ax <= b.   
-00010400: 2020 2020 2020 2020 7768 6572 6520 2020          where   
-00010410: 2020 2020 6c20 3c3d 2020 2078 203c 3d20      l <=   x <= 
-00010420: 750a 0a20 2020 5468 6520 6d61 7472 6978  u..   The matrix
-00010430: 2041 2069 7320 7061 7274 6974 696f 6e65   A is partitione
-00010440: 6420 696e 746f 2074 776f 2063 6f6c 756d  d into two colum
-00010450: 6e20 7365 7473 205b 427c 4e5d 2c20 7768  n sets [B|N], wh
-00010460: 6572 6520 4220 6973 0a20 2020 6120 7371  ere B is.   a sq
-00010470: 7561 7265 206d 6174 7269 7820 6f66 2022  uare matrix of "
-00010480: 6261 7369 7322 2076 6172 6961 626c 6573  basis" variables
-00010490: 2063 6f6e 7461 696e 696e 6720 6e6f 6e2d   containing non-
-000104a0: 6669 7865 640a 2020 2076 6172 6961 626c  fixed.   variabl
-000104b0: 6573 206f 6620 7468 6520 6c69 6e65 6172  es of the linear
-000104c0: 2070 726f 6772 616d 2061 7420 616e 7920   program at any 
-000104d0: 6769 7665 6e20 7374 6167 6520 616e 6420  given stage and 
-000104e0: 4e20 6973 2074 6865 0a20 2020 7375 626d  N is the.   subm
-000104f0: 6174 7269 7820 6f66 2063 6f72 7265 7370  atrix of corresp
-00010500: 6f6e 6469 6e67 206e 6f6e 2d62 6173 6963  onding non-basic
-00010510: 2c20 6669 7865 6420 7661 7269 6162 6c65  , fixed variable
-00010520: 732e 2054 6865 0a20 2020 7661 7269 6162  s. The.   variab
-00010530: 6c65 7320 2863 6f6c 756d 6e73 2920 696e  les (columns) in
-00010540: 204e 206d 6179 2062 6520 6669 7865 6420   N may be fixed 
-00010550: 6174 2074 6865 6972 206c 6f77 6572 206f  at their lower o
-00010560: 7220 7570 7065 7220 6c65 7665 6c73 2e0a  r upper levels..
-00010570: 0a20 2020 5369 6d69 6c61 726c 792c 2074  .   Similarly, t
-00010580: 6865 2063 2076 6563 746f 7220 6973 2070  he c vector is p
-00010590: 6172 7469 7469 6f6e 6564 2069 6e74 6f20  artitioned into 
-000105a0: 7468 6520 6261 7369 6320 616e 6420 6e6f  the basic and no
-000105b0: 6e2d 6261 7369 630a 2020 2070 6172 7473  n-basic.   parts
-000105c0: 205b 7a7c 6e5d 2e0a 0a20 2020 5768 696c   [z|n]...   Whil
-000105d0: 6520 6c70 5f73 6f6c 7665 2073 746f 7265  e lp_solve store
-000105e0: 7320 7468 6520 6f62 6a65 6374 6976 6520  s the objective 
-000105f0: 7665 6374 6f72 2063 2069 6e20 6120 6465  vector c in a de
-00010600: 6e73 6520 666f 726d 6174 2c20 616e 640a  nse format, and.
-00010610: 2020 2074 6865 2063 6f6e 7374 7261 696e     the constrain
-00010620: 7420 6d61 7472 6978 2041 2069 6e20 6120  t matrix A in a 
-00010630: 2866 6169 726c 7920 7374 616e 6461 7264  (fairly standard
-00010640: 2920 7370 6172 7365 2066 6f72 6d61 742c  ) sparse format,
-00010650: 2074 6865 0a20 2020 636f 6c75 6d6e 2076   the.   column v
-00010660: 6563 746f 7273 2070 6173 7365 6420 746f  ectors passed to
-00010670: 2074 6865 2066 6163 746f 7269 7a61 7469   the factorizati
-00010680: 6f6e 2072 6f75 7469 6e65 2069 6e63 6c75  on routine inclu
-00010690: 6465 2074 6865 0a20 2020 6f62 6a65 6374  de the.   object
-000106a0: 6976 6520 636f 6566 6669 6369 656e 7420  ive coefficient 
-000106b0: 6174 2072 6f77 2069 6e64 6578 2030 2e20  at row index 0. 
-000106c0: 2028 496e 2076 6572 7369 6f6e 7320 6f66   (In versions of
-000106d0: 206c 705f 736f 6c76 650a 2020 2062 6566   lp_solve.   bef
-000106e0: 6f72 6520 7635 2e32 2c20 6320 7761 7320  ore v5.2, c was 
-000106f0: 6163 7475 616c 6c79 2065 7870 6c69 6369  actually explici
-00010700: 746c 7920 7374 6f72 6564 2061 7320 7468  tly stored as th
-00010710: 6520 302d 7468 2072 6f77 206f 6620 4129  e 0-th row of A)
-00010720: 2e0a 2020 2054 6865 2065 7870 616e 6465  ..   The expande
-00010730: 6420 6d61 7472 6978 206d 6179 2062 6520  d matrix may be 
-00010740: 6361 6c6c 6564 2074 6865 2022 417e 2220  called the "A~" 
-00010750: 666f 726d 2061 6e64 206c 6f6f 6b73 206c  form and looks l
-00010760: 696b 6520 7468 6973 3a0a 0a20 2020 2020  ike this:..     
-00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010780: 2020 417e 203d 205b 2063 205d 0a20 2020    A~ = [ c ].   
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 205b 2041 205d 0a0a           [ A ]..
-000107b0: 2020 204c 696e 6561 7220 7072 6f67 7261     Linear progra
-000107c0: 6d6d 696e 6720 696e 766f 6c76 6573 2073  mming involves s
-000107d0: 6f6c 7669 6e67 206c 696e 6561 7220 6571  olving linear eq
-000107e0: 7561 7469 6f6e 7320 6261 7365 6420 6f6e  uations based on
-000107f0: 2074 6865 0a20 2020 7371 7561 7265 2062   the.   square b
-00010800: 6173 6973 206d 6174 7269 7820 422c 2077  asis matrix B, w
-00010810: 6869 6368 2069 6e63 6c75 6465 7320 6973  hich includes is
-00010820: 2061 2073 7562 7365 7420 6f66 2063 6f6c   a subset of col
-00010830: 756d 6e73 2066 726f 6d20 417e 2e0a 2020  umns from A~..  
-00010840: 2054 6865 2069 6d70 6c69 6361 7469 6f6e   The implication
-00010850: 7320 6f66 2074 6865 2063 6f6d 6d6f 6e20  s of the common 
-00010860: 7374 6f72 6167 6520 6f66 2063 2061 6e64  storage of c and
-00010870: 2041 2028 652e 672e 2041 7e29 2076 732e   A (e.g. A~) vs.
-00010880: 2074 6865 0a20 2020 696e 7665 7273 6520   the.   inverse 
-00010890: 2f20 6661 6374 6f72 697a 6174 696f 6e20  / factorization 
-000108a0: 6f66 2042 2066 6f72 2074 6865 206f 7065  of B for the ope
-000108b0: 7261 7469 6f6e 7320 616e 6420 7570 6461  rations and upda
-000108c0: 7465 7320 7065 7266 6f72 6d65 640a 2020  tes performed.  
-000108d0: 2062 7920 7468 6520 7369 6d70 6c65 7820   by the simplex 
-000108e0: 726f 7574 696e 6520 7468 6572 6566 6f72  routine therefor
-000108f0: 6520 6e65 6564 7320 746f 2062 6520 756e  e needs to be un
-00010900: 6465 7273 746f 6f64 2e20 2041 7320 6120  derstood.  As a 
-00010910: 636f 6e73 7175 656e 6365 0a20 2020 6f66  consquence.   of
-00010920: 2041 7e2c 2069 6e20 6c70 5f73 6f6c 7665   A~, in lp_solve
-00010930: 2042 2069 7320 7374 6f72 6564 2069 6e20   B is stored in 
-00010940: 616e 2065 7870 616e 6465 642c 2062 6f72  an expanded, bor
-00010950: 6465 7265 6420 666f 726d 6174 2075 7369  dered format usi
-00010960: 6e67 2074 6865 0a20 2020 666f 6c6c 6f77  ng the.   follow
-00010970: 696e 6720 286e 6f6e 2d73 696e 6775 6c61  ing (non-singula
-00010980: 7229 2072 6570 7265 7365 6e74 6174 696f  r) representatio
-00010990: 6e3a 0a0a 2020 2020 2020 2020 2020 2020  n:..            
-000109a0: 2020 2020 2020 2020 2020 2042 7e20 3d20             B~ = 
-000109b0: 5b20 3120 7a20 5d0a 2020 2020 2020 2020  [ 1 z ].        
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 5b20 3020 4220 5d0a 0a20 2020      [ 0 B ]..   
-000109e0: 416e 7920 6261 7369 7320 696e 7665 7273  Any basis invers
-000109f0: 696f 6e20 2f20 6661 6374 6f72 697a 6174  ion / factorizat
-00010a00: 696f 6e20 656e 6769 6e65 2075 7365 6420  ion engine used 
-00010a10: 6279 206c 705f 736f 6c76 6520 6d75 7374  by lp_solve must
-00010a20: 2074 6865 7265 666f 7265 0a20 2020 6578   therefore.   ex
-00010a30: 706c 6963 6974 6c79 2072 6570 7265 7365  plicitly represe
-00010a40: 6e74 2061 6e64 2068 616e 646c 6520 7468  nt and handle th
-00010a50: 6520 696d 706c 6963 6174 696f 6e73 206f  e implications o
-00010a60: 6620 7468 6973 2073 7472 7563 7475 7265  f this structure
-00010a70: 2066 6f72 0a20 2020 6173 736f 6369 6174   for.   associat
-00010a80: 6564 206d 6174 7269 7820 6f70 6572 6174  ed matrix operat
-00010a90: 696f 6e73 2e0a 0a20 2020 5468 6520 7374  ions...   The st
-00010aa0: 616e 6461 7264 206d 6174 7269 7820 666f  andard matrix fo
-00010ab0: 726d 756c 6120 666f 7220 636f 6d70 7574  rmula for comput
-00010ac0: 696e 6720 7468 6520 696e 7665 7273 6520  ing the inverse 
-00010ad0: 6f66 2061 2062 6f72 6465 7265 640a 2020  of a bordered.  
-00010ae0: 206d 6174 7269 7820 7368 6f77 7320 7768   matrix shows wh
-00010af0: 6174 2074 6865 2069 6e76 6572 7369 6f6e  at the inversion
-00010b00: 206f 6620 427e 2061 6374 7561 6c6c 7920   of B~ actually 
-00010b10: 7072 6f64 7563 6573 3a0a 0a20 2020 2020  produces:..     
-00010b20: 2020 2020 2020 2020 2020 2020 2049 6e76               Inv
-00010b30: 2842 7e29 203d 205b 2031 202d 7a2a 496e  (B~) = [ 1 -z*In
-00010b40: 7628 4229 205d 0a20 2020 2020 2020 2020  v(B) ].         
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b60: 2020 205b 2030 2020 2049 6e76 2842 2920     [ 0   Inv(B) 
-00010b70: 205d 0a0a 2020 2054 6865 2041 7e20 616e   ]..   The A~ an
-00010b80: 6420 427e 2072 6570 7265 7365 6e74 6174  d B~ representat
-00010b90: 696f 6e73 2072 6571 7569 7265 2061 7761  ions require awa
-00010ba0: 7265 6e65 7373 2062 7920 7468 6520 6465  reness by the de
-00010bb0: 7665 6c6f 7065 7220 6f66 2074 6865 2073  veloper of the s
-00010bc0: 6964 650a 2020 2065 6666 6563 7473 206f  ide.   effects o
-00010bd0: 6620 7468 6520 7072 6573 656e 6365 206f  f the presence o
-00010be0: 6620 7468 6520 746f 7020 726f 7720 7768  f the top row wh
-00010bf0: 656e 2064 6f69 6e67 2070 726f 6475 6374  en doing product
-00010c00: 206f 7065 7261 7469 6f6e 7320 7375 6368   operations such
-00010c10: 2061 730a 2020 2062 274e 2c20 6274 7261   as.   b'N, btra
-00010c20: 6e20 616e 6420 6674 7261 6e2e 2020 4e6f  n and ftran.  No
-00010c30: 7465 2069 6e20 7061 7274 6963 756c 6172  te in particular
-00010c40: 207a 2a49 6e76 2842 2920 696e 2074 6865   z*Inv(B) in the
-00010c50: 2074 6f70 2072 6f77 206f 6620 496e 7628   top row of Inv(
-00010c60: 427e 292c 0a20 2020 7768 6963 6820 6973  B~),.   which is
-00010c70: 2061 6374 7561 6c6c 7920 7468 6520 6475   actually the du
-00010c80: 616c 2073 6f6c 7574 696f 6e20 7665 6374  al solution vect
-00010c90: 6f72 206f 6620 7468 6520 6769 7665 6e20  or of the given 
-00010ca0: 6261 7369 732e 2020 5468 6973 2066 6163  basis.  This fac
-00010cb0: 740a 2020 206d 616b 6573 2061 2076 6572  t.   makes a ver
-00010cc0: 7920 636f 6d6d 6f6e 2075 7064 6174 6520  y common update 
-00010cd0: 696e 2074 6865 2073 696d 706c 6578 2061  in the simplex a
-00010ce0: 6c67 6f72 6974 686d 2028 7265 6475 6365  lgorithm (reduce
-00010cf0: 6420 636f 7374 7329 2072 6574 7572 6e61  d costs) returna
-00010d00: 626c 650a 2020 2061 7320 6120 7665 6374  ble.   as a vect
-00010d10: 6f72 2073 696d 706c 7920 6279 2073 6574  or simply by set
-00010d20: 7469 6e67 2031 2061 7420 7468 6520 746f  ting 1 at the to
-00010d30: 7020 6f66 2061 2076 6563 746f 7220 6265  p of a vector be
-00010d40: 696e 6720 7072 652d 6d75 6c74 6970 6c69  ing pre-multipli
-00010d50: 6564 0a20 2020 7769 7468 2049 6e76 2842  ed.   with Inv(B
-00010d60: 7e29 2e0a 0a20 2020 486f 7765 7665 722c  ~)...   However,
-00010d70: 2069 6620 7468 6520 6f62 6a65 6374 6976   if the objectiv
-00010d80: 6520 7665 6374 6f72 2028 6329 2069 7320  e vector (c) is 
-00010d90: 6368 616e 6765 642c 2074 6865 2065 7870  changed, the exp
-00010da0: 616e 6465 6420 7265 7072 6573 656e 7461  anded representa
-00010db0: 7469 6f6e 0a20 2020 7265 7175 6972 6573  tion.   requires
-00010dc0: 2074 6861 7420 4220 2f20 427e 2062 6520   that B / B~ be 
-00010dd0: 7265 6661 6374 6f72 697a 6564 2e20 2041  refactorized.  A
-00010de0: 6c73 6f2c 2077 6865 6e20 646f 696e 6720  lso, when doing 
-00010df0: 4654 5241 4e2c 2042 5452 414e 0a20 2020  FTRAN, BTRAN.   
-00010e00: 616e 6420 7827 412d 7479 7065 206f 7065  and x'A-type ope
-00010e10: 7261 7469 6f6e 732c 2079 6f75 2077 696c  rations, you wil
-00010e20: 6c20 7061 7465 6e74 6c79 2067 6574 2074  l patently get t
-00010e30: 6865 2069 6e63 6f72 7265 6374 2072 6573  he incorrect res
-00010e40: 756c 740a 2020 2069 6620 796f 7520 7369  ult.   if you si
-00010e50: 6d70 6c79 2063 6f70 7920 7468 6520 6f70  mply copy the op
-00010e60: 6572 6174 696f 6e73 2067 6976 656e 2069  erations given i
-00010e70: 6e20 7465 7874 626f 6f6b 732e 2020 4669  n textbooks.  Fi
-00010e80: 7273 7420 4927 6c6c 2073 686f 7720 7468  rst I'll show th
-00010e90: 650a 2020 2072 6573 756c 7473 206f 6620  e.   results of 
-00010ea0: 616e 2046 5452 414e 206f 7065 7261 7469  an FTRAN operati
-00010eb0: 6f6e 3a0a 0a20 2020 2020 2020 2020 2020  on:..           
-00010ec0: 2020 2020 2020 2020 4278 203d 2061 2020          Bx = a  
-00010ed0: 3d3d 3e20 2078 203d 2046 5452 414e 2861  ==>  x = FTRAN(a
-00010ee0: 290a 0a20 2020 496e 206c 705f 736f 6c76  )..   In lp_solv
-00010ef0: 652c 2074 6869 7320 6f70 6572 6174 696f  e, this operatio
-00010f00: 6e20 736f 6c76 6573 3a0a 0a20 2020 2020  n solves:..     
-00010f10: 2020 2020 2020 2020 2020 2020 2020 5b20                [ 
-00010f20: 3120 7a20 5d20 5b79 5d20 3d20 5b64 5d0a  1 z ] [y] = [d].
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f40: 2020 205b 2030 2042 205d 205b 785d 2020     [ 0 B ] [x]  
-00010f50: 205b 615d 0a0a 2020 2055 7369 6e67 2074   [a]..   Using t
-00010f60: 6865 2049 6e76 2842 7e29 2065 7870 7265  he Inv(B~) expre
-00010f70: 7373 696f 6e20 6561 726c 6965 722c 2074  ssion earlier, t
-00010f80: 6865 2046 5452 414e 2072 6573 756c 7420  he FTRAN result 
-00010f90: 6973 2074 6865 7265 666f 7265 3a0a 0a20  is therefore:.. 
-00010fa0: 2020 2020 2020 2020 2020 2020 5b79 5d20              [y] 
-00010fb0: 3d20 5b20 3120 2d7a 2a49 6e76 2842 2920  = [ 1 -z*Inv(B) 
-00010fc0: 5d20 5b64 5d20 3d20 5b20 6420 2d20 7a2a  ] [d] = [ d - z*
-00010fd0: 496e 7628 4229 2a61 205d 0a20 2020 2020  Inv(B)*a ].     
-00010fe0: 2020 2020 2020 2020 5b78 5d20 2020 5b20          [x]   [ 
-00010ff0: 3020 2020 496e 7628 4229 2020 5d20 5b61  0   Inv(B)  ] [a
-00011000: 5d20 2020 5b20 2020 496e 7628 4229 2a61  ]   [   Inv(B)*a
-00011010: 2020 2020 205d 0a0a 2020 2041 7320 616e       ]..   As an
-00011020: 2065 7861 6d70 6c65 2c20 7468 6520 7661   example, the va
-00011030: 6c75 6520 6f66 2074 6865 2064 7561 6c20  lue of the dual 
-00011040: 6f62 6a65 6374 6976 6520 6361 6e20 6265  objective can be
-00011050: 2072 6574 7572 6e65 6420 6174 2074 6865   returned at the
-00011060: 0a20 2020 302d 7468 2069 6e64 6578 2062  .   0-th index b
-00011070: 7920 7061 7373 696e 6720 7468 6520 6163  y passing the ac
-00011080: 7469 7665 2052 4853 2076 6563 746f 7220  tive RHS vector 
-00011090: 7769 7468 2030 2061 7420 7468 6520 302d  with 0 at the 0-
-000110a0: 7468 2070 6f73 6974 696f 6e2e 0a0a 2020  th position...  
-000110b0: 2053 696d 696c 6172 696c 792c 2064 6f69   Similarily, doi
-000110c0: 6e67 2074 6865 206c 6566 7420 736f 6c76  ng the left solv
-000110d0: 6520 2d20 7065 7266 6f72 6d69 6e67 2074  e - performing t
-000110e0: 6865 2042 5452 414e 2063 616c 6375 6c61  he BTRAN calcula
-000110f0: 7469 6f6e 3a0a 0a20 2020 2020 2020 2020  tion:..         
-00011100: 2020 2020 2020 2020 2020 5b78 2079 5d20            [x y] 
-00011110: 5b20 3120 7a20 5d20 3d20 5b64 2061 275d  [ 1 z ] = [d a']
-00011120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011130: 2020 2020 2020 2020 2020 5b20 3020 4220            [ 0 B 
-00011140: 5d0a 0a20 2020 2e2e 2e20 7769 6c6c 2070  ]..   ... will p
-00011150: 726f 6475 6365 2074 6865 2066 6f6c 6c6f  roduce the follo
-00011160: 7769 6e67 2072 6573 756c 7420 696e 206c  wing result in l
-00011170: 705f 736f 6c76 653a 0a0a 2020 205b 7820  p_solve:..   [x 
-00011180: 795d 203d 205b 6420 6127 5d20 5b20 3120  y] = [d a'] [ 1 
-00011190: 2d7a 2a49 6e76 2842 2920 5d20 3d20 5b20  -z*Inv(B) ] = [ 
-000111a0: 6420 7c20 2d64 2a7a 2a49 6e76 2842 2920  d | -d*z*Inv(B) 
-000111b0: 2b20 6127 2a49 6e76 2842 2920 5d0a 2020  + a'*Inv(B) ].  
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 5b20 3020 2020 496e 7628 4229 2020 5d0a  [ 0   Inv(B)  ].
-000111e0: 0a20 2020 536f 2c20 6966 2079 6f75 2074  .   So, if you t
-000111f0: 686f 7567 6874 2079 6f75 2077 6572 6520  hought you were 
-00011200: 7369 6d70 6c79 2063 6f6d 7075 7469 6e67  simply computing
-00011210: 2022 6127 2a49 6e76 2842 2922 2c20 6c6f   "a'*Inv(B)", lo
-00011220: 6f6b 2061 6761 696e 2e0a 2020 2049 6e20  ok again..   In 
-00011230: 6f72 6465 7220 746f 2070 726f 6475 6365  order to produce
-00011240: 2074 6865 2064 6573 6972 6564 2072 6573   the desired res
-00011250: 756c 742c 2079 6f75 2068 6176 6520 746f  ult, you have to
-00011260: 2073 6574 2064 2074 6f20 3020 6265 666f   set d to 0 befo
-00011270: 7265 0a20 2020 7468 6520 4254 5241 4e20  re.   the BTRAN 
-00011280: 6f70 6572 6174 696f 6e2e 2020 4f6e 2074  operation.  On t
-00011290: 6865 206f 7468 6572 2068 616e 642c 2069  he other hand, i
-000112a0: 6620 796f 7520 7365 7420 6420 746f 2031  f you set d to 1
-000112b0: 2061 6e64 2061 2074 6f20 302c 0a20 2020   and a to 0,.   
-000112c0: 7468 656e 2079 6f75 2061 7265 2076 6572  then you are ver
-000112d0: 7920 636f 6e76 656e 6965 6e74 6c79 206f  y conveniently o
-000112e0: 6e20 796f 7572 2077 6179 2074 6f20 6f62  n your way to ob
-000112f0: 7461 696e 2074 6865 2072 6564 7563 6564  tain the reduced
-00011300: 2063 6f73 7473 0a20 2020 286e 6565 6473   costs.   (needs
-00011310: 2061 2066 7572 7468 6572 206d 6174 7269   a further matri
-00011320: 7820 7072 656d 756c 7469 706c 6963 6174  x premultiplicat
-00011330: 696f 6e20 7769 7468 206e 6f6e 2d62 6173  ion with non-bas
-00011340: 6963 2076 6172 6961 626c 6573 292e 0a0a  ic variables)...
-00011350: 2020 2049 6e63 6964 656e 7461 6c6c 792c     Incidentally,
-00011360: 2074 6865 2042 5452 414e 2077 6974 6820   the BTRAN with 
-00011370: 5b31 2030 5d20 7468 6174 2079 6965 6c64  [1 0] that yield
-00011380: 7320 5b20 3120 7c20 2d7a 2a49 6e76 2842  s [ 1 | -z*Inv(B
-00011390: 2920 5d20 6361 6e0a 2020 2061 6c73 6f20  ) ] can.   also 
-000113a0: 6265 2075 7365 6420 6173 2061 2066 6173  be used as a fas
-000113b0: 7420 7761 7920 6f66 2063 6865 636b 696e  t way of checkin
-000113c0: 6720 7468 6520 6163 6375 7261 6379 206f  g the accuracy o
-000113d0: 6620 7468 6520 6375 7272 656e 740a 2020  f the current.  
-000113e0: 2066 6163 746f 7269 7a61 7469 6f6e 2e0a   factorization..
-000113f0: 0a20 2020 4571 7569 7070 6564 2077 6974  .   Equipped wit
-00011400: 6820 7468 6973 2075 6e64 6572 7374 616e  h this understan
-00011410: 6469 6e67 2c20 4920 686f 7065 2074 6861  ding, I hope tha
-00011420: 7420 796f 7520 7365 6520 7468 6174 0a20  t you see that. 
-00011430: 2020 7468 6520 6170 7072 6f61 6368 2069    the approach i
-00011440: 6e20 6c70 5f73 6f6c 7665 2069 7320 6163  n lp_solve is ac
-00011450: 7475 616c 6c79 2070 7265 7474 7920 636f  tually pretty co
-00011460: 6e76 656e 6965 6e74 2e20 2049 7420 616c  nvenient.  It al
-00011470: 736f 0a20 2020 6265 636f 6d65 7320 6561  so.   becomes ea
-00011480: 7369 6572 2074 6f20 6578 7465 6e64 2066  sier to extend f
-00011490: 756e 6374 696f 6e61 6c69 7479 2069 6e20  unctionality in 
-000114a0: 6c70 5f73 6f6c 7665 2062 7920 6472 6177  lp_solve by draw
-000114b0: 696e 6720 6f6e 0a20 2020 666f 726d 756c  ing on.   formul
-000114c0: 6173 2061 6e64 2065 7870 7265 7373 696f  as and expressio
-000114d0: 6e73 2066 726f 6d20 4c50 206c 6974 6572  ns from LP liter
-000114e0: 6174 7572 6520 7468 6174 206f 7468 6572  ature that other
-000114f0: 7769 7365 2061 7373 756d 650a 2020 2074  wise assume.   t
-00011500: 6865 206e 6f6e 2d62 6f72 6465 7265 6420  he non-bordered 
-00011510: 7379 6e74 6178 2061 6e64 2072 6570 7265  syntax and repre
-00011520: 7365 6e74 6174 696f 6e2e 0a0a 2020 2020  sentation...    
+000101d0: 2d2d 2d2d 2d2d 2d20 2a2f 0a2f 2a0a 0a20  ------- */./*.. 
+000101e0: 2020 496e 206f 7264 6572 2074 6f20 6265    In order to be
+000101f0: 7474 6572 2075 6e64 6572 7374 616e 6420  tter understand 
+00010200: 7468 6520 6c65 6761 6379 2063 6f64 6520  the legacy code 
+00010210: 666f 7220 6f70 6572 6174 696e 6720 7769  for operating wi
+00010220: 7468 2074 6865 0a20 2020 6261 7369 7320  th the.   basis 
+00010230: 616e 6420 6974 7320 6661 6374 6f72 697a  and its factoriz
+00010240: 6174 696f 6e20 696e 206c 705f 736f 6c76  ation in lp_solv
+00010250: 6520 4920 284b 4529 2077 696c 6c20 6272  e I (KE) will br
+00010260: 6965 666c 7920 6578 706c 6169 6e0a 2020  iefly explain.  
+00010270: 2074 6865 2063 6f6e 7665 6e74 696f 6e73   the conventions
+00010280: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+00010290: 6d61 7472 6978 2061 6c67 6562 7261 2e20  matrix algebra. 
+000102a0: 204e 6f74 6520 7468 6174 2077 6974 6820   Note that with 
+000102b0: 6c70 5f73 6f6c 7665 0a20 2020 7665 7273  lp_solve.   vers
+000102c0: 696f 6e20 352e 352c 2069 7420 6973 2061  ion 5.5, it is a
+000102d0: 6c73 6f20 706f 7373 6962 6c65 2074 6f20  lso possible to 
+000102e0: 6469 7265 6374 206c 705f 736f 6c76 6520  direct lp_solve 
+000102f0: 746f 2075 7365 2074 6865 2074 7261 6469  to use the tradi
+00010300: 7469 6f6e 616c 0a20 2020 2874 6578 7462  tional.   (textb
+00010310: 6f6f 6b29 2066 6f72 6d61 7420 6279 2073  ook) format by s
+00010320: 6574 7469 6e67 2074 6865 206f 626a 5f69  etting the obj_i
+00010330: 6e5f 4220 7061 7261 6d65 7465 7220 746f  n_B parameter to
+00010340: 2046 414c 5345 2e0a 0a20 2020 5468 6520   FALSE...   The 
+00010350: 6d61 7472 6978 2064 6573 6372 6970 7469  matrix descripti
+00010360: 6f6e 206f 6620 6120 6c69 6e65 6172 2070  on of a linear p
+00010370: 726f 6772 616d 2028 6173 2072 6570 7265  rogram (as repre
+00010380: 7365 6e74 6564 2062 7920 6c70 5f73 6f6c  sented by lp_sol
+00010390: 7665 2920 676f 6573 0a20 2020 6c69 6b65  ve) goes.   like
+000103a0: 2074 6869 733a 0a0a 2020 2020 2020 2020   this:..        
+000103b0: 2020 206d 6178 696d 697a 6520 2020 2020     maximize     
+000103c0: 2020 2020 6327 780a 2020 2020 2020 2020      c'x.        
+000103d0: 2020 2073 7562 6a65 6374 2074 6f20 2072     subject to  r
+000103e0: 203c 3d20 2041 7820 3c3d 2062 0a20 2020   <=  Ax <= b.   
+000103f0: 2020 2020 2020 2020 7768 6572 6520 2020          where   
+00010400: 2020 2020 6c20 3c3d 2020 2078 203c 3d20      l <=   x <= 
+00010410: 750a 0a20 2020 5468 6520 6d61 7472 6978  u..   The matrix
+00010420: 2041 2069 7320 7061 7274 6974 696f 6e65   A is partitione
+00010430: 6420 696e 746f 2074 776f 2063 6f6c 756d  d into two colum
+00010440: 6e20 7365 7473 205b 427c 4e5d 2c20 7768  n sets [B|N], wh
+00010450: 6572 6520 4220 6973 0a20 2020 6120 7371  ere B is.   a sq
+00010460: 7561 7265 206d 6174 7269 7820 6f66 2022  uare matrix of "
+00010470: 6261 7369 7322 2076 6172 6961 626c 6573  basis" variables
+00010480: 2063 6f6e 7461 696e 696e 6720 6e6f 6e2d   containing non-
+00010490: 6669 7865 640a 2020 2076 6172 6961 626c  fixed.   variabl
+000104a0: 6573 206f 6620 7468 6520 6c69 6e65 6172  es of the linear
+000104b0: 2070 726f 6772 616d 2061 7420 616e 7920   program at any 
+000104c0: 6769 7665 6e20 7374 6167 6520 616e 6420  given stage and 
+000104d0: 4e20 6973 2074 6865 0a20 2020 7375 626d  N is the.   subm
+000104e0: 6174 7269 7820 6f66 2063 6f72 7265 7370  atrix of corresp
+000104f0: 6f6e 6469 6e67 206e 6f6e 2d62 6173 6963  onding non-basic
+00010500: 2c20 6669 7865 6420 7661 7269 6162 6c65  , fixed variable
+00010510: 732e 2054 6865 0a20 2020 7661 7269 6162  s. The.   variab
+00010520: 6c65 7320 2863 6f6c 756d 6e73 2920 696e  les (columns) in
+00010530: 204e 206d 6179 2062 6520 6669 7865 6420   N may be fixed 
+00010540: 6174 2074 6865 6972 206c 6f77 6572 206f  at their lower o
+00010550: 7220 7570 7065 7220 6c65 7665 6c73 2e0a  r upper levels..
+00010560: 0a20 2020 5369 6d69 6c61 726c 792c 2074  .   Similarly, t
+00010570: 6865 2063 2076 6563 746f 7220 6973 2070  he c vector is p
+00010580: 6172 7469 7469 6f6e 6564 2069 6e74 6f20  artitioned into 
+00010590: 7468 6520 6261 7369 6320 616e 6420 6e6f  the basic and no
+000105a0: 6e2d 6261 7369 630a 2020 2070 6172 7473  n-basic.   parts
+000105b0: 205b 7a7c 6e5d 2e0a 0a20 2020 5768 696c   [z|n]...   Whil
+000105c0: 6520 6c70 5f73 6f6c 7665 2073 746f 7265  e lp_solve store
+000105d0: 7320 7468 6520 6f62 6a65 6374 6976 6520  s the objective 
+000105e0: 7665 6374 6f72 2063 2069 6e20 6120 6465  vector c in a de
+000105f0: 6e73 6520 666f 726d 6174 2c20 616e 640a  nse format, and.
+00010600: 2020 2074 6865 2063 6f6e 7374 7261 696e     the constrain
+00010610: 7420 6d61 7472 6978 2041 2069 6e20 6120  t matrix A in a 
+00010620: 2866 6169 726c 7920 7374 616e 6461 7264  (fairly standard
+00010630: 2920 7370 6172 7365 2066 6f72 6d61 742c  ) sparse format,
+00010640: 2074 6865 0a20 2020 636f 6c75 6d6e 2076   the.   column v
+00010650: 6563 746f 7273 2070 6173 7365 6420 746f  ectors passed to
+00010660: 2074 6865 2066 6163 746f 7269 7a61 7469   the factorizati
+00010670: 6f6e 2072 6f75 7469 6e65 2069 6e63 6c75  on routine inclu
+00010680: 6465 2074 6865 0a20 2020 6f62 6a65 6374  de the.   object
+00010690: 6976 6520 636f 6566 6669 6369 656e 7420  ive coefficient 
+000106a0: 6174 2072 6f77 2069 6e64 6578 2030 2e20  at row index 0. 
+000106b0: 2028 496e 2076 6572 7369 6f6e 7320 6f66   (In versions of
+000106c0: 206c 705f 736f 6c76 650a 2020 2062 6566   lp_solve.   bef
+000106d0: 6f72 6520 7635 2e32 2c20 6320 7761 7320  ore v5.2, c was 
+000106e0: 6163 7475 616c 6c79 2065 7870 6c69 6369  actually explici
+000106f0: 746c 7920 7374 6f72 6564 2061 7320 7468  tly stored as th
+00010700: 6520 302d 7468 2072 6f77 206f 6620 4129  e 0-th row of A)
+00010710: 2e0a 2020 2054 6865 2065 7870 616e 6465  ..   The expande
+00010720: 6420 6d61 7472 6978 206d 6179 2062 6520  d matrix may be 
+00010730: 6361 6c6c 6564 2074 6865 2022 417e 2220  called the "A~" 
+00010740: 666f 726d 2061 6e64 206c 6f6f 6b73 206c  form and looks l
+00010750: 696b 6520 7468 6973 3a0a 0a20 2020 2020  ike this:..     
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2020 417e 203d 205b 2063 205d 0a20 2020    A~ = [ c ].   
+00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010790: 2020 2020 2020 2020 205b 2041 205d 0a0a           [ A ]..
+000107a0: 2020 204c 696e 6561 7220 7072 6f67 7261     Linear progra
+000107b0: 6d6d 696e 6720 696e 766f 6c76 6573 2073  mming involves s
+000107c0: 6f6c 7669 6e67 206c 696e 6561 7220 6571  olving linear eq
+000107d0: 7561 7469 6f6e 7320 6261 7365 6420 6f6e  uations based on
+000107e0: 2074 6865 0a20 2020 7371 7561 7265 2062   the.   square b
+000107f0: 6173 6973 206d 6174 7269 7820 422c 2077  asis matrix B, w
+00010800: 6869 6368 2069 6e63 6c75 6465 7320 6973  hich includes is
+00010810: 2061 2073 7562 7365 7420 6f66 2063 6f6c   a subset of col
+00010820: 756d 6e73 2066 726f 6d20 417e 2e0a 2020  umns from A~..  
+00010830: 2054 6865 2069 6d70 6c69 6361 7469 6f6e   The implication
+00010840: 7320 6f66 2074 6865 2063 6f6d 6d6f 6e20  s of the common 
+00010850: 7374 6f72 6167 6520 6f66 2063 2061 6e64  storage of c and
+00010860: 2041 2028 652e 672e 2041 7e29 2076 732e   A (e.g. A~) vs.
+00010870: 2074 6865 0a20 2020 696e 7665 7273 6520   the.   inverse 
+00010880: 2f20 6661 6374 6f72 697a 6174 696f 6e20  / factorization 
+00010890: 6f66 2042 2066 6f72 2074 6865 206f 7065  of B for the ope
+000108a0: 7261 7469 6f6e 7320 616e 6420 7570 6461  rations and upda
+000108b0: 7465 7320 7065 7266 6f72 6d65 640a 2020  tes performed.  
+000108c0: 2062 7920 7468 6520 7369 6d70 6c65 7820   by the simplex 
+000108d0: 726f 7574 696e 6520 7468 6572 6566 6f72  routine therefor
+000108e0: 6520 6e65 6564 7320 746f 2062 6520 756e  e needs to be un
+000108f0: 6465 7273 746f 6f64 2e20 2041 7320 6120  derstood.  As a 
+00010900: 636f 6e73 7175 656e 6365 0a20 2020 6f66  consquence.   of
+00010910: 2041 7e2c 2069 6e20 6c70 5f73 6f6c 7665   A~, in lp_solve
+00010920: 2042 2069 7320 7374 6f72 6564 2069 6e20   B is stored in 
+00010930: 616e 2065 7870 616e 6465 642c 2062 6f72  an expanded, bor
+00010940: 6465 7265 6420 666f 726d 6174 2075 7369  dered format usi
+00010950: 6e67 2074 6865 0a20 2020 666f 6c6c 6f77  ng the.   follow
+00010960: 696e 6720 286e 6f6e 2d73 696e 6775 6c61  ing (non-singula
+00010970: 7229 2072 6570 7265 7365 6e74 6174 696f  r) representatio
+00010980: 6e3a 0a0a 2020 2020 2020 2020 2020 2020  n:..            
+00010990: 2020 2020 2020 2020 2020 2042 7e20 3d20             B~ = 
+000109a0: 5b20 3120 7a20 5d0a 2020 2020 2020 2020  [ 1 z ].        
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109c0: 2020 2020 5b20 3020 4220 5d0a 0a20 2020      [ 0 B ]..   
+000109d0: 416e 7920 6261 7369 7320 696e 7665 7273  Any basis invers
+000109e0: 696f 6e20 2f20 6661 6374 6f72 697a 6174  ion / factorizat
+000109f0: 696f 6e20 656e 6769 6e65 2075 7365 6420  ion engine used 
+00010a00: 6279 206c 705f 736f 6c76 6520 6d75 7374  by lp_solve must
+00010a10: 2074 6865 7265 666f 7265 0a20 2020 6578   therefore.   ex
+00010a20: 706c 6963 6974 6c79 2072 6570 7265 7365  plicitly represe
+00010a30: 6e74 2061 6e64 2068 616e 646c 6520 7468  nt and handle th
+00010a40: 6520 696d 706c 6963 6174 696f 6e73 206f  e implications o
+00010a50: 6620 7468 6973 2073 7472 7563 7475 7265  f this structure
+00010a60: 2066 6f72 0a20 2020 6173 736f 6369 6174   for.   associat
+00010a70: 6564 206d 6174 7269 7820 6f70 6572 6174  ed matrix operat
+00010a80: 696f 6e73 2e0a 0a20 2020 5468 6520 7374  ions...   The st
+00010a90: 616e 6461 7264 206d 6174 7269 7820 666f  andard matrix fo
+00010aa0: 726d 756c 6120 666f 7220 636f 6d70 7574  rmula for comput
+00010ab0: 696e 6720 7468 6520 696e 7665 7273 6520  ing the inverse 
+00010ac0: 6f66 2061 2062 6f72 6465 7265 640a 2020  of a bordered.  
+00010ad0: 206d 6174 7269 7820 7368 6f77 7320 7768   matrix shows wh
+00010ae0: 6174 2074 6865 2069 6e76 6572 7369 6f6e  at the inversion
+00010af0: 206f 6620 427e 2061 6374 7561 6c6c 7920   of B~ actually 
+00010b00: 7072 6f64 7563 6573 3a0a 0a20 2020 2020  produces:..     
+00010b10: 2020 2020 2020 2020 2020 2020 2049 6e76               Inv
+00010b20: 2842 7e29 203d 205b 2031 202d 7a2a 496e  (B~) = [ 1 -z*In
+00010b30: 7628 4229 205d 0a20 2020 2020 2020 2020  v(B) ].         
+00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2020 205b 2030 2020 2049 6e76 2842 2920     [ 0   Inv(B) 
+00010b60: 205d 0a0a 2020 2054 6865 2041 7e20 616e   ]..   The A~ an
+00010b70: 6420 427e 2072 6570 7265 7365 6e74 6174  d B~ representat
+00010b80: 696f 6e73 2072 6571 7569 7265 2061 7761  ions require awa
+00010b90: 7265 6e65 7373 2062 7920 7468 6520 6465  reness by the de
+00010ba0: 7665 6c6f 7065 7220 6f66 2074 6865 2073  veloper of the s
+00010bb0: 6964 650a 2020 2065 6666 6563 7473 206f  ide.   effects o
+00010bc0: 6620 7468 6520 7072 6573 656e 6365 206f  f the presence o
+00010bd0: 6620 7468 6520 746f 7020 726f 7720 7768  f the top row wh
+00010be0: 656e 2064 6f69 6e67 2070 726f 6475 6374  en doing product
+00010bf0: 206f 7065 7261 7469 6f6e 7320 7375 6368   operations such
+00010c00: 2061 730a 2020 2062 274e 2c20 6274 7261   as.   b'N, btra
+00010c10: 6e20 616e 6420 6674 7261 6e2e 2020 4e6f  n and ftran.  No
+00010c20: 7465 2069 6e20 7061 7274 6963 756c 6172  te in particular
+00010c30: 207a 2a49 6e76 2842 2920 696e 2074 6865   z*Inv(B) in the
+00010c40: 2074 6f70 2072 6f77 206f 6620 496e 7628   top row of Inv(
+00010c50: 427e 292c 0a20 2020 7768 6963 6820 6973  B~),.   which is
+00010c60: 2061 6374 7561 6c6c 7920 7468 6520 6475   actually the du
+00010c70: 616c 2073 6f6c 7574 696f 6e20 7665 6374  al solution vect
+00010c80: 6f72 206f 6620 7468 6520 6769 7665 6e20  or of the given 
+00010c90: 6261 7369 732e 2020 5468 6973 2066 6163  basis.  This fac
+00010ca0: 740a 2020 206d 616b 6573 2061 2076 6572  t.   makes a ver
+00010cb0: 7920 636f 6d6d 6f6e 2075 7064 6174 6520  y common update 
+00010cc0: 696e 2074 6865 2073 696d 706c 6578 2061  in the simplex a
+00010cd0: 6c67 6f72 6974 686d 2028 7265 6475 6365  lgorithm (reduce
+00010ce0: 6420 636f 7374 7329 2072 6574 7572 6e61  d costs) returna
+00010cf0: 626c 650a 2020 2061 7320 6120 7665 6374  ble.   as a vect
+00010d00: 6f72 2073 696d 706c 7920 6279 2073 6574  or simply by set
+00010d10: 7469 6e67 2031 2061 7420 7468 6520 746f  ting 1 at the to
+00010d20: 7020 6f66 2061 2076 6563 746f 7220 6265  p of a vector be
+00010d30: 696e 6720 7072 652d 6d75 6c74 6970 6c69  ing pre-multipli
+00010d40: 6564 0a20 2020 7769 7468 2049 6e76 2842  ed.   with Inv(B
+00010d50: 7e29 2e0a 0a20 2020 486f 7765 7665 722c  ~)...   However,
+00010d60: 2069 6620 7468 6520 6f62 6a65 6374 6976   if the objectiv
+00010d70: 6520 7665 6374 6f72 2028 6329 2069 7320  e vector (c) is 
+00010d80: 6368 616e 6765 642c 2074 6865 2065 7870  changed, the exp
+00010d90: 616e 6465 6420 7265 7072 6573 656e 7461  anded representa
+00010da0: 7469 6f6e 0a20 2020 7265 7175 6972 6573  tion.   requires
+00010db0: 2074 6861 7420 4220 2f20 427e 2062 6520   that B / B~ be 
+00010dc0: 7265 6661 6374 6f72 697a 6564 2e20 2041  refactorized.  A
+00010dd0: 6c73 6f2c 2077 6865 6e20 646f 696e 6720  lso, when doing 
+00010de0: 4654 5241 4e2c 2042 5452 414e 0a20 2020  FTRAN, BTRAN.   
+00010df0: 616e 6420 7827 412d 7479 7065 206f 7065  and x'A-type ope
+00010e00: 7261 7469 6f6e 732c 2079 6f75 2077 696c  rations, you wil
+00010e10: 6c20 7061 7465 6e74 6c79 2067 6574 2074  l patently get t
+00010e20: 6865 2069 6e63 6f72 7265 6374 2072 6573  he incorrect res
+00010e30: 756c 740a 2020 2069 6620 796f 7520 7369  ult.   if you si
+00010e40: 6d70 6c79 2063 6f70 7920 7468 6520 6f70  mply copy the op
+00010e50: 6572 6174 696f 6e73 2067 6976 656e 2069  erations given i
+00010e60: 6e20 7465 7874 626f 6f6b 732e 2020 4669  n textbooks.  Fi
+00010e70: 7273 7420 4927 6c6c 2073 686f 7720 7468  rst I'll show th
+00010e80: 650a 2020 2072 6573 756c 7473 206f 6620  e.   results of 
+00010e90: 616e 2046 5452 414e 206f 7065 7261 7469  an FTRAN operati
+00010ea0: 6f6e 3a0a 0a20 2020 2020 2020 2020 2020  on:..           
+00010eb0: 2020 2020 2020 2020 4278 203d 2061 2020          Bx = a  
+00010ec0: 3d3d 3e20 2078 203d 2046 5452 414e 2861  ==>  x = FTRAN(a
+00010ed0: 290a 0a20 2020 496e 206c 705f 736f 6c76  )..   In lp_solv
+00010ee0: 652c 2074 6869 7320 6f70 6572 6174 696f  e, this operatio
+00010ef0: 6e20 736f 6c76 6573 3a0a 0a20 2020 2020  n solves:..     
+00010f00: 2020 2020 2020 2020 2020 2020 2020 5b20                [ 
+00010f10: 3120 7a20 5d20 5b79 5d20 3d20 5b64 5d0a  1 z ] [y] = [d].
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 205b 2030 2042 205d 205b 785d 2020     [ 0 B ] [x]  
+00010f40: 205b 615d 0a0a 2020 2055 7369 6e67 2074   [a]..   Using t
+00010f50: 6865 2049 6e76 2842 7e29 2065 7870 7265  he Inv(B~) expre
+00010f60: 7373 696f 6e20 6561 726c 6965 722c 2074  ssion earlier, t
+00010f70: 6865 2046 5452 414e 2072 6573 756c 7420  he FTRAN result 
+00010f80: 6973 2074 6865 7265 666f 7265 3a0a 0a20  is therefore:.. 
+00010f90: 2020 2020 2020 2020 2020 2020 5b79 5d20              [y] 
+00010fa0: 3d20 5b20 3120 2d7a 2a49 6e76 2842 2920  = [ 1 -z*Inv(B) 
+00010fb0: 5d20 5b64 5d20 3d20 5b20 6420 2d20 7a2a  ] [d] = [ d - z*
+00010fc0: 496e 7628 4229 2a61 205d 0a20 2020 2020  Inv(B)*a ].     
+00010fd0: 2020 2020 2020 2020 5b78 5d20 2020 5b20          [x]   [ 
+00010fe0: 3020 2020 496e 7628 4229 2020 5d20 5b61  0   Inv(B)  ] [a
+00010ff0: 5d20 2020 5b20 2020 496e 7628 4229 2a61  ]   [   Inv(B)*a
+00011000: 2020 2020 205d 0a0a 2020 2041 7320 616e       ]..   As an
+00011010: 2065 7861 6d70 6c65 2c20 7468 6520 7661   example, the va
+00011020: 6c75 6520 6f66 2074 6865 2064 7561 6c20  lue of the dual 
+00011030: 6f62 6a65 6374 6976 6520 6361 6e20 6265  objective can be
+00011040: 2072 6574 7572 6e65 6420 6174 2074 6865   returned at the
+00011050: 0a20 2020 302d 7468 2069 6e64 6578 2062  .   0-th index b
+00011060: 7920 7061 7373 696e 6720 7468 6520 6163  y passing the ac
+00011070: 7469 7665 2052 4853 2076 6563 746f 7220  tive RHS vector 
+00011080: 7769 7468 2030 2061 7420 7468 6520 302d  with 0 at the 0-
+00011090: 7468 2070 6f73 6974 696f 6e2e 0a0a 2020  th position...  
+000110a0: 2053 696d 696c 6172 696c 792c 2064 6f69   Similarily, doi
+000110b0: 6e67 2074 6865 206c 6566 7420 736f 6c76  ng the left solv
+000110c0: 6520 2d20 7065 7266 6f72 6d69 6e67 2074  e - performing t
+000110d0: 6865 2042 5452 414e 2063 616c 6375 6c61  he BTRAN calcula
+000110e0: 7469 6f6e 3a0a 0a20 2020 2020 2020 2020  tion:..         
+000110f0: 2020 2020 2020 2020 2020 5b78 2079 5d20            [x y] 
+00011100: 5b20 3120 7a20 5d20 3d20 5b64 2061 275d  [ 1 z ] = [d a']
+00011110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011120: 2020 2020 2020 2020 2020 5b20 3020 4220            [ 0 B 
+00011130: 5d0a 0a20 2020 2e2e 2e20 7769 6c6c 2070  ]..   ... will p
+00011140: 726f 6475 6365 2074 6865 2066 6f6c 6c6f  roduce the follo
+00011150: 7769 6e67 2072 6573 756c 7420 696e 206c  wing result in l
+00011160: 705f 736f 6c76 653a 0a0a 2020 205b 7820  p_solve:..   [x 
+00011170: 795d 203d 205b 6420 6127 5d20 5b20 3120  y] = [d a'] [ 1 
+00011180: 2d7a 2a49 6e76 2842 2920 5d20 3d20 5b20  -z*Inv(B) ] = [ 
+00011190: 6420 7c20 2d64 2a7a 2a49 6e76 2842 2920  d | -d*z*Inv(B) 
+000111a0: 2b20 6127 2a49 6e76 2842 2920 5d0a 2020  + a'*Inv(B) ].  
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 5b20 3020 2020 496e 7628 4229 2020 5d0a  [ 0   Inv(B)  ].
+000111d0: 0a20 2020 536f 2c20 6966 2079 6f75 2074  .   So, if you t
+000111e0: 686f 7567 6874 2079 6f75 2077 6572 6520  hought you were 
+000111f0: 7369 6d70 6c79 2063 6f6d 7075 7469 6e67  simply computing
+00011200: 2022 6127 2a49 6e76 2842 2922 2c20 6c6f   "a'*Inv(B)", lo
+00011210: 6f6b 2061 6761 696e 2e0a 2020 2049 6e20  ok again..   In 
+00011220: 6f72 6465 7220 746f 2070 726f 6475 6365  order to produce
+00011230: 2074 6865 2064 6573 6972 6564 2072 6573   the desired res
+00011240: 756c 742c 2079 6f75 2068 6176 6520 746f  ult, you have to
+00011250: 2073 6574 2064 2074 6f20 3020 6265 666f   set d to 0 befo
+00011260: 7265 0a20 2020 7468 6520 4254 5241 4e20  re.   the BTRAN 
+00011270: 6f70 6572 6174 696f 6e2e 2020 4f6e 2074  operation.  On t
+00011280: 6865 206f 7468 6572 2068 616e 642c 2069  he other hand, i
+00011290: 6620 796f 7520 7365 7420 6420 746f 2031  f you set d to 1
+000112a0: 2061 6e64 2061 2074 6f20 302c 0a20 2020   and a to 0,.   
+000112b0: 7468 656e 2079 6f75 2061 7265 2076 6572  then you are ver
+000112c0: 7920 636f 6e76 656e 6965 6e74 6c79 206f  y conveniently o
+000112d0: 6e20 796f 7572 2077 6179 2074 6f20 6f62  n your way to ob
+000112e0: 7461 696e 2074 6865 2072 6564 7563 6564  tain the reduced
+000112f0: 2063 6f73 7473 0a20 2020 286e 6565 6473   costs.   (needs
+00011300: 2061 2066 7572 7468 6572 206d 6174 7269   a further matri
+00011310: 7820 7072 656d 756c 7469 706c 6963 6174  x premultiplicat
+00011320: 696f 6e20 7769 7468 206e 6f6e 2d62 6173  ion with non-bas
+00011330: 6963 2076 6172 6961 626c 6573 292e 0a0a  ic variables)...
+00011340: 2020 2049 6e63 6964 656e 7461 6c6c 792c     Incidentally,
+00011350: 2074 6865 2042 5452 414e 2077 6974 6820   the BTRAN with 
+00011360: 5b31 2030 5d20 7468 6174 2079 6965 6c64  [1 0] that yield
+00011370: 7320 5b20 3120 7c20 2d7a 2a49 6e76 2842  s [ 1 | -z*Inv(B
+00011380: 2920 5d20 6361 6e0a 2020 2061 6c73 6f20  ) ] can.   also 
+00011390: 6265 2075 7365 6420 6173 2061 2066 6173  be used as a fas
+000113a0: 7420 7761 7920 6f66 2063 6865 636b 696e  t way of checkin
+000113b0: 6720 7468 6520 6163 6375 7261 6379 206f  g the accuracy o
+000113c0: 6620 7468 6520 6375 7272 656e 740a 2020  f the current.  
+000113d0: 2066 6163 746f 7269 7a61 7469 6f6e 2e0a   factorization..
+000113e0: 0a20 2020 4571 7569 7070 6564 2077 6974  .   Equipped wit
+000113f0: 6820 7468 6973 2075 6e64 6572 7374 616e  h this understan
+00011400: 6469 6e67 2c20 4920 686f 7065 2074 6861  ding, I hope tha
+00011410: 7420 796f 7520 7365 6520 7468 6174 0a20  t you see that. 
+00011420: 2020 7468 6520 6170 7072 6f61 6368 2069    the approach i
+00011430: 6e20 6c70 5f73 6f6c 7665 2069 7320 6163  n lp_solve is ac
+00011440: 7475 616c 6c79 2070 7265 7474 7920 636f  tually pretty co
+00011450: 6e76 656e 6965 6e74 2e20 2049 7420 616c  nvenient.  It al
+00011460: 736f 0a20 2020 6265 636f 6d65 7320 6561  so.   becomes ea
+00011470: 7369 6572 2074 6f20 6578 7465 6e64 2066  sier to extend f
+00011480: 756e 6374 696f 6e61 6c69 7479 2069 6e20  unctionality in 
+00011490: 6c70 5f73 6f6c 7665 2062 7920 6472 6177  lp_solve by draw
+000114a0: 696e 6720 6f6e 0a20 2020 666f 726d 756c  ing on.   formul
+000114b0: 6173 2061 6e64 2065 7870 7265 7373 696f  as and expressio
+000114c0: 6e73 2066 726f 6d20 4c50 206c 6974 6572  ns from LP liter
+000114d0: 6174 7572 6520 7468 6174 206f 7468 6572  ature that other
+000114e0: 7769 7365 2061 7373 756d 650a 2020 2074  wise assume.   t
+000114f0: 6865 206e 6f6e 2d62 6f72 6465 7265 6420  he non-bordered 
+00011500: 7379 6e74 6178 2061 6e64 2072 6570 7265  syntax and repre
+00011510: 7365 6e74 6174 696f 6e2e 0a0a 2020 2020  sentation...    
+00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 204b 6a65 6c6c 2045 696b 6c61 6e64 202d   Kjell Eikland -
-00011560: 2d20 4e6f 7665 6d62 6572 2032 3030 330a  - November 2003.
+00011540: 204b 6a65 6c6c 2045 696b 6c61 6e64 202d   Kjell Eikland -
+00011550: 2d20 4e6f 7665 6d62 6572 2032 3030 330a  - November 2003.
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 204b 4520 7570 6461 7465 2020       KE update  
-000115a0: 2020 202d 2d20 4170 7269 6c20 3230 3035     -- April 2005
-000115b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 2020 2020 2020 4b45 2075 7064 6174 6520        KE update 
-000115e0: 2020 2020 2d2d 204a 756e 6520 3230 3035      -- June 2005
-000115f0: 0a0a 2a2f 0a0a 5354 4154 4943 204d 5942  ..*/..STATIC MYB
-00011600: 4f4f 4c20 5f5f 5749 4e41 5049 2069 6e76  OOL __WINAPI inv
-00011610: 6572 7428 6c70 7265 6320 2a6c 702c 204d  ert(lprec *lp, M
-00011620: 5942 4f4f 4c20 7368 6966 7462 6f75 6e64  YBOOL shiftbound
-00011630: 732c 204d 5942 4f4f 4c20 6669 6e61 6c29  s, MYBOOL final)
-00011640: 0a7b 0a20 204d 5942 4f4f 4c20 2a75 7365  .{.  MYBOOL *use
-00011650: 6470 6f73 2c20 7265 7365 7462 6173 6973  dpos, resetbasis
-00011660: 3b0a 2020 5245 414c 2020 2074 6573 743b  ;.  REAL   test;
-00011670: 0a20 2069 6e74 2020 2020 6b2c 2069 2c20  .  int    k, i, 
-00011680: 6a3b 0a20 2069 6e74 2020 2020 7369 6e67  j;.  int    sing
-00011690: 756c 6172 6974 6965 732c 2075 7365 7263  ularities, userc
-000116a0: 6f6c 423b 0a0a 202f 2a20 4d61 6b65 2073  olB;.. /* Make s
-000116b0: 7572 6520 7468 6520 7461 6773 2061 7265  ure the tags are
-000116c0: 2063 6f72 7265 6374 202a 2f0a 2020 6966   correct */.  if
-000116d0: 2821 6d61 745f 7661 6c69 6461 7465 286c  (!mat_validate(l
-000116e0: 702d 3e6d 6174 4129 2920 7b0a 2020 2020  p->matA)) {.    
-000116f0: 6c70 2d3e 7370 785f 7374 6174 7573 203d  lp->spx_status =
-00011700: 2049 4e46 4541 5349 424c 453b 0a20 2020   INFEASIBLE;.   
-00011710: 2072 6574 7572 6e28 4641 4c53 4529 3b0a   return(FALSE);.
-00011720: 2020 7d0a 0a20 2f2a 2043 7265 6174 6520    }.. /* Create 
-00011730: 7468 6520 696e 7665 7273 6520 6d61 6e61  the inverse mana
-00011740: 6765 6d65 6e74 206f 626a 6563 7420 6174  gement object at
-00011750: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
-00011760: 746f 2069 6e76 6572 7428 2920 2a2f 0a20  to invert() */. 
-00011770: 2069 6628 6c70 2d3e 696e 7642 203d 3d20   if(lp->invB == 
-00011780: 4e55 4c4c 290a 2020 2020 6c70 2d3e 6266  NULL).    lp->bf
-00011790: 705f 696e 6974 286c 702c 206c 702d 3e72  p_init(lp, lp->r
-000117a0: 6f77 732c 2030 2c20 4e55 4c4c 293b 0a20  ows, 0, NULL);. 
-000117b0: 2065 6c73 650a 2020 2020 6c70 2d3e 6266   else.    lp->bf
-000117c0: 705f 7072 6570 6172 6566 6163 746f 7269  p_preparefactori
-000117d0: 7a61 7469 6f6e 286c 7029 3b0a 2020 7369  zation(lp);.  si
-000117e0: 6e67 756c 6172 6974 6965 7320 3d20 303b  ngularities = 0;
-000117f0: 0a0a 202f 2a20 4d75 7374 2073 6176 6520  .. /* Must save 
-00011800: 7370 785f 7374 6174 7573 2073 696e 6365  spx_status since
-00011810: 2069 7420 6973 2075 7365 6420 746f 2063   it is used to c
-00011820: 6172 7279 2069 6e66 6f72 6d61 7469 6f6e  arry information
-00011830: 2061 626f 7574 0a20 2020 2074 6865 2070   about.    the p
-00011840: 7265 7365 6e63 6520 616e 6420 6861 6e64  resence and hand
-00011850: 6c69 6e67 206f 6620 7369 6e67 756c 6172  ling of singular
-00011860: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
-00011870: 6d61 7472 6978 202a 2f0a 2020 6966 2875  matrix */.  if(u
-00011880: 7365 7261 626f 7274 286c 702c 204d 5347  serabort(lp, MSG
-00011890: 5f49 4e56 4552 5429 290a 2020 2020 7265  _INVERT)).    re
-000118a0: 7475 726e 2846 414c 5345 293b 0a0a 2369  turn(FALSE);..#i
-000118b0: 6664 6566 2050 6172 616e 6f69 610a 2020  fdef Paranoia.  
-000118c0: 6966 286c 702d 3e73 7078 5f74 7261 6365  if(lp->spx_trace
-000118d0: 290a 2020 2020 7265 706f 7274 286c 702c  ).    report(lp,
-000118e0: 2044 4554 4149 4c45 442c 2022 696e 7665   DETAILED, "inve
-000118f0: 7274 3a20 4974 6572 2025 3130 672c 2066  rt: Iter %10g, f
-00011900: 6163 742d 6c65 6e67 7468 2025 3764 2c20  act-length %7d, 
-00011910: 4f46 2022 2052 4553 554c 5456 414c 5545  OF " RESULTVALUE
-00011920: 4d41 534b 2022 2e5c 6e22 2c0a 2020 2020  MASK ".\n",.    
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2028 646f 7562 6c65 2920 6765       (double) ge
-00011950: 745f 746f 7461 6c5f 6974 6572 286c 7029  t_total_iter(lp)
-00011960: 2c20 6c70 2d3e 6266 705f 636f 6c63 6f75  , lp->bfp_colcou
-00011970: 6e74 286c 7029 2c20 2864 6f75 626c 6529  nt(lp), (double)
-00011980: 202d 6c70 2d3e 7268 735b 305d 293b 0a23   -lp->rhs[0]);.#
-00011990: 656e 6469 660a 0a20 2f2a 2053 746f 7265  endif.. /* Store
-000119a0: 2073 7461 7465 206f 6620 7072 652d 6578   state of pre-ex
-000119b0: 6973 7469 6e67 2062 6173 6973 2c20 616e  isting basis, an
-000119c0: 6420 6174 2074 6865 2073 616d 6520 7469  d at the same ti
-000119d0: 6d65 2063 6865 636b 2069 660a 2020 2020  me check if.    
-000119e0: 7468 6520 6261 7369 7320 6973 2049 3b20  the basis is I; 
-000119f0: 696e 2074 6869 7320 6361 7365 2074 616b  in this case tak
-00011a00: 6520 7468 6520 6561 7379 2077 6179 206f  e the easy way o
-00011a10: 7574 202a 2f0a 2020 6966 2821 616c 6c6f  ut */.  if(!allo
-00011a20: 634d 5942 4f4f 4c28 6c70 2c20 2675 7365  cMYBOOL(lp, &use
-00011a30: 6470 6f73 2c20 6c70 2d3e 7375 6d20 2b20  dpos, lp->sum + 
-00011a40: 312c 2054 5255 4529 2920 7b0a 2020 2020  1, TRUE)) {.    
-00011a50: 6c70 2d3e 6262 5f62 7265 616b 203d 2054  lp->bb_break = T
-00011a60: 5255 453b 0a20 2020 2072 6574 7572 6e28  RUE;.    return(
-00011a70: 4641 4c53 4529 3b0a 2020 7d0a 2020 7573  FALSE);.  }.  us
-00011a80: 6564 706f 735b 305d 203d 2054 5255 453b  edpos[0] = TRUE;
-00011a90: 0a20 2075 7365 7263 6f6c 4220 3d20 303b  .  usercolB = 0;
-00011aa0: 0a20 2066 6f72 2869 203d 2031 3b20 6920  .  for(i = 1; i 
-00011ab0: 3c3d 206c 702d 3e72 6f77 733b 2069 2b2b  <= lp->rows; i++
-00011ac0: 2920 7b0a 2020 2020 6b20 3d20 6c70 2d3e  ) {.    k = lp->
-00011ad0: 7661 725f 6261 7369 635b 695d 3b0a 2020  var_basic[i];.  
-00011ae0: 2020 6966 286b 203e 206c 702d 3e72 6f77    if(k > lp->row
-00011af0: 7329 0a20 2020 2020 2075 7365 7263 6f6c  s).      usercol
-00011b00: 422b 2b3b 0a20 2020 2075 7365 6470 6f73  B++;.    usedpos
-00011b10: 5b6b 5d20 3d20 5452 5545 3b0a 2020 7d0a  [k] = TRUE;.  }.
-00011b20: 2369 6664 6566 2050 6172 616e 6f69 610a  #ifdef Paranoia.
-00011b30: 2020 6966 2821 7665 7269 6679 5f62 6173    if(!verify_bas
-00011b40: 6973 286c 7029 290a 2020 2020 7265 706f  is(lp)).    repo
-00011b50: 7274 286c 702c 2053 4556 4552 452c 2022  rt(lp, SEVERE, "
-00011b60: 696e 7665 7274 3a20 496e 7661 6c69 6420  invert: Invalid 
-00011b70: 6261 7369 7320 6465 7465 6374 6564 2028  basis detected (
-00011b80: 6974 6572 2025 6729 2e5c 6e22 2c0a 2020  iter %g).\n",.  
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 2020 2028 646f 7562 6c65 2920 6765       (double) ge
-00011bb0: 745f 746f 7461 6c5f 6974 6572 286c 7029  t_total_iter(lp)
-00011bc0: 293b 0a23 656e 6469 660a 0a20 2f2a 2054  );.#endif.. /* T
-00011bd0: 616c 6c79 206d 6174 7269 7820 6e7a 2d63  ally matrix nz-c
-00011be0: 6f75 6e74 7320 616e 6420 6368 6563 6b20  ounts and check 
-00011bf0: 6966 2077 6520 7368 6f75 6c64 2072 6573  if we should res
-00011c00: 6574 2062 6173 6973 0a20 2020 2069 6e64  et basis.    ind
-00011c10: 6963 6174 6f72 7320 746f 2061 6c6c 2073  icators to all s
-00011c20: 6c61 636b 7320 2a2f 0a20 2072 6573 6574  lacks */.  reset
-00011c30: 6261 7369 7320 3d20 284d 5942 4f4f 4c29  basis = (MYBOOL)
-00011c40: 2028 2875 7365 7263 6f6c 4220 3e20 3029   ((usercolB > 0)
-00011c50: 2026 2620 6c70 2d3e 6266 705f 6361 6e72   && lp->bfp_canr
-00011c60: 6573 6574 6261 7369 7328 6c70 2929 3b0a  esetbasis(lp));.
-00011c70: 2020 6b20 3d20 303b 0a20 2066 6f72 2869    k = 0;.  for(i
-00011c80: 203d 2031 3b20 6920 3c3d 206c 702d 3e72   = 1; i <= lp->r
-00011c90: 6f77 733b 2069 2b2b 2920 7b0a 2020 2020  ows; i++) {.    
-00011ca0: 6966 286c 702d 3e76 6172 5f62 6173 6963  if(lp->var_basic
-00011cb0: 5b69 5d20 3e20 6c70 2d3e 726f 7773 290a  [i] > lp->rows).
-00011cc0: 2020 2020 2020 6b20 2b3d 206d 6174 5f63        k += mat_c
-00011cd0: 6f6c 6c65 6e67 7468 286c 702d 3e6d 6174  ollength(lp->mat
-00011ce0: 412c 206c 702d 3e76 6172 5f62 6173 6963  A, lp->var_basic
-00011cf0: 5b69 5d20 2d20 6c70 2d3e 726f 7773 2920  [i] - lp->rows) 
-00011d00: 2b20 2869 735f 4f46 5f6e 7a28 6c70 2c6c  + (is_OF_nz(lp,l
-00011d10: 702d 3e76 6172 5f62 6173 6963 5b69 5d20  p->var_basic[i] 
-00011d20: 2d20 6c70 2d3e 726f 7773 2920 3f20 3120  - lp->rows) ? 1 
-00011d30: 3a20 3029 3b0a 2020 2020 6966 2872 6573  : 0);.    if(res
-00011d40: 6574 6261 7369 7329 207b 0a20 2020 2020  etbasis) {.     
-00011d50: 206a 203d 206c 702d 3e76 6172 5f62 6173   j = lp->var_bas
-00011d60: 6963 5b69 5d3b 0a20 2020 2020 2069 6628  ic[i];.      if(
-00011d70: 6a20 3e20 6c70 2d3e 726f 7773 290a 2020  j > lp->rows).  
-00011d80: 2020 2020 2020 6c70 2d3e 6973 5f62 6173        lp->is_bas
-00011d90: 6963 5b6a 5d20 3d20 4641 4c53 453b 0a20  ic[j] = FALSE;. 
-00011da0: 2020 2020 206c 702d 3e76 6172 5f62 6173       lp->var_bas
-00011db0: 6963 5b69 5d20 3d20 693b 0a20 2020 2020  ic[i] = i;.     
-00011dc0: 206c 702d 3e69 735f 6261 7369 635b 695d   lp->is_basic[i]
-00011dd0: 203d 2054 5255 453b 0a20 2020 207d 0a20   = TRUE;.    }. 
-00011de0: 207d 0a0a 202f 2a20 4e6f 7720 646f 2074   }.. /* Now do t
-00011df0: 6865 2072 6566 6163 746f 7269 7a61 7469  he refactorizati
-00011e00: 6f6e 202a 2f0a 2020 7369 6e67 756c 6172  on */.  singular
-00011e10: 6974 6965 7320 3d20 6c70 2d3e 6266 705f  ities = lp->bfp_
-00011e20: 6661 6374 6f72 697a 6528 6c70 2c20 7573  factorize(lp, us
-00011e30: 6572 636f 6c42 2c20 6b2c 2075 7365 6470  ercolB, k, usedp
-00011e40: 6f73 2c20 6669 6e61 6c29 3b0a 0a20 2f2a  os, final);.. /*
-00011e50: 2044 6f20 7573 6572 2072 6570 6f72 7469   Do user reporti
-00011e60: 6e67 202a 2f0a 2020 6966 2875 7365 7261  ng */.  if(usera
-00011e70: 626f 7274 286c 702c 204d 5347 5f49 4e56  bort(lp, MSG_INV
-00011e80: 4552 5429 290a 2020 2020 676f 746f 2043  ERT)).    goto C
-00011e90: 6c65 616e 7570 3b0a 0a20 2f2a 2046 696e  leanup;.. /* Fin
-00011ea0: 616c 697a 6520 6661 6374 6f72 697a 6174  alize factorizat
-00011eb0: 696f 6e2f 696e 7665 7273 696f 6e20 2a2f  ion/inversion */
-00011ec0: 0a20 206c 702d 3e62 6670 5f66 696e 6973  .  lp->bfp_finis
-00011ed0: 6866 6163 746f 7269 7a61 7469 6f6e 286c  hfactorization(l
-00011ee0: 7029 3b0a 0a20 202f 2a20 5265 636f 6d70  p);..  /* Recomp
-00011ef0: 7574 6520 7468 6520 5248 5320 2820 5265  ute the RHS ( Re
-00011f00: 662e 206c 705f 736f 6c76 6520 696e 7665  f. lp_solve inve
-00011f10: 7273 6520 6c6f 6769 6320 616e 6420 4368  rse logic and Ch
-00011f20: 7661 7461 6c20 702e 2031 3231 2029 202a  vatal p. 121 ) *
-00011f30: 2f0a 2020 7265 636f 6d70 7574 655f 736f  /.  recompute_so
-00011f40: 6c75 7469 6f6e 286c 702c 2073 6869 6674  lution(lp, shift
-00011f50: 626f 756e 6473 293b 0a20 2072 6573 7461  bounds);.  resta
-00011f60: 7274 5072 6963 6572 286c 702c 2041 5554  rtPricer(lp, AUT
-00011f70: 4f4d 4154 4943 293b 0a0a 436c 6561 6e75  OMATIC);..Cleanu
-00011f80: 703a 0a20 202f 2a20 4368 6563 6b20 666f  p:.  /* Check fo
-00011f90: 7220 6e75 6d65 7269 6361 6c20 696e 7374  r numerical inst
-00011fa0: 6162 696c 6974 7920 696e 6469 6361 7465  ability indicate
-00011fb0: 6420 6279 2066 7265 7175 656e 7420 7265  d by frequent re
-00011fc0: 6661 6374 6f72 697a 6174 696f 6e73 202a  factorizations *
-00011fd0: 2f0a 2020 7465 7374 203d 2067 6574 5f72  /.  test = get_r
-00011fe0: 6566 6163 7466 7265 7175 656e 6379 286c  efactfrequency(l
-00011ff0: 702c 2046 414c 5345 293b 0a20 2069 6628  p, FALSE);.  if(
-00012000: 7465 7374 203c 204d 494e 5f52 4546 4143  test < MIN_REFAC
-00012010: 5446 5245 5155 454e 4359 2920 7b0a 2020  TFREQUENCY) {.  
-00012020: 2020 7465 7374 203d 2067 6574 5f72 6566    test = get_ref
-00012030: 6163 7466 7265 7175 656e 6379 286c 702c  actfrequency(lp,
-00012040: 2054 5255 4529 3b0a 2020 2020 7265 706f   TRUE);.    repo
-00012050: 7274 286c 702c 204e 4f52 4d41 4c2c 2022  rt(lp, NORMAL, "
-00012060: 696e 7665 7274 3a20 5265 6661 6374 6f72  invert: Refactor
-00012070: 697a 6174 696f 6e20 6672 6571 7565 6e63  ization frequenc
-00012080: 7920 252e 3167 2069 6e64 6963 6174 6573  y %.1g indicates
-00012090: 206e 756d 6572 6963 2069 6e73 7461 6269   numeric instabi
-000120a0: 6c69 7479 2e5c 6e22 2c0a 2020 2020 2020  lity.\n",.      
-000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2074 6573 7429 3b0a 2020 2020 6c70 2d3e   test);.    lp->
-000120d0: 7370 785f 7374 6174 7573 203d 204e 554d  spx_status = NUM
-000120e0: 4641 494c 5552 453b 0a20 207d 0a0a 2020  FAILURE;.  }..  
-000120f0: 4652 4545 2875 7365 6470 6f73 293b 0a20  FREE(usedpos);. 
-00012100: 2072 6574 7572 6e28 284d 5942 4f4f 4c29   return((MYBOOL)
-00012110: 2028 7369 6e67 756c 6172 6974 6965 7320   (singularities 
-00012120: 3c3d 2030 2929 3b0a 7d20 2f2a 2069 6e76  <= 0));.} /* inv
-00012130: 6572 7420 2a2f 0a0a 0a53 5441 5449 4320  ert */...STATIC 
-00012140: 4d59 424f 4f4c 2066 696d 7072 6f76 6528  MYBOOL fimprove(
-00012150: 6c70 7265 6320 2a6c 702c 2052 4541 4c20  lprec *lp, REAL 
-00012160: 2a70 636f 6c2c 2069 6e74 202a 6e7a 6964  *pcol, int *nzid
-00012170: 782c 2052 4541 4c20 726f 756e 647a 6572  x, REAL roundzer
-00012180: 6f29 0a7b 0a20 2052 4541 4c20 2020 2a65  o).{.  REAL   *e
-00012190: 7272 6f72 732c 2073 6470 3b0a 2020 696e  rrors, sdp;.  in
-000121a0: 7420 2020 206a 3b0a 2020 4d59 424f 4f4c  t    j;.  MYBOOL
-000121b0: 204f 6b20 3d20 5452 5545 3b0a 0a20 2061   Ok = TRUE;..  a
-000121c0: 6c6c 6f63 5245 414c 286c 702c 2026 6572  llocREAL(lp, &er
-000121d0: 726f 7273 2c20 6c70 2d3e 726f 7773 202b  rors, lp->rows +
-000121e0: 2031 2c20 4641 4c53 4529 3b0a 2020 6966   1, FALSE);.  if
-000121f0: 2865 7272 6f72 7320 3d3d 204e 554c 4c29  (errors == NULL)
-00012200: 207b 0a20 2020 204f 6b20 3d20 4641 4c53   {.    Ok = FALS
-00012210: 453b 0a20 2020 2072 6574 7572 6e28 4f6b  E;.    return(Ok
-00012220: 293b 0a20 207d 0a20 204d 454d 434f 5059  );.  }.  MEMCOPY
-00012230: 2865 7272 6f72 732c 2070 636f 6c2c 206c  (errors, pcol, l
-00012240: 702d 3e72 6f77 7320 2b20 3129 3b0a 2020  p->rows + 1);.  
-00012250: 6c70 2d3e 6266 705f 6674 7261 6e5f 6e6f  lp->bfp_ftran_no
-00012260: 726d 616c 286c 702c 2070 636f 6c2c 206e  rmal(lp, pcol, n
-00012270: 7a69 6478 293b 0a20 2070 726f 645f 4178  zidx);.  prod_Ax
-00012280: 286c 702c 204e 554c 4c2c 2070 636f 6c2c  (lp, NULL, pcol,
-00012290: 204e 554c 4c2c 2030 2e30 2c20 2d31 2c0a   NULL, 0.0, -1,.
+00011580: 2020 2020 204b 4520 7570 6461 7465 2020       KE update  
+00011590: 2020 202d 2d20 4170 7269 6c20 3230 3035     -- April 2005
+000115a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115c0: 2020 2020 2020 4b45 2075 7064 6174 6520        KE update 
+000115d0: 2020 2020 2d2d 204a 756e 6520 3230 3035      -- June 2005
+000115e0: 0a0a 2a2f 0a0a 5354 4154 4943 204d 5942  ..*/..STATIC MYB
+000115f0: 4f4f 4c20 5f5f 5749 4e41 5049 2069 6e76  OOL __WINAPI inv
+00011600: 6572 7428 6c70 7265 6320 2a6c 702c 204d  ert(lprec *lp, M
+00011610: 5942 4f4f 4c20 7368 6966 7462 6f75 6e64  YBOOL shiftbound
+00011620: 732c 204d 5942 4f4f 4c20 6669 6e61 6c29  s, MYBOOL final)
+00011630: 0a7b 0a20 204d 5942 4f4f 4c20 2a75 7365  .{.  MYBOOL *use
+00011640: 6470 6f73 2c20 7265 7365 7462 6173 6973  dpos, resetbasis
+00011650: 3b0a 2020 5245 414c 2020 2074 6573 743b  ;.  REAL   test;
+00011660: 0a20 2069 6e74 2020 2020 6b2c 2069 2c20  .  int    k, i, 
+00011670: 6a3b 0a20 2069 6e74 2020 2020 7369 6e67  j;.  int    sing
+00011680: 756c 6172 6974 6965 732c 2075 7365 7263  ularities, userc
+00011690: 6f6c 423b 0a0a 202f 2a20 4d61 6b65 2073  olB;.. /* Make s
+000116a0: 7572 6520 7468 6520 7461 6773 2061 7265  ure the tags are
+000116b0: 2063 6f72 7265 6374 202a 2f0a 2020 6966   correct */.  if
+000116c0: 2821 6d61 745f 7661 6c69 6461 7465 286c  (!mat_validate(l
+000116d0: 702d 3e6d 6174 4129 2920 7b0a 2020 2020  p->matA)) {.    
+000116e0: 6c70 2d3e 7370 785f 7374 6174 7573 203d  lp->spx_status =
+000116f0: 2049 4e46 4541 5349 424c 453b 0a20 2020   INFEASIBLE;.   
+00011700: 2072 6574 7572 6e28 4641 4c53 4529 3b0a   return(FALSE);.
+00011710: 2020 7d0a 0a20 2f2a 2043 7265 6174 6520    }.. /* Create 
+00011720: 7468 6520 696e 7665 7273 6520 6d61 6e61  the inverse mana
+00011730: 6765 6d65 6e74 206f 626a 6563 7420 6174  gement object at
+00011740: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
+00011750: 746f 2069 6e76 6572 7428 2920 2a2f 0a20  to invert() */. 
+00011760: 2069 6628 6c70 2d3e 696e 7642 203d 3d20   if(lp->invB == 
+00011770: 4e55 4c4c 290a 2020 2020 6c70 2d3e 6266  NULL).    lp->bf
+00011780: 705f 696e 6974 286c 702c 206c 702d 3e72  p_init(lp, lp->r
+00011790: 6f77 732c 2030 2c20 4e55 4c4c 293b 0a20  ows, 0, NULL);. 
+000117a0: 2065 6c73 650a 2020 2020 6c70 2d3e 6266   else.    lp->bf
+000117b0: 705f 7072 6570 6172 6566 6163 746f 7269  p_preparefactori
+000117c0: 7a61 7469 6f6e 286c 7029 3b0a 2020 7369  zation(lp);.  si
+000117d0: 6e67 756c 6172 6974 6965 7320 3d20 303b  ngularities = 0;
+000117e0: 0a0a 202f 2a20 4d75 7374 2073 6176 6520  .. /* Must save 
+000117f0: 7370 785f 7374 6174 7573 2073 696e 6365  spx_status since
+00011800: 2069 7420 6973 2075 7365 6420 746f 2063   it is used to c
+00011810: 6172 7279 2069 6e66 6f72 6d61 7469 6f6e  arry information
+00011820: 2061 626f 7574 0a20 2020 2074 6865 2070   about.    the p
+00011830: 7265 7365 6e63 6520 616e 6420 6861 6e64  resence and hand
+00011840: 6c69 6e67 206f 6620 7369 6e67 756c 6172  ling of singular
+00011850: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+00011860: 6d61 7472 6978 202a 2f0a 2020 6966 2875  matrix */.  if(u
+00011870: 7365 7261 626f 7274 286c 702c 204d 5347  serabort(lp, MSG
+00011880: 5f49 4e56 4552 5429 290a 2020 2020 7265  _INVERT)).    re
+00011890: 7475 726e 2846 414c 5345 293b 0a0a 2369  turn(FALSE);..#i
+000118a0: 6664 6566 2050 6172 616e 6f69 610a 2020  fdef Paranoia.  
+000118b0: 6966 286c 702d 3e73 7078 5f74 7261 6365  if(lp->spx_trace
+000118c0: 290a 2020 2020 7265 706f 7274 286c 702c  ).    report(lp,
+000118d0: 2044 4554 4149 4c45 442c 2022 696e 7665   DETAILED, "inve
+000118e0: 7274 3a20 4974 6572 2025 3130 672c 2066  rt: Iter %10g, f
+000118f0: 6163 742d 6c65 6e67 7468 2025 3764 2c20  act-length %7d, 
+00011900: 4f46 2022 2052 4553 554c 5456 414c 5545  OF " RESULTVALUE
+00011910: 4d41 534b 2022 2e5c 6e22 2c0a 2020 2020  MASK ".\n",.    
+00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011930: 2020 2020 2028 646f 7562 6c65 2920 6765       (double) ge
+00011940: 745f 746f 7461 6c5f 6974 6572 286c 7029  t_total_iter(lp)
+00011950: 2c20 6c70 2d3e 6266 705f 636f 6c63 6f75  , lp->bfp_colcou
+00011960: 6e74 286c 7029 2c20 2864 6f75 626c 6529  nt(lp), (double)
+00011970: 202d 6c70 2d3e 7268 735b 305d 293b 0a23   -lp->rhs[0]);.#
+00011980: 656e 6469 660a 0a20 2f2a 2053 746f 7265  endif.. /* Store
+00011990: 2073 7461 7465 206f 6620 7072 652d 6578   state of pre-ex
+000119a0: 6973 7469 6e67 2062 6173 6973 2c20 616e  isting basis, an
+000119b0: 6420 6174 2074 6865 2073 616d 6520 7469  d at the same ti
+000119c0: 6d65 2063 6865 636b 2069 660a 2020 2020  me check if.    
+000119d0: 7468 6520 6261 7369 7320 6973 2049 3b20  the basis is I; 
+000119e0: 696e 2074 6869 7320 6361 7365 2074 616b  in this case tak
+000119f0: 6520 7468 6520 6561 7379 2077 6179 206f  e the easy way o
+00011a00: 7574 202a 2f0a 2020 6966 2821 616c 6c6f  ut */.  if(!allo
+00011a10: 634d 5942 4f4f 4c28 6c70 2c20 2675 7365  cMYBOOL(lp, &use
+00011a20: 6470 6f73 2c20 6c70 2d3e 7375 6d20 2b20  dpos, lp->sum + 
+00011a30: 312c 2054 5255 4529 2920 7b0a 2020 2020  1, TRUE)) {.    
+00011a40: 6c70 2d3e 6262 5f62 7265 616b 203d 2054  lp->bb_break = T
+00011a50: 5255 453b 0a20 2020 2072 6574 7572 6e28  RUE;.    return(
+00011a60: 4641 4c53 4529 3b0a 2020 7d0a 2020 7573  FALSE);.  }.  us
+00011a70: 6564 706f 735b 305d 203d 2054 5255 453b  edpos[0] = TRUE;
+00011a80: 0a20 2075 7365 7263 6f6c 4220 3d20 303b  .  usercolB = 0;
+00011a90: 0a20 2066 6f72 2869 203d 2031 3b20 6920  .  for(i = 1; i 
+00011aa0: 3c3d 206c 702d 3e72 6f77 733b 2069 2b2b  <= lp->rows; i++
+00011ab0: 2920 7b0a 2020 2020 6b20 3d20 6c70 2d3e  ) {.    k = lp->
+00011ac0: 7661 725f 6261 7369 635b 695d 3b0a 2020  var_basic[i];.  
+00011ad0: 2020 6966 286b 203e 206c 702d 3e72 6f77    if(k > lp->row
+00011ae0: 7329 0a20 2020 2020 2075 7365 7263 6f6c  s).      usercol
+00011af0: 422b 2b3b 0a20 2020 2075 7365 6470 6f73  B++;.    usedpos
+00011b00: 5b6b 5d20 3d20 5452 5545 3b0a 2020 7d0a  [k] = TRUE;.  }.
+00011b10: 2369 6664 6566 2050 6172 616e 6f69 610a  #ifdef Paranoia.
+00011b20: 2020 6966 2821 7665 7269 6679 5f62 6173    if(!verify_bas
+00011b30: 6973 286c 7029 290a 2020 2020 7265 706f  is(lp)).    repo
+00011b40: 7274 286c 702c 2053 4556 4552 452c 2022  rt(lp, SEVERE, "
+00011b50: 696e 7665 7274 3a20 496e 7661 6c69 6420  invert: Invalid 
+00011b60: 6261 7369 7320 6465 7465 6374 6564 2028  basis detected (
+00011b70: 6974 6572 2025 6729 2e5c 6e22 2c0a 2020  iter %g).\n",.  
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 2020 2020 2028 646f 7562 6c65 2920 6765       (double) ge
+00011ba0: 745f 746f 7461 6c5f 6974 6572 286c 7029  t_total_iter(lp)
+00011bb0: 293b 0a23 656e 6469 660a 0a20 2f2a 2054  );.#endif.. /* T
+00011bc0: 616c 6c79 206d 6174 7269 7820 6e7a 2d63  ally matrix nz-c
+00011bd0: 6f75 6e74 7320 616e 6420 6368 6563 6b20  ounts and check 
+00011be0: 6966 2077 6520 7368 6f75 6c64 2072 6573  if we should res
+00011bf0: 6574 2062 6173 6973 0a20 2020 2069 6e64  et basis.    ind
+00011c00: 6963 6174 6f72 7320 746f 2061 6c6c 2073  icators to all s
+00011c10: 6c61 636b 7320 2a2f 0a20 2072 6573 6574  lacks */.  reset
+00011c20: 6261 7369 7320 3d20 284d 5942 4f4f 4c29  basis = (MYBOOL)
+00011c30: 2028 2875 7365 7263 6f6c 4220 3e20 3029   ((usercolB > 0)
+00011c40: 2026 2620 6c70 2d3e 6266 705f 6361 6e72   && lp->bfp_canr
+00011c50: 6573 6574 6261 7369 7328 6c70 2929 3b0a  esetbasis(lp));.
+00011c60: 2020 6b20 3d20 303b 0a20 2066 6f72 2869    k = 0;.  for(i
+00011c70: 203d 2031 3b20 6920 3c3d 206c 702d 3e72   = 1; i <= lp->r
+00011c80: 6f77 733b 2069 2b2b 2920 7b0a 2020 2020  ows; i++) {.    
+00011c90: 6966 286c 702d 3e76 6172 5f62 6173 6963  if(lp->var_basic
+00011ca0: 5b69 5d20 3e20 6c70 2d3e 726f 7773 290a  [i] > lp->rows).
+00011cb0: 2020 2020 2020 6b20 2b3d 206d 6174 5f63        k += mat_c
+00011cc0: 6f6c 6c65 6e67 7468 286c 702d 3e6d 6174  ollength(lp->mat
+00011cd0: 412c 206c 702d 3e76 6172 5f62 6173 6963  A, lp->var_basic
+00011ce0: 5b69 5d20 2d20 6c70 2d3e 726f 7773 2920  [i] - lp->rows) 
+00011cf0: 2b20 2869 735f 4f46 5f6e 7a28 6c70 2c6c  + (is_OF_nz(lp,l
+00011d00: 702d 3e76 6172 5f62 6173 6963 5b69 5d20  p->var_basic[i] 
+00011d10: 2d20 6c70 2d3e 726f 7773 2920 3f20 3120  - lp->rows) ? 1 
+00011d20: 3a20 3029 3b0a 2020 2020 6966 2872 6573  : 0);.    if(res
+00011d30: 6574 6261 7369 7329 207b 0a20 2020 2020  etbasis) {.     
+00011d40: 206a 203d 206c 702d 3e76 6172 5f62 6173   j = lp->var_bas
+00011d50: 6963 5b69 5d3b 0a20 2020 2020 2069 6628  ic[i];.      if(
+00011d60: 6a20 3e20 6c70 2d3e 726f 7773 290a 2020  j > lp->rows).  
+00011d70: 2020 2020 2020 6c70 2d3e 6973 5f62 6173        lp->is_bas
+00011d80: 6963 5b6a 5d20 3d20 4641 4c53 453b 0a20  ic[j] = FALSE;. 
+00011d90: 2020 2020 206c 702d 3e76 6172 5f62 6173       lp->var_bas
+00011da0: 6963 5b69 5d20 3d20 693b 0a20 2020 2020  ic[i] = i;.     
+00011db0: 206c 702d 3e69 735f 6261 7369 635b 695d   lp->is_basic[i]
+00011dc0: 203d 2054 5255 453b 0a20 2020 207d 0a20   = TRUE;.    }. 
+00011dd0: 207d 0a0a 202f 2a20 4e6f 7720 646f 2074   }.. /* Now do t
+00011de0: 6865 2072 6566 6163 746f 7269 7a61 7469  he refactorizati
+00011df0: 6f6e 202a 2f0a 2020 7369 6e67 756c 6172  on */.  singular
+00011e00: 6974 6965 7320 3d20 6c70 2d3e 6266 705f  ities = lp->bfp_
+00011e10: 6661 6374 6f72 697a 6528 6c70 2c20 7573  factorize(lp, us
+00011e20: 6572 636f 6c42 2c20 6b2c 2075 7365 6470  ercolB, k, usedp
+00011e30: 6f73 2c20 6669 6e61 6c29 3b0a 0a20 2f2a  os, final);.. /*
+00011e40: 2044 6f20 7573 6572 2072 6570 6f72 7469   Do user reporti
+00011e50: 6e67 202a 2f0a 2020 6966 2875 7365 7261  ng */.  if(usera
+00011e60: 626f 7274 286c 702c 204d 5347 5f49 4e56  bort(lp, MSG_INV
+00011e70: 4552 5429 290a 2020 2020 676f 746f 2043  ERT)).    goto C
+00011e80: 6c65 616e 7570 3b0a 0a20 2f2a 2046 696e  leanup;.. /* Fin
+00011e90: 616c 697a 6520 6661 6374 6f72 697a 6174  alize factorizat
+00011ea0: 696f 6e2f 696e 7665 7273 696f 6e20 2a2f  ion/inversion */
+00011eb0: 0a20 206c 702d 3e62 6670 5f66 696e 6973  .  lp->bfp_finis
+00011ec0: 6866 6163 746f 7269 7a61 7469 6f6e 286c  hfactorization(l
+00011ed0: 7029 3b0a 0a20 202f 2a20 5265 636f 6d70  p);..  /* Recomp
+00011ee0: 7574 6520 7468 6520 5248 5320 2820 5265  ute the RHS ( Re
+00011ef0: 662e 206c 705f 736f 6c76 6520 696e 7665  f. lp_solve inve
+00011f00: 7273 6520 6c6f 6769 6320 616e 6420 4368  rse logic and Ch
+00011f10: 7661 7461 6c20 702e 2031 3231 2029 202a  vatal p. 121 ) *
+00011f20: 2f0a 2020 7265 636f 6d70 7574 655f 736f  /.  recompute_so
+00011f30: 6c75 7469 6f6e 286c 702c 2073 6869 6674  lution(lp, shift
+00011f40: 626f 756e 6473 293b 0a20 2072 6573 7461  bounds);.  resta
+00011f50: 7274 5072 6963 6572 286c 702c 2041 5554  rtPricer(lp, AUT
+00011f60: 4f4d 4154 4943 293b 0a0a 436c 6561 6e75  OMATIC);..Cleanu
+00011f70: 703a 0a20 202f 2a20 4368 6563 6b20 666f  p:.  /* Check fo
+00011f80: 7220 6e75 6d65 7269 6361 6c20 696e 7374  r numerical inst
+00011f90: 6162 696c 6974 7920 696e 6469 6361 7465  ability indicate
+00011fa0: 6420 6279 2066 7265 7175 656e 7420 7265  d by frequent re
+00011fb0: 6661 6374 6f72 697a 6174 696f 6e73 202a  factorizations *
+00011fc0: 2f0a 2020 7465 7374 203d 2067 6574 5f72  /.  test = get_r
+00011fd0: 6566 6163 7466 7265 7175 656e 6379 286c  efactfrequency(l
+00011fe0: 702c 2046 414c 5345 293b 0a20 2069 6628  p, FALSE);.  if(
+00011ff0: 7465 7374 203c 204d 494e 5f52 4546 4143  test < MIN_REFAC
+00012000: 5446 5245 5155 454e 4359 2920 7b0a 2020  TFREQUENCY) {.  
+00012010: 2020 7465 7374 203d 2067 6574 5f72 6566    test = get_ref
+00012020: 6163 7466 7265 7175 656e 6379 286c 702c  actfrequency(lp,
+00012030: 2054 5255 4529 3b0a 2020 2020 7265 706f   TRUE);.    repo
+00012040: 7274 286c 702c 204e 4f52 4d41 4c2c 2022  rt(lp, NORMAL, "
+00012050: 696e 7665 7274 3a20 5265 6661 6374 6f72  invert: Refactor
+00012060: 697a 6174 696f 6e20 6672 6571 7565 6e63  ization frequenc
+00012070: 7920 252e 3167 2069 6e64 6963 6174 6573  y %.1g indicates
+00012080: 206e 756d 6572 6963 2069 6e73 7461 6269   numeric instabi
+00012090: 6c69 7479 2e5c 6e22 2c0a 2020 2020 2020  lity.\n",.      
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 2074 6573 7429 3b0a 2020 2020 6c70 2d3e   test);.    lp->
+000120c0: 7370 785f 7374 6174 7573 203d 204e 554d  spx_status = NUM
+000120d0: 4641 494c 5552 453b 0a20 207d 0a0a 2020  FAILURE;.  }..  
+000120e0: 4652 4545 2875 7365 6470 6f73 293b 0a20  FREE(usedpos);. 
+000120f0: 2072 6574 7572 6e28 284d 5942 4f4f 4c29   return((MYBOOL)
+00012100: 2028 7369 6e67 756c 6172 6974 6965 7320   (singularities 
+00012110: 3c3d 2030 2929 3b0a 7d20 2f2a 2069 6e76  <= 0));.} /* inv
+00012120: 6572 7420 2a2f 0a0a 0a53 5441 5449 4320  ert */...STATIC 
+00012130: 4d59 424f 4f4c 2066 696d 7072 6f76 6528  MYBOOL fimprove(
+00012140: 6c70 7265 6320 2a6c 702c 2052 4541 4c20  lprec *lp, REAL 
+00012150: 2a70 636f 6c2c 2069 6e74 202a 6e7a 6964  *pcol, int *nzid
+00012160: 782c 2052 4541 4c20 726f 756e 647a 6572  x, REAL roundzer
+00012170: 6f29 0a7b 0a20 2052 4541 4c20 2020 2a65  o).{.  REAL   *e
+00012180: 7272 6f72 732c 2073 6470 3b0a 2020 696e  rrors, sdp;.  in
+00012190: 7420 2020 206a 3b0a 2020 4d59 424f 4f4c  t    j;.  MYBOOL
+000121a0: 204f 6b20 3d20 5452 5545 3b0a 0a20 2061   Ok = TRUE;..  a
+000121b0: 6c6c 6f63 5245 414c 286c 702c 2026 6572  llocREAL(lp, &er
+000121c0: 726f 7273 2c20 6c70 2d3e 726f 7773 202b  rors, lp->rows +
+000121d0: 2031 2c20 4641 4c53 4529 3b0a 2020 6966   1, FALSE);.  if
+000121e0: 2865 7272 6f72 7320 3d3d 204e 554c 4c29  (errors == NULL)
+000121f0: 207b 0a20 2020 204f 6b20 3d20 4641 4c53   {.    Ok = FALS
+00012200: 453b 0a20 2020 2072 6574 7572 6e28 4f6b  E;.    return(Ok
+00012210: 293b 0a20 207d 0a20 204d 454d 434f 5059  );.  }.  MEMCOPY
+00012220: 2865 7272 6f72 732c 2070 636f 6c2c 206c  (errors, pcol, l
+00012230: 702d 3e72 6f77 7320 2b20 3129 3b0a 2020  p->rows + 1);.  
+00012240: 6c70 2d3e 6266 705f 6674 7261 6e5f 6e6f  lp->bfp_ftran_no
+00012250: 726d 616c 286c 702c 2070 636f 6c2c 206e  rmal(lp, pcol, n
+00012260: 7a69 6478 293b 0a20 2070 726f 645f 4178  zidx);.  prod_Ax
+00012270: 286c 702c 204e 554c 4c2c 2070 636f 6c2c  (lp, NULL, pcol,
+00012280: 204e 554c 4c2c 2030 2e30 2c20 2d31 2c0a   NULL, 0.0, -1,.
+00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 6572 726f 7273 2c20 4e55 4c4c 2c20 4d41  errors, NULL, MA
-000122d0: 545f 524f 554e 4444 4546 4155 4c54 293b  T_ROUNDDEFAULT);
-000122e0: 0a20 206c 702d 3e62 6670 5f66 7472 616e  .  lp->bfp_ftran
-000122f0: 5f6e 6f72 6d61 6c28 6c70 2c20 6572 726f  _normal(lp, erro
-00012300: 7273 2c20 4e55 4c4c 293b 0a0a 2020 7364  rs, NULL);..  sd
-00012310: 7020 3d20 303b 0a20 2066 6f72 286a 203d  p = 0;.  for(j =
-00012320: 2031 3b20 6a20 3c3d 206c 702d 3e72 6f77   1; j <= lp->row
-00012330: 733b 206a 2b2b 290a 2020 2020 6966 2866  s; j++).    if(f
-00012340: 6162 7328 6572 726f 7273 5b6a 5d29 3e73  abs(errors[j])>s
-00012350: 6470 290a 2020 2020 2020 7364 7020 3d20  dp).      sdp = 
-00012360: 6661 6273 2865 7272 6f72 735b 6a5d 293b  fabs(errors[j]);
-00012370: 0a20 2069 6628 7364 7020 3e20 6c70 2d3e  .  if(sdp > lp->
-00012380: 6570 736d 6163 6869 6e65 2920 7b0a 2020  epsmachine) {.  
-00012390: 2020 7265 706f 7274 286c 702c 2044 4554    report(lp, DET
-000123a0: 4149 4c45 442c 2022 4974 6572 6174 6976  AILED, "Iterativ
-000123b0: 6520 4654 5241 4e20 636f 7272 6563 7469  e FTRAN correcti
-000123c0: 6f6e 206d 6574 7269 6320 2567 222c 2073  on metric %g", s
-000123d0: 6470 293b 0a20 2020 2066 6f72 286a 203d  dp);.    for(j =
-000123e0: 2031 3b20 6a20 3c3d 206c 702d 3e72 6f77   1; j <= lp->row
-000123f0: 733b 206a 2b2b 2920 7b0a 2020 2020 2020  s; j++) {.      
-00012400: 7063 6f6c 5b6a 5d20 2b3d 2065 7272 6f72  pcol[j] += error
-00012410: 735b 6a5d 3b0a 2020 2020 2020 6d79 5f72  s[j];.      my_r
-00012420: 6f75 6e64 7a65 726f 2870 636f 6c5b 6a5d  oundzero(pcol[j]
-00012430: 2c20 726f 756e 647a 6572 6f29 3b0a 2020  , roundzero);.  
-00012440: 2020 7d0a 2020 7d0a 2020 4652 4545 2865    }.  }.  FREE(e
-00012450: 7272 6f72 7329 3b0a 2020 7265 7475 726e  rrors);.  return
-00012460: 284f 6b29 3b0a 7d0a 0a53 5441 5449 4320  (Ok);.}..STATIC 
-00012470: 4d59 424f 4f4c 2062 696d 7072 6f76 6528  MYBOOL bimprove(
-00012480: 6c70 7265 6320 2a6c 702c 2052 4541 4c20  lprec *lp, REAL 
-00012490: 2a72 6873 7665 6374 6f72 2c20 696e 7420  *rhsvector, int 
-000124a0: 2a6e 7a69 6478 2c20 5245 414c 2072 6f75  *nzidx, REAL rou
-000124b0: 6e64 7a65 726f 290a 7b0a 2020 696e 7420  ndzero).{.  int 
-000124c0: 2020 206a 3b0a 2020 5245 414c 2020 202a     j;.  REAL   *
-000124d0: 6572 726f 7273 2c20 6572 722c 206d 6178  errors, err, max
-000124e0: 6572 723b 0a20 204d 5942 4f4f 4c20 4f6b  err;.  MYBOOL Ok
-000124f0: 203d 2054 5255 453b 0a0a 2020 616c 6c6f   = TRUE;..  allo
-00012500: 6352 4541 4c28 6c70 2c20 2665 7272 6f72  cREAL(lp, &error
-00012510: 732c 206c 702d 3e73 756d 202b 2031 2c20  s, lp->sum + 1, 
-00012520: 4641 4c53 4529 3b0a 2020 6966 2865 7272  FALSE);.  if(err
-00012530: 6f72 7320 3d3d 204e 554c 4c29 207b 0a20  ors == NULL) {. 
-00012540: 2020 204f 6b20 3d20 4641 4c53 453b 0a20     Ok = FALSE;. 
-00012550: 2020 2072 6574 7572 6e28 4f6b 293b 0a20     return(Ok);. 
-00012560: 207d 0a20 204d 454d 434f 5059 2865 7272   }.  MEMCOPY(err
-00012570: 6f72 732c 2072 6873 7665 6374 6f72 2c20  ors, rhsvector, 
-00012580: 6c70 2d3e 7375 6d20 2b20 3129 3b0a 0a20  lp->sum + 1);.. 
-00012590: 202f 2a20 536f 6c76 6520 4178 3d62 2066   /* Solve Ax=b f
-000125a0: 6f72 2078 2c20 636f 6d70 7574 6520 6220  or x, compute b 
-000125b0: 6261 636b 202a 2f0a 2020 6c70 2d3e 6266  back */.  lp->bf
-000125c0: 705f 6274 7261 6e5f 6e6f 726d 616c 286c  p_btran_normal(l
-000125d0: 702c 2065 7272 6f72 732c 206e 7a69 6478  p, errors, nzidx
-000125e0: 293b 0a20 2070 726f 645f 7841 286c 702c  );.  prod_xA(lp,
-000125f0: 204e 554c 4c2c 2065 7272 6f72 732c 204e   NULL, errors, N
-00012600: 554c 4c2c 2030 2e30 2c20 312e 302c 0a20  ULL, 0.0, 1.0,. 
+000122b0: 6572 726f 7273 2c20 4e55 4c4c 2c20 4d41  errors, NULL, MA
+000122c0: 545f 524f 554e 4444 4546 4155 4c54 293b  T_ROUNDDEFAULT);
+000122d0: 0a20 206c 702d 3e62 6670 5f66 7472 616e  .  lp->bfp_ftran
+000122e0: 5f6e 6f72 6d61 6c28 6c70 2c20 6572 726f  _normal(lp, erro
+000122f0: 7273 2c20 4e55 4c4c 293b 0a0a 2020 7364  rs, NULL);..  sd
+00012300: 7020 3d20 303b 0a20 2066 6f72 286a 203d  p = 0;.  for(j =
+00012310: 2031 3b20 6a20 3c3d 206c 702d 3e72 6f77   1; j <= lp->row
+00012320: 733b 206a 2b2b 290a 2020 2020 6966 2866  s; j++).    if(f
+00012330: 6162 7328 6572 726f 7273 5b6a 5d29 3e73  abs(errors[j])>s
+00012340: 6470 290a 2020 2020 2020 7364 7020 3d20  dp).      sdp = 
+00012350: 6661 6273 2865 7272 6f72 735b 6a5d 293b  fabs(errors[j]);
+00012360: 0a20 2069 6628 7364 7020 3e20 6c70 2d3e  .  if(sdp > lp->
+00012370: 6570 736d 6163 6869 6e65 2920 7b0a 2020  epsmachine) {.  
+00012380: 2020 7265 706f 7274 286c 702c 2044 4554    report(lp, DET
+00012390: 4149 4c45 442c 2022 4974 6572 6174 6976  AILED, "Iterativ
+000123a0: 6520 4654 5241 4e20 636f 7272 6563 7469  e FTRAN correcti
+000123b0: 6f6e 206d 6574 7269 6320 2567 222c 2073  on metric %g", s
+000123c0: 6470 293b 0a20 2020 2066 6f72 286a 203d  dp);.    for(j =
+000123d0: 2031 3b20 6a20 3c3d 206c 702d 3e72 6f77   1; j <= lp->row
+000123e0: 733b 206a 2b2b 2920 7b0a 2020 2020 2020  s; j++) {.      
+000123f0: 7063 6f6c 5b6a 5d20 2b3d 2065 7272 6f72  pcol[j] += error
+00012400: 735b 6a5d 3b0a 2020 2020 2020 6d79 5f72  s[j];.      my_r
+00012410: 6f75 6e64 7a65 726f 2870 636f 6c5b 6a5d  oundzero(pcol[j]
+00012420: 2c20 726f 756e 647a 6572 6f29 3b0a 2020  , roundzero);.  
+00012430: 2020 7d0a 2020 7d0a 2020 4652 4545 2865    }.  }.  FREE(e
+00012440: 7272 6f72 7329 3b0a 2020 7265 7475 726e  rrors);.  return
+00012450: 284f 6b29 3b0a 7d0a 0a53 5441 5449 4320  (Ok);.}..STATIC 
+00012460: 4d59 424f 4f4c 2062 696d 7072 6f76 6528  MYBOOL bimprove(
+00012470: 6c70 7265 6320 2a6c 702c 2052 4541 4c20  lprec *lp, REAL 
+00012480: 2a72 6873 7665 6374 6f72 2c20 696e 7420  *rhsvector, int 
+00012490: 2a6e 7a69 6478 2c20 5245 414c 2072 6f75  *nzidx, REAL rou
+000124a0: 6e64 7a65 726f 290a 7b0a 2020 696e 7420  ndzero).{.  int 
+000124b0: 2020 206a 3b0a 2020 5245 414c 2020 202a     j;.  REAL   *
+000124c0: 6572 726f 7273 2c20 6572 722c 206d 6178  errors, err, max
+000124d0: 6572 723b 0a20 204d 5942 4f4f 4c20 4f6b  err;.  MYBOOL Ok
+000124e0: 203d 2054 5255 453b 0a0a 2020 616c 6c6f   = TRUE;..  allo
+000124f0: 6352 4541 4c28 6c70 2c20 2665 7272 6f72  cREAL(lp, &error
+00012500: 732c 206c 702d 3e73 756d 202b 2031 2c20  s, lp->sum + 1, 
+00012510: 4641 4c53 4529 3b0a 2020 6966 2865 7272  FALSE);.  if(err
+00012520: 6f72 7320 3d3d 204e 554c 4c29 207b 0a20  ors == NULL) {. 
+00012530: 2020 204f 6b20 3d20 4641 4c53 453b 0a20     Ok = FALSE;. 
+00012540: 2020 2072 6574 7572 6e28 4f6b 293b 0a20     return(Ok);. 
+00012550: 207d 0a20 204d 454d 434f 5059 2865 7272   }.  MEMCOPY(err
+00012560: 6f72 732c 2072 6873 7665 6374 6f72 2c20  ors, rhsvector, 
+00012570: 6c70 2d3e 7375 6d20 2b20 3129 3b0a 0a20  lp->sum + 1);.. 
+00012580: 202f 2a20 536f 6c76 6520 4178 3d62 2066   /* Solve Ax=b f
+00012590: 6f72 2078 2c20 636f 6d70 7574 6520 6220  or x, compute b 
+000125a0: 6261 636b 202a 2f0a 2020 6c70 2d3e 6266  back */.  lp->bf
+000125b0: 705f 6274 7261 6e5f 6e6f 726d 616c 286c  p_btran_normal(l
+000125c0: 702c 2065 7272 6f72 732c 206e 7a69 6478  p, errors, nzidx
+000125d0: 293b 0a20 2070 726f 645f 7841 286c 702c  );.  prod_xA(lp,
+000125e0: 204e 554c 4c2c 2065 7272 6f72 732c 204e   NULL, errors, N
+000125f0: 554c 4c2c 2030 2e30 2c20 312e 302c 0a20  ULL, 0.0, 1.0,. 
+00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2065 7272 6f72 732c 204e 554c 4c2c 0a20   errors, NULL,. 
+00012620: 2065 7272 6f72 732c 204e 554c 4c2c 0a20   errors, NULL,. 
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012660: 204d 4154 5f52 4f55 4e44 4445 4641 554c   MAT_ROUNDDEFAUL
-00012670: 5429 3b0a 0a20 202f 2a20 5461 6b65 2064  T);..  /* Take d
-00012680: 6966 6665 7265 6e63 6520 7769 7468 2069  ifference with i
-00012690: 6e67 6f69 6e67 2076 616c 7565 732c 2077  ngoing values, w
-000126a0: 6869 6c65 2073 6869 6674 696e 6720 7468  hile shifting th
-000126b0: 6520 636f 6c75 6d6e 2076 616c 7565 730a  e column values.
-000126c0: 2020 2020 2074 6f20 7468 6520 726f 7773       to the rows
-000126d0: 2073 6563 7469 6f6e 2061 6e64 207a 6572   section and zer
-000126e0: 6f69 6e67 2074 6865 2063 6f6c 756d 6e73  oing the columns
-000126f0: 2061 6761 696e 202a 2f0a 2020 666f 7228   again */.  for(
-00012700: 6a20 3d20 313b 206a 203c 3d20 6c70 2d3e  j = 1; j <= lp->
-00012710: 726f 7773 3b20 6a2b 2b29 0a20 2020 2065  rows; j++).    e
-00012720: 7272 6f72 735b 6a5d 203d 2065 7272 6f72  rrors[j] = error
-00012730: 735b 6c70 2d3e 726f 7773 2b6c 702d 3e76  s[lp->rows+lp->v
-00012740: 6172 5f62 6173 6963 5b6a 5d5d 202d 2072  ar_basic[j]] - r
-00012750: 6873 7665 6374 6f72 5b6a 5d3b 0a20 2066  hsvector[j];.  f
-00012760: 6f72 286a 203d 206c 702d 3e72 6f77 733b  or(j = lp->rows;
-00012770: 206a 203c 3d20 6c70 2d3e 7375 6d3b 206a   j <= lp->sum; j
-00012780: 2b2b 290a 2020 2020 6572 726f 7273 5b6a  ++).    errors[j
-00012790: 5d20 3d20 303b 0a0a 2020 2f2a 2053 6f6c  ] = 0;..  /* Sol
-000127a0: 7665 2074 6865 2062 2065 7272 6f72 7320  ve the b errors 
-000127b0: 666f 7220 7468 6520 6974 6572 6174 6976  for the iterativ
-000127c0: 6520 7820 6164 6a75 7374 6d65 6e74 202a  e x adjustment *
-000127d0: 2f0a 2020 6c70 2d3e 6266 705f 6274 7261  /.  lp->bfp_btra
-000127e0: 6e5f 6e6f 726d 616c 286c 702c 2065 7272  n_normal(lp, err
-000127f0: 6f72 732c 204e 554c 4c29 3b0a 0a20 202f  ors, NULL);..  /
-00012800: 2a20 4765 6e65 7261 7465 2074 6865 2061  * Generate the a
-00012810: 646a 7573 746d 656e 7473 2061 6e64 2063  djustments and c
-00012820: 6f6d 7075 7465 2073 7461 7469 7374 6963  ompute statistic
-00012830: 202a 2f0a 2020 6d61 7865 7272 203d 2030   */.  maxerr = 0
-00012840: 3b0a 2020 666f 7228 6a20 3d20 313b 206a  ;.  for(j = 1; j
-00012850: 203c 3d20 6c70 2d3e 726f 7773 3b20 6a2b   <= lp->rows; j+
-00012860: 2b29 207b 0a20 2020 2069 6628 6c70 2d3e  +) {.    if(lp->
-00012870: 7661 725f 6261 7369 635b 6a5d 3c3d 6c70  var_basic[j]<=lp
-00012880: 2d3e 726f 7773 2920 636f 6e74 696e 7565  ->rows) continue
-00012890: 3b0a 2020 2020 6572 7220 3d20 6572 726f  ;.    err = erro
-000128a0: 7273 5b6c 702d 3e72 6f77 732b 6c70 2d3e  rs[lp->rows+lp->
-000128b0: 7661 725f 6261 7369 635b 6a5d 5d3b 0a20  var_basic[j]];. 
-000128c0: 2020 2069 6628 6661 6273 2865 7272 293e     if(fabs(err)>
-000128d0: 6d61 7865 7272 290a 2020 2020 2020 6d61  maxerr).      ma
-000128e0: 7865 7272 203d 2066 6162 7328 6572 7229  xerr = fabs(err)
-000128f0: 3b0a 2020 7d0a 2020 6966 286d 6178 6572  ;.  }.  if(maxer
-00012900: 7220 3e20 6c70 2d3e 6570 736d 6163 6869  r > lp->epsmachi
-00012910: 6e65 2920 7b0a 2020 2020 7265 706f 7274  ne) {.    report
-00012920: 286c 702c 2044 4554 4149 4c45 442c 2022  (lp, DETAILED, "
-00012930: 4974 6572 6174 6976 6520 4254 5241 4e20  Iterative BTRAN 
-00012940: 636f 7272 6563 7469 6f6e 206d 6574 7269  correction metri
-00012950: 6320 2567 222c 206d 6178 6572 7229 3b0a  c %g", maxerr);.
-00012960: 2020 2020 666f 7228 6a20 3d20 313b 206a      for(j = 1; j
-00012970: 203c 3d20 6c70 2d3e 726f 7773 3b20 6a2b   <= lp->rows; j+
-00012980: 2b29 207b 0a20 2020 2020 2069 6628 6c70  +) {.      if(lp
-00012990: 2d3e 7661 725f 6261 7369 635b 6a5d 3c3d  ->var_basic[j]<=
-000129a0: 6c70 2d3e 726f 7773 2920 636f 6e74 696e  lp->rows) contin
-000129b0: 7565 3b0a 2020 2020 2020 7268 7376 6563  ue;.      rhsvec
-000129c0: 746f 725b 6a5d 202b 3d20 6572 726f 7273  tor[j] += errors
-000129d0: 5b6c 702d 3e72 6f77 732b 6c70 2d3e 7661  [lp->rows+lp->va
-000129e0: 725f 6261 7369 635b 6a5d 5d3b 0a20 2020  r_basic[j]];.   
-000129f0: 2020 206d 795f 726f 756e 647a 6572 6f28     my_roundzero(
-00012a00: 7268 7376 6563 746f 725b 6a5d 2c20 726f  rhsvector[j], ro
-00012a10: 756e 647a 6572 6f29 3b0a 2020 2020 7d0a  undzero);.    }.
-00012a20: 2020 7d0a 2020 4652 4545 2865 7272 6f72    }.  FREE(error
-00012a30: 7329 3b0a 2020 7265 7475 726e 284f 6b29  s);.  return(Ok)
-00012a40: 3b0a 7d0a 0a53 5441 5449 4320 766f 6964  ;.}..STATIC void
-00012a50: 2066 7472 616e 286c 7072 6563 202a 6c70   ftran(lprec *lp
-00012a60: 2c20 5245 414c 202a 7268 7376 6563 746f  , REAL *rhsvecto
-00012a70: 722c 2069 6e74 202a 6e7a 6964 782c 2052  r, int *nzidx, R
-00012a80: 4541 4c20 726f 756e 647a 6572 6f29 0a7b  EAL roundzero).{
-00012a90: 0a23 6966 2030 0a20 2069 6628 6973 5f61  .#if 0.  if(is_a
-00012aa0: 6374 696f 6e28 6c70 2d3e 696d 7072 6f76  ction(lp->improv
-00012ab0: 652c 2049 4d50 524f 5645 5f53 4f4c 5554  e, IMPROVE_SOLUT
-00012ac0: 494f 4e29 2026 2620 6c70 2d3e 6266 705f  ION) && lp->bfp_
-00012ad0: 7069 766f 7463 6f75 6e74 286c 7029 290a  pivotcount(lp)).
-00012ae0: 2020 2020 6669 6d70 726f 7665 286c 702c      fimprove(lp,
-00012af0: 2072 6873 7665 6374 6f72 2c20 6e7a 6964   rhsvector, nzid
-00012b00: 782c 2072 6f75 6e64 7a65 726f 293b 0a20  x, roundzero);. 
-00012b10: 2065 6c73 650a 2365 6e64 6966 0a20 2020   else.#endif.   
-00012b20: 206c 702d 3e62 6670 5f66 7472 616e 5f6e   lp->bfp_ftran_n
-00012b30: 6f72 6d61 6c28 6c70 2c20 7268 7376 6563  ormal(lp, rhsvec
-00012b40: 746f 722c 206e 7a69 6478 293b 0a7d 0a0a  tor, nzidx);.}..
-00012b50: 5354 4154 4943 2076 6f69 6420 6274 7261  STATIC void btra
-00012b60: 6e28 6c70 7265 6320 2a6c 702c 2052 4541  n(lprec *lp, REA
-00012b70: 4c20 2a72 6873 7665 6374 6f72 2c20 696e  L *rhsvector, in
-00012b80: 7420 2a6e 7a69 6478 2c20 5245 414c 2072  t *nzidx, REAL r
-00012b90: 6f75 6e64 7a65 726f 290a 7b0a 2369 6620  oundzero).{.#if 
-00012ba0: 300a 2020 6966 2869 735f 6163 7469 6f6e  0.  if(is_action
-00012bb0: 286c 702d 3e69 6d70 726f 7665 2c20 494d  (lp->improve, IM
-00012bc0: 5052 4f56 455f 534f 4c55 5449 4f4e 2920  PROVE_SOLUTION) 
-00012bd0: 2626 206c 702d 3e62 6670 5f70 6976 6f74  && lp->bfp_pivot
-00012be0: 636f 756e 7428 6c70 2929 0a20 2020 2062  count(lp)).    b
-00012bf0: 696d 7072 6f76 6528 6c70 2c20 7268 7376  improve(lp, rhsv
-00012c00: 6563 746f 722c 206e 7a69 6478 2c20 726f  ector, nzidx, ro
-00012c10: 756e 647a 6572 6f29 3b0a 2020 656c 7365  undzero);.  else
-00012c20: 0a23 656e 6469 660a 2020 2020 6c70 2d3e  .#endif.    lp->
-00012c30: 6266 705f 6274 7261 6e5f 6e6f 726d 616c  bfp_btran_normal
-00012c40: 286c 702c 2072 6873 7665 6374 6f72 2c20  (lp, rhsvector, 
-00012c50: 6e7a 6964 7829 3b0a 7d0a 0a53 5441 5449  nzidx);.}..STATI
-00012c60: 4320 4d59 424f 4f4c 2066 736f 6c76 6528  C MYBOOL fsolve(
-00012c70: 6c70 7265 6320 2a6c 702c 2069 6e74 2076  lprec *lp, int v
-00012c80: 6172 696e 2c20 5245 414c 202a 7063 6f6c  arin, REAL *pcol
-00012c90: 2c20 696e 7420 2a6e 7a69 6478 2c20 5245  , int *nzidx, RE
-00012ca0: 414c 2072 6f75 6e64 7a65 726f 2c20 5245  AL roundzero, RE
-00012cb0: 414c 206f 6673 6361 6c61 722c 204d 5942  AL ofscalar, MYB
-00012cc0: 4f4f 4c20 7072 6570 6172 6575 7064 6174  OOL prepareupdat
-00012cd0: 6529 0a2f 2a20 5761 7320 7365 7470 6976  e)./* Was setpiv
-00012ce0: 636f 6c20 696e 2076 6572 7369 6f6e 7320  col in versions 
-00012cf0: 6561 726c 6965 7220 7468 616e 2034 2e30  earlier than 4.0
-00012d00: 2e31 2e38 202d 204b 4520 2a2f 0a7b 0a20  .1.8 - KE */.{. 
-00012d10: 204d 5942 4f4f 4c20 6f6b 203d 2054 5255   MYBOOL ok = TRU
-00012d20: 453b 0a0a 2020 6966 2876 6172 696e 203e  E;..  if(varin >
-00012d30: 2030 290a 2020 2020 6f62 7461 696e 5f63   0).    obtain_c
-00012d40: 6f6c 756d 6e28 6c70 2c20 7661 7269 6e2c  olumn(lp, varin,
-00012d50: 2070 636f 6c2c 206e 7a69 6478 2c20 4e55   pcol, nzidx, NU
-00012d60: 4c4c 293b 0a0a 202f 2a20 536f 6c76 652c  LL);.. /* Solve,
-00012d70: 2061 646a 7573 7465 6420 666f 7220 6f62   adjusted for ob
-00012d80: 6a65 6374 6976 6520 6675 6e63 7469 6f6e  jective function
-00012d90: 2073 6361 6c61 7220 2a2f 0a20 2070 636f   scalar */.  pco
-00012da0: 6c5b 305d 202a 3d20 6f66 7363 616c 6172  l[0] *= ofscalar
-00012db0: 3b0a 2020 6966 2870 7265 7061 7265 7570  ;.  if(prepareup
-00012dc0: 6461 7465 290a 2020 2020 6c70 2d3e 6266  date).    lp->bf
-00012dd0: 705f 6674 7261 6e5f 7072 6570 6172 6528  p_ftran_prepare(
-00012de0: 6c70 2c20 7063 6f6c 2c20 6e7a 6964 7829  lp, pcol, nzidx)
-00012df0: 3b0a 2020 656c 7365 0a20 2020 2066 7472  ;.  else.    ftr
-00012e00: 616e 286c 702c 2070 636f 6c2c 206e 7a69  an(lp, pcol, nzi
-00012e10: 6478 2c20 726f 756e 647a 6572 6f29 3b0a  dx, roundzero);.
-00012e20: 0a20 2072 6574 7572 6e28 6f6b 293b 0a0a  .  return(ok);..
-00012e30: 7d20 2f2a 2066 736f 6c76 6520 2a2f 0a0a  } /* fsolve */..
-00012e40: 0a53 5441 5449 4320 4d59 424f 4f4c 2062  .STATIC MYBOOL b
-00012e50: 736f 6c76 6528 6c70 7265 6320 2a6c 702c  solve(lprec *lp,
-00012e60: 2069 6e74 2072 6f77 5f6e 722c 2052 4541   int row_nr, REA
-00012e70: 4c20 2a72 6873 7665 6374 6f72 2c20 696e  L *rhsvector, in
-00012e80: 7420 2a6e 7a69 6478 2c20 5245 414c 2072  t *nzidx, REAL r
-00012e90: 6f75 6e64 7a65 726f 2c20 5245 414c 206f  oundzero, REAL o
-00012ea0: 6673 6361 6c61 7229 0a7b 0a20 204d 5942  fscalar).{.  MYB
-00012eb0: 4f4f 4c20 6f6b 203d 2054 5255 453b 0a0a  OOL ok = TRUE;..
-00012ec0: 2020 6966 2872 6f77 5f6e 7220 3e3d 2030    if(row_nr >= 0
-00012ed0: 2920 2f2a 204e 6f74 6520 7468 6174 2072  ) /* Note that r
-00012ee0: 6f77 5f6e 7220 3d3d 2030 2072 6574 7572  ow_nr == 0 retur
-00012ef0: 6e73 2074 6865 205b 312c 2030 2e2e 2e30  ns the [1, 0...0
-00012f00: 205d 2076 6563 746f 7220 2a2f 0a20 2020   ] vector */.   
-00012f10: 2072 6f77 5f6e 7220 3d20 6f62 7461 696e   row_nr = obtain
-00012f20: 5f63 6f6c 756d 6e28 6c70 2c20 726f 775f  _column(lp, row_
-00012f30: 6e72 2c20 7268 7376 6563 746f 722c 206e  nr, rhsvector, n
-00012f40: 7a69 6478 2c20 4e55 4c4c 293b 0a0a 2020  zidx, NULL);..  
-00012f50: 2f2a 2053 6f6c 7665 2c20 6164 6a75 7374  /* Solve, adjust
-00012f60: 6564 2066 6f72 206f 626a 6563 7469 7665  ed for objective
-00012f70: 2066 756e 6374 696f 6e20 7363 616c 6172   function scalar
-00012f80: 202a 2f0a 2020 7268 7376 6563 746f 725b   */.  rhsvector[
-00012f90: 305d 202a 3d20 6f66 7363 616c 6172 3b0a  0] *= ofscalar;.
-00012fa0: 2020 6274 7261 6e28 6c70 2c20 7268 7376    btran(lp, rhsv
-00012fb0: 6563 746f 722c 206e 7a69 6478 2c20 726f  ector, nzidx, ro
-00012fc0: 756e 647a 6572 6f29 3b0a 0a20 2072 6574  undzero);..  ret
-00012fd0: 7572 6e28 6f6b 293b 0a0a 7d20 2f2a 2062  urn(ok);..} /* b
-00012fe0: 736f 6c76 6520 2a2f 0a0a 0a2f 2a20 5665  solve */.../* Ve
-00012ff0: 6374 6f72 2063 6f6d 7072 6573 7369 6f6e  ctor compression
-00013000: 2061 6e64 2065 7870 616e 7369 6f6e 2072   and expansion r
-00013010: 6f75 7469 6e65 7320 2a2f 0a53 5441 5449  outines */.STATI
-00013020: 4320 4d59 424f 4f4c 2076 6563 5f63 6f6d  C MYBOOL vec_com
-00013030: 7072 6573 7328 5245 414c 202a 6465 6e73  press(REAL *dens
-00013040: 6576 6563 746f 722c 2069 6e74 2073 7461  evector, int sta
-00013050: 7274 706f 732c 2069 6e74 2065 6e64 706f  rtpos, int endpo
-00013060: 732c 2052 4541 4c20 6570 7369 6c6f 6e2c  s, REAL epsilon,
-00013070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013080: 2020 2020 2020 2020 2020 2020 5245 414c              REAL
-00013090: 202a 6e7a 7665 6374 6f72 2c20 696e 7420   *nzvector, int 
-000130a0: 2a6e 7a69 6e64 6578 290a 7b0a 2020 696e  *nzindex).{.  in
-000130b0: 7420 6e3b 0a0a 2020 6966 2828 6465 6e73  t n;..  if((dens
-000130c0: 6576 6563 746f 7220 3d3d 204e 554c 4c29  evector == NULL)
-000130d0: 207c 7c20 286e 7a69 6e64 6578 203d 3d20   || (nzindex == 
-000130e0: 4e55 4c4c 2920 7c7c 2028 7374 6172 7470  NULL) || (startp
-000130f0: 6f73 203e 2065 6e64 706f 7329 290a 2020  os > endpos)).  
-00013100: 2020 7265 7475 726e 2820 4641 4c53 4520    return( FALSE 
-00013110: 293b 0a0a 2020 6e20 3d20 303b 0a20 2064  );..  n = 0;.  d
-00013120: 656e 7365 7665 6374 6f72 202b 3d20 7374  ensevector += st
-00013130: 6172 7470 6f73 3b0a 2020 7768 696c 6528  artpos;.  while(
-00013140: 7374 6172 7470 6f73 203c 3d20 656e 6470  startpos <= endp
-00013150: 6f73 2920 7b0a 2020 2020 6966 2866 6162  os) {.    if(fab
-00013160: 7328 2a64 656e 7365 7665 6374 6f72 2920  s(*densevector) 
-00013170: 3e20 6570 7369 6c6f 6e29 207b 2020 2f2a  > epsilon) {  /*
-00013180: 2041 7070 6c79 207a 6572 6f2d 7468 7265   Apply zero-thre
-00013190: 7368 6f6c 6420 2a2f 0a20 2020 2020 2069  shold */.      i
-000131a0: 6628 6e7a 7665 6374 6f72 2021 3d20 4e55  f(nzvector != NU
-000131b0: 4c4c 2920 2020 2020 2020 2020 2020 2020  LL)             
-000131c0: 2020 2020 2020 2020 2020 2f2a 204f 6e6c            /* Onl
-000131d0: 7920 7072 6f64 7563 6520 696e 6465 7820  y produce index 
-000131e0: 6966 206e 6f20 6e7a 7665 6374 6f72 2069  if no nzvector i
-000131f0: 7320 6769 7665 6e20 2a2f 0a20 2020 2020  s given */.     
-00013200: 2020 206e 7a76 6563 746f 725b 6e5d 203d     nzvector[n] =
-00013210: 202a 6465 6e73 6576 6563 746f 723b 0a20   *densevector;. 
-00013220: 2020 2020 206e 2b2b 3b0a 2020 2020 2020       n++;.      
-00013230: 6e7a 696e 6465 785b 6e5d 203d 2073 7461  nzindex[n] = sta
-00013240: 7274 706f 733b 0a20 2020 207d 0a20 2020  rtpos;.    }.   
-00013250: 2073 7461 7274 706f 732b 2b3b 0a20 2020   startpos++;.   
-00013260: 2064 656e 7365 7665 6374 6f72 2b2b 3b0a   densevector++;.
-00013270: 2020 7d0a 2020 6e7a 696e 6465 785b 305d    }.  nzindex[0]
-00013280: 203d 206e 3b0a 2020 7265 7475 726e 2820   = n;.  return( 
-00013290: 5452 5545 2029 3b0a 7d0a 0a53 5441 5449  TRUE );.}..STATI
-000132a0: 4320 4d59 424f 4f4c 2076 6563 5f65 7870  C MYBOOL vec_exp
-000132b0: 616e 6428 5245 414c 202a 6e7a 7665 6374  and(REAL *nzvect
-000132c0: 6f72 2c20 696e 7420 2a6e 7a69 6e64 6578  or, int *nzindex
-000132d0: 2c20 5245 414c 202a 6465 6e73 6576 6563  , REAL *densevec
-000132e0: 746f 722c 2069 6e74 2073 7461 7274 706f  tor, int startpo
-000132f0: 732c 2069 6e74 2065 6e64 706f 7329 0a7b  s, int endpos).{
-00013300: 0a20 2069 6e74 2069 2c20 6e3b 0a0a 2020  .  int i, n;..  
-00013310: 6e20 3d20 6e7a 696e 6465 785b 305d 3b0a  n = nzindex[0];.
-00013320: 2020 6920 3d20 6e7a 696e 6465 785b 6e5d    i = nzindex[n]
-00013330: 3b0a 2020 6465 6e73 6576 6563 746f 7220  ;.  densevector 
-00013340: 2b3d 2065 6e64 706f 733b 0a20 2077 6869  += endpos;.  whi
-00013350: 6c65 2865 6e64 706f 7320 3e3d 2073 7461  le(endpos >= sta
-00013360: 7274 706f 7329 207b 2020 2020 2020 2020  rtpos) {        
-00013370: 2020 2020 2020 2020 2020 2020 202f 2a20               /* 
-00013380: 4c6f 6f70 2066 726f 6d20 6265 6869 6e64  Loop from behind
-00013390: 2074 6f20 616c 6c6f 7720 6465 6e73 6576   to allow densev
-000133a0: 6563 746f 7220 3d3d 206e 7a76 6563 746f  ector == nzvecto
-000133b0: 7220 2a2f 0a20 2020 2069 6628 656e 6470  r */.    if(endp
-000133c0: 6f73 203d 3d20 6929 207b 0a20 2020 2020  os == i) {.     
-000133d0: 206e 2d2d 3b0a 2020 2020 2020 2a64 656e   n--;.      *den
-000133e0: 7365 7665 6374 6f72 203d 206e 7a76 6563  sevector = nzvec
-000133f0: 746f 725b 6e5d 3b0a 2020 2020 2020 6920  tor[n];.      i 
-00013400: 3d20 6e7a 696e 6465 785b 6e5d 3b0a 2020  = nzindex[n];.  
-00013410: 2020 7d0a 2020 2020 656c 7365 0a20 2020    }.    else.   
-00013420: 2020 202a 6465 6e73 6576 6563 746f 7220     *densevector 
-00013430: 3d20 303b 0a20 2020 2065 6e64 706f 732d  = 0;.    endpos-
-00013440: 2d3b 0a20 2020 2064 656e 7365 7665 6374  -;.    densevect
-00013450: 6f72 2d2d 3b0a 2020 7d0a 2020 7265 7475  or--;.  }.  retu
-00013460: 726e 2820 5452 5545 2029 3b0a 7d0a 0a0a  rn( TRUE );.}...
-00013470: 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /* -------------
+00012650: 204d 4154 5f52 4f55 4e44 4445 4641 554c   MAT_ROUNDDEFAUL
+00012660: 5429 3b0a 0a20 202f 2a20 5461 6b65 2064  T);..  /* Take d
+00012670: 6966 6665 7265 6e63 6520 7769 7468 2069  ifference with i
+00012680: 6e67 6f69 6e67 2076 616c 7565 732c 2077  ngoing values, w
+00012690: 6869 6c65 2073 6869 6674 696e 6720 7468  hile shifting th
+000126a0: 6520 636f 6c75 6d6e 2076 616c 7565 730a  e column values.
+000126b0: 2020 2020 2074 6f20 7468 6520 726f 7773       to the rows
+000126c0: 2073 6563 7469 6f6e 2061 6e64 207a 6572   section and zer
+000126d0: 6f69 6e67 2074 6865 2063 6f6c 756d 6e73  oing the columns
+000126e0: 2061 6761 696e 202a 2f0a 2020 666f 7228   again */.  for(
+000126f0: 6a20 3d20 313b 206a 203c 3d20 6c70 2d3e  j = 1; j <= lp->
+00012700: 726f 7773 3b20 6a2b 2b29 0a20 2020 2065  rows; j++).    e
+00012710: 7272 6f72 735b 6a5d 203d 2065 7272 6f72  rrors[j] = error
+00012720: 735b 6c70 2d3e 726f 7773 2b6c 702d 3e76  s[lp->rows+lp->v
+00012730: 6172 5f62 6173 6963 5b6a 5d5d 202d 2072  ar_basic[j]] - r
+00012740: 6873 7665 6374 6f72 5b6a 5d3b 0a20 2066  hsvector[j];.  f
+00012750: 6f72 286a 203d 206c 702d 3e72 6f77 733b  or(j = lp->rows;
+00012760: 206a 203c 3d20 6c70 2d3e 7375 6d3b 206a   j <= lp->sum; j
+00012770: 2b2b 290a 2020 2020 6572 726f 7273 5b6a  ++).    errors[j
+00012780: 5d20 3d20 303b 0a0a 2020 2f2a 2053 6f6c  ] = 0;..  /* Sol
+00012790: 7665 2074 6865 2062 2065 7272 6f72 7320  ve the b errors 
+000127a0: 666f 7220 7468 6520 6974 6572 6174 6976  for the iterativ
+000127b0: 6520 7820 6164 6a75 7374 6d65 6e74 202a  e x adjustment *
+000127c0: 2f0a 2020 6c70 2d3e 6266 705f 6274 7261  /.  lp->bfp_btra
+000127d0: 6e5f 6e6f 726d 616c 286c 702c 2065 7272  n_normal(lp, err
+000127e0: 6f72 732c 204e 554c 4c29 3b0a 0a20 202f  ors, NULL);..  /
+000127f0: 2a20 4765 6e65 7261 7465 2074 6865 2061  * Generate the a
+00012800: 646a 7573 746d 656e 7473 2061 6e64 2063  djustments and c
+00012810: 6f6d 7075 7465 2073 7461 7469 7374 6963  ompute statistic
+00012820: 202a 2f0a 2020 6d61 7865 7272 203d 2030   */.  maxerr = 0
+00012830: 3b0a 2020 666f 7228 6a20 3d20 313b 206a  ;.  for(j = 1; j
+00012840: 203c 3d20 6c70 2d3e 726f 7773 3b20 6a2b   <= lp->rows; j+
+00012850: 2b29 207b 0a20 2020 2069 6628 6c70 2d3e  +) {.    if(lp->
+00012860: 7661 725f 6261 7369 635b 6a5d 3c3d 6c70  var_basic[j]<=lp
+00012870: 2d3e 726f 7773 2920 636f 6e74 696e 7565  ->rows) continue
+00012880: 3b0a 2020 2020 6572 7220 3d20 6572 726f  ;.    err = erro
+00012890: 7273 5b6c 702d 3e72 6f77 732b 6c70 2d3e  rs[lp->rows+lp->
+000128a0: 7661 725f 6261 7369 635b 6a5d 5d3b 0a20  var_basic[j]];. 
+000128b0: 2020 2069 6628 6661 6273 2865 7272 293e     if(fabs(err)>
+000128c0: 6d61 7865 7272 290a 2020 2020 2020 6d61  maxerr).      ma
+000128d0: 7865 7272 203d 2066 6162 7328 6572 7229  xerr = fabs(err)
+000128e0: 3b0a 2020 7d0a 2020 6966 286d 6178 6572  ;.  }.  if(maxer
+000128f0: 7220 3e20 6c70 2d3e 6570 736d 6163 6869  r > lp->epsmachi
+00012900: 6e65 2920 7b0a 2020 2020 7265 706f 7274  ne) {.    report
+00012910: 286c 702c 2044 4554 4149 4c45 442c 2022  (lp, DETAILED, "
+00012920: 4974 6572 6174 6976 6520 4254 5241 4e20  Iterative BTRAN 
+00012930: 636f 7272 6563 7469 6f6e 206d 6574 7269  correction metri
+00012940: 6320 2567 222c 206d 6178 6572 7229 3b0a  c %g", maxerr);.
+00012950: 2020 2020 666f 7228 6a20 3d20 313b 206a      for(j = 1; j
+00012960: 203c 3d20 6c70 2d3e 726f 7773 3b20 6a2b   <= lp->rows; j+
+00012970: 2b29 207b 0a20 2020 2020 2069 6628 6c70  +) {.      if(lp
+00012980: 2d3e 7661 725f 6261 7369 635b 6a5d 3c3d  ->var_basic[j]<=
+00012990: 6c70 2d3e 726f 7773 2920 636f 6e74 696e  lp->rows) contin
+000129a0: 7565 3b0a 2020 2020 2020 7268 7376 6563  ue;.      rhsvec
+000129b0: 746f 725b 6a5d 202b 3d20 6572 726f 7273  tor[j] += errors
+000129c0: 5b6c 702d 3e72 6f77 732b 6c70 2d3e 7661  [lp->rows+lp->va
+000129d0: 725f 6261 7369 635b 6a5d 5d3b 0a20 2020  r_basic[j]];.   
+000129e0: 2020 206d 795f 726f 756e 647a 6572 6f28     my_roundzero(
+000129f0: 7268 7376 6563 746f 725b 6a5d 2c20 726f  rhsvector[j], ro
+00012a00: 756e 647a 6572 6f29 3b0a 2020 2020 7d0a  undzero);.    }.
+00012a10: 2020 7d0a 2020 4652 4545 2865 7272 6f72    }.  FREE(error
+00012a20: 7329 3b0a 2020 7265 7475 726e 284f 6b29  s);.  return(Ok)
+00012a30: 3b0a 7d0a 0a53 5441 5449 4320 766f 6964  ;.}..STATIC void
+00012a40: 2066 7472 616e 286c 7072 6563 202a 6c70   ftran(lprec *lp
+00012a50: 2c20 5245 414c 202a 7268 7376 6563 746f  , REAL *rhsvecto
+00012a60: 722c 2069 6e74 202a 6e7a 6964 782c 2052  r, int *nzidx, R
+00012a70: 4541 4c20 726f 756e 647a 6572 6f29 0a7b  EAL roundzero).{
+00012a80: 0a23 6966 2030 0a20 2069 6628 6973 5f61  .#if 0.  if(is_a
+00012a90: 6374 696f 6e28 6c70 2d3e 696d 7072 6f76  ction(lp->improv
+00012aa0: 652c 2049 4d50 524f 5645 5f53 4f4c 5554  e, IMPROVE_SOLUT
+00012ab0: 494f 4e29 2026 2620 6c70 2d3e 6266 705f  ION) && lp->bfp_
+00012ac0: 7069 766f 7463 6f75 6e74 286c 7029 290a  pivotcount(lp)).
+00012ad0: 2020 2020 6669 6d70 726f 7665 286c 702c      fimprove(lp,
+00012ae0: 2072 6873 7665 6374 6f72 2c20 6e7a 6964   rhsvector, nzid
+00012af0: 782c 2072 6f75 6e64 7a65 726f 293b 0a20  x, roundzero);. 
+00012b00: 2065 6c73 650a 2365 6e64 6966 0a20 2020   else.#endif.   
+00012b10: 206c 702d 3e62 6670 5f66 7472 616e 5f6e   lp->bfp_ftran_n
+00012b20: 6f72 6d61 6c28 6c70 2c20 7268 7376 6563  ormal(lp, rhsvec
+00012b30: 746f 722c 206e 7a69 6478 293b 0a7d 0a0a  tor, nzidx);.}..
+00012b40: 5354 4154 4943 2076 6f69 6420 6274 7261  STATIC void btra
+00012b50: 6e28 6c70 7265 6320 2a6c 702c 2052 4541  n(lprec *lp, REA
+00012b60: 4c20 2a72 6873 7665 6374 6f72 2c20 696e  L *rhsvector, in
+00012b70: 7420 2a6e 7a69 6478 2c20 5245 414c 2072  t *nzidx, REAL r
+00012b80: 6f75 6e64 7a65 726f 290a 7b0a 2369 6620  oundzero).{.#if 
+00012b90: 300a 2020 6966 2869 735f 6163 7469 6f6e  0.  if(is_action
+00012ba0: 286c 702d 3e69 6d70 726f 7665 2c20 494d  (lp->improve, IM
+00012bb0: 5052 4f56 455f 534f 4c55 5449 4f4e 2920  PROVE_SOLUTION) 
+00012bc0: 2626 206c 702d 3e62 6670 5f70 6976 6f74  && lp->bfp_pivot
+00012bd0: 636f 756e 7428 6c70 2929 0a20 2020 2062  count(lp)).    b
+00012be0: 696d 7072 6f76 6528 6c70 2c20 7268 7376  improve(lp, rhsv
+00012bf0: 6563 746f 722c 206e 7a69 6478 2c20 726f  ector, nzidx, ro
+00012c00: 756e 647a 6572 6f29 3b0a 2020 656c 7365  undzero);.  else
+00012c10: 0a23 656e 6469 660a 2020 2020 6c70 2d3e  .#endif.    lp->
+00012c20: 6266 705f 6274 7261 6e5f 6e6f 726d 616c  bfp_btran_normal
+00012c30: 286c 702c 2072 6873 7665 6374 6f72 2c20  (lp, rhsvector, 
+00012c40: 6e7a 6964 7829 3b0a 7d0a 0a53 5441 5449  nzidx);.}..STATI
+00012c50: 4320 4d59 424f 4f4c 2066 736f 6c76 6528  C MYBOOL fsolve(
+00012c60: 6c70 7265 6320 2a6c 702c 2069 6e74 2076  lprec *lp, int v
+00012c70: 6172 696e 2c20 5245 414c 202a 7063 6f6c  arin, REAL *pcol
+00012c80: 2c20 696e 7420 2a6e 7a69 6478 2c20 5245  , int *nzidx, RE
+00012c90: 414c 2072 6f75 6e64 7a65 726f 2c20 5245  AL roundzero, RE
+00012ca0: 414c 206f 6673 6361 6c61 722c 204d 5942  AL ofscalar, MYB
+00012cb0: 4f4f 4c20 7072 6570 6172 6575 7064 6174  OOL prepareupdat
+00012cc0: 6529 0a2f 2a20 5761 7320 7365 7470 6976  e)./* Was setpiv
+00012cd0: 636f 6c20 696e 2076 6572 7369 6f6e 7320  col in versions 
+00012ce0: 6561 726c 6965 7220 7468 616e 2034 2e30  earlier than 4.0
+00012cf0: 2e31 2e38 202d 204b 4520 2a2f 0a7b 0a20  .1.8 - KE */.{. 
+00012d00: 204d 5942 4f4f 4c20 6f6b 203d 2054 5255   MYBOOL ok = TRU
+00012d10: 453b 0a0a 2020 6966 2876 6172 696e 203e  E;..  if(varin >
+00012d20: 2030 290a 2020 2020 6f62 7461 696e 5f63   0).    obtain_c
+00012d30: 6f6c 756d 6e28 6c70 2c20 7661 7269 6e2c  olumn(lp, varin,
+00012d40: 2070 636f 6c2c 206e 7a69 6478 2c20 4e55   pcol, nzidx, NU
+00012d50: 4c4c 293b 0a0a 202f 2a20 536f 6c76 652c  LL);.. /* Solve,
+00012d60: 2061 646a 7573 7465 6420 666f 7220 6f62   adjusted for ob
+00012d70: 6a65 6374 6976 6520 6675 6e63 7469 6f6e  jective function
+00012d80: 2073 6361 6c61 7220 2a2f 0a20 2070 636f   scalar */.  pco
+00012d90: 6c5b 305d 202a 3d20 6f66 7363 616c 6172  l[0] *= ofscalar
+00012da0: 3b0a 2020 6966 2870 7265 7061 7265 7570  ;.  if(prepareup
+00012db0: 6461 7465 290a 2020 2020 6c70 2d3e 6266  date).    lp->bf
+00012dc0: 705f 6674 7261 6e5f 7072 6570 6172 6528  p_ftran_prepare(
+00012dd0: 6c70 2c20 7063 6f6c 2c20 6e7a 6964 7829  lp, pcol, nzidx)
+00012de0: 3b0a 2020 656c 7365 0a20 2020 2066 7472  ;.  else.    ftr
+00012df0: 616e 286c 702c 2070 636f 6c2c 206e 7a69  an(lp, pcol, nzi
+00012e00: 6478 2c20 726f 756e 647a 6572 6f29 3b0a  dx, roundzero);.
+00012e10: 0a20 2072 6574 7572 6e28 6f6b 293b 0a0a  .  return(ok);..
+00012e20: 7d20 2f2a 2066 736f 6c76 6520 2a2f 0a0a  } /* fsolve */..
+00012e30: 0a53 5441 5449 4320 4d59 424f 4f4c 2062  .STATIC MYBOOL b
+00012e40: 736f 6c76 6528 6c70 7265 6320 2a6c 702c  solve(lprec *lp,
+00012e50: 2069 6e74 2072 6f77 5f6e 722c 2052 4541   int row_nr, REA
+00012e60: 4c20 2a72 6873 7665 6374 6f72 2c20 696e  L *rhsvector, in
+00012e70: 7420 2a6e 7a69 6478 2c20 5245 414c 2072  t *nzidx, REAL r
+00012e80: 6f75 6e64 7a65 726f 2c20 5245 414c 206f  oundzero, REAL o
+00012e90: 6673 6361 6c61 7229 0a7b 0a20 204d 5942  fscalar).{.  MYB
+00012ea0: 4f4f 4c20 6f6b 203d 2054 5255 453b 0a0a  OOL ok = TRUE;..
+00012eb0: 2020 6966 2872 6f77 5f6e 7220 3e3d 2030    if(row_nr >= 0
+00012ec0: 2920 2f2a 204e 6f74 6520 7468 6174 2072  ) /* Note that r
+00012ed0: 6f77 5f6e 7220 3d3d 2030 2072 6574 7572  ow_nr == 0 retur
+00012ee0: 6e73 2074 6865 205b 312c 2030 2e2e 2e30  ns the [1, 0...0
+00012ef0: 205d 2076 6563 746f 7220 2a2f 0a20 2020   ] vector */.   
+00012f00: 2072 6f77 5f6e 7220 3d20 6f62 7461 696e   row_nr = obtain
+00012f10: 5f63 6f6c 756d 6e28 6c70 2c20 726f 775f  _column(lp, row_
+00012f20: 6e72 2c20 7268 7376 6563 746f 722c 206e  nr, rhsvector, n
+00012f30: 7a69 6478 2c20 4e55 4c4c 293b 0a0a 2020  zidx, NULL);..  
+00012f40: 2f2a 2053 6f6c 7665 2c20 6164 6a75 7374  /* Solve, adjust
+00012f50: 6564 2066 6f72 206f 626a 6563 7469 7665  ed for objective
+00012f60: 2066 756e 6374 696f 6e20 7363 616c 6172   function scalar
+00012f70: 202a 2f0a 2020 7268 7376 6563 746f 725b   */.  rhsvector[
+00012f80: 305d 202a 3d20 6f66 7363 616c 6172 3b0a  0] *= ofscalar;.
+00012f90: 2020 6274 7261 6e28 6c70 2c20 7268 7376    btran(lp, rhsv
+00012fa0: 6563 746f 722c 206e 7a69 6478 2c20 726f  ector, nzidx, ro
+00012fb0: 756e 647a 6572 6f29 3b0a 0a20 2072 6574  undzero);..  ret
+00012fc0: 7572 6e28 6f6b 293b 0a0a 7d20 2f2a 2062  urn(ok);..} /* b
+00012fd0: 736f 6c76 6520 2a2f 0a0a 0a2f 2a20 5665  solve */.../* Ve
+00012fe0: 6374 6f72 2063 6f6d 7072 6573 7369 6f6e  ctor compression
+00012ff0: 2061 6e64 2065 7870 616e 7369 6f6e 2072   and expansion r
+00013000: 6f75 7469 6e65 7320 2a2f 0a53 5441 5449  outines */.STATI
+00013010: 4320 4d59 424f 4f4c 2076 6563 5f63 6f6d  C MYBOOL vec_com
+00013020: 7072 6573 7328 5245 414c 202a 6465 6e73  press(REAL *dens
+00013030: 6576 6563 746f 722c 2069 6e74 2073 7461  evector, int sta
+00013040: 7274 706f 732c 2069 6e74 2065 6e64 706f  rtpos, int endpo
+00013050: 732c 2052 4541 4c20 6570 7369 6c6f 6e2c  s, REAL epsilon,
+00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013070: 2020 2020 2020 2020 2020 2020 5245 414c              REAL
+00013080: 202a 6e7a 7665 6374 6f72 2c20 696e 7420   *nzvector, int 
+00013090: 2a6e 7a69 6e64 6578 290a 7b0a 2020 696e  *nzindex).{.  in
+000130a0: 7420 6e3b 0a0a 2020 6966 2828 6465 6e73  t n;..  if((dens
+000130b0: 6576 6563 746f 7220 3d3d 204e 554c 4c29  evector == NULL)
+000130c0: 207c 7c20 286e 7a69 6e64 6578 203d 3d20   || (nzindex == 
+000130d0: 4e55 4c4c 2920 7c7c 2028 7374 6172 7470  NULL) || (startp
+000130e0: 6f73 203e 2065 6e64 706f 7329 290a 2020  os > endpos)).  
+000130f0: 2020 7265 7475 726e 2820 4641 4c53 4520    return( FALSE 
+00013100: 293b 0a0a 2020 6e20 3d20 303b 0a20 2064  );..  n = 0;.  d
+00013110: 656e 7365 7665 6374 6f72 202b 3d20 7374  ensevector += st
+00013120: 6172 7470 6f73 3b0a 2020 7768 696c 6528  artpos;.  while(
+00013130: 7374 6172 7470 6f73 203c 3d20 656e 6470  startpos <= endp
+00013140: 6f73 2920 7b0a 2020 2020 6966 2866 6162  os) {.    if(fab
+00013150: 7328 2a64 656e 7365 7665 6374 6f72 2920  s(*densevector) 
+00013160: 3e20 6570 7369 6c6f 6e29 207b 2020 2f2a  > epsilon) {  /*
+00013170: 2041 7070 6c79 207a 6572 6f2d 7468 7265   Apply zero-thre
+00013180: 7368 6f6c 6420 2a2f 0a20 2020 2020 2069  shold */.      i
+00013190: 6628 6e7a 7665 6374 6f72 2021 3d20 4e55  f(nzvector != NU
+000131a0: 4c4c 2920 2020 2020 2020 2020 2020 2020  LL)             
+000131b0: 2020 2020 2020 2020 2020 2f2a 204f 6e6c            /* Onl
+000131c0: 7920 7072 6f64 7563 6520 696e 6465 7820  y produce index 
+000131d0: 6966 206e 6f20 6e7a 7665 6374 6f72 2069  if no nzvector i
+000131e0: 7320 6769 7665 6e20 2a2f 0a20 2020 2020  s given */.     
+000131f0: 2020 206e 7a76 6563 746f 725b 6e5d 203d     nzvector[n] =
+00013200: 202a 6465 6e73 6576 6563 746f 723b 0a20   *densevector;. 
+00013210: 2020 2020 206e 2b2b 3b0a 2020 2020 2020       n++;.      
+00013220: 6e7a 696e 6465 785b 6e5d 203d 2073 7461  nzindex[n] = sta
+00013230: 7274 706f 733b 0a20 2020 207d 0a20 2020  rtpos;.    }.   
+00013240: 2073 7461 7274 706f 732b 2b3b 0a20 2020   startpos++;.   
+00013250: 2064 656e 7365 7665 6374 6f72 2b2b 3b0a   densevector++;.
+00013260: 2020 7d0a 2020 6e7a 696e 6465 785b 305d    }.  nzindex[0]
+00013270: 203d 206e 3b0a 2020 7265 7475 726e 2820   = n;.  return( 
+00013280: 5452 5545 2029 3b0a 7d0a 0a53 5441 5449  TRUE );.}..STATI
+00013290: 4320 4d59 424f 4f4c 2076 6563 5f65 7870  C MYBOOL vec_exp
+000132a0: 616e 6428 5245 414c 202a 6e7a 7665 6374  and(REAL *nzvect
+000132b0: 6f72 2c20 696e 7420 2a6e 7a69 6e64 6578  or, int *nzindex
+000132c0: 2c20 5245 414c 202a 6465 6e73 6576 6563  , REAL *densevec
+000132d0: 746f 722c 2069 6e74 2073 7461 7274 706f  tor, int startpo
+000132e0: 732c 2069 6e74 2065 6e64 706f 7329 0a7b  s, int endpos).{
+000132f0: 0a20 2069 6e74 2069 2c20 6e3b 0a0a 2020  .  int i, n;..  
+00013300: 6e20 3d20 6e7a 696e 6465 785b 305d 3b0a  n = nzindex[0];.
+00013310: 2020 6920 3d20 6e7a 696e 6465 785b 6e5d    i = nzindex[n]
+00013320: 3b0a 2020 6465 6e73 6576 6563 746f 7220  ;.  densevector 
+00013330: 2b3d 2065 6e64 706f 733b 0a20 2077 6869  += endpos;.  whi
+00013340: 6c65 2865 6e64 706f 7320 3e3d 2073 7461  le(endpos >= sta
+00013350: 7274 706f 7329 207b 2020 2020 2020 2020  rtpos) {        
+00013360: 2020 2020 2020 2020 2020 2020 202f 2a20               /* 
+00013370: 4c6f 6f70 2066 726f 6d20 6265 6869 6e64  Loop from behind
+00013380: 2074 6f20 616c 6c6f 7720 6465 6e73 6576   to allow densev
+00013390: 6563 746f 7220 3d3d 206e 7a76 6563 746f  ector == nzvecto
+000133a0: 7220 2a2f 0a20 2020 2069 6628 656e 6470  r */.    if(endp
+000133b0: 6f73 203d 3d20 6929 207b 0a20 2020 2020  os == i) {.     
+000133c0: 206e 2d2d 3b0a 2020 2020 2020 2a64 656e   n--;.      *den
+000133d0: 7365 7665 6374 6f72 203d 206e 7a76 6563  sevector = nzvec
+000133e0: 746f 725b 6e5d 3b0a 2020 2020 2020 6920  tor[n];.      i 
+000133f0: 3d20 6e7a 696e 6465 785b 6e5d 3b0a 2020  = nzindex[n];.  
+00013400: 2020 7d0a 2020 2020 656c 7365 0a20 2020    }.    else.   
+00013410: 2020 202a 6465 6e73 6576 6563 746f 7220     *densevector 
+00013420: 3d20 303b 0a20 2020 2065 6e64 706f 732d  = 0;.    endpos-
+00013430: 2d3b 0a20 2020 2064 656e 7365 7665 6374  -;.    densevect
+00013440: 6f72 2d2d 3b0a 2020 7d0a 2020 7265 7475  or--;.  }.  retu
+00013450: 726e 2820 5452 5545 2029 3b0a 7d0a 0a0a  rn( TRUE );.}...
+00013460: 2f2a 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /* -------------
+00013470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000134a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000134b0: 2d2d 2d2d 2d2d 2d2d 2d2d 202a 2f0a 2f2a  ---------- */./*
-000134c0: 2053 7061 7273 6520 6d61 7472 6978 2070   Sparse matrix p
-000134d0: 726f 6475 6374 2072 6f75 7469 6e65 7320  roduct routines 
-000134e0: 616e 6420 7574 696c 6974 7920 2020 2020  and utility     
-000134f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013500: 2020 2020 2020 2020 202a 2f0a 2f2a 202d           */./* -
+000134a0: 2d2d 2d2d 2d2d 2d2d 2d2d 202a 2f0a 2f2a  ---------- */./*
+000134b0: 2053 7061 7273 6520 6d61 7472 6978 2070   Sparse matrix p
+000134c0: 726f 6475 6374 2072 6f75 7469 6e65 7320  roduct routines 
+000134d0: 616e 6420 7574 696c 6974 7920 2020 2020  and utility     
+000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134f0: 2020 2020 2020 2020 202a 2f0a 2f2a 202d           */./* -
+00013500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013550: 2d2d 2d2d 2d2d 202a 2f0a 0a53 5441 5449  ------ */..STATI
-00013560: 4320 4d59 424f 4f4c 2067 6574 5f63 6f6c  C MYBOOL get_col
-00013570: 496e 6465 7841 286c 7072 6563 202a 6c70  IndexA(lprec *lp
-00013580: 2c20 696e 7420 7661 7273 6574 2c20 696e  , int varset, in
-00013590: 7420 2a63 6f6c 696e 6465 782c 204d 5942  t *colindex, MYB
-000135a0: 4f4f 4c20 6170 7065 6e64 290a 7b0a 2020  OOL append).{.  
-000135b0: 696e 7420 2020 2020 2069 2c20 7661 726e  int      i, varn
-000135c0: 722c 2050 3165 7874 7261 4469 6d2c 2076  r, P1extraDim, v
-000135d0: 622c 2076 652c 206e 2c20 6e72 6f77 7320  b, ve, n, nrows 
-000135e0: 3d20 6c70 2d3e 726f 7773 2c20 6e73 756d  = lp->rows, nsum
-000135f0: 203d 206c 702d 3e73 756d 3b0a 2020 4d59   = lp->sum;.  MY
-00013600: 424f 4f4c 2020 206f 6d69 7466 6978 6564  BOOL   omitfixed
-00013610: 2c20 6f6d 6974 6e6f 6e66 6978 6564 3b0a  , omitnonfixed;.
-00013620: 2020 5245 414c 2020 2020 2076 3b0a 0a20    REAL     v;.. 
-00013630: 202f 2a20 4669 6e64 2077 6861 7420 7661   /* Find what va
-00013640: 7269 6162 6c65 2072 616e 6765 2074 6f20  riable range to 
-00013650: 7363 616e 202d 2064 6566 6175 6c74 2069  scan - default i
-00013660: 7320 7b53 4341 4e5f 5553 4552 5641 5253  s {SCAN_USERVARS
-00013670: 7d20 2a2f 0a20 202f 2a20 4669 7273 7420  } */.  /* First 
-00013680: 6465 7465 726d 696e 6520 7468 6520 7374  determine the st
-00013690: 6172 7469 6e67 2070 6f73 6974 696f 6e3b  arting position;
-000136a0: 2061 6464 2066 726f 6d20 7468 6520 746f   add from the to
-000136b0: 702c 2067 6f69 6e67 2064 6f77 6e20 2a2f  p, going down */
-000136c0: 0a20 2050 3165 7874 7261 4469 6d20 3d20  .  P1extraDim = 
-000136d0: 6162 7328 6c70 2d3e 5031 6578 7472 6144  abs(lp->P1extraD
-000136e0: 696d 293b 0a20 2076 6220 3d20 6e72 6f77  im);.  vb = nrow
-000136f0: 7320 2b20 313b 0a20 2069 6628 7661 7273  s + 1;.  if(vars
-00013700: 6574 2026 2053 4341 4e5f 4152 5449 4649  et & SCAN_ARTIFI
-00013710: 4349 414c 5641 5253 290a 2020 2020 7662  CIALVARS).    vb
-00013720: 203d 206e 7375 6d20 2d20 5031 6578 7472   = nsum - P1extr
-00013730: 6144 696d 202b 2031 3b0a 2020 6966 2876  aDim + 1;.  if(v
-00013740: 6172 7365 7420 2620 5343 414e 5f55 5345  arset & SCAN_USE
-00013750: 5256 4152 5329 0a20 2020 2076 6220 3d20  RVARS).    vb = 
-00013760: 6e72 6f77 7320 2b20 313b 0a20 2069 6628  nrows + 1;.  if(
-00013770: 7661 7273 6574 2026 2053 4341 4e5f 534c  varset & SCAN_SL
-00013780: 4143 4b56 4152 5329 0a20 2020 2076 6220  ACKVARS).    vb 
-00013790: 3d20 313b 0a0a 2020 2f2a 2054 6865 6e20  = 1;..  /* Then 
-000137a0: 6465 7465 726d 696e 6520 7468 6520 656e  determine the en
-000137b0: 6469 6e67 2070 6f73 6974 696f 6e2c 2061  ding position, a
-000137c0: 6464 2066 726f 6d20 7468 6520 626f 7474  dd from the bott
-000137d0: 6f6d 2c20 676f 696e 6720 7570 202a 2f0a  om, going up */.
-000137e0: 2020 7665 203d 206e 7375 6d3b 0a20 2069    ve = nsum;.  i
-000137f0: 6628 7661 7273 6574 2026 2053 4341 4e5f  f(varset & SCAN_
-00013800: 534c 4143 4b56 4152 5329 0a20 2020 2076  SLACKVARS).    v
-00013810: 6520 3d20 6e72 6f77 733b 0a20 2069 6628  e = nrows;.  if(
-00013820: 7661 7273 6574 2026 2053 4341 4e5f 5553  varset & SCAN_US
-00013830: 4552 5641 5253 290a 2020 2020 7665 203d  ERVARS).    ve =
-00013840: 206e 7375 6d20 2d20 5031 6578 7472 6144   nsum - P1extraD
-00013850: 696d 3b0a 2020 6966 2876 6172 7365 7420  im;.  if(varset 
-00013860: 2620 5343 414e 5f41 5254 4946 4943 4941  & SCAN_ARTIFICIA
-00013870: 4c56 4152 5329 0a20 2020 2076 6520 3d20  LVARS).    ve = 
-00013880: 6e73 756d 3b0a 0a20 202f 2a20 4164 6a75  nsum;..  /* Adju
-00013890: 7374 2066 6f72 2070 6172 7469 616c 2070  st for partial p
-000138a0: 7269 6369 6e67 202a 2f0a 2020 6966 2876  ricing */.  if(v
-000138b0: 6172 7365 7420 2620 5343 414e 5f50 4152  arset & SCAN_PAR
-000138c0: 5449 414c 424c 4f43 4b29 207b 0a20 2020  TIALBLOCK) {.   
-000138d0: 2053 4554 4d41 5828 7662 2c20 7061 7274   SETMAX(vb, part
-000138e0: 6961 6c5f 626c 6f63 6b53 7461 7274 286c  ial_blockStart(l
-000138f0: 702c 2046 414c 5345 2929 3b0a 2020 2020  p, FALSE));.    
-00013900: 5345 544d 494e 2876 652c 2070 6172 7469  SETMIN(ve, parti
-00013910: 616c 5f62 6c6f 636b 456e 6428 6c70 2c20  al_blockEnd(lp, 
-00013920: 4641 4c53 4529 293b 0a20 207d 0a0a 2020  FALSE));.  }..  
-00013930: 2f2a 2044 6574 6572 6d69 6e65 2065 7863  /* Determine exc
-00013940: 6c75 7369 6f6e 2063 6f6c 756d 6e73 202a  lusion columns *
-00013950: 2f0a 2020 6f6d 6974 6669 7865 6420 3d20  /.  omitfixed = 
-00013960: 284d 5942 4f4f 4c29 2028 2876 6172 7365  (MYBOOL) ((varse
-00013970: 7420 2620 4f4d 4954 5f46 4958 4544 2920  t & OMIT_FIXED) 
-00013980: 213d 2030 293b 0a20 206f 6d69 746e 6f6e  != 0);.  omitnon
-00013990: 6669 7865 6420 3d20 284d 5942 4f4f 4c29  fixed = (MYBOOL)
-000139a0: 2028 2876 6172 7365 7420 2620 4f4d 4954   ((varset & OMIT
-000139b0: 5f4e 4f4e 4649 5845 4429 2021 3d20 3029  _NONFIXED) != 0)
-000139c0: 3b0a 2020 6966 286f 6d69 7466 6978 6564  ;.  if(omitfixed
-000139d0: 2026 2620 6f6d 6974 6e6f 6e66 6978 6564   && omitnonfixed
-000139e0: 290a 2020 2020 7265 7475 726e 2846 414c  ).    return(FAL
-000139f0: 5345 293b 0a0a 2020 2f2a 2053 6361 6e20  SE);..  /* Scan 
-00013a00: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
-00013a10: 7320 2a2f 0a20 2069 6628 6170 7065 6e64  s */.  if(append
-00013a20: 290a 2020 2020 6e20 3d20 636f 6c69 6e64  ).    n = colind
-00013a30: 6578 5b30 5d3b 0a20 2065 6c73 650a 2020  ex[0];.  else.  
-00013a40: 2020 6e20 3d20 303b 0a20 2066 6f72 2876    n = 0;.  for(v
-00013a50: 6172 6e72 203d 2076 623b 2076 6172 6e72  arnr = vb; varnr
-00013a60: 203c 3d20 7665 3b20 7661 726e 722b 2b29   <= ve; varnr++)
-00013a70: 207b 0a0a 2020 2020 2f2a 2053 6b69 7020   {..    /* Skip 
-00013a80: 6761 7020 696e 2074 6865 2073 7065 6369  gap in the speci
-00013a90: 6669 6564 2063 6f6c 756d 6e20 7363 616e  fied column scan
-00013aa0: 2072 616e 6765 2028 706f 7373 6962 6c79   range (possibly
-00013ab0: 2075 7365 7220 7661 7269 6162 6c65 7329   user variables)
-00013ac0: 202a 2f0a 2020 2020 6966 2876 6172 6e72   */.    if(varnr
-00013ad0: 203e 206e 726f 7773 2920 7b0a 2020 2020   > nrows) {.    
-00013ae0: 2020 6966 2828 7661 726e 7220 3c3d 206e    if((varnr <= n
-00013af0: 7375 6d2d 5031 6578 7472 6144 696d 2920  sum-P1extraDim) 
-00013b00: 2626 2021 2876 6172 7365 7420 2620 5343  && !(varset & SC
-00013b10: 414e 5f55 5345 5256 4152 5329 290a 2020  AN_USERVARS)).  
-00013b20: 2020 2020 2020 636f 6e74 696e 7565 3b0a        continue;.
-00013b30: 2369 6620 310a 2020 2020 2020 2f2a 2053  #if 1.      /* S
-00013b40: 6b69 7020 656d 7074 7920 636f 6c75 6d6e  kip empty column
-00013b50: 7320 2a2f 0a20 2020 2020 2069 6628 2f2a  s */.      if(/*
-00013b60: 286c 702d 3e50 3165 7874 7261 5661 6c20  (lp->P1extraVal 
-00013b70: 3d3d 2030 2920 2626 2a2f 0a20 2020 2020  == 0) &&*/.     
-00013b80: 2020 2020 286d 6174 5f63 6f6c 6c65 6e67      (mat_colleng
-00013b90: 7468 286c 702d 3e6d 6174 412c 2076 6172  th(lp->matA, var
-00013ba0: 6e72 2d6e 726f 7773 2920 3d3d 2030 2929  nr-nrows) == 0))
-00013bb0: 0a20 2020 2020 2020 2063 6f6e 7469 6e75  .        continu
-00013bc0: 653b 0a23 656e 6469 660a 2020 2020 7d0a  e;.#endif.    }.
-00013bd0: 0a20 2020 202f 2a20 4669 6e64 2069 6620  .    /* Find if 
-00013be0: 7468 6520 7661 7269 6162 6c65 2069 7320  the variable is 
-00013bf0: 696e 2074 6865 2073 636f 7065 202d 2064  in the scope - d
-00013c00: 6566 6175 6c74 2069 7320 7bd8 7d20 2a2f  efault is {.} */
-00013c10: 0a20 2020 2069 203d 206c 702d 3e69 735f  .    i = lp->is_
-00013c20: 6261 7369 635b 7661 726e 725d 3b0a 2020  basic[varnr];.  
-00013c30: 2020 6966 2828 7661 7273 6574 2026 2055    if((varset & U
-00013c40: 5345 5f42 4153 4943 5641 5253 2920 3e20  SE_BASICVARS) > 
-00013c50: 3020 2626 2028 6929 290a 2020 2020 2020  0 && (i)).      
-00013c60: 3b0a 2020 2020 656c 7365 2069 6628 2876  ;.    else if((v
-00013c70: 6172 7365 7420 2620 5553 455f 4e4f 4e42  arset & USE_NONB
-00013c80: 4153 4943 5641 5253 2920 3e20 3020 2626  ASICVARS) > 0 &&
-00013c90: 2028 2169 2929 0a20 2020 2020 203b 0a20   (!i)).      ;. 
-00013ca0: 2020 2065 6c73 650a 2020 2020 2020 636f     else.      co
-00013cb0: 6e74 696e 7565 3b0a 0a20 2020 2076 203d  ntinue;..    v =
-00013cc0: 206c 702d 3e75 7062 6f5b 7661 726e 725d   lp->upbo[varnr]
-00013cd0: 3b0a 2020 2020 6966 2828 6f6d 6974 6669  ;.    if((omitfi
-00013ce0: 7865 6420 2626 2028 7620 3d3d 2030 2929  xed && (v == 0))
-00013cf0: 207c 7c0a 2020 2020 2020 2028 6f6d 6974   ||.       (omit
-00013d00: 6e6f 6e66 6978 6564 2026 2620 2876 2021  nonfixed && (v !
-00013d10: 3d20 3029 2929 0a20 2020 2020 2063 6f6e  = 0))).      con
-00013d20: 7469 6e75 653b 0a0a 2020 2020 2f2a 2041  tinue;..    /* A
-00013d30: 7070 656e 6420 746f 206c 6973 7420 2a2f  ppend to list */
-00013d40: 0a20 2020 206e 2b2b 3b0a 2020 2020 636f  .    n++;.    co
-00013d50: 6c69 6e64 6578 5b6e 5d20 3d20 7661 726e  lindex[n] = varn
-00013d60: 723b 0a20 207d 0a20 2063 6f6c 696e 6465  r;.  }.  colinde
-00013d70: 785b 305d 203d 206e 3b0a 0a20 2072 6574  x[0] = n;..  ret
-00013d80: 7572 6e28 5452 5545 293b 0a7d 0a0a 5354  urn(TRUE);.}..ST
-00013d90: 4154 4943 2069 6e74 2070 726f 645f 4178  ATIC int prod_Ax
-00013da0: 286c 7072 6563 202a 6c70 2c20 696e 7420  (lprec *lp, int 
-00013db0: 2a63 6f6c 7461 7267 6574 2c20 5245 414c  *coltarget, REAL
-00013dc0: 202a 696e 7075 742c 2069 6e74 202a 6e7a   *input, int *nz
-00013dd0: 696e 7075 742c 0a20 2020 2020 2020 2020  input,.         
-00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 2020 2052 4541 4c20 726f 756e 647a       REAL roundz
-00013e00: 6572 6f2c 2052 4541 4c20 6f66 7363 616c  ero, REAL ofscal
-00013e10: 6172 2c0a 2020 2020 2020 2020 2020 2020  ar,.            
-00013e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e30: 2020 5245 414c 202a 6f75 7470 7574 2c20    REAL *output, 
-00013e40: 696e 7420 2a6e 7a6f 7574 7075 742c 2069  int *nzoutput, i
-00013e50: 6e74 2072 6f75 6e64 6d6f 6465 290a 2f2a  nt roundmode)./*
-00013e60: 2070 726f 645f 4178 2069 7320 6f6e 6c79   prod_Ax is only
-00013e70: 2075 7365 6420 696e 2066 696d 7072 6f76   used in fimprov
-00013e80: 653b 206e 6f74 6520 7468 6174 2069 7420  e; note that it 
-00013e90: 6973 204e 4f54 2056 414c 4944 4154 4544  is NOT VALIDATED
-00013ea0: 2f76 6572 6966 6965 6420 6173 206f 6620  /verified as of 
-00013eb0: 3230 3033 3038 3031 202d 204b 4520 2a2f  20030801 - KE */
-00013ec0: 0a7b 0a20 2069 6e74 2020 2020 2020 6a2c  .{.  int      j,
-00013ed0: 2063 6f6c 6e72 2c20 6962 2c20 6965 2c20   colnr, ib, ie, 
-00013ee0: 7662 3b20 2f2a 2c20 7665 3b20 2a2f 0a20  vb; /*, ve; */. 
-00013ef0: 204d 5942 4f4f 4c20 2020 6c6f 6361 6c73   MYBOOL   locals
-00013f00: 6574 2c20 6c6f 6361 6c6e 7a20 3d20 4641  et, localnz = FA
-00013f10: 4c53 452c 2069 7352 433b 0a20 204d 4154  LSE, isRC;.  MAT
-00013f20: 7265 6320 2020 2a6d 6174 203d 206c 702d  rec   *mat = lp-
-00013f30: 3e6d 6174 413b 0a20 2052 4541 4c20 2020  >matA;.  REAL   
-00013f40: 2020 7364 703b 0a20 2052 4541 4c20 2020    sdp;.  REAL   
-00013f50: 2020 2a76 616c 7565 3b0a 2020 696e 7420    *value;.  int 
-00013f60: 2020 2020 202a 726f 776e 723b 0a0a 2020       *rownr;..  
-00013f70: 2f2a 2046 696e 6420 7768 6174 2076 6172  /* Find what var
-00013f80: 6961 626c 6520 7261 6e67 6520 746f 2073  iable range to s
-00013f90: 6361 6e20 2d20 6465 6661 756c 7420 6973  can - default is
-00013fa0: 207b 5343 414e 5f55 5345 5256 4152 537d   {SCAN_USERVARS}
-00013fb0: 202a 2f0a 2020 2f2a 2044 6566 696e 6520   */.  /* Define 
-00013fc0: 6465 6661 756c 7420 636f 6c75 6d6e 2074  default column t
-00013fd0: 6172 6765 7420 6966 206e 6f6e 6520 7761  arget if none wa
-00013fe0: 7320 7072 6f76 6964 6564 202a 2f0a 2020  s provided */.  
-00013ff0: 6973 5243 203d 2028 4d59 424f 4f4c 2920  isRC = (MYBOOL) 
-00014000: 2828 726f 756e 646d 6f64 6520 2620 4d41  ((roundmode & MA
-00014010: 545f 524f 554e 4452 4329 2021 3d20 3029  T_ROUNDRC) != 0)
-00014020: 3b0a 2020 6c6f 6361 6c73 6574 203d 2028  ;.  localset = (
-00014030: 4d59 424f 4f4c 2920 2863 6f6c 7461 7267  MYBOOL) (coltarg
-00014040: 6574 203d 3d20 4e55 4c4c 293b 0a20 2069  et == NULL);.  i
-00014050: 6628 6c6f 6361 6c73 6574 2920 7b0a 2020  f(localset) {.  
-00014060: 2020 696e 7420 7661 7273 6574 203d 2053    int varset = S
-00014070: 4341 4e5f 534c 4143 4b56 4152 5320 7c20  CAN_SLACKVARS | 
-00014080: 5343 414e 5f55 5345 5256 4152 5320 7c0a  SCAN_USERVARS |.
-00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2055 5345 5f42 4153 4943 5641 5253 207c   USE_BASICVARS |
-000140b0: 204f 4d49 545f 4649 5845 443b 0a20 2020   OMIT_FIXED;.   
-000140c0: 2069 6628 6973 5243 2026 2620 6973 5f70   if(isRC && is_p
-000140d0: 6976 5f6d 6f64 6528 6c70 2c20 5052 4943  iv_mode(lp, PRIC
-000140e0: 455f 5041 5254 4941 4c29 2026 2620 2169  E_PARTIAL) && !i
-000140f0: 735f 7069 765f 6d6f 6465 286c 702c 2050  s_piv_mode(lp, P
-00014100: 5249 4345 5f46 4f52 4345 4655 4c4c 2929  RICE_FORCEFULL))
-00014110: 0a20 2020 2020 2076 6172 7365 7420 7c3d  .      varset |=
-00014120: 2053 4341 4e5f 5041 5254 4941 4c42 4c4f   SCAN_PARTIALBLO
-00014130: 434b 3b0a 2020 2020 636f 6c74 6172 6765  CK;.    coltarge
-00014140: 7420 3d20 2869 6e74 202a 2920 6d65 6d70  t = (int *) memp
-00014150: 6f6f 6c5f 6f62 7461 696e 5665 6374 6f72  ool_obtainVector
-00014160: 286c 702d 3e77 6f72 6b61 7272 6179 732c  (lp->workarrays,
-00014170: 206c 702d 3e73 756d 2b31 2c20 7369 7a65   lp->sum+1, size
-00014180: 6f66 282a 636f 6c74 6172 6765 7429 293b  of(*coltarget));
-00014190: 0a20 2020 2069 6628 2167 6574 5f63 6f6c  .    if(!get_col
-000141a0: 496e 6465 7841 286c 702c 2076 6172 7365  IndexA(lp, varse
-000141b0: 742c 2063 6f6c 7461 7267 6574 2c20 4641  t, coltarget, FA
-000141c0: 4c53 4529 2920 7b0a 2020 2020 2020 6d65  LSE)) {.      me
-000141d0: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
-000141e0: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
-000141f0: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
-00014200: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
-00014210: 2020 2020 2020 7265 7475 726e 2846 414c        return(FAL
-00014220: 5345 293b 0a20 2020 207d 0a20 207d 0a20  SE);.    }.  }. 
-00014230: 206c 6f63 616c 6e7a 203d 2028 4d59 424f   localnz = (MYBO
-00014240: 4f4c 2920 286e 7a69 6e70 7574 203d 3d20  OL) (nzinput == 
-00014250: 4e55 4c4c 293b 0a20 2069 6628 6c6f 6361  NULL);.  if(loca
-00014260: 6c6e 7a29 207b 0a20 2020 206e 7a69 6e70  lnz) {.    nzinp
-00014270: 7574 203d 2028 696e 7420 2a29 206d 656d  ut = (int *) mem
-00014280: 706f 6f6c 5f6f 6274 6169 6e56 6563 746f  pool_obtainVecto
-00014290: 7228 6c70 2d3e 776f 726b 6172 7261 7973  r(lp->workarrays
-000142a0: 2c20 6c70 2d3e 726f 7773 2b31 2c20 7369  , lp->rows+1, si
-000142b0: 7a65 6f66 282a 6e7a 696e 7075 7429 293b  zeof(*nzinput));
-000142c0: 0a20 2020 2076 6563 5f63 6f6d 7072 6573  .    vec_compres
-000142d0: 7328 696e 7075 742c 2030 2c20 6c70 2d3e  s(input, 0, lp->
-000142e0: 726f 7773 2c20 6c70 2d3e 6d61 7441 2d3e  rows, lp->matA->
-000142f0: 6570 7376 616c 7565 2c20 4e55 4c4c 2c20  epsvalue, NULL, 
-00014300: 6e7a 696e 7075 7429 3b0a 2020 7d0a 0a20  nzinput);.  }.. 
-00014310: 202f 2a20 5363 616e 2074 6865 2063 6f6c   /* Scan the col
-00014320: 756d 6e73 202a 2f0a 2020 7662 203d 2031  umns */.  vb = 1
-00014330: 3b0a 2020 2f2a 2076 6520 3d20 636f 6c74  ;.  /* ve = colt
-00014340: 6172 6765 745b 305d 3b20 2a2f 0a20 2066  arget[0]; */.  f
-00014350: 6f72 2876 6220 3d20 313b 2076 6220 3c3d  or(vb = 1; vb <=
-00014360: 2063 6f6c 7461 7267 6574 5b30 5d3b 2076   coltarget[0]; v
-00014370: 622b 2b29 207b 0a20 2020 2063 6f6c 6e72  b++) {.    colnr
-00014380: 203d 2063 6f6c 7461 7267 6574 5b76 625d   = coltarget[vb]
-00014390: 3b0a 2020 2020 6a20 3d20 6c70 2d3e 6973  ;.    j = lp->is
-000143a0: 5f62 6173 6963 5b63 6f6c 6e72 5d3b 0a0a  _basic[colnr];..
-000143b0: 2020 2020 2f2a 2050 6572 666f 726d 2074      /* Perform t
-000143c0: 6865 206d 756c 7469 706c 6963 6174 696f  he multiplicatio
-000143d0: 6e20 2a2f 0a20 2020 2073 6470 203d 206f  n */.    sdp = o
-000143e0: 6673 6361 6c61 722a 696e 7075 745b 6a5d  fscalar*input[j]
-000143f0: 3b0a 2020 2020 6966 2863 6f6c 6e72 203c  ;.    if(colnr <
-00014400: 3d20 6c70 2d3e 726f 7773 2920 2020 2020  = lp->rows)     
-00014410: 2020 2020 2020 2020 2020 2f2a 2041 2073            /* A s
-00014420: 6c61 636b 2076 6172 6961 626c 6520 6973  lack variable is
-00014430: 2069 6e20 7468 6520 6261 7369 7320 2a2f   in the basis */
-00014440: 0a20 2020 2020 206f 7574 7075 745b 636f  .      output[co
-00014450: 6c6e 725d 202b 3d20 7364 703b 0a20 2020  lnr] += sdp;.   
-00014460: 2065 6c73 6520 7b20 2020 2020 2020 2020   else {         
-00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014480: 2020 2020 202f 2a20 4120 6e6f 726d 616c       /* A normal
-00014490: 2076 6172 6961 626c 6520 6973 2069 6e20   variable is in 
-000144a0: 7468 6520 6261 7369 7320 2a2f 0a20 2020  the basis */.   
-000144b0: 2020 2063 6f6c 6e72 202d 3d20 6c70 2d3e     colnr -= lp->
-000144c0: 726f 7773 3b0a 2020 2020 2020 6962 203d  rows;.      ib =
-000144d0: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
-000144e0: 6c6e 7220 2d20 315d 3b0a 2020 2020 2020  lnr - 1];.      
-000144f0: 6965 203d 206d 6174 2d3e 636f 6c5f 656e  ie = mat->col_en
-00014500: 645b 636f 6c6e 725d 3b0a 2020 2020 2020  d[colnr];.      
-00014510: 726f 776e 7220 3d20 2643 4f4c 5f4d 4154  rownr = &COL_MAT
-00014520: 5f52 4f57 4e52 2869 6229 3b0a 2020 2020  _ROWNR(ib);.    
-00014530: 2020 7661 6c75 6520 3d20 2643 4f4c 5f4d    value = &COL_M
-00014540: 4154 5f56 414c 5545 2869 6229 3b0a 2020  AT_VALUE(ib);.  
-00014550: 2020 2020 666f 7228 3b20 6962 203c 2069      for(; ib < i
-00014560: 653b 0a20 2020 2020 2020 2020 2069 622b  e;.          ib+
-00014570: 2b2c 2072 6f77 6e72 202b 3d20 6d61 7452  +, rownr += matR
-00014580: 6f77 436f 6c53 7465 702c 2076 616c 7565  owColStep, value
-00014590: 202b 3d20 6d61 7456 616c 7565 5374 6570   += matValueStep
-000145a0: 2920 7b0a 2020 2020 2020 2020 6f75 7470  ) {.        outp
-000145b0: 7574 5b2a 726f 776e 725d 202b 3d20 282a  ut[*rownr] += (*
-000145c0: 7661 6c75 6529 2a73 6470 3b0a 2020 2020  value)*sdp;.    
-000145d0: 2020 7d0a 2020 2020 7d0a 2020 7d0a 2020    }.    }.  }.  
-000145e0: 726f 756e 6456 6563 746f 7228 6f75 7470  roundVector(outp
-000145f0: 7574 2b31 2c20 6c70 2d3e 726f 7773 2d31  ut+1, lp->rows-1
-00014600: 2c20 726f 756e 647a 6572 6f29 3b0a 0a20  , roundzero);.. 
-00014610: 202f 2a20 436c 6561 6e20 7570 2061 6e64   /* Clean up and
-00014620: 2072 6574 7572 6e20 2a2f 0a20 2069 6628   return */.  if(
-00014630: 6c6f 6361 6c73 6574 290a 2020 2020 6d65  localset).    me
-00014640: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
-00014650: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
-00014660: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
-00014670: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
-00014680: 2020 6966 286c 6f63 616c 6e7a 290a 2020    if(localnz).  
-00014690: 2020 6d65 6d70 6f6f 6c5f 7265 6c65 6173    mempool_releas
-000146a0: 6556 6563 746f 7228 6c70 2d3e 776f 726b  eVector(lp->work
-000146b0: 6172 7261 7973 2c20 2863 6861 7220 2a29  arrays, (char *)
-000146c0: 206e 7a69 6e70 7574 2c20 4641 4c53 4529   nzinput, FALSE)
-000146d0: 3b0a 0a20 2072 6574 7572 6e28 5452 5545  ;..  return(TRUE
-000146e0: 293b 0a7d 0a0a 5354 4154 4943 2069 6e74  );.}..STATIC int
-000146f0: 2070 726f 645f 7841 286c 7072 6563 202a   prod_xA(lprec *
-00014700: 6c70 2c20 696e 7420 2a63 6f6c 7461 7267  lp, int *coltarg
-00014710: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-00014720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014730: 2020 5245 414c 202a 696e 7075 742c 2069    REAL *input, i
-00014740: 6e74 202a 6e7a 696e 7075 742c 2052 4541  nt *nzinput, REA
-00014750: 4c20 726f 756e 647a 6572 6f2c 2052 4541  L roundzero, REA
-00014760: 4c20 6f66 7363 616c 6172 2c0a 2020 2020  L ofscalar,.    
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 2020 2020 2020 2020 5245 414c 202a            REAL *
-00014790: 6f75 7470 7574 2c20 696e 7420 2a6e 7a6f  output, int *nzo
-000147a0: 7574 7075 742c 2069 6e74 2072 6f75 6e64  utput, int round
-000147b0: 6d6f 6465 290a 2f2a 204e 6f74 6520 7468  mode)./* Note th
-000147c0: 6174 2074 6865 2064 6f74 2070 726f 6475  at the dot produ
-000147d0: 6374 2078 6120 6973 2073 746f 7265 6420  ct xa is stored 
-000147e0: 6174 2074 6865 2061 6374 6976 6520 636f  at the active co
-000147f0: 6c75 6d6e 2069 6e64 6578 206f 6620 412c  lumn index of A,
-00014800: 2069 2e65 2e20 6f66 2061 2e0a 2020 2054   i.e. of a..   T
-00014810: 6869 7320 6d65 616e 7320 7468 6174 2069  his means that i
-00014820: 6620 7468 6520 6261 7369 7320 6f6e 6c79  f the basis only
-00014830: 2063 6f6e 7461 696e 7320 6e6f 6e2d 736c   contains non-sl
-00014840: 6163 6b20 7661 7269 6162 6c65 732c 206f  ack variables, o
-00014850: 7574 7075 7420 6d61 7920 706f 696e 7420  utput may point 
-00014860: 746f 0a20 2020 7468 6520 7361 6d65 2076  to.   the same v
-00014870: 6563 746f 7220 6173 2069 6e70 7574 2c20  ector as input, 
-00014880: 7769 7468 6f75 7420 6f76 6572 7772 6974  without overwrit
-00014890: 696e 6720 7468 6520 5b30 2e2e 726f 7773  ing the [0..rows
-000148a0: 5d20 656c 656d 656e 7473 2e20 2a2f 0a7b  ] elements. */.{
-000148b0: 0a20 2069 6e74 2020 2020 2020 636f 6c6e  .  int      coln
-000148c0: 722c 2072 6f77 6e72 2c20 7661 726e 722c  r, rownr, varnr,
-000148d0: 2069 622c 2069 652c 2076 622c 2076 652c   ib, ie, vb, ve,
-000148e0: 206e 726f 7773 203d 206c 702d 3e72 6f77   nrows = lp->row
-000148f0: 733b 0a20 204d 5942 4f4f 4c20 2020 6c6f  s;.  MYBOOL   lo
-00014900: 6361 6c73 6574 2c20 6c6f 6361 6c6e 7a20  calset, localnz 
-00014910: 3d20 4641 4c53 452c 2069 6e63 6c75 6465  = FALSE, include
-00014920: 4f46 2c20 6973 5243 3b0a 2020 5245 414c  OF, isRC;.  REAL
-00014930: 5850 2020 2076 6d61 783b 0a20 2072 6567  XP   vmax;.  reg
-00014940: 6973 7465 7220 5245 414c 5850 2076 3b0a  ister REALXP v;.
-00014950: 2020 696e 7420 2020 2020 2069 6e7a 2c20    int      inz, 
-00014960: 2a72 6f77 696e 2c20 636f 756e 744e 5a20  *rowin, countNZ 
-00014970: 3d20 303b 0a20 204d 4154 7265 6320 2020  = 0;.  MATrec   
-00014980: 2a6d 6174 203d 206c 702d 3e6d 6174 413b  *mat = lp->matA;
-00014990: 0a20 2072 6567 6973 7465 7220 5245 414c  .  register REAL
-000149a0: 2020 2020 202a 6d61 7456 616c 7565 3b0a       *matValue;.
-000149b0: 2020 7265 6769 7374 6572 2069 6e74 2020    register int  
-000149c0: 2020 2020 2a6d 6174 526f 776e 723b 0a0a      *matRownr;..
-000149d0: 2020 2f2a 2043 6c65 616e 206f 7574 7075    /* Clean outpu
-000149e0: 7420 6172 6561 2028 6f6e 6c79 206e 6563  t area (only nec
-000149f0: 6573 7361 7279 2069 6620 7765 2061 7265  essary if we are
-00014a00: 2072 6574 7572 6e69 6e67 2074 6865 2066   returning the f
-00014a10: 756c 6c20 7665 6374 6f72 2920 2a2f 0a20  ull vector) */. 
-00014a20: 2069 7352 4320 3d20 284d 5942 4f4f 4c29   isRC = (MYBOOL)
-00014a30: 2028 2872 6f75 6e64 6d6f 6465 2026 204d   ((roundmode & M
-00014a40: 4154 5f52 4f55 4e44 5243 2920 213d 2030  AT_ROUNDRC) != 0
-00014a50: 293b 0a20 2069 6628 6e7a 6f75 7470 7574  );.  if(nzoutput
-00014a60: 203d 3d20 4e55 4c4c 2920 7b0a 2020 2020   == NULL) {.    
-00014a70: 6966 2869 6e70 7574 203d 3d20 6f75 7470  if(input == outp
-00014a80: 7574 290a 2020 2020 2020 4d45 4d43 4c45  ut).      MEMCLE
-00014a90: 4152 286f 7574 7075 742b 6e72 6f77 732b  AR(output+nrows+
-00014aa0: 312c 206c 702d 3e63 6f6c 756d 6e73 293b  1, lp->columns);
-00014ab0: 0a20 2020 2065 6c73 650a 2020 2020 2020  .    else.      
-00014ac0: 4d45 4d43 4c45 4152 286f 7574 7075 742c  MEMCLEAR(output,
-00014ad0: 206c 702d 3e73 756d 2b31 293b 0a20 207d   lp->sum+1);.  }
-00014ae0: 0a0a 2020 2f2a 2046 696e 6420 7768 6174  ..  /* Find what
-00014af0: 2076 6172 6961 626c 6520 7261 6e67 6520   variable range 
-00014b00: 746f 2073 6361 6e20 2d20 6465 6661 756c  to scan - defaul
-00014b10: 7420 6973 207b 5343 414e 5f55 5345 5256  t is {SCAN_USERV
-00014b20: 4152 537d 202a 2f0a 2020 2f2a 2044 6566  ARS} */.  /* Def
-00014b30: 696e 6520 6465 6661 756c 7420 636f 6c75  ine default colu
-00014b40: 6d6e 2074 6172 6765 7420 6966 206e 6f6e  mn target if non
-00014b50: 6520 7761 7320 7072 6f76 6964 6564 202a  e was provided *
-00014b60: 2f0a 2020 6c6f 6361 6c73 6574 203d 2028  /.  localset = (
-00014b70: 4d59 424f 4f4c 2920 2863 6f6c 7461 7267  MYBOOL) (coltarg
-00014b80: 6574 203d 3d20 4e55 4c4c 293b 0a20 2069  et == NULL);.  i
-00014b90: 6628 6c6f 6361 6c73 6574 2920 7b0a 2020  f(localset) {.  
-00014ba0: 2020 696e 7420 7661 7273 6574 203d 2053    int varset = S
-00014bb0: 4341 4e5f 534c 4143 4b56 4152 5320 7c20  CAN_SLACKVARS | 
-00014bc0: 5343 414e 5f55 5345 5256 4152 5320 7c0a  SCAN_USERVARS |.
-00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2055 5345 5f4e 4f4e 4241 5349 4356 4152   USE_NONBASICVAR
-00014bf0: 5320 7c20 4f4d 4954 5f46 4958 4544 3b0a  S | OMIT_FIXED;.
-00014c00: 2020 2020 6966 2869 7352 4320 2626 2069      if(isRC && i
-00014c10: 735f 7069 765f 6d6f 6465 286c 702c 2050  s_piv_mode(lp, P
-00014c20: 5249 4345 5f50 4152 5449 414c 2920 2626  RICE_PARTIAL) &&
-00014c30: 2021 6973 5f70 6976 5f6d 6f64 6528 6c70   !is_piv_mode(lp
-00014c40: 2c20 5052 4943 455f 464f 5243 4546 554c  , PRICE_FORCEFUL
-00014c50: 4c29 290a 2020 2020 2020 7661 7273 6574  L)).      varset
-00014c60: 207c 3d20 5343 414e 5f50 4152 5449 414c   |= SCAN_PARTIAL
-00014c70: 424c 4f43 4b3b 0a20 2020 2063 6f6c 7461  BLOCK;.    colta
-00014c80: 7267 6574 203d 2028 696e 7420 2a29 206d  rget = (int *) m
-00014c90: 656d 706f 6f6c 5f6f 6274 6169 6e56 6563  empool_obtainVec
-00014ca0: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
-00014cb0: 7973 2c20 6c70 2d3e 7375 6d2b 312c 2073  ys, lp->sum+1, s
-00014cc0: 697a 656f 6628 2a63 6f6c 7461 7267 6574  izeof(*coltarget
-00014cd0: 2929 3b0a 2020 2020 6966 2821 6765 745f  ));.    if(!get_
-00014ce0: 636f 6c49 6e64 6578 4128 6c70 2c20 7661  colIndexA(lp, va
-00014cf0: 7273 6574 2c20 636f 6c74 6172 6765 742c  rset, coltarget,
-00014d00: 2046 414c 5345 2929 207b 0a20 2020 2020   FALSE)) {.     
-00014d10: 206d 656d 706f 6f6c 5f72 656c 6561 7365   mempool_release
-00014d20: 5665 6374 6f72 286c 702d 3e77 6f72 6b61  Vector(lp->worka
-00014d30: 7272 6179 732c 2028 6368 6172 202a 2920  rrays, (char *) 
-00014d40: 636f 6c74 6172 6765 742c 2046 414c 5345  coltarget, FALSE
-00014d50: 293b 0a20 2020 2020 2072 6574 7572 6e28  );.      return(
-00014d60: 4641 4c53 4529 3b0a 2020 2020 7d0a 2020  FALSE);.    }.  
-00014d70: 7d0a 2f2a 2364 6566 696e 6520 5573 654c  }./*#define UseL
-00014d80: 6f63 616c 4e5a 2a2f 0a23 6966 6465 6620  ocalNZ*/.#ifdef 
-00014d90: 5573 654c 6f63 616c 4e5a 0a20 206c 6f63  UseLocalNZ.  loc
-00014da0: 616c 6e7a 203d 2028 4d59 424f 4f4c 2920  alnz = (MYBOOL) 
-00014db0: 286e 7a69 6e70 7574 203d 3d20 4e55 4c4c  (nzinput == NULL
-00014dc0: 293b 0a20 2069 6628 6c6f 6361 6c6e 7a29  );.  if(localnz)
-00014dd0: 207b 0a20 2020 206e 7a69 6e70 7574 203d   {.    nzinput =
-00014de0: 2028 696e 7420 2a29 206d 656d 706f 6f6c   (int *) mempool
-00014df0: 5f6f 6274 6169 6e56 6563 746f 7228 6c70  _obtainVector(lp
-00014e00: 2d3e 776f 726b 6172 7261 7973 2c20 6e72  ->workarrays, nr
-00014e10: 6f77 732b 312c 2073 697a 656f 6628 2a6e  ows+1, sizeof(*n
-00014e20: 7a69 6e70 7574 2929 3b0a 2020 2020 7665  zinput));.    ve
-00014e30: 635f 636f 6d70 7265 7373 2869 6e70 7574  c_compress(input
-00014e40: 2c20 302c 206e 726f 7773 2c20 6c70 2d3e  , 0, nrows, lp->
-00014e50: 6d61 7441 2d3e 6570 7376 616c 7565 2c20  matA->epsvalue, 
-00014e60: 4e55 4c4c 2c20 6e7a 696e 7075 7429 3b0a  NULL, nzinput);.
-00014e70: 2020 7d0a 2365 6e64 6966 0a20 2069 6e63    }.#endif.  inc
-00014e80: 6c75 6465 4f46 203d 2028 4d59 424f 4f4c  ludeOF = (MYBOOL
-00014e90: 2920 2828 286e 7a69 6e70 7574 203d 3d20  ) (((nzinput == 
-00014ea0: 4e55 4c4c 2920 7c7c 2028 6e7a 696e 7075  NULL) || (nzinpu
-00014eb0: 745b 315d 203d 3d20 3029 2920 2626 0a20  t[1] == 0)) &&. 
-00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ed0: 2020 2020 2020 2028 696e 7075 745b 305d         (input[0]
-00014ee0: 2021 3d20 3029 2026 2620 6c70 2d3e 6f62   != 0) && lp->ob
-00014ef0: 6a5f 696e 5f62 6173 6973 293b 0a0a 2020  j_in_basis);..  
-00014f00: 2f2a 2053 6361 6e20 7468 6520 7461 7267  /* Scan the targ
-00014f10: 6574 2063 6f6c 756d 7320 2a2f 0a20 2076  et colums */.  v
-00014f20: 6d61 7820 3d20 303b 0a20 2076 6520 3d20  max = 0;.  ve = 
-00014f30: 636f 6c74 6172 6765 745b 305d 3b0a 2020  coltarget[0];.  
-00014f40: 666f 7228 7662 203d 2031 3b20 7662 203c  for(vb = 1; vb <
-00014f50: 3d20 7665 3b20 7662 2b2b 2920 7b0a 0a20  = ve; vb++) {.. 
-00014f60: 2020 2076 6172 6e72 203d 2063 6f6c 7461     varnr = colta
-00014f70: 7267 6574 5b76 625d 3b0a 0a20 2020 2069  rget[vb];..    i
-00014f80: 6628 7661 726e 7220 3c3d 206e 726f 7773  f(varnr <= nrows
-00014f90: 2920 7b0a 2020 2020 2020 7620 3d20 696e  ) {.      v = in
-00014fa0: 7075 745b 7661 726e 725d 3b0a 2020 2020  put[varnr];.    
-00014fb0: 7d0a 2020 2020 656c 7365 207b 0a20 2020  }.    else {.   
-00014fc0: 2020 2063 6f6c 6e72 203d 2076 6172 6e72     colnr = varnr
-00014fd0: 202d 206e 726f 7773 3b0a 2020 2020 2020   - nrows;.      
-00014fe0: 7620 3d20 303b 0a20 2020 2020 2069 6220  v = 0;.      ib 
-00014ff0: 3d20 6d61 742d 3e63 6f6c 5f65 6e64 5b63  = mat->col_end[c
-00015000: 6f6c 6e72 202d 2031 5d3b 0a20 2020 2020  olnr - 1];.     
-00015010: 2069 6520 3d20 6d61 742d 3e63 6f6c 5f65   ie = mat->col_e
-00015020: 6e64 5b63 6f6c 6e72 5d3b 0a20 2020 2020  nd[colnr];.     
-00015030: 2069 6628 6962 203c 2069 6529 207b 0a0a   if(ib < ie) {..
-00015040: 2020 2020 2020 2020 2f2a 2044 6f20 6465          /* Do de
-00015050: 6e73 6520 696e 7075 7420 7665 6374 6f72  nse input vector
-00015060: 2076 6572 7369 6f6e 202a 2f0a 2369 6664   version */.#ifd
-00015070: 6566 2055 7365 4c6f 6361 6c4e 5a0a 2020  ef UseLocalNZ.  
-00015080: 2020 2020 2020 6966 286c 6f63 616c 6e7a        if(localnz
-00015090: 207c 7c20 286e 7a69 6e70 7574 203d 3d20   || (nzinput == 
-000150a0: 4e55 4c4c 2929 207b 0a23 656c 7365 0a20  NULL)) {.#else. 
-000150b0: 2020 2020 2020 2069 6628 6e7a 696e 7075         if(nzinpu
-000150c0: 7420 3d3d 204e 554c 4c29 207b 0a23 656e  t == NULL) {.#en
-000150d0: 6469 660a 2020 2020 2020 2020 2020 2f2a  dif.          /*
-000150e0: 2044 6f20 7468 6520 4f46 202a 2f0a 2020   Do the OF */.  
-000150f0: 2020 2020 2020 2020 6966 2869 6e63 6c75          if(inclu
-00015100: 6465 4f46 290a 2369 6664 6566 2044 6972  deOF).#ifdef Dir
-00015110: 6563 7441 7272 6179 4f46 0a20 2020 2020  ectArrayOF.     
-00015120: 2020 2020 2020 2076 202b 3d20 696e 7075         v += inpu
-00015130: 745b 305d 202a 206c 702d 3e6f 626a 5b63  t[0] * lp->obj[c
-00015140: 6f6c 6e72 5d20 2a20 6f66 7363 616c 6172  olnr] * ofscalar
-00015150: 3b0a 2365 6c73 650a 2020 2020 2020 2020  ;.#else.        
-00015160: 2020 2020 7620 2b3d 2069 6e70 7574 5b30      v += input[0
-00015170: 5d20 2a20 6765 745f 4f46 5f61 6374 6976  ] * get_OF_activ
-00015180: 6528 6c70 2c20 7661 726e 722c 206f 6673  e(lp, varnr, ofs
-00015190: 6361 6c61 7229 3b0a 2365 6e64 6966 0a0a  calar);.#endif..
-000151a0: 2020 2020 2020 2020 2020 2f2a 2049 6e69            /* Ini
-000151b0: 7469 616c 697a 6520 706f 696e 7465 7273  tialize pointers
-000151c0: 202a 2f0a 2020 2020 2020 2020 2020 6d61   */.          ma
-000151d0: 7452 6f77 6e72 203d 2026 434f 4c5f 4d41  tRownr = &COL_MA
-000151e0: 545f 524f 574e 5228 6962 293b 0a20 2020  T_ROWNR(ib);.   
-000151f0: 2020 2020 2020 206d 6174 5661 6c75 6520         matValue 
-00015200: 3d20 2643 4f4c 5f4d 4154 5f56 414c 5545  = &COL_MAT_VALUE
-00015210: 2869 6229 3b0a 0a20 2020 2020 2020 2020  (ib);..         
-00015220: 202f 2a20 446f 2065 7874 7261 206c 6f6f   /* Do extra loo
-00015230: 7020 6f70 7469 6d69 7a61 7469 6f6e 2062  p optimization b
-00015240: 6173 6564 206f 6e20 7461 7267 6574 2077  ased on target w
-00015250: 696e 646f 7720 6f76 6572 6c61 7073 202a  indow overlaps *
-00015260: 2f0a 2369 6664 6566 2055 7365 4c6f 6361  /.#ifdef UseLoca
-00015270: 6c4e 5a0a 2020 2020 2020 2020 2020 6966  lNZ.          if
-00015280: 2828 6962 203c 2069 6529 0a20 2020 2020  ((ib < ie).     
-00015290: 2020 2020 2020 2020 2626 2028 636f 6c6e          && (coln
-000152a0: 7220 3c3d 202a 6e7a 696e 7075 7429 0a20  r <= *nzinput). 
-000152b0: 2020 2020 2020 2020 2020 2020 2626 2028              && (
-000152c0: 434f 4c5f 4d41 545f 524f 574e 5228 6965  COL_MAT_ROWNR(ie
-000152d0: 2d31 2920 3e3d 206e 7a69 6e70 7574 5b63  -1) >= nzinput[c
-000152e0: 6f6c 6e72 5d29 0a20 2020 2020 2020 2020  olnr]).         
-000152f0: 2020 2020 2626 2028 2a6d 6174 526f 776e      && (*matRown
-00015300: 7220 3c3d 206e 7a69 6e70 7574 5b2a 6e7a  r <= nzinput[*nz
-00015310: 696e 7075 745d 290a 2020 2020 2020 2020  input]).        
-00015320: 2020 2020 2029 0a23 656e 6469 660a 2369       ).#endif.#i
-00015330: 6664 6566 204e 6f4c 6f6f 7055 6e72 6f6c  fdef NoLoopUnrol
-00015340: 6c0a 2020 2020 2020 2020 2020 2f2a 2054  l.          /* T
-00015350: 6865 6e20 6c6f 6f70 206f 7665 7220 616c  hen loop over al
-00015360: 6c20 7265 6775 6c61 7220 726f 7773 202a  l regular rows *
-00015370: 2f0a 2020 2020 2020 2020 2020 666f 7228  /.          for(
-00015380: 3b20 6962 203c 2069 653b 2069 622b 2b29  ; ib < ie; ib++)
-00015390: 207b 0a20 2020 2020 2020 2020 2020 2076   {.            v
-000153a0: 202b 3d20 696e 7075 745b 2a6d 6174 526f   += input[*matRo
-000153b0: 776e 725d 202a 2028 2a6d 6174 5661 6c75  wnr] * (*matValu
-000153c0: 6529 3b0a 2020 2020 2020 2020 2020 2020  e);.            
-000153d0: 6d61 7456 616c 7565 202b 3d20 6d61 7456  matValue += matV
-000153e0: 616c 7565 5374 6570 3b0a 2020 2020 2020  alueStep;.      
-000153f0: 2020 2020 2020 6d61 7452 6f77 6e72 202b        matRownr +
-00015400: 3d20 6d61 7452 6f77 436f 6c53 7465 703b  = matRowColStep;
-00015410: 0a20 2020 2020 2020 2020 207d 0a23 656c  .          }.#el
-00015420: 7365 0a20 2020 2020 2020 2020 202f 2a20  se.          /* 
-00015430: 5072 6570 6172 6520 666f 7220 7369 6d70  Prepare for simp
-00015440: 6c65 206c 6f6f 7020 756e 726f 6c6c 696e  le loop unrollin
-00015450: 6720 2a2f 0a20 2020 2020 2020 2020 2069  g */.          i
-00015460: 6628 2828 6965 2d69 6229 2025 2032 2920  f(((ie-ib) % 2) 
-00015470: 3d3d 2031 2920 7b0a 2020 2020 2020 2020  == 1) {.        
-00015480: 2020 2020 7620 2b3d 2069 6e70 7574 5b2a      v += input[*
-00015490: 6d61 7452 6f77 6e72 5d20 2a20 282a 6d61  matRownr] * (*ma
-000154a0: 7456 616c 7565 293b 0a20 2020 2020 2020  tValue);.       
-000154b0: 2020 2020 2069 622b 2b3b 0a20 2020 2020       ib++;.     
-000154c0: 2020 2020 2020 206d 6174 5661 6c75 6520         matValue 
-000154d0: 2b3d 206d 6174 5661 6c75 6553 7465 703b  += matValueStep;
-000154e0: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
-000154f0: 526f 776e 7220 2b3d 206d 6174 526f 7743  Rownr += matRowC
-00015500: 6f6c 5374 6570 3b0a 2020 2020 2020 2020  olStep;.        
-00015510: 2020 7d0a 0a20 2020 2020 2020 2020 202f    }..          /
-00015520: 2a20 5468 656e 206c 6f6f 7020 6f76 6572  * Then loop over
-00015530: 2072 656d 6169 6e69 6e67 2070 6169 7273   remaining pairs
-00015540: 206f 6620 7265 6775 6c61 7220 726f 7773   of regular rows
-00015550: 202a 2f0a 2020 2020 2020 2020 2020 7768   */.          wh
-00015560: 696c 6528 6962 203c 2069 6529 207b 0a20  ile(ib < ie) {. 
-00015570: 2020 2020 2020 2020 2020 2076 202b 3d20             v += 
-00015580: 696e 7075 745b 2a6d 6174 526f 776e 725d  input[*matRownr]
-00015590: 202a 2028 2a6d 6174 5661 6c75 6529 3b0a   * (*matValue);.
-000155a0: 2020 2020 2020 2020 2020 2020 7620 2b3d              v +=
-000155b0: 2069 6e70 7574 5b2a 286d 6174 526f 776e   input[*(matRown
-000155c0: 722b 6d61 7452 6f77 436f 6c53 7465 7029  r+matRowColStep)
-000155d0: 5d20 2a20 282a 286d 6174 5661 6c75 652b  ] * (*(matValue+
-000155e0: 6d61 7456 616c 7565 5374 6570 2929 3b0a  matValueStep));.
-000155f0: 2020 2020 2020 2020 2020 2020 6962 202b              ib +
-00015600: 3d20 323b 0a20 2020 2020 2020 2020 2020  = 2;.           
-00015610: 206d 6174 5661 6c75 6520 2b3d 2032 2a6d   matValue += 2*m
-00015620: 6174 5661 6c75 6553 7465 703b 0a20 2020  atValueStep;.   
-00015630: 2020 2020 2020 2020 206d 6174 526f 776e           matRown
-00015640: 7220 2b3d 2032 2a6d 6174 526f 7743 6f6c  r += 2*matRowCol
-00015650: 5374 6570 3b0a 2020 2020 2020 2020 2020  Step;.          
-00015660: 7d0a 2365 6e64 6966 0a20 2020 2020 2020  }.#endif.       
-00015670: 207d 0a20 2020 2020 2020 202f 2a20 446f   }.        /* Do
-00015680: 2073 7061 7273 6520 696e 7075 7420 7665   sparse input ve
-00015690: 6374 6f72 2076 6572 7369 6f6e 202a 2f0a  ctor version */.
-000156a0: 2020 2020 2020 2020 656c 7365 207b 0a0a          else {..
-000156b0: 2020 2020 2020 2020 2020 2f2a 2044 6f20            /* Do 
-000156c0: 7468 6520 4f46 202a 2f0a 2020 2020 2020  the OF */.      
-000156d0: 2020 2020 6966 2869 6e63 6c75 6465 4f46      if(includeOF
-000156e0: 290a 2369 6664 6566 2044 6972 6563 7441  ).#ifdef DirectA
-000156f0: 7272 6179 4f46 0a20 2020 2020 2020 2020  rrayOF.         
-00015700: 2020 2076 202b 3d20 696e 7075 745b 305d     v += input[0]
-00015710: 202a 206c 702d 3e6f 626a 5b63 6f6c 6e72   * lp->obj[colnr
-00015720: 5d20 2a20 6f66 7363 616c 6172 3b0a 2365  ] * ofscalar;.#e
-00015730: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00015740: 7620 2b3d 2069 6e70 7574 5b30 5d20 2a20  v += input[0] * 
-00015750: 6765 745f 4f46 5f61 6374 6976 6528 6c70  get_OF_active(lp
-00015760: 2c20 7661 726e 722c 206f 6673 6361 6c61  , varnr, ofscala
-00015770: 7229 3b0a 2365 6e64 6966 0a0a 2020 2020  r);.#endif..    
-00015780: 2020 2020 2020 2f2a 2049 6e69 7469 616c        /* Initial
-00015790: 697a 6520 706f 696e 7465 7273 202a 2f0a  ize pointers */.
-000157a0: 2020 2020 2020 2020 2020 696e 7a20 3d20            inz = 
-000157b0: 313b 0a20 2020 2020 2020 2020 2072 6f77  1;.          row
-000157c0: 696e 203d 206e 7a69 6e70 7574 2b69 6e7a  in = nzinput+inz
-000157d0: 3b0a 2020 2020 2020 2020 2020 6d61 7452  ;.          matR
-000157e0: 6f77 6e72 203d 2026 434f 4c5f 4d41 545f  ownr = &COL_MAT_
-000157f0: 524f 574e 5228 6962 293b 0a20 2020 2020  ROWNR(ib);.     
-00015800: 2020 2020 206d 6174 5661 6c75 6520 3d20       matValue = 
-00015810: 2643 4f4c 5f4d 4154 5f56 414c 5545 2869  &COL_MAT_VALUE(i
-00015820: 6229 3b0a 2020 2020 2020 2020 2020 6965  b);.          ie
-00015830: 2d2d 3b0a 0a20 2020 2020 2020 2020 202f  --;..          /
-00015840: 2a20 5468 656e 206c 6f6f 7020 6f76 6572  * Then loop over
-00015850: 2061 6c6c 206e 6f6e 2d4f 4620 726f 7773   all non-OF rows
-00015860: 202a 2f0a 2020 2020 2020 2020 2020 7768   */.          wh
-00015870: 696c 6528 2869 6e7a 203c 3d20 2a6e 7a69  ile((inz <= *nzi
-00015880: 6e70 7574 2920 2626 2028 6962 203c 3d20  nput) && (ib <= 
-00015890: 6965 2929 207b 0a0a 2020 2020 2020 2020  ie)) {..        
-000158a0: 2020 202f 2a20 5472 7920 746f 2073 796e     /* Try to syn
-000158b0: 6368 726f 6e69 7a65 2061 7420 7269 6768  chronize at righ
-000158c0: 7420 2a2f 0a20 2020 2020 2020 2020 2020  t */.           
-000158d0: 2077 6869 6c65 2828 2a72 6f77 696e 203e   while((*rowin >
-000158e0: 202a 6d61 7452 6f77 6e72 2920 2626 2028   *matRownr) && (
-000158f0: 6962 203c 2069 6529 2920 7b0a 2020 2020  ib < ie)) {.    
-00015900: 2020 2020 2020 2020 2020 6962 2b2b 3b0a            ib++;.
+00013540: 2d2d 2d2d 2d2d 202a 2f0a 0a53 5441 5449  ------ */..STATI
+00013550: 4320 4d59 424f 4f4c 2067 6574 5f63 6f6c  C MYBOOL get_col
+00013560: 496e 6465 7841 286c 7072 6563 202a 6c70  IndexA(lprec *lp
+00013570: 2c20 696e 7420 7661 7273 6574 2c20 696e  , int varset, in
+00013580: 7420 2a63 6f6c 696e 6465 782c 204d 5942  t *colindex, MYB
+00013590: 4f4f 4c20 6170 7065 6e64 290a 7b0a 2020  OOL append).{.  
+000135a0: 696e 7420 2020 2020 2069 2c20 7661 726e  int      i, varn
+000135b0: 722c 2050 3165 7874 7261 4469 6d2c 2076  r, P1extraDim, v
+000135c0: 622c 2076 652c 206e 2c20 6e72 6f77 7320  b, ve, n, nrows 
+000135d0: 3d20 6c70 2d3e 726f 7773 2c20 6e73 756d  = lp->rows, nsum
+000135e0: 203d 206c 702d 3e73 756d 3b0a 2020 4d59   = lp->sum;.  MY
+000135f0: 424f 4f4c 2020 206f 6d69 7466 6978 6564  BOOL   omitfixed
+00013600: 2c20 6f6d 6974 6e6f 6e66 6978 6564 3b0a  , omitnonfixed;.
+00013610: 2020 5245 414c 2020 2020 2076 3b0a 0a20    REAL     v;.. 
+00013620: 202f 2a20 4669 6e64 2077 6861 7420 7661   /* Find what va
+00013630: 7269 6162 6c65 2072 616e 6765 2074 6f20  riable range to 
+00013640: 7363 616e 202d 2064 6566 6175 6c74 2069  scan - default i
+00013650: 7320 7b53 4341 4e5f 5553 4552 5641 5253  s {SCAN_USERVARS
+00013660: 7d20 2a2f 0a20 202f 2a20 4669 7273 7420  } */.  /* First 
+00013670: 6465 7465 726d 696e 6520 7468 6520 7374  determine the st
+00013680: 6172 7469 6e67 2070 6f73 6974 696f 6e3b  arting position;
+00013690: 2061 6464 2066 726f 6d20 7468 6520 746f   add from the to
+000136a0: 702c 2067 6f69 6e67 2064 6f77 6e20 2a2f  p, going down */
+000136b0: 0a20 2050 3165 7874 7261 4469 6d20 3d20  .  P1extraDim = 
+000136c0: 6162 7328 6c70 2d3e 5031 6578 7472 6144  abs(lp->P1extraD
+000136d0: 696d 293b 0a20 2076 6220 3d20 6e72 6f77  im);.  vb = nrow
+000136e0: 7320 2b20 313b 0a20 2069 6628 7661 7273  s + 1;.  if(vars
+000136f0: 6574 2026 2053 4341 4e5f 4152 5449 4649  et & SCAN_ARTIFI
+00013700: 4349 414c 5641 5253 290a 2020 2020 7662  CIALVARS).    vb
+00013710: 203d 206e 7375 6d20 2d20 5031 6578 7472   = nsum - P1extr
+00013720: 6144 696d 202b 2031 3b0a 2020 6966 2876  aDim + 1;.  if(v
+00013730: 6172 7365 7420 2620 5343 414e 5f55 5345  arset & SCAN_USE
+00013740: 5256 4152 5329 0a20 2020 2076 6220 3d20  RVARS).    vb = 
+00013750: 6e72 6f77 7320 2b20 313b 0a20 2069 6628  nrows + 1;.  if(
+00013760: 7661 7273 6574 2026 2053 4341 4e5f 534c  varset & SCAN_SL
+00013770: 4143 4b56 4152 5329 0a20 2020 2076 6220  ACKVARS).    vb 
+00013780: 3d20 313b 0a0a 2020 2f2a 2054 6865 6e20  = 1;..  /* Then 
+00013790: 6465 7465 726d 696e 6520 7468 6520 656e  determine the en
+000137a0: 6469 6e67 2070 6f73 6974 696f 6e2c 2061  ding position, a
+000137b0: 6464 2066 726f 6d20 7468 6520 626f 7474  dd from the bott
+000137c0: 6f6d 2c20 676f 696e 6720 7570 202a 2f0a  om, going up */.
+000137d0: 2020 7665 203d 206e 7375 6d3b 0a20 2069    ve = nsum;.  i
+000137e0: 6628 7661 7273 6574 2026 2053 4341 4e5f  f(varset & SCAN_
+000137f0: 534c 4143 4b56 4152 5329 0a20 2020 2076  SLACKVARS).    v
+00013800: 6520 3d20 6e72 6f77 733b 0a20 2069 6628  e = nrows;.  if(
+00013810: 7661 7273 6574 2026 2053 4341 4e5f 5553  varset & SCAN_US
+00013820: 4552 5641 5253 290a 2020 2020 7665 203d  ERVARS).    ve =
+00013830: 206e 7375 6d20 2d20 5031 6578 7472 6144   nsum - P1extraD
+00013840: 696d 3b0a 2020 6966 2876 6172 7365 7420  im;.  if(varset 
+00013850: 2620 5343 414e 5f41 5254 4946 4943 4941  & SCAN_ARTIFICIA
+00013860: 4c56 4152 5329 0a20 2020 2076 6520 3d20  LVARS).    ve = 
+00013870: 6e73 756d 3b0a 0a20 202f 2a20 4164 6a75  nsum;..  /* Adju
+00013880: 7374 2066 6f72 2070 6172 7469 616c 2070  st for partial p
+00013890: 7269 6369 6e67 202a 2f0a 2020 6966 2876  ricing */.  if(v
+000138a0: 6172 7365 7420 2620 5343 414e 5f50 4152  arset & SCAN_PAR
+000138b0: 5449 414c 424c 4f43 4b29 207b 0a20 2020  TIALBLOCK) {.   
+000138c0: 2053 4554 4d41 5828 7662 2c20 7061 7274   SETMAX(vb, part
+000138d0: 6961 6c5f 626c 6f63 6b53 7461 7274 286c  ial_blockStart(l
+000138e0: 702c 2046 414c 5345 2929 3b0a 2020 2020  p, FALSE));.    
+000138f0: 5345 544d 494e 2876 652c 2070 6172 7469  SETMIN(ve, parti
+00013900: 616c 5f62 6c6f 636b 456e 6428 6c70 2c20  al_blockEnd(lp, 
+00013910: 4641 4c53 4529 293b 0a20 207d 0a0a 2020  FALSE));.  }..  
+00013920: 2f2a 2044 6574 6572 6d69 6e65 2065 7863  /* Determine exc
+00013930: 6c75 7369 6f6e 2063 6f6c 756d 6e73 202a  lusion columns *
+00013940: 2f0a 2020 6f6d 6974 6669 7865 6420 3d20  /.  omitfixed = 
+00013950: 284d 5942 4f4f 4c29 2028 2876 6172 7365  (MYBOOL) ((varse
+00013960: 7420 2620 4f4d 4954 5f46 4958 4544 2920  t & OMIT_FIXED) 
+00013970: 213d 2030 293b 0a20 206f 6d69 746e 6f6e  != 0);.  omitnon
+00013980: 6669 7865 6420 3d20 284d 5942 4f4f 4c29  fixed = (MYBOOL)
+00013990: 2028 2876 6172 7365 7420 2620 4f4d 4954   ((varset & OMIT
+000139a0: 5f4e 4f4e 4649 5845 4429 2021 3d20 3029  _NONFIXED) != 0)
+000139b0: 3b0a 2020 6966 286f 6d69 7466 6978 6564  ;.  if(omitfixed
+000139c0: 2026 2620 6f6d 6974 6e6f 6e66 6978 6564   && omitnonfixed
+000139d0: 290a 2020 2020 7265 7475 726e 2846 414c  ).    return(FAL
+000139e0: 5345 293b 0a0a 2020 2f2a 2053 6361 6e20  SE);..  /* Scan 
+000139f0: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00013a00: 7320 2a2f 0a20 2069 6628 6170 7065 6e64  s */.  if(append
+00013a10: 290a 2020 2020 6e20 3d20 636f 6c69 6e64  ).    n = colind
+00013a20: 6578 5b30 5d3b 0a20 2065 6c73 650a 2020  ex[0];.  else.  
+00013a30: 2020 6e20 3d20 303b 0a20 2066 6f72 2876    n = 0;.  for(v
+00013a40: 6172 6e72 203d 2076 623b 2076 6172 6e72  arnr = vb; varnr
+00013a50: 203c 3d20 7665 3b20 7661 726e 722b 2b29   <= ve; varnr++)
+00013a60: 207b 0a0a 2020 2020 2f2a 2053 6b69 7020   {..    /* Skip 
+00013a70: 6761 7020 696e 2074 6865 2073 7065 6369  gap in the speci
+00013a80: 6669 6564 2063 6f6c 756d 6e20 7363 616e  fied column scan
+00013a90: 2072 616e 6765 2028 706f 7373 6962 6c79   range (possibly
+00013aa0: 2075 7365 7220 7661 7269 6162 6c65 7329   user variables)
+00013ab0: 202a 2f0a 2020 2020 6966 2876 6172 6e72   */.    if(varnr
+00013ac0: 203e 206e 726f 7773 2920 7b0a 2020 2020   > nrows) {.    
+00013ad0: 2020 6966 2828 7661 726e 7220 3c3d 206e    if((varnr <= n
+00013ae0: 7375 6d2d 5031 6578 7472 6144 696d 2920  sum-P1extraDim) 
+00013af0: 2626 2021 2876 6172 7365 7420 2620 5343  && !(varset & SC
+00013b00: 414e 5f55 5345 5256 4152 5329 290a 2020  AN_USERVARS)).  
+00013b10: 2020 2020 2020 636f 6e74 696e 7565 3b0a        continue;.
+00013b20: 2369 6620 310a 2020 2020 2020 2f2a 2053  #if 1.      /* S
+00013b30: 6b69 7020 656d 7074 7920 636f 6c75 6d6e  kip empty column
+00013b40: 7320 2a2f 0a20 2020 2020 2069 6628 2f2a  s */.      if(/*
+00013b50: 286c 702d 3e50 3165 7874 7261 5661 6c20  (lp->P1extraVal 
+00013b60: 3d3d 2030 2920 2626 2a2f 0a20 2020 2020  == 0) &&*/.     
+00013b70: 2020 2020 286d 6174 5f63 6f6c 6c65 6e67      (mat_colleng
+00013b80: 7468 286c 702d 3e6d 6174 412c 2076 6172  th(lp->matA, var
+00013b90: 6e72 2d6e 726f 7773 2920 3d3d 2030 2929  nr-nrows) == 0))
+00013ba0: 0a20 2020 2020 2020 2063 6f6e 7469 6e75  .        continu
+00013bb0: 653b 0a23 656e 6469 660a 2020 2020 7d0a  e;.#endif.    }.
+00013bc0: 0a20 2020 202f 2a20 4669 6e64 2069 6620  .    /* Find if 
+00013bd0: 7468 6520 7661 7269 6162 6c65 2069 7320  the variable is 
+00013be0: 696e 2074 6865 2073 636f 7065 202d 2064  in the scope - d
+00013bf0: 6566 6175 6c74 2069 7320 7b30 7d20 2a2f  efault is {0} */
+00013c00: 0a20 2020 2069 203d 206c 702d 3e69 735f  .    i = lp->is_
+00013c10: 6261 7369 635b 7661 726e 725d 3b0a 2020  basic[varnr];.  
+00013c20: 2020 6966 2828 7661 7273 6574 2026 2055    if((varset & U
+00013c30: 5345 5f42 4153 4943 5641 5253 2920 3e20  SE_BASICVARS) > 
+00013c40: 3020 2626 2028 6929 290a 2020 2020 2020  0 && (i)).      
+00013c50: 3b0a 2020 2020 656c 7365 2069 6628 2876  ;.    else if((v
+00013c60: 6172 7365 7420 2620 5553 455f 4e4f 4e42  arset & USE_NONB
+00013c70: 4153 4943 5641 5253 2920 3e20 3020 2626  ASICVARS) > 0 &&
+00013c80: 2028 2169 2929 0a20 2020 2020 203b 0a20   (!i)).      ;. 
+00013c90: 2020 2065 6c73 650a 2020 2020 2020 636f     else.      co
+00013ca0: 6e74 696e 7565 3b0a 0a20 2020 2076 203d  ntinue;..    v =
+00013cb0: 206c 702d 3e75 7062 6f5b 7661 726e 725d   lp->upbo[varnr]
+00013cc0: 3b0a 2020 2020 6966 2828 6f6d 6974 6669  ;.    if((omitfi
+00013cd0: 7865 6420 2626 2028 7620 3d3d 2030 2929  xed && (v == 0))
+00013ce0: 207c 7c0a 2020 2020 2020 2028 6f6d 6974   ||.       (omit
+00013cf0: 6e6f 6e66 6978 6564 2026 2620 2876 2021  nonfixed && (v !
+00013d00: 3d20 3029 2929 0a20 2020 2020 2063 6f6e  = 0))).      con
+00013d10: 7469 6e75 653b 0a0a 2020 2020 2f2a 2041  tinue;..    /* A
+00013d20: 7070 656e 6420 746f 206c 6973 7420 2a2f  ppend to list */
+00013d30: 0a20 2020 206e 2b2b 3b0a 2020 2020 636f  .    n++;.    co
+00013d40: 6c69 6e64 6578 5b6e 5d20 3d20 7661 726e  lindex[n] = varn
+00013d50: 723b 0a20 207d 0a20 2063 6f6c 696e 6465  r;.  }.  colinde
+00013d60: 785b 305d 203d 206e 3b0a 0a20 2072 6574  x[0] = n;..  ret
+00013d70: 7572 6e28 5452 5545 293b 0a7d 0a0a 5354  urn(TRUE);.}..ST
+00013d80: 4154 4943 2069 6e74 2070 726f 645f 4178  ATIC int prod_Ax
+00013d90: 286c 7072 6563 202a 6c70 2c20 696e 7420  (lprec *lp, int 
+00013da0: 2a63 6f6c 7461 7267 6574 2c20 5245 414c  *coltarget, REAL
+00013db0: 202a 696e 7075 742c 2069 6e74 202a 6e7a   *input, int *nz
+00013dc0: 696e 7075 742c 0a20 2020 2020 2020 2020  input,.         
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013de0: 2020 2020 2052 4541 4c20 726f 756e 647a       REAL roundz
+00013df0: 6572 6f2c 2052 4541 4c20 6f66 7363 616c  ero, REAL ofscal
+00013e00: 6172 2c0a 2020 2020 2020 2020 2020 2020  ar,.            
+00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e20: 2020 5245 414c 202a 6f75 7470 7574 2c20    REAL *output, 
+00013e30: 696e 7420 2a6e 7a6f 7574 7075 742c 2069  int *nzoutput, i
+00013e40: 6e74 2072 6f75 6e64 6d6f 6465 290a 2f2a  nt roundmode)./*
+00013e50: 2070 726f 645f 4178 2069 7320 6f6e 6c79   prod_Ax is only
+00013e60: 2075 7365 6420 696e 2066 696d 7072 6f76   used in fimprov
+00013e70: 653b 206e 6f74 6520 7468 6174 2069 7420  e; note that it 
+00013e80: 6973 204e 4f54 2056 414c 4944 4154 4544  is NOT VALIDATED
+00013e90: 2f76 6572 6966 6965 6420 6173 206f 6620  /verified as of 
+00013ea0: 3230 3033 3038 3031 202d 204b 4520 2a2f  20030801 - KE */
+00013eb0: 0a7b 0a20 2069 6e74 2020 2020 2020 6a2c  .{.  int      j,
+00013ec0: 2063 6f6c 6e72 2c20 6962 2c20 6965 2c20   colnr, ib, ie, 
+00013ed0: 7662 3b20 2f2a 2c20 7665 3b20 2a2f 0a20  vb; /*, ve; */. 
+00013ee0: 204d 5942 4f4f 4c20 2020 6c6f 6361 6c73   MYBOOL   locals
+00013ef0: 6574 2c20 6c6f 6361 6c6e 7a20 3d20 4641  et, localnz = FA
+00013f00: 4c53 452c 2069 7352 433b 0a20 204d 4154  LSE, isRC;.  MAT
+00013f10: 7265 6320 2020 2a6d 6174 203d 206c 702d  rec   *mat = lp-
+00013f20: 3e6d 6174 413b 0a20 2052 4541 4c20 2020  >matA;.  REAL   
+00013f30: 2020 7364 703b 0a20 2052 4541 4c20 2020    sdp;.  REAL   
+00013f40: 2020 2a76 616c 7565 3b0a 2020 696e 7420    *value;.  int 
+00013f50: 2020 2020 202a 726f 776e 723b 0a0a 2020       *rownr;..  
+00013f60: 2f2a 2046 696e 6420 7768 6174 2076 6172  /* Find what var
+00013f70: 6961 626c 6520 7261 6e67 6520 746f 2073  iable range to s
+00013f80: 6361 6e20 2d20 6465 6661 756c 7420 6973  can - default is
+00013f90: 207b 5343 414e 5f55 5345 5256 4152 537d   {SCAN_USERVARS}
+00013fa0: 202a 2f0a 2020 2f2a 2044 6566 696e 6520   */.  /* Define 
+00013fb0: 6465 6661 756c 7420 636f 6c75 6d6e 2074  default column t
+00013fc0: 6172 6765 7420 6966 206e 6f6e 6520 7761  arget if none wa
+00013fd0: 7320 7072 6f76 6964 6564 202a 2f0a 2020  s provided */.  
+00013fe0: 6973 5243 203d 2028 4d59 424f 4f4c 2920  isRC = (MYBOOL) 
+00013ff0: 2828 726f 756e 646d 6f64 6520 2620 4d41  ((roundmode & MA
+00014000: 545f 524f 554e 4452 4329 2021 3d20 3029  T_ROUNDRC) != 0)
+00014010: 3b0a 2020 6c6f 6361 6c73 6574 203d 2028  ;.  localset = (
+00014020: 4d59 424f 4f4c 2920 2863 6f6c 7461 7267  MYBOOL) (coltarg
+00014030: 6574 203d 3d20 4e55 4c4c 293b 0a20 2069  et == NULL);.  i
+00014040: 6628 6c6f 6361 6c73 6574 2920 7b0a 2020  f(localset) {.  
+00014050: 2020 696e 7420 7661 7273 6574 203d 2053    int varset = S
+00014060: 4341 4e5f 534c 4143 4b56 4152 5320 7c20  CAN_SLACKVARS | 
+00014070: 5343 414e 5f55 5345 5256 4152 5320 7c0a  SCAN_USERVARS |.
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014090: 2055 5345 5f42 4153 4943 5641 5253 207c   USE_BASICVARS |
+000140a0: 204f 4d49 545f 4649 5845 443b 0a20 2020   OMIT_FIXED;.   
+000140b0: 2069 6628 6973 5243 2026 2620 6973 5f70   if(isRC && is_p
+000140c0: 6976 5f6d 6f64 6528 6c70 2c20 5052 4943  iv_mode(lp, PRIC
+000140d0: 455f 5041 5254 4941 4c29 2026 2620 2169  E_PARTIAL) && !i
+000140e0: 735f 7069 765f 6d6f 6465 286c 702c 2050  s_piv_mode(lp, P
+000140f0: 5249 4345 5f46 4f52 4345 4655 4c4c 2929  RICE_FORCEFULL))
+00014100: 0a20 2020 2020 2076 6172 7365 7420 7c3d  .      varset |=
+00014110: 2053 4341 4e5f 5041 5254 4941 4c42 4c4f   SCAN_PARTIALBLO
+00014120: 434b 3b0a 2020 2020 636f 6c74 6172 6765  CK;.    coltarge
+00014130: 7420 3d20 2869 6e74 202a 2920 6d65 6d70  t = (int *) memp
+00014140: 6f6f 6c5f 6f62 7461 696e 5665 6374 6f72  ool_obtainVector
+00014150: 286c 702d 3e77 6f72 6b61 7272 6179 732c  (lp->workarrays,
+00014160: 206c 702d 3e73 756d 2b31 2c20 7369 7a65   lp->sum+1, size
+00014170: 6f66 282a 636f 6c74 6172 6765 7429 293b  of(*coltarget));
+00014180: 0a20 2020 2069 6628 2167 6574 5f63 6f6c  .    if(!get_col
+00014190: 496e 6465 7841 286c 702c 2076 6172 7365  IndexA(lp, varse
+000141a0: 742c 2063 6f6c 7461 7267 6574 2c20 4641  t, coltarget, FA
+000141b0: 4c53 4529 2920 7b0a 2020 2020 2020 6d65  LSE)) {.      me
+000141c0: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
+000141d0: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
+000141e0: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
+000141f0: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
+00014200: 2020 2020 2020 7265 7475 726e 2846 414c        return(FAL
+00014210: 5345 293b 0a20 2020 207d 0a20 207d 0a20  SE);.    }.  }. 
+00014220: 206c 6f63 616c 6e7a 203d 2028 4d59 424f   localnz = (MYBO
+00014230: 4f4c 2920 286e 7a69 6e70 7574 203d 3d20  OL) (nzinput == 
+00014240: 4e55 4c4c 293b 0a20 2069 6628 6c6f 6361  NULL);.  if(loca
+00014250: 6c6e 7a29 207b 0a20 2020 206e 7a69 6e70  lnz) {.    nzinp
+00014260: 7574 203d 2028 696e 7420 2a29 206d 656d  ut = (int *) mem
+00014270: 706f 6f6c 5f6f 6274 6169 6e56 6563 746f  pool_obtainVecto
+00014280: 7228 6c70 2d3e 776f 726b 6172 7261 7973  r(lp->workarrays
+00014290: 2c20 6c70 2d3e 726f 7773 2b31 2c20 7369  , lp->rows+1, si
+000142a0: 7a65 6f66 282a 6e7a 696e 7075 7429 293b  zeof(*nzinput));
+000142b0: 0a20 2020 2076 6563 5f63 6f6d 7072 6573  .    vec_compres
+000142c0: 7328 696e 7075 742c 2030 2c20 6c70 2d3e  s(input, 0, lp->
+000142d0: 726f 7773 2c20 6c70 2d3e 6d61 7441 2d3e  rows, lp->matA->
+000142e0: 6570 7376 616c 7565 2c20 4e55 4c4c 2c20  epsvalue, NULL, 
+000142f0: 6e7a 696e 7075 7429 3b0a 2020 7d0a 0a20  nzinput);.  }.. 
+00014300: 202f 2a20 5363 616e 2074 6865 2063 6f6c   /* Scan the col
+00014310: 756d 6e73 202a 2f0a 2020 7662 203d 2031  umns */.  vb = 1
+00014320: 3b0a 2020 2f2a 2076 6520 3d20 636f 6c74  ;.  /* ve = colt
+00014330: 6172 6765 745b 305d 3b20 2a2f 0a20 2066  arget[0]; */.  f
+00014340: 6f72 2876 6220 3d20 313b 2076 6220 3c3d  or(vb = 1; vb <=
+00014350: 2063 6f6c 7461 7267 6574 5b30 5d3b 2076   coltarget[0]; v
+00014360: 622b 2b29 207b 0a20 2020 2063 6f6c 6e72  b++) {.    colnr
+00014370: 203d 2063 6f6c 7461 7267 6574 5b76 625d   = coltarget[vb]
+00014380: 3b0a 2020 2020 6a20 3d20 6c70 2d3e 6973  ;.    j = lp->is
+00014390: 5f62 6173 6963 5b63 6f6c 6e72 5d3b 0a0a  _basic[colnr];..
+000143a0: 2020 2020 2f2a 2050 6572 666f 726d 2074      /* Perform t
+000143b0: 6865 206d 756c 7469 706c 6963 6174 696f  he multiplicatio
+000143c0: 6e20 2a2f 0a20 2020 2073 6470 203d 206f  n */.    sdp = o
+000143d0: 6673 6361 6c61 722a 696e 7075 745b 6a5d  fscalar*input[j]
+000143e0: 3b0a 2020 2020 6966 2863 6f6c 6e72 203c  ;.    if(colnr <
+000143f0: 3d20 6c70 2d3e 726f 7773 2920 2020 2020  = lp->rows)     
+00014400: 2020 2020 2020 2020 2020 2f2a 2041 2073            /* A s
+00014410: 6c61 636b 2076 6172 6961 626c 6520 6973  lack variable is
+00014420: 2069 6e20 7468 6520 6261 7369 7320 2a2f   in the basis */
+00014430: 0a20 2020 2020 206f 7574 7075 745b 636f  .      output[co
+00014440: 6c6e 725d 202b 3d20 7364 703b 0a20 2020  lnr] += sdp;.   
+00014450: 2065 6c73 6520 7b20 2020 2020 2020 2020   else {         
+00014460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014470: 2020 2020 202f 2a20 4120 6e6f 726d 616c       /* A normal
+00014480: 2076 6172 6961 626c 6520 6973 2069 6e20   variable is in 
+00014490: 7468 6520 6261 7369 7320 2a2f 0a20 2020  the basis */.   
+000144a0: 2020 2063 6f6c 6e72 202d 3d20 6c70 2d3e     colnr -= lp->
+000144b0: 726f 7773 3b0a 2020 2020 2020 6962 203d  rows;.      ib =
+000144c0: 206d 6174 2d3e 636f 6c5f 656e 645b 636f   mat->col_end[co
+000144d0: 6c6e 7220 2d20 315d 3b0a 2020 2020 2020  lnr - 1];.      
+000144e0: 6965 203d 206d 6174 2d3e 636f 6c5f 656e  ie = mat->col_en
+000144f0: 645b 636f 6c6e 725d 3b0a 2020 2020 2020  d[colnr];.      
+00014500: 726f 776e 7220 3d20 2643 4f4c 5f4d 4154  rownr = &COL_MAT
+00014510: 5f52 4f57 4e52 2869 6229 3b0a 2020 2020  _ROWNR(ib);.    
+00014520: 2020 7661 6c75 6520 3d20 2643 4f4c 5f4d    value = &COL_M
+00014530: 4154 5f56 414c 5545 2869 6229 3b0a 2020  AT_VALUE(ib);.  
+00014540: 2020 2020 666f 7228 3b20 6962 203c 2069      for(; ib < i
+00014550: 653b 0a20 2020 2020 2020 2020 2069 622b  e;.          ib+
+00014560: 2b2c 2072 6f77 6e72 202b 3d20 6d61 7452  +, rownr += matR
+00014570: 6f77 436f 6c53 7465 702c 2076 616c 7565  owColStep, value
+00014580: 202b 3d20 6d61 7456 616c 7565 5374 6570   += matValueStep
+00014590: 2920 7b0a 2020 2020 2020 2020 6f75 7470  ) {.        outp
+000145a0: 7574 5b2a 726f 776e 725d 202b 3d20 282a  ut[*rownr] += (*
+000145b0: 7661 6c75 6529 2a73 6470 3b0a 2020 2020  value)*sdp;.    
+000145c0: 2020 7d0a 2020 2020 7d0a 2020 7d0a 2020    }.    }.  }.  
+000145d0: 726f 756e 6456 6563 746f 7228 6f75 7470  roundVector(outp
+000145e0: 7574 2b31 2c20 6c70 2d3e 726f 7773 2d31  ut+1, lp->rows-1
+000145f0: 2c20 726f 756e 647a 6572 6f29 3b0a 0a20  , roundzero);.. 
+00014600: 202f 2a20 436c 6561 6e20 7570 2061 6e64   /* Clean up and
+00014610: 2072 6574 7572 6e20 2a2f 0a20 2069 6628   return */.  if(
+00014620: 6c6f 6361 6c73 6574 290a 2020 2020 6d65  localset).    me
+00014630: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
+00014640: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
+00014650: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
+00014660: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
+00014670: 2020 6966 286c 6f63 616c 6e7a 290a 2020    if(localnz).  
+00014680: 2020 6d65 6d70 6f6f 6c5f 7265 6c65 6173    mempool_releas
+00014690: 6556 6563 746f 7228 6c70 2d3e 776f 726b  eVector(lp->work
+000146a0: 6172 7261 7973 2c20 2863 6861 7220 2a29  arrays, (char *)
+000146b0: 206e 7a69 6e70 7574 2c20 4641 4c53 4529   nzinput, FALSE)
+000146c0: 3b0a 0a20 2072 6574 7572 6e28 5452 5545  ;..  return(TRUE
+000146d0: 293b 0a7d 0a0a 5354 4154 4943 2069 6e74  );.}..STATIC int
+000146e0: 2070 726f 645f 7841 286c 7072 6563 202a   prod_xA(lprec *
+000146f0: 6c70 2c20 696e 7420 2a63 6f6c 7461 7267  lp, int *coltarg
+00014700: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014720: 2020 5245 414c 202a 696e 7075 742c 2069    REAL *input, i
+00014730: 6e74 202a 6e7a 696e 7075 742c 2052 4541  nt *nzinput, REA
+00014740: 4c20 726f 756e 647a 6572 6f2c 2052 4541  L roundzero, REA
+00014750: 4c20 6f66 7363 616c 6172 2c0a 2020 2020  L ofscalar,.    
+00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014770: 2020 2020 2020 2020 2020 5245 414c 202a            REAL *
+00014780: 6f75 7470 7574 2c20 696e 7420 2a6e 7a6f  output, int *nzo
+00014790: 7574 7075 742c 2069 6e74 2072 6f75 6e64  utput, int round
+000147a0: 6d6f 6465 290a 2f2a 204e 6f74 6520 7468  mode)./* Note th
+000147b0: 6174 2074 6865 2064 6f74 2070 726f 6475  at the dot produ
+000147c0: 6374 2078 6120 6973 2073 746f 7265 6420  ct xa is stored 
+000147d0: 6174 2074 6865 2061 6374 6976 6520 636f  at the active co
+000147e0: 6c75 6d6e 2069 6e64 6578 206f 6620 412c  lumn index of A,
+000147f0: 2069 2e65 2e20 6f66 2061 2e0a 2020 2054   i.e. of a..   T
+00014800: 6869 7320 6d65 616e 7320 7468 6174 2069  his means that i
+00014810: 6620 7468 6520 6261 7369 7320 6f6e 6c79  f the basis only
+00014820: 2063 6f6e 7461 696e 7320 6e6f 6e2d 736c   contains non-sl
+00014830: 6163 6b20 7661 7269 6162 6c65 732c 206f  ack variables, o
+00014840: 7574 7075 7420 6d61 7920 706f 696e 7420  utput may point 
+00014850: 746f 0a20 2020 7468 6520 7361 6d65 2076  to.   the same v
+00014860: 6563 746f 7220 6173 2069 6e70 7574 2c20  ector as input, 
+00014870: 7769 7468 6f75 7420 6f76 6572 7772 6974  without overwrit
+00014880: 696e 6720 7468 6520 5b30 2e2e 726f 7773  ing the [0..rows
+00014890: 5d20 656c 656d 656e 7473 2e20 2a2f 0a7b  ] elements. */.{
+000148a0: 0a20 2069 6e74 2020 2020 2020 636f 6c6e  .  int      coln
+000148b0: 722c 2072 6f77 6e72 2c20 7661 726e 722c  r, rownr, varnr,
+000148c0: 2069 622c 2069 652c 2076 622c 2076 652c   ib, ie, vb, ve,
+000148d0: 206e 726f 7773 203d 206c 702d 3e72 6f77   nrows = lp->row
+000148e0: 733b 0a20 204d 5942 4f4f 4c20 2020 6c6f  s;.  MYBOOL   lo
+000148f0: 6361 6c73 6574 2c20 6c6f 6361 6c6e 7a20  calset, localnz 
+00014900: 3d20 4641 4c53 452c 2069 6e63 6c75 6465  = FALSE, include
+00014910: 4f46 2c20 6973 5243 3b0a 2020 5245 414c  OF, isRC;.  REAL
+00014920: 5850 2020 2076 6d61 783b 0a20 2020 5245  XP   vmax;.   RE
+00014930: 414c 5850 2076 3b0a 2020 696e 7420 2020  ALXP v;.  int   
+00014940: 2020 2069 6e7a 2c20 2a72 6f77 696e 2c20     inz, *rowin, 
+00014950: 636f 756e 744e 5a20 3d20 303b 0a20 204d  countNZ = 0;.  M
+00014960: 4154 7265 6320 2020 2a6d 6174 203d 206c  ATrec   *mat = l
+00014970: 702d 3e6d 6174 413b 0a20 2020 5245 414c  p->matA;.   REAL
+00014980: 2020 2020 202a 6d61 7456 616c 7565 3b0a       *matValue;.
+00014990: 2020 2069 6e74 2020 2020 2020 2a6d 6174     int      *mat
+000149a0: 526f 776e 723b 0a0a 2020 2f2a 2043 6c65  Rownr;..  /* Cle
+000149b0: 616e 206f 7574 7075 7420 6172 6561 2028  an output area (
+000149c0: 6f6e 6c79 206e 6563 6573 7361 7279 2069  only necessary i
+000149d0: 6620 7765 2061 7265 2072 6574 7572 6e69  f we are returni
+000149e0: 6e67 2074 6865 2066 756c 6c20 7665 6374  ng the full vect
+000149f0: 6f72 2920 2a2f 0a20 2069 7352 4320 3d20  or) */.  isRC = 
+00014a00: 284d 5942 4f4f 4c29 2028 2872 6f75 6e64  (MYBOOL) ((round
+00014a10: 6d6f 6465 2026 204d 4154 5f52 4f55 4e44  mode & MAT_ROUND
+00014a20: 5243 2920 213d 2030 293b 0a20 2069 6628  RC) != 0);.  if(
+00014a30: 6e7a 6f75 7470 7574 203d 3d20 4e55 4c4c  nzoutput == NULL
+00014a40: 2920 7b0a 2020 2020 6966 2869 6e70 7574  ) {.    if(input
+00014a50: 203d 3d20 6f75 7470 7574 290a 2020 2020   == output).    
+00014a60: 2020 4d45 4d43 4c45 4152 286f 7574 7075    MEMCLEAR(outpu
+00014a70: 742b 6e72 6f77 732b 312c 206c 702d 3e63  t+nrows+1, lp->c
+00014a80: 6f6c 756d 6e73 293b 0a20 2020 2065 6c73  olumns);.    els
+00014a90: 650a 2020 2020 2020 4d45 4d43 4c45 4152  e.      MEMCLEAR
+00014aa0: 286f 7574 7075 742c 206c 702d 3e73 756d  (output, lp->sum
+00014ab0: 2b31 293b 0a20 207d 0a0a 2020 2f2a 2046  +1);.  }..  /* F
+00014ac0: 696e 6420 7768 6174 2076 6172 6961 626c  ind what variabl
+00014ad0: 6520 7261 6e67 6520 746f 2073 6361 6e20  e range to scan 
+00014ae0: 2d20 6465 6661 756c 7420 6973 207b 5343  - default is {SC
+00014af0: 414e 5f55 5345 5256 4152 537d 202a 2f0a  AN_USERVARS} */.
+00014b00: 2020 2f2a 2044 6566 696e 6520 6465 6661    /* Define defa
+00014b10: 756c 7420 636f 6c75 6d6e 2074 6172 6765  ult column targe
+00014b20: 7420 6966 206e 6f6e 6520 7761 7320 7072  t if none was pr
+00014b30: 6f76 6964 6564 202a 2f0a 2020 6c6f 6361  ovided */.  loca
+00014b40: 6c73 6574 203d 2028 4d59 424f 4f4c 2920  lset = (MYBOOL) 
+00014b50: 2863 6f6c 7461 7267 6574 203d 3d20 4e55  (coltarget == NU
+00014b60: 4c4c 293b 0a20 2069 6628 6c6f 6361 6c73  LL);.  if(locals
+00014b70: 6574 2920 7b0a 2020 2020 696e 7420 7661  et) {.    int va
+00014b80: 7273 6574 203d 2053 4341 4e5f 534c 4143  rset = SCAN_SLAC
+00014b90: 4b56 4152 5320 7c20 5343 414e 5f55 5345  KVARS | SCAN_USE
+00014ba0: 5256 4152 5320 7c0a 2020 2020 2020 2020  RVARS |.        
+00014bb0: 2020 2020 2020 2020 2055 5345 5f4e 4f4e           USE_NON
+00014bc0: 4241 5349 4356 4152 5320 7c20 4f4d 4954  BASICVARS | OMIT
+00014bd0: 5f46 4958 4544 3b0a 2020 2020 6966 2869  _FIXED;.    if(i
+00014be0: 7352 4320 2626 2069 735f 7069 765f 6d6f  sRC && is_piv_mo
+00014bf0: 6465 286c 702c 2050 5249 4345 5f50 4152  de(lp, PRICE_PAR
+00014c00: 5449 414c 2920 2626 2021 6973 5f70 6976  TIAL) && !is_piv
+00014c10: 5f6d 6f64 6528 6c70 2c20 5052 4943 455f  _mode(lp, PRICE_
+00014c20: 464f 5243 4546 554c 4c29 290a 2020 2020  FORCEFULL)).    
+00014c30: 2020 7661 7273 6574 207c 3d20 5343 414e    varset |= SCAN
+00014c40: 5f50 4152 5449 414c 424c 4f43 4b3b 0a20  _PARTIALBLOCK;. 
+00014c50: 2020 2063 6f6c 7461 7267 6574 203d 2028     coltarget = (
+00014c60: 696e 7420 2a29 206d 656d 706f 6f6c 5f6f  int *) mempool_o
+00014c70: 6274 6169 6e56 6563 746f 7228 6c70 2d3e  btainVector(lp->
+00014c80: 776f 726b 6172 7261 7973 2c20 6c70 2d3e  workarrays, lp->
+00014c90: 7375 6d2b 312c 2073 697a 656f 6628 2a63  sum+1, sizeof(*c
+00014ca0: 6f6c 7461 7267 6574 2929 3b0a 2020 2020  oltarget));.    
+00014cb0: 6966 2821 6765 745f 636f 6c49 6e64 6578  if(!get_colIndex
+00014cc0: 4128 6c70 2c20 7661 7273 6574 2c20 636f  A(lp, varset, co
+00014cd0: 6c74 6172 6765 742c 2046 414c 5345 2929  ltarget, FALSE))
+00014ce0: 207b 0a20 2020 2020 206d 656d 706f 6f6c   {.      mempool
+00014cf0: 5f72 656c 6561 7365 5665 6374 6f72 286c  _releaseVector(l
+00014d00: 702d 3e77 6f72 6b61 7272 6179 732c 2028  p->workarrays, (
+00014d10: 6368 6172 202a 2920 636f 6c74 6172 6765  char *) coltarge
+00014d20: 742c 2046 414c 5345 293b 0a20 2020 2020  t, FALSE);.     
+00014d30: 2072 6574 7572 6e28 4641 4c53 4529 3b0a   return(FALSE);.
+00014d40: 2020 2020 7d0a 2020 7d0a 2f2a 2364 6566      }.  }./*#def
+00014d50: 696e 6520 5573 654c 6f63 616c 4e5a 2a2f  ine UseLocalNZ*/
+00014d60: 0a23 6966 6465 6620 5573 654c 6f63 616c  .#ifdef UseLocal
+00014d70: 4e5a 0a20 206c 6f63 616c 6e7a 203d 2028  NZ.  localnz = (
+00014d80: 4d59 424f 4f4c 2920 286e 7a69 6e70 7574  MYBOOL) (nzinput
+00014d90: 203d 3d20 4e55 4c4c 293b 0a20 2069 6628   == NULL);.  if(
+00014da0: 6c6f 6361 6c6e 7a29 207b 0a20 2020 206e  localnz) {.    n
+00014db0: 7a69 6e70 7574 203d 2028 696e 7420 2a29  zinput = (int *)
+00014dc0: 206d 656d 706f 6f6c 5f6f 6274 6169 6e56   mempool_obtainV
+00014dd0: 6563 746f 7228 6c70 2d3e 776f 726b 6172  ector(lp->workar
+00014de0: 7261 7973 2c20 6e72 6f77 732b 312c 2073  rays, nrows+1, s
+00014df0: 697a 656f 6628 2a6e 7a69 6e70 7574 2929  izeof(*nzinput))
+00014e00: 3b0a 2020 2020 7665 635f 636f 6d70 7265  ;.    vec_compre
+00014e10: 7373 2869 6e70 7574 2c20 302c 206e 726f  ss(input, 0, nro
+00014e20: 7773 2c20 6c70 2d3e 6d61 7441 2d3e 6570  ws, lp->matA->ep
+00014e30: 7376 616c 7565 2c20 4e55 4c4c 2c20 6e7a  svalue, NULL, nz
+00014e40: 696e 7075 7429 3b0a 2020 7d0a 2365 6e64  input);.  }.#end
+00014e50: 6966 0a20 2069 6e63 6c75 6465 4f46 203d  if.  includeOF =
+00014e60: 2028 4d59 424f 4f4c 2920 2828 286e 7a69   (MYBOOL) (((nzi
+00014e70: 6e70 7574 203d 3d20 4e55 4c4c 2920 7c7c  nput == NULL) ||
+00014e80: 2028 6e7a 696e 7075 745b 315d 203d 3d20   (nzinput[1] == 
+00014e90: 3029 2920 2626 0a20 2020 2020 2020 2020  0)) &&.         
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00014eb0: 696e 7075 745b 305d 2021 3d20 3029 2026  input[0] != 0) &
+00014ec0: 2620 6c70 2d3e 6f62 6a5f 696e 5f62 6173  & lp->obj_in_bas
+00014ed0: 6973 293b 0a0a 2020 2f2a 2053 6361 6e20  is);..  /* Scan 
+00014ee0: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00014ef0: 7320 2a2f 0a20 2076 6d61 7820 3d20 303b  s */.  vmax = 0;
+00014f00: 0a20 2076 6520 3d20 636f 6c74 6172 6765  .  ve = coltarge
+00014f10: 745b 305d 3b0a 2020 666f 7228 7662 203d  t[0];.  for(vb =
+00014f20: 2031 3b20 7662 203c 3d20 7665 3b20 7662   1; vb <= ve; vb
+00014f30: 2b2b 2920 7b0a 0a20 2020 2076 6172 6e72  ++) {..    varnr
+00014f40: 203d 2063 6f6c 7461 7267 6574 5b76 625d   = coltarget[vb]
+00014f50: 3b0a 0a20 2020 2069 6628 7661 726e 7220  ;..    if(varnr 
+00014f60: 3c3d 206e 726f 7773 2920 7b0a 2020 2020  <= nrows) {.    
+00014f70: 2020 7620 3d20 696e 7075 745b 7661 726e    v = input[varn
+00014f80: 725d 3b0a 2020 2020 7d0a 2020 2020 656c  r];.    }.    el
+00014f90: 7365 207b 0a20 2020 2020 2063 6f6c 6e72  se {.      colnr
+00014fa0: 203d 2076 6172 6e72 202d 206e 726f 7773   = varnr - nrows
+00014fb0: 3b0a 2020 2020 2020 7620 3d20 303b 0a20  ;.      v = 0;. 
+00014fc0: 2020 2020 2069 6220 3d20 6d61 742d 3e63       ib = mat->c
+00014fd0: 6f6c 5f65 6e64 5b63 6f6c 6e72 202d 2031  ol_end[colnr - 1
+00014fe0: 5d3b 0a20 2020 2020 2069 6520 3d20 6d61  ];.      ie = ma
+00014ff0: 742d 3e63 6f6c 5f65 6e64 5b63 6f6c 6e72  t->col_end[colnr
+00015000: 5d3b 0a20 2020 2020 2069 6628 6962 203c  ];.      if(ib <
+00015010: 2069 6529 207b 0a0a 2020 2020 2020 2020   ie) {..        
+00015020: 2f2a 2044 6f20 6465 6e73 6520 696e 7075  /* Do dense inpu
+00015030: 7420 7665 6374 6f72 2076 6572 7369 6f6e  t vector version
+00015040: 202a 2f0a 2369 6664 6566 2055 7365 4c6f   */.#ifdef UseLo
+00015050: 6361 6c4e 5a0a 2020 2020 2020 2020 6966  calNZ.        if
+00015060: 286c 6f63 616c 6e7a 207c 7c20 286e 7a69  (localnz || (nzi
+00015070: 6e70 7574 203d 3d20 4e55 4c4c 2929 207b  nput == NULL)) {
+00015080: 0a23 656c 7365 0a20 2020 2020 2020 2069  .#else.        i
+00015090: 6628 6e7a 696e 7075 7420 3d3d 204e 554c  f(nzinput == NUL
+000150a0: 4c29 207b 0a23 656e 6469 660a 2020 2020  L) {.#endif.    
+000150b0: 2020 2020 2020 2f2a 2044 6f20 7468 6520        /* Do the 
+000150c0: 4f46 202a 2f0a 2020 2020 2020 2020 2020  OF */.          
+000150d0: 6966 2869 6e63 6c75 6465 4f46 290a 2369  if(includeOF).#i
+000150e0: 6664 6566 2044 6972 6563 7441 7272 6179  fdef DirectArray
+000150f0: 4f46 0a20 2020 2020 2020 2020 2020 2076  OF.            v
+00015100: 202b 3d20 696e 7075 745b 305d 202a 206c   += input[0] * l
+00015110: 702d 3e6f 626a 5b63 6f6c 6e72 5d20 2a20  p->obj[colnr] * 
+00015120: 6f66 7363 616c 6172 3b0a 2365 6c73 650a  ofscalar;.#else.
+00015130: 2020 2020 2020 2020 2020 2020 7620 2b3d              v +=
+00015140: 2069 6e70 7574 5b30 5d20 2a20 6765 745f   input[0] * get_
+00015150: 4f46 5f61 6374 6976 6528 6c70 2c20 7661  OF_active(lp, va
+00015160: 726e 722c 206f 6673 6361 6c61 7229 3b0a  rnr, ofscalar);.
+00015170: 2365 6e64 6966 0a0a 2020 2020 2020 2020  #endif..        
+00015180: 2020 2f2a 2049 6e69 7469 616c 697a 6520    /* Initialize 
+00015190: 706f 696e 7465 7273 202a 2f0a 2020 2020  pointers */.    
+000151a0: 2020 2020 2020 6d61 7452 6f77 6e72 203d        matRownr =
+000151b0: 2026 434f 4c5f 4d41 545f 524f 574e 5228   &COL_MAT_ROWNR(
+000151c0: 6962 293b 0a20 2020 2020 2020 2020 206d  ib);.          m
+000151d0: 6174 5661 6c75 6520 3d20 2643 4f4c 5f4d  atValue = &COL_M
+000151e0: 4154 5f56 414c 5545 2869 6229 3b0a 0a20  AT_VALUE(ib);.. 
+000151f0: 2020 2020 2020 2020 202f 2a20 446f 2065           /* Do e
+00015200: 7874 7261 206c 6f6f 7020 6f70 7469 6d69  xtra loop optimi
+00015210: 7a61 7469 6f6e 2062 6173 6564 206f 6e20  zation based on 
+00015220: 7461 7267 6574 2077 696e 646f 7720 6f76  target window ov
+00015230: 6572 6c61 7073 202a 2f0a 2369 6664 6566  erlaps */.#ifdef
+00015240: 2055 7365 4c6f 6361 6c4e 5a0a 2020 2020   UseLocalNZ.    
+00015250: 2020 2020 2020 6966 2828 6962 203c 2069        if((ib < i
+00015260: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00015270: 2626 2028 636f 6c6e 7220 3c3d 202a 6e7a  && (colnr <= *nz
+00015280: 696e 7075 7429 0a20 2020 2020 2020 2020  input).         
+00015290: 2020 2020 2626 2028 434f 4c5f 4d41 545f      && (COL_MAT_
+000152a0: 524f 574e 5228 6965 2d31 2920 3e3d 206e  ROWNR(ie-1) >= n
+000152b0: 7a69 6e70 7574 5b63 6f6c 6e72 5d29 0a20  zinput[colnr]). 
+000152c0: 2020 2020 2020 2020 2020 2020 2626 2028              && (
+000152d0: 2a6d 6174 526f 776e 7220 3c3d 206e 7a69  *matRownr <= nzi
+000152e0: 6e70 7574 5b2a 6e7a 696e 7075 745d 290a  nput[*nzinput]).
+000152f0: 2020 2020 2020 2020 2020 2020 2029 0a23               ).#
+00015300: 656e 6469 660a 2369 6664 6566 204e 6f4c  endif.#ifdef NoL
+00015310: 6f6f 7055 6e72 6f6c 6c0a 2020 2020 2020  oopUnroll.      
+00015320: 2020 2020 2f2a 2054 6865 6e20 6c6f 6f70      /* Then loop
+00015330: 206f 7665 7220 616c 6c20 7265 6775 6c61   over all regula
+00015340: 7220 726f 7773 202a 2f0a 2020 2020 2020  r rows */.      
+00015350: 2020 2020 666f 7228 3b20 6962 203c 2069      for(; ib < i
+00015360: 653b 2069 622b 2b29 207b 0a20 2020 2020  e; ib++) {.     
+00015370: 2020 2020 2020 2076 202b 3d20 696e 7075         v += inpu
+00015380: 745b 2a6d 6174 526f 776e 725d 202a 2028  t[*matRownr] * (
+00015390: 2a6d 6174 5661 6c75 6529 3b0a 2020 2020  *matValue);.    
+000153a0: 2020 2020 2020 2020 6d61 7456 616c 7565          matValue
+000153b0: 202b 3d20 6d61 7456 616c 7565 5374 6570   += matValueStep
+000153c0: 3b0a 2020 2020 2020 2020 2020 2020 6d61  ;.            ma
+000153d0: 7452 6f77 6e72 202b 3d20 6d61 7452 6f77  tRownr += matRow
+000153e0: 436f 6c53 7465 703b 0a20 2020 2020 2020  ColStep;.       
+000153f0: 2020 207d 0a23 656c 7365 0a20 2020 2020     }.#else.     
+00015400: 2020 2020 202f 2a20 5072 6570 6172 6520       /* Prepare 
+00015410: 666f 7220 7369 6d70 6c65 206c 6f6f 7020  for simple loop 
+00015420: 756e 726f 6c6c 696e 6720 2a2f 0a20 2020  unrolling */.   
+00015430: 2020 2020 2020 2069 6628 2828 6965 2d69         if(((ie-i
+00015440: 6229 2025 2032 2920 3d3d 2031 2920 7b0a  b) % 2) == 1) {.
+00015450: 2020 2020 2020 2020 2020 2020 7620 2b3d              v +=
+00015460: 2069 6e70 7574 5b2a 6d61 7452 6f77 6e72   input[*matRownr
+00015470: 5d20 2a20 282a 6d61 7456 616c 7565 293b  ] * (*matValue);
+00015480: 0a20 2020 2020 2020 2020 2020 2069 622b  .            ib+
+00015490: 2b3b 0a20 2020 2020 2020 2020 2020 206d  +;.            m
+000154a0: 6174 5661 6c75 6520 2b3d 206d 6174 5661  atValue += matVa
+000154b0: 6c75 6553 7465 703b 0a20 2020 2020 2020  lueStep;.       
+000154c0: 2020 2020 206d 6174 526f 776e 7220 2b3d       matRownr +=
+000154d0: 206d 6174 526f 7743 6f6c 5374 6570 3b0a   matRowColStep;.
+000154e0: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
+000154f0: 2020 2020 2020 202f 2a20 5468 656e 206c         /* Then l
+00015500: 6f6f 7020 6f76 6572 2072 656d 6169 6e69  oop over remaini
+00015510: 6e67 2070 6169 7273 206f 6620 7265 6775  ng pairs of regu
+00015520: 6c61 7220 726f 7773 202a 2f0a 2020 2020  lar rows */.    
+00015530: 2020 2020 2020 7768 696c 6528 6962 203c        while(ib <
+00015540: 2069 6529 207b 0a20 2020 2020 2020 2020   ie) {.         
+00015550: 2020 2076 202b 3d20 696e 7075 745b 2a6d     v += input[*m
+00015560: 6174 526f 776e 725d 202a 2028 2a6d 6174  atRownr] * (*mat
+00015570: 5661 6c75 6529 3b0a 2020 2020 2020 2020  Value);.        
+00015580: 2020 2020 7620 2b3d 2069 6e70 7574 5b2a      v += input[*
+00015590: 286d 6174 526f 776e 722b 6d61 7452 6f77  (matRownr+matRow
+000155a0: 436f 6c53 7465 7029 5d20 2a20 282a 286d  ColStep)] * (*(m
+000155b0: 6174 5661 6c75 652b 6d61 7456 616c 7565  atValue+matValue
+000155c0: 5374 6570 2929 3b0a 2020 2020 2020 2020  Step));.        
+000155d0: 2020 2020 6962 202b 3d20 323b 0a20 2020      ib += 2;.   
+000155e0: 2020 2020 2020 2020 206d 6174 5661 6c75           matValu
+000155f0: 6520 2b3d 2032 2a6d 6174 5661 6c75 6553  e += 2*matValueS
+00015600: 7465 703b 0a20 2020 2020 2020 2020 2020  tep;.           
+00015610: 206d 6174 526f 776e 7220 2b3d 2032 2a6d   matRownr += 2*m
+00015620: 6174 526f 7743 6f6c 5374 6570 3b0a 2020  atRowColStep;.  
+00015630: 2020 2020 2020 2020 7d0a 2365 6e64 6966          }.#endif
+00015640: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00015650: 2020 202f 2a20 446f 2073 7061 7273 6520     /* Do sparse 
+00015660: 696e 7075 7420 7665 6374 6f72 2076 6572  input vector ver
+00015670: 7369 6f6e 202a 2f0a 2020 2020 2020 2020  sion */.        
+00015680: 656c 7365 207b 0a0a 2020 2020 2020 2020  else {..        
+00015690: 2020 2f2a 2044 6f20 7468 6520 4f46 202a    /* Do the OF *
+000156a0: 2f0a 2020 2020 2020 2020 2020 6966 2869  /.          if(i
+000156b0: 6e63 6c75 6465 4f46 290a 2369 6664 6566  ncludeOF).#ifdef
+000156c0: 2044 6972 6563 7441 7272 6179 4f46 0a20   DirectArrayOF. 
+000156d0: 2020 2020 2020 2020 2020 2076 202b 3d20             v += 
+000156e0: 696e 7075 745b 305d 202a 206c 702d 3e6f  input[0] * lp->o
+000156f0: 626a 5b63 6f6c 6e72 5d20 2a20 6f66 7363  bj[colnr] * ofsc
+00015700: 616c 6172 3b0a 2365 6c73 650a 2020 2020  alar;.#else.    
+00015710: 2020 2020 2020 2020 7620 2b3d 2069 6e70          v += inp
+00015720: 7574 5b30 5d20 2a20 6765 745f 4f46 5f61  ut[0] * get_OF_a
+00015730: 6374 6976 6528 6c70 2c20 7661 726e 722c  ctive(lp, varnr,
+00015740: 206f 6673 6361 6c61 7229 3b0a 2365 6e64   ofscalar);.#end
+00015750: 6966 0a0a 2020 2020 2020 2020 2020 2f2a  if..          /*
+00015760: 2049 6e69 7469 616c 697a 6520 706f 696e   Initialize poin
+00015770: 7465 7273 202a 2f0a 2020 2020 2020 2020  ters */.        
+00015780: 2020 696e 7a20 3d20 313b 0a20 2020 2020    inz = 1;.     
+00015790: 2020 2020 2072 6f77 696e 203d 206e 7a69       rowin = nzi
+000157a0: 6e70 7574 2b69 6e7a 3b0a 2020 2020 2020  nput+inz;.      
+000157b0: 2020 2020 6d61 7452 6f77 6e72 203d 2026      matRownr = &
+000157c0: 434f 4c5f 4d41 545f 524f 574e 5228 6962  COL_MAT_ROWNR(ib
+000157d0: 293b 0a20 2020 2020 2020 2020 206d 6174  );.          mat
+000157e0: 5661 6c75 6520 3d20 2643 4f4c 5f4d 4154  Value = &COL_MAT
+000157f0: 5f56 414c 5545 2869 6229 3b0a 2020 2020  _VALUE(ib);.    
+00015800: 2020 2020 2020 6965 2d2d 3b0a 0a20 2020        ie--;..   
+00015810: 2020 2020 2020 202f 2a20 5468 656e 206c         /* Then l
+00015820: 6f6f 7020 6f76 6572 2061 6c6c 206e 6f6e  oop over all non
+00015830: 2d4f 4620 726f 7773 202a 2f0a 2020 2020  -OF rows */.    
+00015840: 2020 2020 2020 7768 696c 6528 2869 6e7a        while((inz
+00015850: 203c 3d20 2a6e 7a69 6e70 7574 2920 2626   <= *nzinput) &&
+00015860: 2028 6962 203c 3d20 6965 2929 207b 0a0a   (ib <= ie)) {..
+00015870: 2020 2020 2020 2020 2020 202f 2a20 5472             /* Tr
+00015880: 7920 746f 2073 796e 6368 726f 6e69 7a65  y to synchronize
+00015890: 2061 7420 7269 6768 7420 2a2f 0a20 2020   at right */.   
+000158a0: 2020 2020 2020 2020 2077 6869 6c65 2828           while((
+000158b0: 2a72 6f77 696e 203e 202a 6d61 7452 6f77  *rowin > *matRow
+000158c0: 6e72 2920 2626 2028 6962 203c 2069 6529  nr) && (ib < ie)
+000158d0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+000158e0: 2020 6962 2b2b 3b0a 2020 2020 2020 2020    ib++;.        
+000158f0: 2020 2020 2020 6d61 7456 616c 7565 202b        matValue +
+00015900: 3d20 6d61 7456 616c 7565 5374 6570 3b0a  = matValueStep;.
 00015910: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00015920: 7456 616c 7565 202b 3d20 6d61 7456 616c  tValue += matVal
-00015930: 7565 5374 6570 3b0a 2020 2020 2020 2020  ueStep;.        
-00015940: 2020 2020 2020 6d61 7452 6f77 6e72 202b        matRownr +
-00015950: 3d20 6d61 7452 6f77 436f 6c53 7465 703b  = matRowColStep;
-00015960: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00015970: 2020 2020 2020 2020 2020 202f 2a20 5472             /* Tr
-00015980: 7920 746f 2073 796e 6368 726f 6e69 7a65  y to synchronize
-00015990: 2061 7420 6c65 6674 202a 2f0a 2020 2020   at left */.    
-000159a0: 2020 2020 2020 2020 7768 696c 6528 282a          while((*
-000159b0: 726f 7769 6e20 3c20 2a6d 6174 526f 776e  rowin < *matRown
-000159c0: 7229 2026 2620 2869 6e7a 203c 202a 6e7a  r) && (inz < *nz
-000159d0: 696e 7075 7429 2920 7b0a 2020 2020 2020  input)) {.      
-000159e0: 2020 2020 2020 2020 696e 7a2b 2b3b 0a20          inz++;. 
-000159f0: 2020 2020 2020 2020 2020 2020 2072 6f77               row
-00015a00: 696e 2b2b 3b0a 2020 2020 2020 2020 2020  in++;.          
-00015a10: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00015a20: 2f2a 2050 6572 666f 726d 2064 6f74 2070  /* Perform dot p
-00015a30: 726f 6475 6374 206f 7065 7261 7469 6f6e  roduct operation
-00015a40: 2069 6620 7468 6572 6520 7761 7320 6120   if there was a 
-00015a50: 6d61 7463 6820 2a2f 0a20 2020 2020 2020  match */.       
-00015a60: 2020 2020 2069 6628 2a72 6f77 696e 203d       if(*rowin =
-00015a70: 3d20 2a6d 6174 526f 776e 7229 207b 0a20  = *matRownr) {. 
-00015a80: 2020 2020 2020 2020 2020 2020 2076 202b               v +
-00015a90: 3d20 696e 7075 745b 2a72 6f77 696e 5d20  = input[*rowin] 
-00015aa0: 2a20 282a 6d61 7456 616c 7565 293b 0a20  * (*matValue);. 
-00015ab0: 2020 2020 2020 2020 2020 2020 202f 2a20               /* 
-00015ac0: 5374 6570 2066 6f72 7761 7264 2061 7420  Step forward at 
-00015ad0: 6c65 6674 202a 2f0a 2020 2020 2020 2020  left */.        
-00015ae0: 2020 2020 2020 696e 7a2b 2b3b 0a20 2020        inz++;.   
-00015af0: 2020 2020 2020 2020 2020 2072 6f77 696e             rowin
-00015b00: 2b2b 3b0a 2020 2020 2020 2020 2020 2020  ++;.            
-00015b10: 7d0a 2020 2020 2020 2020 2020 7d0a 2020  }.          }.  
-00015b20: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
-00015b30: 2020 2020 2020 6966 2828 726f 756e 646d        if((roundm
-00015b40: 6f64 6520 2620 4d41 545f 524f 554e 4441  ode & MAT_ROUNDA
-00015b50: 4253 2920 213d 2030 2920 7b0a 2020 2020  BS) != 0) {.    
-00015b60: 2020 2020 6d79 5f72 6f75 6e64 7a65 726f      my_roundzero
-00015b70: 2876 2c20 726f 756e 647a 6572 6f29 3b0a  (v, roundzero);.
-00015b80: 2020 2020 2020 7d0a 2020 2020 7d0a 0a20        }.    }.. 
-00015b90: 2020 202f 2a20 5370 6563 6961 6c20 6861     /* Special ha
-00015ba0: 6e64 6c69 6e67 206f 6620 736d 616c 6c20  ndling of small 
-00015bb0: 7265 6475 6365 6420 636f 7374 2076 616c  reduced cost val
-00015bc0: 7565 7320 2a2f 0a20 2020 2069 6628 2169  ues */.    if(!i
-00015bd0: 7352 4320 7c7c 2028 6d79 5f63 6873 6967  sRC || (my_chsig
-00015be0: 6e28 6c70 2d3e 6973 5f6c 6f77 6572 5b76  n(lp->is_lower[v
-00015bf0: 6172 6e72 5d2c 2076 2920 3c20 3029 2920  arnr], v) < 0)) 
-00015c00: 7b0a 2020 2020 2020 5345 544d 4158 2876  {.      SETMAX(v
-00015c10: 6d61 782c 2066 6162 7328 2852 4541 4c29  max, fabs((REAL)
-00015c20: 2076 2929 3b0a 2020 2020 7d0a 2020 2020   v));.    }.    
-00015c30: 6966 2876 2021 3d20 3029 207b 0a20 2020  if(v != 0) {.   
-00015c40: 2020 2063 6f75 6e74 4e5a 2b2b 3b0a 2020     countNZ++;.  
-00015c50: 2020 2020 6966 286e 7a6f 7574 7075 7420      if(nzoutput 
-00015c60: 213d 204e 554c 4c29 0a20 2020 2020 2020  != NULL).       
-00015c70: 206e 7a6f 7574 7075 745b 636f 756e 744e   nzoutput[countN
-00015c80: 5a5d 203d 2076 6172 6e72 3b0a 2020 2020  Z] = varnr;.    
-00015c90: 7d0a 2020 2020 6f75 7470 7574 5b76 6172  }.    output[var
-00015ca0: 6e72 5d20 3d20 2852 4541 4c29 2076 3b0a  nr] = (REAL) v;.
-00015cb0: 2020 7d0a 0a20 202f 2a20 436f 6d70 7574    }..  /* Comput
-00015cc0: 6520 7265 6475 6365 6420 636f 7374 2069  e reduced cost i
-00015cd0: 6620 7468 6973 206f 7074 696f 6e20 6973  f this option is
-00015ce0: 2061 6374 6976 6520 2a2f 0a20 2069 6628   active */.  if(
-00015cf0: 6973 5243 2026 2620 216c 702d 3e6f 626a  isRC && !lp->obj
-00015d00: 5f69 6e5f 6261 7369 7329 0a20 2020 2063  _in_basis).    c
-00015d10: 6f75 6e74 4e5a 203d 2067 6574 5f62 6173  ountNZ = get_bas
-00015d20: 6973 4f46 286c 702c 2063 6f6c 7461 7267  isOF(lp, coltarg
-00015d30: 6574 2c20 6f75 7470 7574 2c20 6e7a 6f75  et, output, nzou
-00015d40: 7470 7574 293b 0a0a 2020 2f2a 2043 6865  tput);..  /* Che
-00015d50: 636b 2069 6620 7765 2073 686f 756c 6420  ck if we should 
-00015d60: 646f 2072 656c 6174 6976 6520 726f 756e  do relative roun
-00015d70: 6469 6e67 202a 2f0a 2020 6966 2828 726f  ding */.  if((ro
-00015d80: 756e 646d 6f64 6520 2620 4d41 545f 524f  undmode & MAT_RO
-00015d90: 554e 4452 454c 2920 213d 2030 2920 7b0a  UNDREL) != 0) {.
-00015da0: 2020 2020 6966 2828 726f 756e 647a 6572      if((roundzer
-00015db0: 6f20 3e20 3029 2026 2620 286e 7a6f 7574  o > 0) && (nzout
-00015dc0: 7075 7420 213d 204e 554c 4c29 2920 7b0a  put != NULL)) {.
-00015dd0: 2020 2020 2020 6965 203d 2030 3b0a 2020        ie = 0;.  
-00015de0: 2020 2020 6966 2869 7352 4329 207b 0a20      if(isRC) {. 
-00015df0: 2020 2020 2020 2053 4554 4d41 5828 766d         SETMAX(vm
-00015e00: 6178 2c20 4d41 545f 524f 554e 4452 434d  ax, MAT_ROUNDRCM
-00015e10: 494e 293b 2020 2f2a 204d 616b 6520 7375  IN);  /* Make su
-00015e20: 7265 2077 6520 646f 6e27 7420 7573 6520  re we don't use 
-00015e30: 7665 7279 2073 6d61 6c6c 2076 616c 7565  very small value
-00015e40: 7320 2a2f 0a20 2020 2020 207d 0a20 2020  s */.      }.   
-00015e50: 2020 2076 6d61 7820 2a3d 2072 6f75 6e64     vmax *= round
-00015e60: 7a65 726f 3b0a 2020 2020 2020 666f 7228  zero;.      for(
-00015e70: 6962 203d 2031 3b20 6962 203c 3d20 636f  ib = 1; ib <= co
-00015e80: 756e 744e 5a3b 2020 6962 2b2b 2920 7b0a  untNZ;  ib++) {.
-00015e90: 2020 2020 2020 2020 726f 776e 7220 3d20          rownr = 
-00015ea0: 6e7a 6f75 7470 7574 5b69 625d 3b0a 2020  nzoutput[ib];.  
-00015eb0: 2020 2020 2020 6966 2866 6162 7328 6f75        if(fabs(ou
-00015ec0: 7470 7574 5b72 6f77 6e72 5d29 203c 2076  tput[rownr]) < v
-00015ed0: 6d61 7829 0a20 2020 2020 2020 2020 206f  max).          o
-00015ee0: 7574 7075 745b 726f 776e 725d 203d 2030  utput[rownr] = 0
-00015ef0: 3b0a 2020 2020 2020 2020 656c 7365 207b  ;.        else {
-00015f00: 0a20 2020 2020 2020 2020 2069 652b 2b3b  .          ie++;
-00015f10: 0a20 2020 2020 2020 2020 206e 7a6f 7574  .          nzout
-00015f20: 7075 745b 6965 5d20 3d20 726f 776e 723b  put[ie] = rownr;
-00015f30: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00015f40: 207d 0a20 2020 2020 2063 6f75 6e74 4e5a   }.      countNZ
-00015f50: 203d 2069 653b 0a20 2020 207d 0a20 207d   = ie;.    }.  }
-00015f60: 0a0a 2020 2f2a 2043 6c65 616e 2075 7020  ..  /* Clean up 
-00015f70: 616e 6420 7265 7475 726e 202a 2f0a 2020  and return */.  
-00015f80: 6966 286c 6f63 616c 7365 7429 0a20 2020  if(localset).   
-00015f90: 206d 656d 706f 6f6c 5f72 656c 6561 7365   mempool_release
-00015fa0: 5665 6374 6f72 286c 702d 3e77 6f72 6b61  Vector(lp->worka
-00015fb0: 7272 6179 732c 2028 6368 6172 202a 2920  rrays, (char *) 
-00015fc0: 636f 6c74 6172 6765 742c 2046 414c 5345  coltarget, FALSE
-00015fd0: 293b 0a20 2069 6628 6c6f 6361 6c6e 7a29  );.  if(localnz)
-00015fe0: 0a20 2020 206d 656d 706f 6f6c 5f72 656c  .    mempool_rel
-00015ff0: 6561 7365 5665 6374 6f72 286c 702d 3e77  easeVector(lp->w
-00016000: 6f72 6b61 7272 6179 732c 2028 6368 6172  orkarrays, (char
-00016010: 202a 2920 6e7a 696e 7075 742c 2046 414c   *) nzinput, FAL
-00016020: 5345 293b 0a0a 2020 6966 286e 7a6f 7574  SE);..  if(nzout
-00016030: 7075 7420 213d 204e 554c 4c29 0a20 2020  put != NULL).   
-00016040: 202a 6e7a 6f75 7470 7574 203d 2063 6f75   *nzoutput = cou
-00016050: 6e74 4e5a 3b0a 2020 7265 7475 726e 2863  ntNZ;.  return(c
-00016060: 6f75 6e74 4e5a 293b 0a7d 0a0a 5354 4154  ountNZ);.}..STAT
-00016070: 4943 204d 5942 4f4f 4c20 7072 6f64 5f78  IC MYBOOL prod_x
-00016080: 4132 286c 7072 6563 202a 6c70 2c20 696e  A2(lprec *lp, in
-00016090: 7420 2a63 6f6c 7461 7267 6574 2c0a 2020  t *coltarget,.  
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160c0: 5245 414c 202a 7072 6f77 2c20 5245 414c  REAL *prow, REAL
-000160d0: 2070 726f 756e 647a 6572 6f2c 2069 6e74   proundzero, int
-000160e0: 202a 6e7a 7072 6f77 2c0a 2020 2020 2020   *nzprow,.      
-000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016100: 2020 2020 2020 2020 2020 2020 5245 414c              REAL
-00016110: 202a 6472 6f77 2c20 5245 414c 2064 726f   *drow, REAL dro
-00016120: 756e 647a 6572 6f2c 2069 6e74 202a 6e7a  undzero, int *nz
-00016130: 6472 6f77 2c0a 2020 2020 2020 2020 2020  drow,.          
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 2020 2020 2020 2020 5245 414c 206f 6673          REAL ofs
-00016160: 6361 6c61 722c 2069 6e74 2072 6f75 6e64  calar, int round
-00016170: 6d6f 6465 290a 7b0a 2020 696e 7420 2020  mode).{.  int   
-00016180: 2020 2076 6172 6e72 2c20 636f 6c6e 722c     varnr, colnr,
-00016190: 2069 622c 2069 652c 2076 622c 2076 652c   ib, ie, vb, ve,
-000161a0: 206e 726f 7773 203d 206c 702d 3e72 6f77   nrows = lp->row
-000161b0: 733b 0a20 204d 5942 4f4f 4c20 2020 696e  s;.  MYBOOL   in
-000161c0: 636c 7564 654f 462c 2069 7352 433b 0a20  cludeOF, isRC;. 
-000161d0: 2052 4541 4c58 5020 2020 646d 6178 2c20   REALXP   dmax, 
-000161e0: 706d 6178 3b0a 2020 7265 6769 7374 6572  pmax;.  register
-000161f0: 2052 4541 4c58 5020 642c 2070 3b0a 2020   REALXP d, p;.  
-00016200: 4d41 5472 6563 2020 202a 6d61 7420 3d20  MATrec   *mat = 
-00016210: 6c70 2d3e 6d61 7441 3b0a 2020 5245 414c  lp->matA;.  REAL
-00016220: 2020 2020 2076 616c 7565 3b0a 2020 7265       value;.  re
-00016230: 6769 7374 6572 2052 4541 4c20 2020 2020  gister REAL     
-00016240: 2a6d 6174 5661 6c75 653b 0a20 2072 6567  *matValue;.  reg
-00016250: 6973 7465 7220 696e 7420 2020 2020 202a  ister int      *
-00016260: 6d61 7452 6f77 6e72 3b0a 2020 4d59 424f  matRownr;.  MYBO
-00016270: 4f4c 206c 6f63 616c 7365 743b 0a0a 2020  OL localset;..  
-00016280: 2f2a 2046 696e 6420 7768 6174 2076 6172  /* Find what var
-00016290: 6961 626c 6520 7261 6e67 6520 746f 2073  iable range to s
-000162a0: 6361 6e20 2d20 6465 6661 756c 7420 6973  can - default is
-000162b0: 207b 5343 414e 5f55 5345 5256 4152 537d   {SCAN_USERVARS}
-000162c0: 202a 2f0a 2020 2f2a 2046 6972 7374 2064   */.  /* First d
-000162d0: 6574 6572 6d69 6e65 2074 6865 2073 7461  etermine the sta
-000162e0: 7274 696e 6720 706f 7369 7469 6f6e 3b20  rting position; 
-000162f0: 6164 6420 6672 6f6d 2074 6865 2074 6f70  add from the top
-00016300: 2c20 676f 696e 6720 646f 776e 202a 2f0a  , going down */.
-00016310: 2020 6c6f 6361 6c73 6574 203d 2028 4d59    localset = (MY
-00016320: 424f 4f4c 2920 2863 6f6c 7461 7267 6574  BOOL) (coltarget
-00016330: 203d 3d20 4e55 4c4c 293b 0a20 2069 6628   == NULL);.  if(
-00016340: 6c6f 6361 6c73 6574 2920 7b0a 2020 2020  localset) {.    
-00016350: 696e 7420 7661 7273 6574 203d 2053 4341  int varset = SCA
-00016360: 4e5f 534c 4143 4b56 4152 5320 2b20 5343  N_SLACKVARS + SC
-00016370: 414e 5f55 5345 5256 4152 5320 2b20 2f2a  AN_USERVARS + /*
-00016380: 5343 414e 5f41 4c4c 5641 5253 202b 2a2f  SCAN_ALLVARS +*/
-00016390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000163a0: 2020 2f2a 5343 414e 5f50 4152 5449 414c    /*SCAN_PARTIAL
-000163b0: 424c 4f43 4b2b 2a2f 0a20 2020 2020 2020  BLOCK+*/.       
-000163c0: 2020 2020 2020 2020 2020 5553 455f 4e4f            USE_NO
-000163d0: 4e42 4153 4943 5641 5253 2b4f 4d49 545f  NBASICVARS+OMIT_
-000163e0: 4649 5845 443b 0a20 2020 2063 6f6c 7461  FIXED;.    colta
-000163f0: 7267 6574 203d 2028 696e 7420 2a29 206d  rget = (int *) m
-00016400: 656d 706f 6f6c 5f6f 6274 6169 6e56 6563  empool_obtainVec
-00016410: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
-00016420: 7973 2c20 6c70 2d3e 7375 6d2b 312c 2073  ys, lp->sum+1, s
-00016430: 697a 656f 6628 2a63 6f6c 7461 7267 6574  izeof(*coltarget
-00016440: 2929 3b0a 2020 2020 6966 2821 6765 745f  ));.    if(!get_
-00016450: 636f 6c49 6e64 6578 4128 6c70 2c20 7661  colIndexA(lp, va
-00016460: 7273 6574 2c20 636f 6c74 6172 6765 742c  rset, coltarget,
-00016470: 2046 414c 5345 2929 207b 0a20 2020 2020   FALSE)) {.     
-00016480: 206d 656d 706f 6f6c 5f72 656c 6561 7365   mempool_release
-00016490: 5665 6374 6f72 286c 702d 3e77 6f72 6b61  Vector(lp->worka
-000164a0: 7272 6179 732c 2028 6368 6172 202a 2920  rrays, (char *) 
-000164b0: 636f 6c74 6172 6765 742c 2046 414c 5345  coltarget, FALSE
-000164c0: 293b 0a20 2020 2020 2072 6574 7572 6e28  );.      return(
-000164d0: 4641 4c53 4529 3b0a 2020 2020 7d0a 2020  FALSE);.    }.  
-000164e0: 7d0a 0a20 202f 2a20 496e 6974 6961 6c69  }..  /* Initiali
-000164f0: 7a65 2076 6172 6961 626c 6573 202a 2f0a  ze variables */.
-00016500: 2020 6973 5243 203d 2028 4d59 424f 4f4c    isRC = (MYBOOL
-00016510: 2920 2828 726f 756e 646d 6f64 6520 2620  ) ((roundmode & 
-00016520: 4d41 545f 524f 554e 4452 4329 2021 3d20  MAT_ROUNDRC) != 
-00016530: 3029 3b0a 2020 706d 6178 203d 2030 3b0a  0);.  pmax = 0;.
-00016540: 2020 646d 6178 203d 2030 3b0a 2020 6966    dmax = 0;.  if
-00016550: 286e 7a70 726f 7720 213d 204e 554c 4c29  (nzprow != NULL)
-00016560: 0a20 2020 202a 6e7a 7072 6f77 203d 2030  .    *nzprow = 0
-00016570: 3b0a 2020 6966 286e 7a64 726f 7720 213d  ;.  if(nzdrow !=
-00016580: 204e 554c 4c29 0a20 2020 202a 6e7a 6472   NULL).    *nzdr
-00016590: 6f77 203d 2030 3b0a 2020 696e 636c 7564  ow = 0;.  includ
-000165a0: 654f 4620 3d20 284d 5942 4f4f 4c29 2028  eOF = (MYBOOL) (
-000165b0: 2828 7072 6f77 5b30 5d20 213d 2030 2920  ((prow[0] != 0) 
-000165c0: 7c7c 2028 6472 6f77 5b30 5d20 213d 2030  || (drow[0] != 0
-000165d0: 2929 2026 260a 2020 2020 2020 2020 2020  )) &&.          
-000165e0: 2020 2020 2020 2020 2020 2020 2020 6c70                lp
-000165f0: 2d3e 6f62 6a5f 696e 5f62 6173 6973 293b  ->obj_in_basis);
-00016600: 0a0a 2020 2f2a 2053 6361 6e20 7468 6520  ..  /* Scan the 
-00016610: 7461 7267 6574 2063 6f6c 756d 7320 2a2f  target colums */
-00016620: 0a20 2076 6520 3d20 636f 6c74 6172 6765  .  ve = coltarge
-00016630: 745b 305d 3b0a 2020 666f 7228 7662 203d  t[0];.  for(vb =
-00016640: 2031 3b20 7662 203c 3d20 7665 3b20 7662   1; vb <= ve; vb
-00016650: 2b2b 2920 7b0a 0a20 2020 2076 6172 6e72  ++) {..    varnr
-00016660: 203d 2063 6f6c 7461 7267 6574 5b76 625d   = coltarget[vb]
-00016670: 3b0a 0a20 2020 2069 6628 7661 726e 7220  ;..    if(varnr 
-00016680: 3c3d 206e 726f 7773 2920 7b0a 2020 2020  <= nrows) {.    
-00016690: 2020 7020 3d20 7072 6f77 5b76 6172 6e72    p = prow[varnr
-000166a0: 5d3b 0a20 2020 2020 2064 203d 2064 726f  ];.      d = dro
-000166b0: 775b 7661 726e 725d 3b0a 2020 2020 7d0a  w[varnr];.    }.
-000166c0: 2020 2020 656c 7365 207b 0a0a 2020 2020      else {..    
-000166d0: 2020 636f 6c6e 7220 3d20 7661 726e 7220    colnr = varnr 
-000166e0: 2d20 6e72 6f77 733b 0a0a 2020 2020 2020  - nrows;..      
-000166f0: 7020 3d20 303b 0a20 2020 2020 2064 203d  p = 0;.      d =
-00016700: 2030 3b0a 2020 2020 2020 6962 203d 206d   0;.      ib = m
-00016710: 6174 2d3e 636f 6c5f 656e 645b 636f 6c6e  at->col_end[coln
-00016720: 7220 2d20 315d 3b0a 2020 2020 2020 6965  r - 1];.      ie
-00016730: 203d 206d 6174 2d3e 636f 6c5f 656e 645b   = mat->col_end[
-00016740: 636f 6c6e 725d 3b0a 0a20 2020 2020 2069  colnr];..      i
-00016750: 6628 6962 203c 2069 6529 207b 0a0a 2020  f(ib < ie) {..  
-00016760: 2020 2020 2020 2f2a 2044 6f20 7468 6520        /* Do the 
-00016770: 4f46 202a 2f0a 2020 2020 2020 2020 6966  OF */.        if
-00016780: 2869 6e63 6c75 6465 4f46 2920 7b0a 2369  (includeOF) {.#i
-00016790: 6664 6566 2044 6972 6563 7441 7272 6179  fdef DirectArray
-000167a0: 4f46 0a20 2020 2020 2020 2020 2076 616c  OF.          val
-000167b0: 7565 203d 206c 702d 3e6f 626a 5b63 6f6c  ue = lp->obj[col
-000167c0: 6e72 5d20 2a20 6f66 7363 616c 6172 3b0a  nr] * ofscalar;.
-000167d0: 2365 6c73 650a 2020 2020 2020 2020 2020  #else.          
-000167e0: 7661 6c75 6520 3d20 6765 745f 4f46 5f61  value = get_OF_a
-000167f0: 6374 6976 6528 6c70 2c20 7661 726e 722c  ctive(lp, varnr,
-00016800: 206f 6673 6361 6c61 7229 3b0a 2365 6e64   ofscalar);.#end
-00016810: 6966 0a20 2020 2020 2020 2020 2070 202b  if.          p +
-00016820: 3d20 7072 6f77 5b30 5d20 2a20 7661 6c75  = prow[0] * valu
-00016830: 653b 0a20 2020 2020 2020 2020 2064 202b  e;.          d +
-00016840: 3d20 6472 6f77 5b30 5d20 2a20 7661 6c75  = drow[0] * valu
-00016850: 653b 0a20 2020 2020 2020 207d 0a0a 2020  e;.        }..  
-00016860: 2020 2020 2020 2f2a 2054 6865 6e20 6c6f        /* Then lo
-00016870: 6f70 206f 7665 7220 616c 6c20 7265 6775  op over all regu
-00016880: 6c61 7220 726f 7773 202a 2f0a 2020 2020  lar rows */.    
-00016890: 2020 2020 6d61 7452 6f77 6e72 203d 2026      matRownr = &
-000168a0: 434f 4c5f 4d41 545f 524f 574e 5228 6962  COL_MAT_ROWNR(ib
-000168b0: 293b 0a20 2020 2020 2020 206d 6174 5661  );.        matVa
-000168c0: 6c75 6520 3d20 2643 4f4c 5f4d 4154 5f56  lue = &COL_MAT_V
-000168d0: 414c 5545 2869 6229 3b0a 2369 6664 6566  ALUE(ib);.#ifdef
-000168e0: 204e 6f4c 6f6f 7055 6e72 6f6c 6c0a 2020   NoLoopUnroll.  
-000168f0: 2020 2020 2020 666f 7228 203b 2069 6220        for( ; ib 
-00016900: 3c20 6965 3b20 6962 2b2b 2920 7b0a 2020  < ie; ib++) {.  
-00016910: 2020 2020 2020 2020 7020 2b3d 2070 726f          p += pro
-00016920: 775b 2a6d 6174 526f 776e 725d 202a 2028  w[*matRownr] * (
-00016930: 2a6d 6174 5661 6c75 6529 3b0a 2020 2020  *matValue);.    
-00016940: 2020 2020 2020 6420 2b3d 2064 726f 775b        d += drow[
-00016950: 2a6d 6174 526f 776e 725d 202a 2028 2a6d  *matRownr] * (*m
-00016960: 6174 5661 6c75 6529 3b0a 2020 2020 2020  atValue);.      
-00016970: 2020 2020 6d61 7456 616c 7565 202b 3d20      matValue += 
-00016980: 6d61 7456 616c 7565 5374 6570 3b0a 2020  matValueStep;.  
-00016990: 2020 2020 2020 2020 6d61 7452 6f77 6e72          matRownr
-000169a0: 202b 3d20 6d61 7452 6f77 436f 6c53 7465   += matRowColSte
-000169b0: 703b 0a20 2020 2020 2020 207d 0a23 656c  p;.        }.#el
-000169c0: 7365 0a20 2020 2020 2020 202f 2a20 5072  se.        /* Pr
-000169d0: 6570 6172 6520 666f 7220 7369 6d70 6c65  epare for simple
-000169e0: 206c 6f6f 7020 756e 726f 6c6c 696e 6720   loop unrolling 
-000169f0: 2a2f 0a20 2020 2020 2020 2069 6628 2828  */.        if(((
-00016a00: 6965 2d69 6229 2025 2032 2920 3d3d 2031  ie-ib) % 2) == 1
-00016a10: 2920 7b0a 2020 2020 2020 2020 2020 7020  ) {.          p 
-00016a20: 2b3d 2070 726f 775b 2a6d 6174 526f 776e  += prow[*matRown
-00016a30: 725d 202a 2028 2a6d 6174 5661 6c75 6529  r] * (*matValue)
-00016a40: 3b0a 2020 2020 2020 2020 2020 6420 2b3d  ;.          d +=
-00016a50: 2064 726f 775b 2a6d 6174 526f 776e 725d   drow[*matRownr]
-00016a60: 202a 2028 2a6d 6174 5661 6c75 6529 3b0a   * (*matValue);.
-00016a70: 2020 2020 2020 2020 2020 6962 2b2b 3b0a            ib++;.
-00016a80: 2020 2020 2020 2020 2020 6d61 7456 616c            matVal
-00016a90: 7565 202b 3d20 6d61 7456 616c 7565 5374  ue += matValueSt
-00016aa0: 6570 3b0a 2020 2020 2020 2020 2020 6d61  ep;.          ma
-00016ab0: 7452 6f77 6e72 202b 3d20 6d61 7452 6f77  tRownr += matRow
-00016ac0: 436f 6c53 7465 703b 0a20 2020 2020 2020  ColStep;.       
-00016ad0: 207d 0a0a 2020 2020 2020 2020 2f2a 2054   }..        /* T
-00016ae0: 6865 6e20 6c6f 6f70 206f 7665 7220 7265  hen loop over re
-00016af0: 6d61 696e 696e 6720 7061 6972 7320 6f66  maining pairs of
-00016b00: 2072 6567 756c 6172 2072 6f77 7320 2a2f   regular rows */
-00016b10: 0a20 2020 2020 2020 2077 6869 6c65 2869  .        while(i
-00016b20: 6220 3c20 6965 2920 7b0a 2020 2020 2020  b < ie) {.      
-00016b30: 2020 2020 7020 2b3d 2070 726f 775b 2a6d      p += prow[*m
-00016b40: 6174 526f 776e 725d 202a 2028 2a6d 6174  atRownr] * (*mat
-00016b50: 5661 6c75 6529 3b0a 2020 2020 2020 2020  Value);.        
-00016b60: 2020 7020 2b3d 2070 726f 775b 2a28 6d61    p += prow[*(ma
-00016b70: 7452 6f77 6e72 2b6d 6174 526f 7743 6f6c  tRownr+matRowCol
-00016b80: 5374 6570 295d 202a 2028 2a28 6d61 7456  Step)] * (*(matV
-00016b90: 616c 7565 2b6d 6174 5661 6c75 6553 7465  alue+matValueSte
-00016ba0: 7029 293b 0a20 2020 2020 2020 2020 2064  p));.          d
-00016bb0: 202b 3d20 6472 6f77 5b2a 6d61 7452 6f77   += drow[*matRow
-00016bc0: 6e72 5d20 2a20 282a 6d61 7456 616c 7565  nr] * (*matValue
-00016bd0: 293b 0a20 2020 2020 2020 2020 2064 202b  );.          d +
-00016be0: 3d20 6472 6f77 5b2a 286d 6174 526f 776e  = drow[*(matRown
-00016bf0: 722b 6d61 7452 6f77 436f 6c53 7465 7029  r+matRowColStep)
-00016c00: 5d20 2a20 282a 286d 6174 5661 6c75 652b  ] * (*(matValue+
-00016c10: 6d61 7456 616c 7565 5374 6570 2929 3b0a  matValueStep));.
-00016c20: 2020 2020 2020 2020 2020 6962 202b 3d20            ib += 
-00016c30: 323b 0a20 2020 2020 2020 2020 206d 6174  2;.          mat
-00016c40: 5661 6c75 6520 2b3d 2032 2a6d 6174 5661  Value += 2*matVa
-00016c50: 6c75 6553 7465 703b 0a20 2020 2020 2020  lueStep;.       
-00016c60: 2020 206d 6174 526f 776e 7220 2b3d 2032     matRownr += 2
-00016c70: 2a6d 6174 526f 7743 6f6c 5374 6570 3b0a  *matRowColStep;.
-00016c80: 2020 2020 2020 2020 7d0a 2365 6e64 6966          }.#endif
-00016c90: 0a0a 2020 2020 2020 7d0a 2020 2020 2020  ..      }.      
-00016ca0: 6966 2828 726f 756e 646d 6f64 6520 2620  if((roundmode & 
-00016cb0: 4d41 545f 524f 554e 4441 4253 2920 213d  MAT_ROUNDABS) !=
-00016cc0: 2030 2920 7b0a 2020 2020 2020 2020 6d79   0) {.        my
-00016cd0: 5f72 6f75 6e64 7a65 726f 2870 2c20 7072  _roundzero(p, pr
-00016ce0: 6f75 6e64 7a65 726f 293b 0a20 2020 2020  oundzero);.     
-00016cf0: 2020 206d 795f 726f 756e 647a 6572 6f28     my_roundzero(
-00016d00: 642c 2064 726f 756e 647a 6572 6f29 3b0a  d, droundzero);.
-00016d10: 2020 2020 2020 7d0a 2020 2020 7d0a 0a20        }.    }.. 
-00016d20: 2020 2053 4554 4d41 5828 706d 6178 2c20     SETMAX(pmax, 
-00016d30: 6661 6273 2828 5245 414c 2920 7029 293b  fabs((REAL) p));
-00016d40: 0a20 2020 2070 726f 775b 7661 726e 725d  .    prow[varnr]
-00016d50: 203d 2028 5245 414c 2920 703b 0a20 2020   = (REAL) p;.   
-00016d60: 2069 6628 286e 7a70 726f 7720 213d 204e   if((nzprow != N
-00016d70: 554c 4c29 2026 2620 2870 2021 3d20 3029  ULL) && (p != 0)
-00016d80: 2920 7b0a 2020 2020 2020 282a 6e7a 7072  ) {.      (*nzpr
-00016d90: 6f77 292b 2b3b 0a20 2020 2020 206e 7a70  ow)++;.      nzp
-00016da0: 726f 775b 2a6e 7a70 726f 775d 203d 2076  row[*nzprow] = v
-00016db0: 6172 6e72 3b0a 2020 2020 7d0a 0a20 2020  arnr;.    }..   
-00016dc0: 202f 2a20 5370 6563 6961 6c20 6861 6e64   /* Special hand
-00016dd0: 6c69 6e67 206f 6620 7265 6475 6365 6420  ling of reduced 
-00016de0: 636f 7374 2072 6f75 6e64 696e 6720 2a2f  cost rounding */
-00016df0: 0a20 2020 2069 6628 2169 7352 4320 7c7c  .    if(!isRC ||
-00016e00: 2028 6d79 5f63 6873 6967 6e28 6c70 2d3e   (my_chsign(lp->
-00016e10: 6973 5f6c 6f77 6572 5b76 6172 6e72 5d2c  is_lower[varnr],
-00016e20: 2064 2920 3c20 3029 2920 7b0a 2020 2020   d) < 0)) {.    
-00016e30: 2020 5345 544d 4158 2864 6d61 782c 2066    SETMAX(dmax, f
-00016e40: 6162 7328 2852 4541 4c29 2064 2929 3b0a  abs((REAL) d));.
-00016e50: 2020 2020 7d0a 2020 2020 6472 6f77 5b76      }.    drow[v
-00016e60: 6172 6e72 5d20 3d20 2852 4541 4c29 2064  arnr] = (REAL) d
-00016e70: 3b0a 2020 2020 6966 2828 6e7a 6472 6f77  ;.    if((nzdrow
-00016e80: 2021 3d20 4e55 4c4c 2920 2626 2028 6420   != NULL) && (d 
-00016e90: 213d 2030 2929 207b 0a20 2020 2020 2028  != 0)) {.      (
-00016ea0: 2a6e 7a64 726f 7729 2b2b 3b0a 2020 2020  *nzdrow)++;.    
-00016eb0: 2020 6e7a 6472 6f77 5b2a 6e7a 6472 6f77    nzdrow[*nzdrow
-00016ec0: 5d20 3d20 7661 726e 723b 0a20 2020 207d  ] = varnr;.    }
-00016ed0: 0a20 207d 0a0a 2020 2f2a 2043 6f6d 7075  .  }..  /* Compu
-00016ee0: 7465 2072 6564 7563 6564 2063 6f73 7420  te reduced cost 
-00016ef0: 6865 7265 2069 6620 7468 6973 206f 7074  here if this opt
-00016f00: 696f 6e20 6973 2061 6374 6976 6520 2a2f  ion is active */
-00016f10: 0a20 2069 6628 2864 726f 7720 213d 2030  .  if((drow != 0
-00016f20: 2920 2626 2021 6c70 2d3e 6f62 6a5f 696e  ) && !lp->obj_in
-00016f30: 5f62 6173 6973 290a 2020 2020 6765 745f  _basis).    get_
-00016f40: 6261 7369 734f 4628 6c70 2c20 636f 6c74  basisOF(lp, colt
-00016f50: 6172 6765 742c 2064 726f 772c 206e 7a64  arget, drow, nzd
-00016f60: 726f 7729 3b0a 0a20 202f 2a20 4368 6563  row);..  /* Chec
-00016f70: 6b20 6966 2077 6520 7368 6f75 6c64 2064  k if we should d
-00016f80: 6f20 7265 6c61 7469 7665 2072 6f75 6e64  o relative round
-00016f90: 696e 6720 2a2f 0a20 2069 6628 2872 6f75  ing */.  if((rou
-00016fa0: 6e64 6d6f 6465 2026 204d 4154 5f52 4f55  ndmode & MAT_ROU
-00016fb0: 4e44 5245 4c29 2021 3d20 3029 207b 0a20  NDREL) != 0) {. 
-00016fc0: 2020 2069 6628 2870 726f 756e 647a 6572     if((proundzer
-00016fd0: 6f20 3e20 3029 2026 2620 286e 7a70 726f  o > 0) && (nzpro
-00016fe0: 7720 213d 204e 554c 4c29 2920 7b0a 2020  w != NULL)) {.  
-00016ff0: 2020 2020 6965 203d 2030 3b0a 2020 2020      ie = 0;.    
-00017000: 2020 706d 6178 202a 3d20 7072 6f75 6e64    pmax *= pround
-00017010: 7a65 726f 3b0a 2020 2020 2020 666f 7228  zero;.      for(
-00017020: 6962 203d 2031 3b20 6962 203c 3d20 2a6e  ib = 1; ib <= *n
-00017030: 7a70 726f 773b 2020 6962 2b2b 2920 7b0a  zprow;  ib++) {.
-00017040: 2020 2020 2020 2020 7661 726e 7220 3d20          varnr = 
-00017050: 6e7a 7072 6f77 5b69 625d 3b0a 2020 2020  nzprow[ib];.    
-00017060: 2020 2020 6966 2866 6162 7328 7072 6f77      if(fabs(prow
-00017070: 5b76 6172 6e72 5d29 203c 2070 6d61 7829  [varnr]) < pmax)
-00017080: 0a20 2020 2020 2020 2020 2070 726f 775b  .          prow[
-00017090: 7661 726e 725d 203d 2030 3b0a 2020 2020  varnr] = 0;.    
-000170a0: 2020 2020 656c 7365 207b 0a20 2020 2020      else {.     
-000170b0: 2020 2020 2069 652b 2b3b 0a20 2020 2020       ie++;.     
-000170c0: 2020 2020 206e 7a70 726f 775b 6965 5d20       nzprow[ie] 
-000170d0: 3d20 7661 726e 723b 0a20 2020 2020 2020  = varnr;.       
-000170e0: 207d 0a20 2020 2020 207d 0a20 2020 2020   }.      }.     
-000170f0: 202a 6e7a 7072 6f77 203d 2069 653b 0a20   *nzprow = ie;. 
-00017100: 2020 207d 0a20 2020 2069 6628 2864 726f     }.    if((dro
-00017110: 756e 647a 6572 6f20 3e20 3029 2026 2620  undzero > 0) && 
-00017120: 286e 7a64 726f 7720 213d 204e 554c 4c29  (nzdrow != NULL)
-00017130: 2920 7b0a 2020 2020 2020 6965 203d 2030  ) {.      ie = 0
-00017140: 3b0a 2020 2020 2020 6966 2869 7352 4329  ;.      if(isRC)
-00017150: 207b 0a20 2020 2020 2020 2053 4554 4d41   {.        SETMA
-00017160: 5828 646d 6178 2c20 4d41 545f 524f 554e  X(dmax, MAT_ROUN
-00017170: 4452 434d 494e 293b 2020 2f2a 204d 616b  DRCMIN);  /* Mak
-00017180: 6520 7375 7265 2077 6520 646f 6e27 7420  e sure we don't 
-00017190: 7573 6520 7665 7279 2073 6d61 6c6c 2076  use very small v
-000171a0: 616c 7565 7320 2a2f 0a20 2020 2020 207d  alues */.      }
-000171b0: 0a20 2020 2020 2064 6d61 7820 2a3d 2064  .      dmax *= d
-000171c0: 726f 756e 647a 6572 6f3b 0a20 2020 2020  roundzero;.     
-000171d0: 2066 6f72 2869 6220 3d20 313b 2069 6220   for(ib = 1; ib 
-000171e0: 3c3d 202a 6e7a 6472 6f77 3b20 2069 622b  <= *nzdrow;  ib+
-000171f0: 2b29 207b 0a20 2020 2020 2020 2076 6172  +) {.        var
-00017200: 6e72 203d 206e 7a64 726f 775b 6962 5d3b  nr = nzdrow[ib];
-00017210: 0a20 2020 2020 2020 2069 6628 6661 6273  .        if(fabs
-00017220: 2864 726f 775b 7661 726e 725d 2920 3c20  (drow[varnr]) < 
-00017230: 646d 6178 290a 2020 2020 2020 2020 2020  dmax).          
-00017240: 6472 6f77 5b76 6172 6e72 5d20 3d20 303b  drow[varnr] = 0;
-00017250: 0a20 2020 2020 2020 2065 6c73 6520 7b0a  .        else {.
-00017260: 2020 2020 2020 2020 2020 6965 2b2b 3b0a            ie++;.
-00017270: 2020 2020 2020 2020 2020 6e7a 6472 6f77            nzdrow
-00017280: 5b69 655d 203d 2076 6172 6e72 3b0a 2020  [ie] = varnr;.  
-00017290: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
-000172a0: 2020 2020 2020 2a6e 7a64 726f 7720 3d20        *nzdrow = 
-000172b0: 6965 3b0a 2020 2020 7d0a 2020 7d0a 0a20  ie;.    }.  }.. 
-000172c0: 202f 2a20 436c 6561 6e20 7570 2061 6e64   /* Clean up and
-000172d0: 2072 6574 7572 6e20 2a2f 0a20 2069 6628   return */.  if(
-000172e0: 6c6f 6361 6c73 6574 290a 2020 2020 6d65  localset).    me
-000172f0: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
-00017300: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
-00017310: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
-00017320: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
-00017330: 2020 7265 7475 726e 2820 5452 5545 2029    return( TRUE )
-00017340: 3b0a 7d0a 0a53 5441 5449 4320 766f 6964  ;.}..STATIC void
-00017350: 2062 736f 6c76 655f 7841 3228 6c70 7265   bsolve_xA2(lpre
-00017360: 6320 2a6c 702c 2069 6e74 2a20 636f 6c74  c *lp, int* colt
-00017370: 6172 6765 742c 0a20 2020 2020 2020 2020  arget,.         
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 2020 2020 2020 2069 6e74 2072 6f77           int row
-000173a0: 5f6e 7231 2c20 5245 414c 202a 7665 6374  _nr1, REAL *vect
-000173b0: 6f72 312c 2052 4541 4c20 726f 756e 647a  or1, REAL roundz
-000173c0: 6572 6f31 2c20 696e 7420 2a6e 7a76 6563  ero1, int *nzvec
-000173d0: 746f 7231 2c0a 2020 2020 2020 2020 2020  tor1,.          
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 696e 7420 726f 775f          int row_
-00017400: 6e72 322c 2052 4541 4c20 2a76 6563 746f  nr2, REAL *vecto
-00017410: 7232 2c20 5245 414c 2072 6f75 6e64 7a65  r2, REAL roundze
-00017420: 726f 322c 2069 6e74 202a 6e7a 7665 6374  ro2, int *nzvect
-00017430: 6f72 322c 2069 6e74 2072 6f75 6e64 6d6f  or2, int roundmo
-00017440: 6465 290a 7b0a 2020 5245 414c 206f 6673  de).{.  REAL ofs
-00017450: 6361 6c61 7220 3d20 312e 303b 0a0a 202f  calar = 1.0;.. /
-00017460: 2a20 436c 6561 7220 616e 6420 696e 6974  * Clear and init
-00017470: 6961 6c69 7a65 2066 6972 7374 2076 6563  ialize first vec
-00017480: 746f 7220 2a2f 0a20 2069 6628 6e7a 7665  tor */.  if(nzve
-00017490: 6374 6f72 3120 3d3d 204e 554c 4c29 0a20  ctor1 == NULL). 
-000174a0: 2020 204d 454d 434c 4541 5228 7665 6374     MEMCLEAR(vect
-000174b0: 6f72 312c 206c 702d 3e73 756d 202b 2031  or1, lp->sum + 1
-000174c0: 293b 0a20 2065 6c73 650a 2020 2020 4d45  );.  else.    ME
-000174d0: 4d43 4c45 4152 2876 6563 746f 7231 2c20  MCLEAR(vector1, 
-000174e0: 6c70 2d3e 726f 7773 202b 2031 293b 0a20  lp->rows + 1);. 
-000174f0: 2076 6563 746f 7231 5b72 6f77 5f6e 7231   vector1[row_nr1
-00017500: 5d20 3d20 313b 0a2f 2a20 2077 6f72 6b49  ] = 1;./*  workI
-00017510: 4e54 5b30 5d20 3d20 313b 0a20 2077 6f72  NT[0] = 1;.  wor
-00017520: 6b49 4e54 5b31 5d20 3d20 726f 775f 6e72  kINT[1] = row_nr
-00017530: 313b 202a 2f0a 0a20 2069 6628 7665 6374  1; */..  if(vect
-00017540: 6f72 3220 3d3d 204e 554c 4c29 207b 0a20  or2 == NULL) {. 
-00017550: 2020 206c 702d 3e62 6670 5f62 7472 616e     lp->bfp_btran
-00017560: 5f6e 6f72 6d61 6c28 6c70 2c20 7665 6374  _normal(lp, vect
-00017570: 6f72 312c 204e 554c 4c29 3b0a 2020 2020  or1, NULL);.    
-00017580: 7072 6f64 5f78 4128 6c70 2c20 636f 6c74  prod_xA(lp, colt
-00017590: 6172 6765 742c 2076 6563 746f 7231 2c20  arget, vector1, 
-000175a0: 4e55 4c4c 2c20 726f 756e 647a 6572 6f31  NULL, roundzero1
-000175b0: 2c20 6f66 7363 616c 6172 2a30 2c0a 2020  , ofscalar*0,.  
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 2020 2020 2020 2076 6563 746f 7231           vector1
-000175e0: 2c20 6e7a 7665 6374 6f72 312c 2072 6f75  , nzvector1, rou
-000175f0: 6e64 6d6f 6465 293b 0a20 207d 0a20 2065  ndmode);.  }.  e
-00017600: 6c73 6520 7b0a 0a20 2020 2f2a 2043 6c65  lse {..   /* Cle
-00017610: 6172 2061 6e64 2069 6e69 7469 616c 697a  ar and initializ
-00017620: 6520 7365 636f 6e64 2076 6563 746f 7220  e second vector 
-00017630: 2a2f 0a20 2020 2069 6628 6e7a 7665 6374  */.    if(nzvect
-00017640: 6f72 3220 3d3d 204e 554c 4c29 0a20 2020  or2 == NULL).   
-00017650: 2020 204d 454d 434c 4541 5228 7665 6374     MEMCLEAR(vect
-00017660: 6f72 322c 206c 702d 3e73 756d 202b 2031  or2, lp->sum + 1
-00017670: 293b 0a20 2020 2065 6c73 650a 2020 2020  );.    else.    
-00017680: 2020 4d45 4d43 4c45 4152 2876 6563 746f    MEMCLEAR(vecto
-00017690: 7232 2c20 6c70 2d3e 726f 7773 202b 2031  r2, lp->rows + 1
-000176a0: 293b 0a20 2020 2069 6628 6c70 2d3e 6f62  );.    if(lp->ob
-000176b0: 6a5f 696e 5f62 6173 6973 207c 7c20 2872  j_in_basis || (r
-000176c0: 6f77 5f6e 7232 203e 2030 2929 207b 0a20  ow_nr2 > 0)) {. 
-000176d0: 2020 2020 2076 6563 746f 7232 5b72 6f77       vector2[row
-000176e0: 5f6e 7232 5d20 3d20 313b 0a2f 2a20 2020  _nr2] = 1;./*   
-000176f0: 2020 2077 6f72 6b49 4e54 5b32 5d20 3d20     workINT[2] = 
-00017700: 313b 0a20 2020 2020 2077 6f72 6b49 4e54  1;.      workINT
-00017710: 5b33 5d20 3d20 726f 775f 6e72 323b 202a  [3] = row_nr2; *
-00017720: 2f0a 2020 2020 7d0a 2020 2020 656c 7365  /.    }.    else
-00017730: 0a20 2020 2020 2067 6574 5f62 6173 6973  .      get_basis
-00017740: 4f46 286c 702c 204e 554c 4c2c 2076 6563  OF(lp, NULL, vec
-00017750: 746f 7232 2c20 6e7a 7665 6374 6f72 3229  tor2, nzvector2)
-00017760: 3b0a 0a20 2020 2f2a 2041 2064 6f75 626c  ;..   /* A doubl
-00017770: 6520 4254 5241 4e20 6571 7561 7469 6f6e  e BTRAN equation
-00017780: 2073 6f6c 7665 7220 7072 6f63 6573 7320   solver process 
-00017790: 6973 2069 6d70 6c65 6d65 6e74 6564 2022  is implemented "
-000177a0: 696e 2d6c 696e 6522 2062 656c 6f77 2069  in-line" below i
-000177b0: 6e0a 2020 2020 2020 6f72 6465 7220 746f  n.      order to
-000177c0: 2073 6176 6520 7469 6d65 2061 6e64 2074   save time and t
-000177d0: 6f20 696d 706c 656d 656e 7420 6469 6666  o implement diff
-000177e0: 6572 656e 7420 726f 756e 6469 6e67 2066  erent rounding f
-000177f0: 6f72 2074 6865 2074 776f 202a 2f0a 2020  or the two */.  
-00017800: 2020 6c70 2d3e 6266 705f 6274 7261 6e5f    lp->bfp_btran_
-00017810: 646f 7562 6c65 286c 702c 2076 6563 746f  double(lp, vecto
-00017820: 7231 2c20 4e55 4c4c 2c20 7665 6374 6f72  r1, NULL, vector
-00017830: 322c 204e 554c 4c29 3b0a 0a20 2020 2f2a  2, NULL);..   /*
-00017840: 204d 756c 7469 706c 7920 736f 6c75 7469   Multiply soluti
-00017850: 6f6e 2076 6563 746f 7273 2077 6974 6820  on vectors with 
-00017860: 6d61 7472 6978 2076 616c 7565 7320 2a2f  matrix values */
-00017870: 0a20 2020 2070 726f 645f 7841 3228 6c70  .    prod_xA2(lp
-00017880: 2c20 636f 6c74 6172 6765 742c 2076 6563  , coltarget, vec
-00017890: 746f 7231 2c20 726f 756e 647a 6572 6f31  tor1, roundzero1
-000178a0: 2c20 6e7a 7665 6374 6f72 312c 0a20 2020  , nzvector1,.   
+00015920: 7452 6f77 6e72 202b 3d20 6d61 7452 6f77  tRownr += matRow
+00015930: 436f 6c53 7465 703b 0a20 2020 2020 2020  ColStep;.       
+00015940: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00015950: 2020 202f 2a20 5472 7920 746f 2073 796e     /* Try to syn
+00015960: 6368 726f 6e69 7a65 2061 7420 6c65 6674  chronize at left
+00015970: 202a 2f0a 2020 2020 2020 2020 2020 2020   */.            
+00015980: 7768 696c 6528 282a 726f 7769 6e20 3c20  while((*rowin < 
+00015990: 2a6d 6174 526f 776e 7229 2026 2620 2869  *matRownr) && (i
+000159a0: 6e7a 203c 202a 6e7a 696e 7075 7429 2920  nz < *nzinput)) 
+000159b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000159c0: 696e 7a2b 2b3b 0a20 2020 2020 2020 2020  inz++;.         
+000159d0: 2020 2020 2072 6f77 696e 2b2b 3b0a 2020       rowin++;.  
+000159e0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000159f0: 2020 2020 2020 2020 2f2a 2050 6572 666f          /* Perfo
+00015a00: 726d 2064 6f74 2070 726f 6475 6374 206f  rm dot product o
+00015a10: 7065 7261 7469 6f6e 2069 6620 7468 6572  peration if ther
+00015a20: 6520 7761 7320 6120 6d61 7463 6820 2a2f  e was a match */
+00015a30: 0a20 2020 2020 2020 2020 2020 2069 6628  .            if(
+00015a40: 2a72 6f77 696e 203d 3d20 2a6d 6174 526f  *rowin == *matRo
+00015a50: 776e 7229 207b 0a20 2020 2020 2020 2020  wnr) {.         
+00015a60: 2020 2020 2076 202b 3d20 696e 7075 745b       v += input[
+00015a70: 2a72 6f77 696e 5d20 2a20 282a 6d61 7456  *rowin] * (*matV
+00015a80: 616c 7565 293b 0a20 2020 2020 2020 2020  alue);.         
+00015a90: 2020 2020 202f 2a20 5374 6570 2066 6f72       /* Step for
+00015aa0: 7761 7264 2061 7420 6c65 6674 202a 2f0a  ward at left */.
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00015ac0: 7a2b 2b3b 0a20 2020 2020 2020 2020 2020  z++;.           
+00015ad0: 2020 2072 6f77 696e 2b2b 3b0a 2020 2020     rowin++;.    
+00015ae0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00015af0: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00015b00: 2020 2020 2020 7d0a 2020 2020 2020 6966        }.      if
+00015b10: 2828 726f 756e 646d 6f64 6520 2620 4d41  ((roundmode & MA
+00015b20: 545f 524f 554e 4441 4253 2920 213d 2030  T_ROUNDABS) != 0
+00015b30: 2920 7b0a 2020 2020 2020 2020 6d79 5f72  ) {.        my_r
+00015b40: 6f75 6e64 7a65 726f 2876 2c20 726f 756e  oundzero(v, roun
+00015b50: 647a 6572 6f29 3b0a 2020 2020 2020 7d0a  dzero);.      }.
+00015b60: 2020 2020 7d0a 0a20 2020 202f 2a20 5370      }..    /* Sp
+00015b70: 6563 6961 6c20 6861 6e64 6c69 6e67 206f  ecial handling o
+00015b80: 6620 736d 616c 6c20 7265 6475 6365 6420  f small reduced 
+00015b90: 636f 7374 2076 616c 7565 7320 2a2f 0a20  cost values */. 
+00015ba0: 2020 2069 6628 2169 7352 4320 7c7c 2028     if(!isRC || (
+00015bb0: 6d79 5f63 6873 6967 6e28 6c70 2d3e 6973  my_chsign(lp->is
+00015bc0: 5f6c 6f77 6572 5b76 6172 6e72 5d2c 2076  _lower[varnr], v
+00015bd0: 2920 3c20 3029 2920 7b0a 2020 2020 2020  ) < 0)) {.      
+00015be0: 5345 544d 4158 2876 6d61 782c 2066 6162  SETMAX(vmax, fab
+00015bf0: 7328 2852 4541 4c29 2076 2929 3b0a 2020  s((REAL) v));.  
+00015c00: 2020 7d0a 2020 2020 6966 2876 2021 3d20    }.    if(v != 
+00015c10: 3029 207b 0a20 2020 2020 2063 6f75 6e74  0) {.      count
+00015c20: 4e5a 2b2b 3b0a 2020 2020 2020 6966 286e  NZ++;.      if(n
+00015c30: 7a6f 7574 7075 7420 213d 204e 554c 4c29  zoutput != NULL)
+00015c40: 0a20 2020 2020 2020 206e 7a6f 7574 7075  .        nzoutpu
+00015c50: 745b 636f 756e 744e 5a5d 203d 2076 6172  t[countNZ] = var
+00015c60: 6e72 3b0a 2020 2020 7d0a 2020 2020 6f75  nr;.    }.    ou
+00015c70: 7470 7574 5b76 6172 6e72 5d20 3d20 2852  tput[varnr] = (R
+00015c80: 4541 4c29 2076 3b0a 2020 7d0a 0a20 202f  EAL) v;.  }..  /
+00015c90: 2a20 436f 6d70 7574 6520 7265 6475 6365  * Compute reduce
+00015ca0: 6420 636f 7374 2069 6620 7468 6973 206f  d cost if this o
+00015cb0: 7074 696f 6e20 6973 2061 6374 6976 6520  ption is active 
+00015cc0: 2a2f 0a20 2069 6628 6973 5243 2026 2620  */.  if(isRC && 
+00015cd0: 216c 702d 3e6f 626a 5f69 6e5f 6261 7369  !lp->obj_in_basi
+00015ce0: 7329 0a20 2020 2063 6f75 6e74 4e5a 203d  s).    countNZ =
+00015cf0: 2067 6574 5f62 6173 6973 4f46 286c 702c   get_basisOF(lp,
+00015d00: 2063 6f6c 7461 7267 6574 2c20 6f75 7470   coltarget, outp
+00015d10: 7574 2c20 6e7a 6f75 7470 7574 293b 0a0a  ut, nzoutput);..
+00015d20: 2020 2f2a 2043 6865 636b 2069 6620 7765    /* Check if we
+00015d30: 2073 686f 756c 6420 646f 2072 656c 6174   should do relat
+00015d40: 6976 6520 726f 756e 6469 6e67 202a 2f0a  ive rounding */.
+00015d50: 2020 6966 2828 726f 756e 646d 6f64 6520    if((roundmode 
+00015d60: 2620 4d41 545f 524f 554e 4452 454c 2920  & MAT_ROUNDREL) 
+00015d70: 213d 2030 2920 7b0a 2020 2020 6966 2828  != 0) {.    if((
+00015d80: 726f 756e 647a 6572 6f20 3e20 3029 2026  roundzero > 0) &
+00015d90: 2620 286e 7a6f 7574 7075 7420 213d 204e  & (nzoutput != N
+00015da0: 554c 4c29 2920 7b0a 2020 2020 2020 6965  ULL)) {.      ie
+00015db0: 203d 2030 3b0a 2020 2020 2020 6966 2869   = 0;.      if(i
+00015dc0: 7352 4329 207b 0a20 2020 2020 2020 2053  sRC) {.        S
+00015dd0: 4554 4d41 5828 766d 6178 2c20 4d41 545f  ETMAX(vmax, MAT_
+00015de0: 524f 554e 4452 434d 494e 293b 2020 2f2a  ROUNDRCMIN);  /*
+00015df0: 204d 616b 6520 7375 7265 2077 6520 646f   Make sure we do
+00015e00: 6e27 7420 7573 6520 7665 7279 2073 6d61  n't use very sma
+00015e10: 6c6c 2076 616c 7565 7320 2a2f 0a20 2020  ll values */.   
+00015e20: 2020 207d 0a20 2020 2020 2076 6d61 7820     }.      vmax 
+00015e30: 2a3d 2072 6f75 6e64 7a65 726f 3b0a 2020  *= roundzero;.  
+00015e40: 2020 2020 666f 7228 6962 203d 2031 3b20      for(ib = 1; 
+00015e50: 6962 203c 3d20 636f 756e 744e 5a3b 2020  ib <= countNZ;  
+00015e60: 6962 2b2b 2920 7b0a 2020 2020 2020 2020  ib++) {.        
+00015e70: 726f 776e 7220 3d20 6e7a 6f75 7470 7574  rownr = nzoutput
+00015e80: 5b69 625d 3b0a 2020 2020 2020 2020 6966  [ib];.        if
+00015e90: 2866 6162 7328 6f75 7470 7574 5b72 6f77  (fabs(output[row
+00015ea0: 6e72 5d29 203c 2076 6d61 7829 0a20 2020  nr]) < vmax).   
+00015eb0: 2020 2020 2020 206f 7574 7075 745b 726f         output[ro
+00015ec0: 776e 725d 203d 2030 3b0a 2020 2020 2020  wnr] = 0;.      
+00015ed0: 2020 656c 7365 207b 0a20 2020 2020 2020    else {.       
+00015ee0: 2020 2069 652b 2b3b 0a20 2020 2020 2020     ie++;.       
+00015ef0: 2020 206e 7a6f 7574 7075 745b 6965 5d20     nzoutput[ie] 
+00015f00: 3d20 726f 776e 723b 0a20 2020 2020 2020  = rownr;.       
+00015f10: 207d 0a20 2020 2020 207d 0a20 2020 2020   }.      }.     
+00015f20: 2063 6f75 6e74 4e5a 203d 2069 653b 0a20   countNZ = ie;. 
+00015f30: 2020 207d 0a20 207d 0a0a 2020 2f2a 2043     }.  }..  /* C
+00015f40: 6c65 616e 2075 7020 616e 6420 7265 7475  lean up and retu
+00015f50: 726e 202a 2f0a 2020 6966 286c 6f63 616c  rn */.  if(local
+00015f60: 7365 7429 0a20 2020 206d 656d 706f 6f6c  set).    mempool
+00015f70: 5f72 656c 6561 7365 5665 6374 6f72 286c  _releaseVector(l
+00015f80: 702d 3e77 6f72 6b61 7272 6179 732c 2028  p->workarrays, (
+00015f90: 6368 6172 202a 2920 636f 6c74 6172 6765  char *) coltarge
+00015fa0: 742c 2046 414c 5345 293b 0a20 2069 6628  t, FALSE);.  if(
+00015fb0: 6c6f 6361 6c6e 7a29 0a20 2020 206d 656d  localnz).    mem
+00015fc0: 706f 6f6c 5f72 656c 6561 7365 5665 6374  pool_releaseVect
+00015fd0: 6f72 286c 702d 3e77 6f72 6b61 7272 6179  or(lp->workarray
+00015fe0: 732c 2028 6368 6172 202a 2920 6e7a 696e  s, (char *) nzin
+00015ff0: 7075 742c 2046 414c 5345 293b 0a0a 2020  put, FALSE);..  
+00016000: 6966 286e 7a6f 7574 7075 7420 213d 204e  if(nzoutput != N
+00016010: 554c 4c29 0a20 2020 202a 6e7a 6f75 7470  ULL).    *nzoutp
+00016020: 7574 203d 2063 6f75 6e74 4e5a 3b0a 2020  ut = countNZ;.  
+00016030: 7265 7475 726e 2863 6f75 6e74 4e5a 293b  return(countNZ);
+00016040: 0a7d 0a0a 5354 4154 4943 204d 5942 4f4f  .}..STATIC MYBOO
+00016050: 4c20 7072 6f64 5f78 4132 286c 7072 6563  L prod_xA2(lprec
+00016060: 202a 6c70 2c20 696e 7420 2a63 6f6c 7461   *lp, int *colta
+00016070: 7267 6574 2c0a 2020 2020 2020 2020 2020  rget,.          
+00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016090: 2020 2020 2020 2020 5245 414c 202a 7072          REAL *pr
+000160a0: 6f77 2c20 5245 414c 2070 726f 756e 647a  ow, REAL proundz
+000160b0: 6572 6f2c 2069 6e74 202a 6e7a 7072 6f77  ero, int *nzprow
+000160c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000160d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160e0: 2020 2020 5245 414c 202a 6472 6f77 2c20      REAL *drow, 
+000160f0: 5245 414c 2064 726f 756e 647a 6572 6f2c  REAL droundzero,
+00016100: 2069 6e74 202a 6e7a 6472 6f77 2c0a 2020   int *nzdrow,.  
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016130: 5245 414c 206f 6673 6361 6c61 722c 2069  REAL ofscalar, i
+00016140: 6e74 2072 6f75 6e64 6d6f 6465 290a 7b0a  nt roundmode).{.
+00016150: 2020 696e 7420 2020 2020 2076 6172 6e72    int      varnr
+00016160: 2c20 636f 6c6e 722c 2069 622c 2069 652c  , colnr, ib, ie,
+00016170: 2076 622c 2076 652c 206e 726f 7773 203d   vb, ve, nrows =
+00016180: 206c 702d 3e72 6f77 733b 0a20 204d 5942   lp->rows;.  MYB
+00016190: 4f4f 4c20 2020 696e 636c 7564 654f 462c  OOL   includeOF,
+000161a0: 2069 7352 433b 0a20 2052 4541 4c58 5020   isRC;.  REALXP 
+000161b0: 2020 646d 6178 2c20 706d 6178 3b0a 2020    dmax, pmax;.  
+000161c0: 2052 4541 4c58 5020 642c 2070 3b0a 2020   REALXP d, p;.  
+000161d0: 4d41 5472 6563 2020 202a 6d61 7420 3d20  MATrec   *mat = 
+000161e0: 6c70 2d3e 6d61 7441 3b0a 2020 5245 414c  lp->matA;.  REAL
+000161f0: 2020 2020 2076 616c 7565 3b0a 2020 2052       value;.   R
+00016200: 4541 4c20 2020 2020 2a6d 6174 5661 6c75  EAL     *matValu
+00016210: 653b 0a20 2020 696e 7420 2020 2020 202a  e;.   int      *
+00016220: 6d61 7452 6f77 6e72 3b0a 2020 4d59 424f  matRownr;.  MYBO
+00016230: 4f4c 206c 6f63 616c 7365 743b 0a0a 2020  OL localset;..  
+00016240: 2f2a 2046 696e 6420 7768 6174 2076 6172  /* Find what var
+00016250: 6961 626c 6520 7261 6e67 6520 746f 2073  iable range to s
+00016260: 6361 6e20 2d20 6465 6661 756c 7420 6973  can - default is
+00016270: 207b 5343 414e 5f55 5345 5256 4152 537d   {SCAN_USERVARS}
+00016280: 202a 2f0a 2020 2f2a 2046 6972 7374 2064   */.  /* First d
+00016290: 6574 6572 6d69 6e65 2074 6865 2073 7461  etermine the sta
+000162a0: 7274 696e 6720 706f 7369 7469 6f6e 3b20  rting position; 
+000162b0: 6164 6420 6672 6f6d 2074 6865 2074 6f70  add from the top
+000162c0: 2c20 676f 696e 6720 646f 776e 202a 2f0a  , going down */.
+000162d0: 2020 6c6f 6361 6c73 6574 203d 2028 4d59    localset = (MY
+000162e0: 424f 4f4c 2920 2863 6f6c 7461 7267 6574  BOOL) (coltarget
+000162f0: 203d 3d20 4e55 4c4c 293b 0a20 2069 6628   == NULL);.  if(
+00016300: 6c6f 6361 6c73 6574 2920 7b0a 2020 2020  localset) {.    
+00016310: 696e 7420 7661 7273 6574 203d 2053 4341  int varset = SCA
+00016320: 4e5f 534c 4143 4b56 4152 5320 2b20 5343  N_SLACKVARS + SC
+00016330: 414e 5f55 5345 5256 4152 5320 2b20 2f2a  AN_USERVARS + /*
+00016340: 5343 414e 5f41 4c4c 5641 5253 202b 2a2f  SCAN_ALLVARS +*/
+00016350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016360: 2020 2f2a 5343 414e 5f50 4152 5449 414c    /*SCAN_PARTIAL
+00016370: 424c 4f43 4b2b 2a2f 0a20 2020 2020 2020  BLOCK+*/.       
+00016380: 2020 2020 2020 2020 2020 5553 455f 4e4f            USE_NO
+00016390: 4e42 4153 4943 5641 5253 2b4f 4d49 545f  NBASICVARS+OMIT_
+000163a0: 4649 5845 443b 0a20 2020 2063 6f6c 7461  FIXED;.    colta
+000163b0: 7267 6574 203d 2028 696e 7420 2a29 206d  rget = (int *) m
+000163c0: 656d 706f 6f6c 5f6f 6274 6169 6e56 6563  empool_obtainVec
+000163d0: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
+000163e0: 7973 2c20 6c70 2d3e 7375 6d2b 312c 2073  ys, lp->sum+1, s
+000163f0: 697a 656f 6628 2a63 6f6c 7461 7267 6574  izeof(*coltarget
+00016400: 2929 3b0a 2020 2020 6966 2821 6765 745f  ));.    if(!get_
+00016410: 636f 6c49 6e64 6578 4128 6c70 2c20 7661  colIndexA(lp, va
+00016420: 7273 6574 2c20 636f 6c74 6172 6765 742c  rset, coltarget,
+00016430: 2046 414c 5345 2929 207b 0a20 2020 2020   FALSE)) {.     
+00016440: 206d 656d 706f 6f6c 5f72 656c 6561 7365   mempool_release
+00016450: 5665 6374 6f72 286c 702d 3e77 6f72 6b61  Vector(lp->worka
+00016460: 7272 6179 732c 2028 6368 6172 202a 2920  rrays, (char *) 
+00016470: 636f 6c74 6172 6765 742c 2046 414c 5345  coltarget, FALSE
+00016480: 293b 0a20 2020 2020 2072 6574 7572 6e28  );.      return(
+00016490: 4641 4c53 4529 3b0a 2020 2020 7d0a 2020  FALSE);.    }.  
+000164a0: 7d0a 0a20 202f 2a20 496e 6974 6961 6c69  }..  /* Initiali
+000164b0: 7a65 2076 6172 6961 626c 6573 202a 2f0a  ze variables */.
+000164c0: 2020 6973 5243 203d 2028 4d59 424f 4f4c    isRC = (MYBOOL
+000164d0: 2920 2828 726f 756e 646d 6f64 6520 2620  ) ((roundmode & 
+000164e0: 4d41 545f 524f 554e 4452 4329 2021 3d20  MAT_ROUNDRC) != 
+000164f0: 3029 3b0a 2020 706d 6178 203d 2030 3b0a  0);.  pmax = 0;.
+00016500: 2020 646d 6178 203d 2030 3b0a 2020 6966    dmax = 0;.  if
+00016510: 286e 7a70 726f 7720 213d 204e 554c 4c29  (nzprow != NULL)
+00016520: 0a20 2020 202a 6e7a 7072 6f77 203d 2030  .    *nzprow = 0
+00016530: 3b0a 2020 6966 286e 7a64 726f 7720 213d  ;.  if(nzdrow !=
+00016540: 204e 554c 4c29 0a20 2020 202a 6e7a 6472   NULL).    *nzdr
+00016550: 6f77 203d 2030 3b0a 2020 696e 636c 7564  ow = 0;.  includ
+00016560: 654f 4620 3d20 284d 5942 4f4f 4c29 2028  eOF = (MYBOOL) (
+00016570: 2828 7072 6f77 5b30 5d20 213d 2030 2920  ((prow[0] != 0) 
+00016580: 7c7c 2028 6472 6f77 5b30 5d20 213d 2030  || (drow[0] != 0
+00016590: 2929 2026 260a 2020 2020 2020 2020 2020  )) &&.          
+000165a0: 2020 2020 2020 2020 2020 2020 2020 6c70                lp
+000165b0: 2d3e 6f62 6a5f 696e 5f62 6173 6973 293b  ->obj_in_basis);
+000165c0: 0a0a 2020 2f2a 2053 6361 6e20 7468 6520  ..  /* Scan the 
+000165d0: 7461 7267 6574 2063 6f6c 756d 7320 2a2f  target colums */
+000165e0: 0a20 2076 6520 3d20 636f 6c74 6172 6765  .  ve = coltarge
+000165f0: 745b 305d 3b0a 2020 666f 7228 7662 203d  t[0];.  for(vb =
+00016600: 2031 3b20 7662 203c 3d20 7665 3b20 7662   1; vb <= ve; vb
+00016610: 2b2b 2920 7b0a 0a20 2020 2076 6172 6e72  ++) {..    varnr
+00016620: 203d 2063 6f6c 7461 7267 6574 5b76 625d   = coltarget[vb]
+00016630: 3b0a 0a20 2020 2069 6628 7661 726e 7220  ;..    if(varnr 
+00016640: 3c3d 206e 726f 7773 2920 7b0a 2020 2020  <= nrows) {.    
+00016650: 2020 7020 3d20 7072 6f77 5b76 6172 6e72    p = prow[varnr
+00016660: 5d3b 0a20 2020 2020 2064 203d 2064 726f  ];.      d = dro
+00016670: 775b 7661 726e 725d 3b0a 2020 2020 7d0a  w[varnr];.    }.
+00016680: 2020 2020 656c 7365 207b 0a0a 2020 2020      else {..    
+00016690: 2020 636f 6c6e 7220 3d20 7661 726e 7220    colnr = varnr 
+000166a0: 2d20 6e72 6f77 733b 0a0a 2020 2020 2020  - nrows;..      
+000166b0: 7020 3d20 303b 0a20 2020 2020 2064 203d  p = 0;.      d =
+000166c0: 2030 3b0a 2020 2020 2020 6962 203d 206d   0;.      ib = m
+000166d0: 6174 2d3e 636f 6c5f 656e 645b 636f 6c6e  at->col_end[coln
+000166e0: 7220 2d20 315d 3b0a 2020 2020 2020 6965  r - 1];.      ie
+000166f0: 203d 206d 6174 2d3e 636f 6c5f 656e 645b   = mat->col_end[
+00016700: 636f 6c6e 725d 3b0a 0a20 2020 2020 2069  colnr];..      i
+00016710: 6628 6962 203c 2069 6529 207b 0a0a 2020  f(ib < ie) {..  
+00016720: 2020 2020 2020 2f2a 2044 6f20 7468 6520        /* Do the 
+00016730: 4f46 202a 2f0a 2020 2020 2020 2020 6966  OF */.        if
+00016740: 2869 6e63 6c75 6465 4f46 2920 7b0a 2369  (includeOF) {.#i
+00016750: 6664 6566 2044 6972 6563 7441 7272 6179  fdef DirectArray
+00016760: 4f46 0a20 2020 2020 2020 2020 2076 616c  OF.          val
+00016770: 7565 203d 206c 702d 3e6f 626a 5b63 6f6c  ue = lp->obj[col
+00016780: 6e72 5d20 2a20 6f66 7363 616c 6172 3b0a  nr] * ofscalar;.
+00016790: 2365 6c73 650a 2020 2020 2020 2020 2020  #else.          
+000167a0: 7661 6c75 6520 3d20 6765 745f 4f46 5f61  value = get_OF_a
+000167b0: 6374 6976 6528 6c70 2c20 7661 726e 722c  ctive(lp, varnr,
+000167c0: 206f 6673 6361 6c61 7229 3b0a 2365 6e64   ofscalar);.#end
+000167d0: 6966 0a20 2020 2020 2020 2020 2070 202b  if.          p +
+000167e0: 3d20 7072 6f77 5b30 5d20 2a20 7661 6c75  = prow[0] * valu
+000167f0: 653b 0a20 2020 2020 2020 2020 2064 202b  e;.          d +
+00016800: 3d20 6472 6f77 5b30 5d20 2a20 7661 6c75  = drow[0] * valu
+00016810: 653b 0a20 2020 2020 2020 207d 0a0a 2020  e;.        }..  
+00016820: 2020 2020 2020 2f2a 2054 6865 6e20 6c6f        /* Then lo
+00016830: 6f70 206f 7665 7220 616c 6c20 7265 6775  op over all regu
+00016840: 6c61 7220 726f 7773 202a 2f0a 2020 2020  lar rows */.    
+00016850: 2020 2020 6d61 7452 6f77 6e72 203d 2026      matRownr = &
+00016860: 434f 4c5f 4d41 545f 524f 574e 5228 6962  COL_MAT_ROWNR(ib
+00016870: 293b 0a20 2020 2020 2020 206d 6174 5661  );.        matVa
+00016880: 6c75 6520 3d20 2643 4f4c 5f4d 4154 5f56  lue = &COL_MAT_V
+00016890: 414c 5545 2869 6229 3b0a 2369 6664 6566  ALUE(ib);.#ifdef
+000168a0: 204e 6f4c 6f6f 7055 6e72 6f6c 6c0a 2020   NoLoopUnroll.  
+000168b0: 2020 2020 2020 666f 7228 203b 2069 6220        for( ; ib 
+000168c0: 3c20 6965 3b20 6962 2b2b 2920 7b0a 2020  < ie; ib++) {.  
+000168d0: 2020 2020 2020 2020 7020 2b3d 2070 726f          p += pro
+000168e0: 775b 2a6d 6174 526f 776e 725d 202a 2028  w[*matRownr] * (
+000168f0: 2a6d 6174 5661 6c75 6529 3b0a 2020 2020  *matValue);.    
+00016900: 2020 2020 2020 6420 2b3d 2064 726f 775b        d += drow[
+00016910: 2a6d 6174 526f 776e 725d 202a 2028 2a6d  *matRownr] * (*m
+00016920: 6174 5661 6c75 6529 3b0a 2020 2020 2020  atValue);.      
+00016930: 2020 2020 6d61 7456 616c 7565 202b 3d20      matValue += 
+00016940: 6d61 7456 616c 7565 5374 6570 3b0a 2020  matValueStep;.  
+00016950: 2020 2020 2020 2020 6d61 7452 6f77 6e72          matRownr
+00016960: 202b 3d20 6d61 7452 6f77 436f 6c53 7465   += matRowColSte
+00016970: 703b 0a20 2020 2020 2020 207d 0a23 656c  p;.        }.#el
+00016980: 7365 0a20 2020 2020 2020 202f 2a20 5072  se.        /* Pr
+00016990: 6570 6172 6520 666f 7220 7369 6d70 6c65  epare for simple
+000169a0: 206c 6f6f 7020 756e 726f 6c6c 696e 6720   loop unrolling 
+000169b0: 2a2f 0a20 2020 2020 2020 2069 6628 2828  */.        if(((
+000169c0: 6965 2d69 6229 2025 2032 2920 3d3d 2031  ie-ib) % 2) == 1
+000169d0: 2920 7b0a 2020 2020 2020 2020 2020 7020  ) {.          p 
+000169e0: 2b3d 2070 726f 775b 2a6d 6174 526f 776e  += prow[*matRown
+000169f0: 725d 202a 2028 2a6d 6174 5661 6c75 6529  r] * (*matValue)
+00016a00: 3b0a 2020 2020 2020 2020 2020 6420 2b3d  ;.          d +=
+00016a10: 2064 726f 775b 2a6d 6174 526f 776e 725d   drow[*matRownr]
+00016a20: 202a 2028 2a6d 6174 5661 6c75 6529 3b0a   * (*matValue);.
+00016a30: 2020 2020 2020 2020 2020 6962 2b2b 3b0a            ib++;.
+00016a40: 2020 2020 2020 2020 2020 6d61 7456 616c            matVal
+00016a50: 7565 202b 3d20 6d61 7456 616c 7565 5374  ue += matValueSt
+00016a60: 6570 3b0a 2020 2020 2020 2020 2020 6d61  ep;.          ma
+00016a70: 7452 6f77 6e72 202b 3d20 6d61 7452 6f77  tRownr += matRow
+00016a80: 436f 6c53 7465 703b 0a20 2020 2020 2020  ColStep;.       
+00016a90: 207d 0a0a 2020 2020 2020 2020 2f2a 2054   }..        /* T
+00016aa0: 6865 6e20 6c6f 6f70 206f 7665 7220 7265  hen loop over re
+00016ab0: 6d61 696e 696e 6720 7061 6972 7320 6f66  maining pairs of
+00016ac0: 2072 6567 756c 6172 2072 6f77 7320 2a2f   regular rows */
+00016ad0: 0a20 2020 2020 2020 2077 6869 6c65 2869  .        while(i
+00016ae0: 6220 3c20 6965 2920 7b0a 2020 2020 2020  b < ie) {.      
+00016af0: 2020 2020 7020 2b3d 2070 726f 775b 2a6d      p += prow[*m
+00016b00: 6174 526f 776e 725d 202a 2028 2a6d 6174  atRownr] * (*mat
+00016b10: 5661 6c75 6529 3b0a 2020 2020 2020 2020  Value);.        
+00016b20: 2020 7020 2b3d 2070 726f 775b 2a28 6d61    p += prow[*(ma
+00016b30: 7452 6f77 6e72 2b6d 6174 526f 7743 6f6c  tRownr+matRowCol
+00016b40: 5374 6570 295d 202a 2028 2a28 6d61 7456  Step)] * (*(matV
+00016b50: 616c 7565 2b6d 6174 5661 6c75 6553 7465  alue+matValueSte
+00016b60: 7029 293b 0a20 2020 2020 2020 2020 2064  p));.          d
+00016b70: 202b 3d20 6472 6f77 5b2a 6d61 7452 6f77   += drow[*matRow
+00016b80: 6e72 5d20 2a20 282a 6d61 7456 616c 7565  nr] * (*matValue
+00016b90: 293b 0a20 2020 2020 2020 2020 2064 202b  );.          d +
+00016ba0: 3d20 6472 6f77 5b2a 286d 6174 526f 776e  = drow[*(matRown
+00016bb0: 722b 6d61 7452 6f77 436f 6c53 7465 7029  r+matRowColStep)
+00016bc0: 5d20 2a20 282a 286d 6174 5661 6c75 652b  ] * (*(matValue+
+00016bd0: 6d61 7456 616c 7565 5374 6570 2929 3b0a  matValueStep));.
+00016be0: 2020 2020 2020 2020 2020 6962 202b 3d20            ib += 
+00016bf0: 323b 0a20 2020 2020 2020 2020 206d 6174  2;.          mat
+00016c00: 5661 6c75 6520 2b3d 2032 2a6d 6174 5661  Value += 2*matVa
+00016c10: 6c75 6553 7465 703b 0a20 2020 2020 2020  lueStep;.       
+00016c20: 2020 206d 6174 526f 776e 7220 2b3d 2032     matRownr += 2
+00016c30: 2a6d 6174 526f 7743 6f6c 5374 6570 3b0a  *matRowColStep;.
+00016c40: 2020 2020 2020 2020 7d0a 2365 6e64 6966          }.#endif
+00016c50: 0a0a 2020 2020 2020 7d0a 2020 2020 2020  ..      }.      
+00016c60: 6966 2828 726f 756e 646d 6f64 6520 2620  if((roundmode & 
+00016c70: 4d41 545f 524f 554e 4441 4253 2920 213d  MAT_ROUNDABS) !=
+00016c80: 2030 2920 7b0a 2020 2020 2020 2020 6d79   0) {.        my
+00016c90: 5f72 6f75 6e64 7a65 726f 2870 2c20 7072  _roundzero(p, pr
+00016ca0: 6f75 6e64 7a65 726f 293b 0a20 2020 2020  oundzero);.     
+00016cb0: 2020 206d 795f 726f 756e 647a 6572 6f28     my_roundzero(
+00016cc0: 642c 2064 726f 756e 647a 6572 6f29 3b0a  d, droundzero);.
+00016cd0: 2020 2020 2020 7d0a 2020 2020 7d0a 0a20        }.    }.. 
+00016ce0: 2020 2053 4554 4d41 5828 706d 6178 2c20     SETMAX(pmax, 
+00016cf0: 6661 6273 2828 5245 414c 2920 7029 293b  fabs((REAL) p));
+00016d00: 0a20 2020 2070 726f 775b 7661 726e 725d  .    prow[varnr]
+00016d10: 203d 2028 5245 414c 2920 703b 0a20 2020   = (REAL) p;.   
+00016d20: 2069 6628 286e 7a70 726f 7720 213d 204e   if((nzprow != N
+00016d30: 554c 4c29 2026 2620 2870 2021 3d20 3029  ULL) && (p != 0)
+00016d40: 2920 7b0a 2020 2020 2020 282a 6e7a 7072  ) {.      (*nzpr
+00016d50: 6f77 292b 2b3b 0a20 2020 2020 206e 7a70  ow)++;.      nzp
+00016d60: 726f 775b 2a6e 7a70 726f 775d 203d 2076  row[*nzprow] = v
+00016d70: 6172 6e72 3b0a 2020 2020 7d0a 0a20 2020  arnr;.    }..   
+00016d80: 202f 2a20 5370 6563 6961 6c20 6861 6e64   /* Special hand
+00016d90: 6c69 6e67 206f 6620 7265 6475 6365 6420  ling of reduced 
+00016da0: 636f 7374 2072 6f75 6e64 696e 6720 2a2f  cost rounding */
+00016db0: 0a20 2020 2069 6628 2169 7352 4320 7c7c  .    if(!isRC ||
+00016dc0: 2028 6d79 5f63 6873 6967 6e28 6c70 2d3e   (my_chsign(lp->
+00016dd0: 6973 5f6c 6f77 6572 5b76 6172 6e72 5d2c  is_lower[varnr],
+00016de0: 2064 2920 3c20 3029 2920 7b0a 2020 2020   d) < 0)) {.    
+00016df0: 2020 5345 544d 4158 2864 6d61 782c 2066    SETMAX(dmax, f
+00016e00: 6162 7328 2852 4541 4c29 2064 2929 3b0a  abs((REAL) d));.
+00016e10: 2020 2020 7d0a 2020 2020 6472 6f77 5b76      }.    drow[v
+00016e20: 6172 6e72 5d20 3d20 2852 4541 4c29 2064  arnr] = (REAL) d
+00016e30: 3b0a 2020 2020 6966 2828 6e7a 6472 6f77  ;.    if((nzdrow
+00016e40: 2021 3d20 4e55 4c4c 2920 2626 2028 6420   != NULL) && (d 
+00016e50: 213d 2030 2929 207b 0a20 2020 2020 2028  != 0)) {.      (
+00016e60: 2a6e 7a64 726f 7729 2b2b 3b0a 2020 2020  *nzdrow)++;.    
+00016e70: 2020 6e7a 6472 6f77 5b2a 6e7a 6472 6f77    nzdrow[*nzdrow
+00016e80: 5d20 3d20 7661 726e 723b 0a20 2020 207d  ] = varnr;.    }
+00016e90: 0a20 207d 0a0a 2020 2f2a 2043 6f6d 7075  .  }..  /* Compu
+00016ea0: 7465 2072 6564 7563 6564 2063 6f73 7420  te reduced cost 
+00016eb0: 6865 7265 2069 6620 7468 6973 206f 7074  here if this opt
+00016ec0: 696f 6e20 6973 2061 6374 6976 6520 2a2f  ion is active */
+00016ed0: 0a20 2069 6628 2864 726f 7720 213d 2030  .  if((drow != 0
+00016ee0: 2920 2626 2021 6c70 2d3e 6f62 6a5f 696e  ) && !lp->obj_in
+00016ef0: 5f62 6173 6973 290a 2020 2020 6765 745f  _basis).    get_
+00016f00: 6261 7369 734f 4628 6c70 2c20 636f 6c74  basisOF(lp, colt
+00016f10: 6172 6765 742c 2064 726f 772c 206e 7a64  arget, drow, nzd
+00016f20: 726f 7729 3b0a 0a20 202f 2a20 4368 6563  row);..  /* Chec
+00016f30: 6b20 6966 2077 6520 7368 6f75 6c64 2064  k if we should d
+00016f40: 6f20 7265 6c61 7469 7665 2072 6f75 6e64  o relative round
+00016f50: 696e 6720 2a2f 0a20 2069 6628 2872 6f75  ing */.  if((rou
+00016f60: 6e64 6d6f 6465 2026 204d 4154 5f52 4f55  ndmode & MAT_ROU
+00016f70: 4e44 5245 4c29 2021 3d20 3029 207b 0a20  NDREL) != 0) {. 
+00016f80: 2020 2069 6628 2870 726f 756e 647a 6572     if((proundzer
+00016f90: 6f20 3e20 3029 2026 2620 286e 7a70 726f  o > 0) && (nzpro
+00016fa0: 7720 213d 204e 554c 4c29 2920 7b0a 2020  w != NULL)) {.  
+00016fb0: 2020 2020 6965 203d 2030 3b0a 2020 2020      ie = 0;.    
+00016fc0: 2020 706d 6178 202a 3d20 7072 6f75 6e64    pmax *= pround
+00016fd0: 7a65 726f 3b0a 2020 2020 2020 666f 7228  zero;.      for(
+00016fe0: 6962 203d 2031 3b20 6962 203c 3d20 2a6e  ib = 1; ib <= *n
+00016ff0: 7a70 726f 773b 2020 6962 2b2b 2920 7b0a  zprow;  ib++) {.
+00017000: 2020 2020 2020 2020 7661 726e 7220 3d20          varnr = 
+00017010: 6e7a 7072 6f77 5b69 625d 3b0a 2020 2020  nzprow[ib];.    
+00017020: 2020 2020 6966 2866 6162 7328 7072 6f77      if(fabs(prow
+00017030: 5b76 6172 6e72 5d29 203c 2070 6d61 7829  [varnr]) < pmax)
+00017040: 0a20 2020 2020 2020 2020 2070 726f 775b  .          prow[
+00017050: 7661 726e 725d 203d 2030 3b0a 2020 2020  varnr] = 0;.    
+00017060: 2020 2020 656c 7365 207b 0a20 2020 2020      else {.     
+00017070: 2020 2020 2069 652b 2b3b 0a20 2020 2020       ie++;.     
+00017080: 2020 2020 206e 7a70 726f 775b 6965 5d20       nzprow[ie] 
+00017090: 3d20 7661 726e 723b 0a20 2020 2020 2020  = varnr;.       
+000170a0: 207d 0a20 2020 2020 207d 0a20 2020 2020   }.      }.     
+000170b0: 202a 6e7a 7072 6f77 203d 2069 653b 0a20   *nzprow = ie;. 
+000170c0: 2020 207d 0a20 2020 2069 6628 2864 726f     }.    if((dro
+000170d0: 756e 647a 6572 6f20 3e20 3029 2026 2620  undzero > 0) && 
+000170e0: 286e 7a64 726f 7720 213d 204e 554c 4c29  (nzdrow != NULL)
+000170f0: 2920 7b0a 2020 2020 2020 6965 203d 2030  ) {.      ie = 0
+00017100: 3b0a 2020 2020 2020 6966 2869 7352 4329  ;.      if(isRC)
+00017110: 207b 0a20 2020 2020 2020 2053 4554 4d41   {.        SETMA
+00017120: 5828 646d 6178 2c20 4d41 545f 524f 554e  X(dmax, MAT_ROUN
+00017130: 4452 434d 494e 293b 2020 2f2a 204d 616b  DRCMIN);  /* Mak
+00017140: 6520 7375 7265 2077 6520 646f 6e27 7420  e sure we don't 
+00017150: 7573 6520 7665 7279 2073 6d61 6c6c 2076  use very small v
+00017160: 616c 7565 7320 2a2f 0a20 2020 2020 207d  alues */.      }
+00017170: 0a20 2020 2020 2064 6d61 7820 2a3d 2064  .      dmax *= d
+00017180: 726f 756e 647a 6572 6f3b 0a20 2020 2020  roundzero;.     
+00017190: 2066 6f72 2869 6220 3d20 313b 2069 6220   for(ib = 1; ib 
+000171a0: 3c3d 202a 6e7a 6472 6f77 3b20 2069 622b  <= *nzdrow;  ib+
+000171b0: 2b29 207b 0a20 2020 2020 2020 2076 6172  +) {.        var
+000171c0: 6e72 203d 206e 7a64 726f 775b 6962 5d3b  nr = nzdrow[ib];
+000171d0: 0a20 2020 2020 2020 2069 6628 6661 6273  .        if(fabs
+000171e0: 2864 726f 775b 7661 726e 725d 2920 3c20  (drow[varnr]) < 
+000171f0: 646d 6178 290a 2020 2020 2020 2020 2020  dmax).          
+00017200: 6472 6f77 5b76 6172 6e72 5d20 3d20 303b  drow[varnr] = 0;
+00017210: 0a20 2020 2020 2020 2065 6c73 6520 7b0a  .        else {.
+00017220: 2020 2020 2020 2020 2020 6965 2b2b 3b0a            ie++;.
+00017230: 2020 2020 2020 2020 2020 6e7a 6472 6f77            nzdrow
+00017240: 5b69 655d 203d 2076 6172 6e72 3b0a 2020  [ie] = varnr;.  
+00017250: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+00017260: 2020 2020 2020 2a6e 7a64 726f 7720 3d20        *nzdrow = 
+00017270: 6965 3b0a 2020 2020 7d0a 2020 7d0a 0a20  ie;.    }.  }.. 
+00017280: 202f 2a20 436c 6561 6e20 7570 2061 6e64   /* Clean up and
+00017290: 2072 6574 7572 6e20 2a2f 0a20 2069 6628   return */.  if(
+000172a0: 6c6f 6361 6c73 6574 290a 2020 2020 6d65  localset).    me
+000172b0: 6d70 6f6f 6c5f 7265 6c65 6173 6556 6563  mpool_releaseVec
+000172c0: 746f 7228 6c70 2d3e 776f 726b 6172 7261  tor(lp->workarra
+000172d0: 7973 2c20 2863 6861 7220 2a29 2063 6f6c  ys, (char *) col
+000172e0: 7461 7267 6574 2c20 4641 4c53 4529 3b0a  target, FALSE);.
+000172f0: 2020 7265 7475 726e 2820 5452 5545 2029    return( TRUE )
+00017300: 3b0a 7d0a 0a53 5441 5449 4320 766f 6964  ;.}..STATIC void
+00017310: 2062 736f 6c76 655f 7841 3228 6c70 7265   bsolve_xA2(lpre
+00017320: 6320 2a6c 702c 2069 6e74 2a20 636f 6c74  c *lp, int* colt
+00017330: 6172 6765 742c 0a20 2020 2020 2020 2020  arget,.         
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2020 2020 2020 2020 2069 6e74 2072 6f77           int row
+00017360: 5f6e 7231 2c20 5245 414c 202a 7665 6374  _nr1, REAL *vect
+00017370: 6f72 312c 2052 4541 4c20 726f 756e 647a  or1, REAL roundz
+00017380: 6572 6f31 2c20 696e 7420 2a6e 7a76 6563  ero1, int *nzvec
+00017390: 746f 7231 2c0a 2020 2020 2020 2020 2020  tor1,.          
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173b0: 2020 2020 2020 2020 696e 7420 726f 775f          int row_
+000173c0: 6e72 322c 2052 4541 4c20 2a76 6563 746f  nr2, REAL *vecto
+000173d0: 7232 2c20 5245 414c 2072 6f75 6e64 7a65  r2, REAL roundze
+000173e0: 726f 322c 2069 6e74 202a 6e7a 7665 6374  ro2, int *nzvect
+000173f0: 6f72 322c 2069 6e74 2072 6f75 6e64 6d6f  or2, int roundmo
+00017400: 6465 290a 7b0a 2020 5245 414c 206f 6673  de).{.  REAL ofs
+00017410: 6361 6c61 7220 3d20 312e 303b 0a0a 202f  calar = 1.0;.. /
+00017420: 2a20 436c 6561 7220 616e 6420 696e 6974  * Clear and init
+00017430: 6961 6c69 7a65 2066 6972 7374 2076 6563  ialize first vec
+00017440: 746f 7220 2a2f 0a20 2069 6628 6e7a 7665  tor */.  if(nzve
+00017450: 6374 6f72 3120 3d3d 204e 554c 4c29 0a20  ctor1 == NULL). 
+00017460: 2020 204d 454d 434c 4541 5228 7665 6374     MEMCLEAR(vect
+00017470: 6f72 312c 206c 702d 3e73 756d 202b 2031  or1, lp->sum + 1
+00017480: 293b 0a20 2065 6c73 650a 2020 2020 4d45  );.  else.    ME
+00017490: 4d43 4c45 4152 2876 6563 746f 7231 2c20  MCLEAR(vector1, 
+000174a0: 6c70 2d3e 726f 7773 202b 2031 293b 0a20  lp->rows + 1);. 
+000174b0: 2076 6563 746f 7231 5b72 6f77 5f6e 7231   vector1[row_nr1
+000174c0: 5d20 3d20 313b 0a2f 2a20 2077 6f72 6b49  ] = 1;./*  workI
+000174d0: 4e54 5b30 5d20 3d20 313b 0a20 2077 6f72  NT[0] = 1;.  wor
+000174e0: 6b49 4e54 5b31 5d20 3d20 726f 775f 6e72  kINT[1] = row_nr
+000174f0: 313b 202a 2f0a 0a20 2069 6628 7665 6374  1; */..  if(vect
+00017500: 6f72 3220 3d3d 204e 554c 4c29 207b 0a20  or2 == NULL) {. 
+00017510: 2020 206c 702d 3e62 6670 5f62 7472 616e     lp->bfp_btran
+00017520: 5f6e 6f72 6d61 6c28 6c70 2c20 7665 6374  _normal(lp, vect
+00017530: 6f72 312c 204e 554c 4c29 3b0a 2020 2020  or1, NULL);.    
+00017540: 7072 6f64 5f78 4128 6c70 2c20 636f 6c74  prod_xA(lp, colt
+00017550: 6172 6765 742c 2076 6563 746f 7231 2c20  arget, vector1, 
+00017560: 4e55 4c4c 2c20 726f 756e 647a 6572 6f31  NULL, roundzero1
+00017570: 2c20 6f66 7363 616c 6172 2a30 2c0a 2020  , ofscalar*0,.  
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 2020 2020 2020 2020 2076 6563 746f 7231           vector1
+000175a0: 2c20 6e7a 7665 6374 6f72 312c 2072 6f75  , nzvector1, rou
+000175b0: 6e64 6d6f 6465 293b 0a20 207d 0a20 2065  ndmode);.  }.  e
+000175c0: 6c73 6520 7b0a 0a20 2020 2f2a 2043 6c65  lse {..   /* Cle
+000175d0: 6172 2061 6e64 2069 6e69 7469 616c 697a  ar and initializ
+000175e0: 6520 7365 636f 6e64 2076 6563 746f 7220  e second vector 
+000175f0: 2a2f 0a20 2020 2069 6628 6e7a 7665 6374  */.    if(nzvect
+00017600: 6f72 3220 3d3d 204e 554c 4c29 0a20 2020  or2 == NULL).   
+00017610: 2020 204d 454d 434c 4541 5228 7665 6374     MEMCLEAR(vect
+00017620: 6f72 322c 206c 702d 3e73 756d 202b 2031  or2, lp->sum + 1
+00017630: 293b 0a20 2020 2065 6c73 650a 2020 2020  );.    else.    
+00017640: 2020 4d45 4d43 4c45 4152 2876 6563 746f    MEMCLEAR(vecto
+00017650: 7232 2c20 6c70 2d3e 726f 7773 202b 2031  r2, lp->rows + 1
+00017660: 293b 0a20 2020 2069 6628 6c70 2d3e 6f62  );.    if(lp->ob
+00017670: 6a5f 696e 5f62 6173 6973 207c 7c20 2872  j_in_basis || (r
+00017680: 6f77 5f6e 7232 203e 2030 2929 207b 0a20  ow_nr2 > 0)) {. 
+00017690: 2020 2020 2076 6563 746f 7232 5b72 6f77       vector2[row
+000176a0: 5f6e 7232 5d20 3d20 313b 0a2f 2a20 2020  _nr2] = 1;./*   
+000176b0: 2020 2077 6f72 6b49 4e54 5b32 5d20 3d20     workINT[2] = 
+000176c0: 313b 0a20 2020 2020 2077 6f72 6b49 4e54  1;.      workINT
+000176d0: 5b33 5d20 3d20 726f 775f 6e72 323b 202a  [3] = row_nr2; *
+000176e0: 2f0a 2020 2020 7d0a 2020 2020 656c 7365  /.    }.    else
+000176f0: 0a20 2020 2020 2067 6574 5f62 6173 6973  .      get_basis
+00017700: 4f46 286c 702c 204e 554c 4c2c 2076 6563  OF(lp, NULL, vec
+00017710: 746f 7232 2c20 6e7a 7665 6374 6f72 3229  tor2, nzvector2)
+00017720: 3b0a 0a20 2020 2f2a 2041 2064 6f75 626c  ;..   /* A doubl
+00017730: 6520 4254 5241 4e20 6571 7561 7469 6f6e  e BTRAN equation
+00017740: 2073 6f6c 7665 7220 7072 6f63 6573 7320   solver process 
+00017750: 6973 2069 6d70 6c65 6d65 6e74 6564 2022  is implemented "
+00017760: 696e 2d6c 696e 6522 2062 656c 6f77 2069  in-line" below i
+00017770: 6e0a 2020 2020 2020 6f72 6465 7220 746f  n.      order to
+00017780: 2073 6176 6520 7469 6d65 2061 6e64 2074   save time and t
+00017790: 6f20 696d 706c 656d 656e 7420 6469 6666  o implement diff
+000177a0: 6572 656e 7420 726f 756e 6469 6e67 2066  erent rounding f
+000177b0: 6f72 2074 6865 2074 776f 202a 2f0a 2020  or the two */.  
+000177c0: 2020 6c70 2d3e 6266 705f 6274 7261 6e5f    lp->bfp_btran_
+000177d0: 646f 7562 6c65 286c 702c 2076 6563 746f  double(lp, vecto
+000177e0: 7231 2c20 4e55 4c4c 2c20 7665 6374 6f72  r1, NULL, vector
+000177f0: 322c 204e 554c 4c29 3b0a 0a20 2020 2f2a  2, NULL);..   /*
+00017800: 204d 756c 7469 706c 7920 736f 6c75 7469   Multiply soluti
+00017810: 6f6e 2076 6563 746f 7273 2077 6974 6820  on vectors with 
+00017820: 6d61 7472 6978 2076 616c 7565 7320 2a2f  matrix values */
+00017830: 0a20 2020 2070 726f 645f 7841 3228 6c70  .    prod_xA2(lp
+00017840: 2c20 636f 6c74 6172 6765 742c 2076 6563  , coltarget, vec
+00017850: 746f 7231 2c20 726f 756e 647a 6572 6f31  tor1, roundzero1
+00017860: 2c20 6e7a 7665 6374 6f72 312c 0a20 2020  , nzvector1,.   
+00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017880: 2020 2020 2020 2020 2076 6563 746f 7232           vector2
+00017890: 2c20 726f 756e 647a 6572 6f32 2c20 6e7a  , roundzero2, nz
+000178a0: 7665 6374 6f72 322c 0a20 2020 2020 2020  vector2,.       
 000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178c0: 2020 2020 2020 2020 2076 6563 746f 7232           vector2
-000178d0: 2c20 726f 756e 647a 6572 6f32 2c20 6e7a  , roundzero2, nz
-000178e0: 7665 6374 6f72 322c 0a20 2020 2020 2020  vector2,.       
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 2020 2020 206f 6673 6361 6c61 722c 2072       ofscalar, r
-00017910: 6f75 6e64 6d6f 6465 293b 0a20 207d 0a7d  oundmode);.  }.}
-00017920: 0a0a                                     ..
+000178c0: 2020 2020 206f 6673 6361 6c61 722c 2072       ofscalar, r
+000178d0: 6f75 6e64 6d6f 6465 293b 0a20 207d 0a7d  oundmode);.  }.}
+000178e0: 0a0a                                     ..
```

### Comparing `pyfmtools-0.81/src/lp_matrix.h` & `pyfmtools-5.1/src/lp_matrix.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_mipbb.c` & `pyfmtools-5.1/src/lp_mipbb.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_mipbb.h` & `pyfmtools-5.1/src/lp_mipbb.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_params.c` & `pyfmtools-5.1/src/lp_params.c`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 #include "generaldefs.h"
 
 #include "commonlib.h"
 #include "lp_lib.h"
 #include "lp_report.h"
 #include "ini.h"
 
+int mysprintf3(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf3
+
 typedef int (__WINAPI int_get_function)(lprec *lp);
 typedef long (__WINAPI long_get_function)(lprec *lp);
 typedef MYBOOL (__WINAPI MYBOOL_get_function)(lprec *lp);
 typedef REAL (__WINAPI REAL_get_function)(lprec *lp);
 typedef void (__WINAPI int_set_function)(lprec *lp, int value);
 typedef void (__WINAPI long_set_function)(lprec *lp, long value);
 typedef void (__WINAPI MYBOOL_set_function)(lprec *lp, MYBOOL value);
```

### Comparing `pyfmtools-0.81/src/lp_presolve.c` & `pyfmtools-5.1/src/lp_presolve.c`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,23 @@
 #include "lp_scale.h"
 #include "lp_report.h"
 
 #ifdef FORTIFY
 # include "lp_fortify.h"
 #endif
 
+int mysprintf4(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf4
+
 
 #define presolve_setstatus(one, two)  presolve_setstatusex(one, two, __LINE__, __FILE__)
 
 INLINE int presolve_nextrow(presolverec *psdata, int colnr, int *previtem);
 INLINE int presolve_nextcol(presolverec *psdata, int rownr, int *previtem);
 
 INLINE int presolve_rowlength(presolverec *psdata, int rownr)
```

### Comparing `pyfmtools-0.81/src/lp_presolve.h` & `pyfmtools-5.1/src/lp_presolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_price.c` & `pyfmtools-5.1/src/lp_price.c`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 
 INLINE REAL normalizeEdge(lprec *lp, int item, REAL edge, MYBOOL isdual);
 
 /* Comparison operators for entering and leaving variables for both the primal and
    dual simplexes.  The functions compare a candidate variable with an incumbent. */
 int CMP_CALLMODEL compareImprovementVar(const pricerec *current, const pricerec *candidate)
 {
-  register int   result = COMP_PREFERNONE;
-  register lprec *lp = current->lp;
-  register REAL  testvalue, margin = PREC_IMPROVEGAP;
+   int   result = COMP_PREFERNONE;
+   lprec *lp = current->lp;
+   REAL  testvalue, margin = PREC_IMPROVEGAP;
   int currentcolno, currentvarno = current->varno,
       candidatecolno, candidatevarno = candidate->varno;
   MYBOOL isdual = candidate->isdual;
 
   if(isdual) {
     candidatevarno = lp->var_basic[candidatevarno];
     currentvarno   = lp->var_basic[currentvarno];
@@ -158,17 +158,17 @@
 Finish:
   return( result );
 
 }
 
 int CMP_CALLMODEL compareSubstitutionVar(const pricerec *current, const pricerec *candidate)
 {
-  register int    result = COMP_PREFERNONE;
-  register lprec  *lp = current->lp;
-  register REAL   testvalue = candidate->theta,
+   int    result = COMP_PREFERNONE;
+   lprec  *lp = current->lp;
+   REAL   testvalue = candidate->theta,
                   margin = current->theta;
   MYBOOL isdual = candidate->isdual, candbetter;
   int    currentcolno, currentvarno = current->varno,
          candidatecolno, candidatevarno = candidate->varno;
 
   if(!isdual) {
     candidatevarno = lp->var_basic[candidatevarno];
@@ -305,17 +305,17 @@
   }
 
 Finish:
   return( result );
 }
 int CMP_CALLMODEL compareBoundFlipVar(const pricerec *current, const pricerec *candidate)
 {
-  register REAL  testvalue, margin;
-  register int   result = COMP_PREFERNONE;
-  register lprec *lp = current->lp;
+   REAL  testvalue, margin;
+   int   result = COMP_PREFERNONE;
+   lprec *lp = current->lp;
   MYBOOL    candbetter;
   int currentvarno = current->varno,
       candidatevarno = candidate->varno;
 
   if(!current->isdual) {
     candidatevarno = lp->var_basic[candidatevarno];
     currentvarno   = lp->var_basic[currentvarno];
@@ -385,27 +385,27 @@
 }
 
 /* Validity operators for entering and leaving columns for both the primal and dual
    simplex.  All candidates must satisfy these tests to qualify to be allowed to be
    a subject for the comparison functions/operators. */
 STATIC MYBOOL validImprovementVar(pricerec *candidate)
 {
-  register REAL candidatepivot = fabs(candidate->pivot);
+   REAL candidatepivot = fabs(candidate->pivot);
 
 #ifdef Paranoia
   return( (MYBOOL) ((candidate->varno > 0) && (candidatepivot > candidate->lp->epsvalue)) );
 #else
   return( (MYBOOL) (candidatepivot > candidate->lp->epsvalue) );
 #endif
 }
 
 STATIC MYBOOL validSubstitutionVar(pricerec *candidate)
 {
-  register lprec *lp   = candidate->lp;
-  register REAL  theta = (candidate->isdual ? fabs(candidate->theta) : candidate->theta);
+   lprec *lp   = candidate->lp;
+   REAL  theta = (candidate->isdual ? fabs(candidate->theta) : candidate->theta);
 
 #ifdef Paranoia
   if(candidate->varno <= 0)
     return( FALSE );
   else
 #endif
   if(fabs(candidate->pivot) >= lp->infinite)
@@ -1183,15 +1183,15 @@
 } /* rowprim */
 
 
 /* Find the dual simplex leaving basic variable */
 STATIC int rowdual(lprec *lp, REAL *rhvec, MYBOOL forceoutEQ, MYBOOL updateinfeas, REAL *xviol)
 {
   int       k, i, iy, iz, ii, ninfeas;
-  register REAL     rh;
+   REAL     rh;
   REAL      up, lo = 0,
             epsvalue, sinfeas, xinfeas;
   pricerec  current, candidate;
   MYBOOL    collectMP = FALSE;
 
   /* Initialize */
   if(rhvec == NULL)
```

### Comparing `pyfmtools-0.81/src/lp_price.h` & `pyfmtools-5.1/src/lp_price.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_pricePSE.c` & `pyfmtools-5.1/src/lp_pricePSE.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_pricePSE.h` & `pyfmtools-5.1/src/lp_pricePSE.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_report.c` & `pyfmtools-5.1/src/lp_report.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_report.h` & `pyfmtools-5.1/src/lp_report.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_rlp.h` & `pyfmtools-5.1/src/lp_rlp.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_scale.c` & `pyfmtools-5.1/src/lp_scale.c`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 /* Compute the scale factor by the formulae:
       FALSE: SUM (log |Aij|) ^ 2
       TRUE:  SUM (log |Aij| - RowScale[i] - ColScale[j]) ^ 2 */
 REAL CurtisReidMeasure(lprec *lp, MYBOOL _Advanced, REAL *FRowScale, REAL *FColScale)
 {
   int      i, nz;
   REAL     absvalue, logvalue;
-  register REAL result;
+   REAL result;
   MATrec   *mat = lp->matA;
   REAL     *value;
   int      *rownr, *colnr;
 
   /* Do OF part */
   result = 0;
   for(i = 1; i <= lp->columns; i++) {
```

### Comparing `pyfmtools-0.81/src/lp_scale.h` & `pyfmtools-5.1/src/lp_scale.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_simplex.c` & `pyfmtools-5.1/src/lp_simplex.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_simplex.h` & `pyfmtools-5.1/src/lp_simplex.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_types.h` & `pyfmtools-5.1/src/lp_types.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_utils.c` & `pyfmtools-5.1/src/lp_utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -979,15 +979,15 @@
   return((MYBOOL) (itemnr == 0));
 }
 
 /* Packed vector routines */
 STATIC PVrec *createPackedVector(int size, REAL *values, int *workvector)
 {
   int      i, k;
-  REGISTER REAL  ref;
+   REAL  ref;
   PVrec    *newPV = NULL;
   MYBOOL   localWV = (MYBOOL) (workvector == NULL);
 
   if(localWV)
     workvector = (int *) malloc((size+1)*sizeof(*workvector));
 
   /* Tally equal-valued vector entries - also check if it is worth compressing */
@@ -1026,15 +1026,15 @@
 
   return( newPV );
 }
 
 STATIC MYBOOL unpackPackedVector(PVrec *PV, REAL **target)
 {
   int      i, ii, k;
-  REGISTER REAL ref;
+   REAL ref;
 
   /* Test for validity of the target and create it if necessary */
   if(target == NULL)
     return( FALSE );
   if(*target == NULL)
     allocREAL(NULL, target, PV->startpos[PV->count], FALSE);
```

### Comparing `pyfmtools-0.81/src/lp_utils.h` & `pyfmtools-5.1/src/lp_utils.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lp_wlp.c` & `pyfmtools-5.1/src/lp_wlp.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 #include "generaldefs.h"
 #include <stdio.h>
 #include <stdarg.h>
 #include <string.h>
 
 #include "lp_lib.h"
 #include "lp_scale.h"
@@ -17,31 +18,34 @@
 # if defined _MSC_VER
 #  define vsnprintf _vsnprintf
 # endif
 
 /* ------------------------------------------------------------------------- */
 /* Input and output of lp format model files for lp_solve                    */
 /* ------------------------------------------------------------------------- */
-
+#ifndef WRITEDATA
+#define WRITEDATA
 static void write_data(void *userhandle, write_modeldata_func write_modeldata, char *format, ...)
 {
   char buff[DEF_STRBUFSIZE+1];
   va_list ap;
 
   va_start(ap, format);
   vsnprintf(buff, DEF_STRBUFSIZE, format, ap);
   write_modeldata(userhandle, buff);
   va_end(ap);
 }
-
+#endif
 STATIC void write_lpcomment(void *userhandle, write_modeldata_func write_modeldata, char *string, MYBOOL newlinebefore)
 {
   write_data(userhandle, write_modeldata, "%s/* %s */\n", (newlinebefore) ? "\n" : "", string);
 }
 
+
+
 STATIC MYBOOL write_lprow(lprec *lp, int rowno, void *userhandle, write_modeldata_func write_modeldata)
 {
   int     i, ie, j;
   REAL    a;
   MATrec  *mat = lp->matA;
   MYBOOL  first = TRUE, rowwritten;
 
@@ -298,19 +302,24 @@
   }
 
   ok = TRUE;
 
   return(ok);
 }
 
+
+#ifndef WRITECOMMENT
+#define WRITECOMMENT
+
 static int __WINAPI write_lpdata(void *userhandle, char *buf)
 {
   fputs(buf, (FILE *) userhandle);
   return(TRUE);
 }
+#endif
 
 MYBOOL LP_writefile(lprec *lp, char *filename)
 {
   FILE *output; /* = stdout; */
   MYBOOL ok;
 
   ok = ((output = fopen(filename, "w")) != NULL);
```

### Comparing `pyfmtools-0.81/src/lpkit.h` & `pyfmtools-5.1/src/lpkit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lpslink56.c` & `pyfmtools-5.1/src/lpslink56.c`

 * *Files 0% similar despite different names*

```diff
@@ -551,32 +551,32 @@
 else
     set_minim (lp);
 
 /*
 ** Add constraints. There are r_count row-type constraints, plus c_count
 ** col_type constraints.
 */
-row_vals = calloc (cc, sizeof (double));
-col_inds = calloc (cc, sizeof (int));
+row_vals =(double*) calloc (cc, sizeof (double));
+col_inds = (int*)calloc (cc, sizeof (int));
 
 for (row_ind_ctr = 0L; row_ind_ctr < rc; row_ind_ctr++)
 {
     for (col_ind_ctr = 0; col_ind_ctr < cc; col_ind_ctr++) {
         row_vals[col_ind_ctr] = 1.0;
         this_element = 1 + (col_ind_ctr * rc) + row_ind_ctr;
         col_inds[col_ind_ctr] = this_element;
     }
     add_constraintex (lp, cc, row_vals, col_inds, r_signs[row_ind_ctr], r_rhs[row_ind_ctr]);
 }
 
 free (row_vals);
 free (col_inds);
 
-col_vals = calloc (rc, sizeof (double));
-row_inds = calloc (rc, sizeof (int));
+col_vals = (double*) calloc (rc, sizeof (double));
+row_inds = (int*)calloc (rc, sizeof (int));
 
 for (col_ind_ctr = 0L; col_ind_ctr < cc; col_ind_ctr++)
 {
     for (row_ind_ctr = 0; row_ind_ctr < rc; row_ind_ctr++) {
         col_vals[row_ind_ctr] = 1.0;
         this_element = 1 + row_ind_ctr + col_ind_ctr * rc;
         row_inds[row_ind_ctr] = this_element;
```

### Comparing `pyfmtools-0.81/src/lpsolve.h` & `pyfmtools-5.1/src/lpsolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusol.c` & `pyfmtools-5.1/src/lusol.c`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,25 @@
 #include <math.h>
 #include "lusol.h"
 #include "myblas.h"
 #ifdef MATLAB
   #include "mex.h"
 #endif
 
+int myvsprintf(char *str, const char *format, va_list arg){
+	// do nothing
+	return 0;
+}
+
+#ifdef vsprintf
+#undef vsprintf
+#endif
+
+#define vsprintf myvsprintf
+
 /* LUSOL Object creation and destruction */
 
 void *clean_realloc(void *oldptr, int width, int newsize, int oldsize)
 {
   newsize *= width;
   oldsize *= width;
   oldptr = LUSOL_REALLOC(oldptr, newsize);
```

### Comparing `pyfmtools-0.81/src/lusol.h` & `pyfmtools-5.1/src/lusol.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusol1.h` & `pyfmtools-5.1/src/lusol1.h`

 * *Files 0% similar despite different names*

```diff
@@ -34,20 +34,20 @@
    ================================================================== */
 void LU1DCP(LUSOLrec *LUSOL, REAL DA[], int LDA, int M, int N, REAL SMALL,
             int *NSING, int IPVT[], int IX[])
 {
 
   int       I, J, K, KP1, L, LAST, LENCOL, IMAX, JMAX, JLAST, JNEW;
   REAL      AIJMAX, AJMAX;
-  register REAL T;
+   REAL T;
 #ifdef LUSOLFastDenseIndex
-  register REAL *DA1, *DA2;
+   REAL *DA1, *DA2;
   int IDA1, IDA2;
 #else
-  register int IDA1, IDA2;
+   int IDA1, IDA2;
 #endif
 
   *NSING = 0;
   LENCOL = M+1;
   LAST = N;
 /*     -----------------------------------------------------------------
         Start of elimination loop.
@@ -226,20 +226,20 @@
    21 Dec 1994: Bug found via example from Steve Dirkse.
                 Loop 100 added to set ipvt(*) for singular rows.
    ================================================================== */
 void LU1DPP(LUSOLrec *LUSOL, REAL DA[], int LDA, int M, int N, REAL SMALL,
             int *NSING, int IPVT[], int IX[])
 {
   int            I, J, K, KP1, L, LAST, LENCOL;
-  register REAL T;
+   REAL T;
 #ifdef LUSOLFastDenseIndex
-  register REAL *DA1, *DA2;
+   REAL *DA1, *DA2;
   int IDA1, IDA2;
 #else
-  register int IDA1, IDA2;
+   int IDA1, IDA2;
 #endif
 
   *NSING = 0;
   K = 1;
   LAST = N;
 /*      ------------------------------------------------------------------
         Start of elimination loop.
@@ -664,15 +664,15 @@
             int LFREE, int MINFRE, int ILAST, int *JLAST, int *LROW, int *LCOL,
             int *LU, int *NFILL,
             int MARK[],  REAL AL[], int MARKL[], REAL AU[], int IFILL[], int JFILL[])
 {
   MYBOOL ATEND;
   int    LR, J, LENJ, NFREE, LC1, LC2, NDONE, NDROP, L, I, LL, K,
          LR1, LAST, LREP, L1, L2, LC, LENI;
-  register REAL UJ;
+   REAL UJ;
   REAL   AIJ;
 
   for(LR = *LFIRST; LR <= LPIVR2; LR++) {
     J = LUSOL->indr[LR];
     LENJ = LUSOL->lenc[J];
     NFREE = LFREE - *LCOL;
     if(NFREE<MINFRE)
```

### Comparing `pyfmtools-0.81/src/lusol2.h` & `pyfmtools-5.1/src/lusol2.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusol6a.h` & `pyfmtools-5.1/src/lusol6a.h`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
    15 Dec 2002: First version derived from lu6sol.
    15 Dec 2002: Current version.
    ------------------------------------------------------------------ */
 void LU6L(LUSOLrec *LUSOL, int *INFORM, REAL V[], int NZidx[])
 {
   int  JPIV, K, L, L1, LEN, LENL, LENL0, NUML, NUML0;
   REAL SMALL;
-  register REAL VPIV;
+   REAL VPIV;
 #ifdef LUSOLFastSolve
   REAL *aptr;
   int  *iptr, *jptr;
 #else
   int  I, J;
 #endif
 
@@ -444,15 +444,15 @@
    15 Dec 2002: First version of lu6LD.
    15 Dec 2002: Current version.
    ================================================================== */
 void LU6LD(LUSOLrec *LUSOL, int *INFORM, int MODE, REAL V[], int NZidx[])
 {
   int  IPIV, K, L, L1, LEN, NUML0;
   REAL DIAG, SMALL;
-  register REAL VPIV;
+   REAL VPIV;
 #ifdef LUSOLFastSolve
   REAL *aptr;
   int  *jptr;
 #else
   int  J;
 #endif
 
@@ -508,16 +508,16 @@
 void LU6LT(LUSOLrec *LUSOL, int *INFORM, REAL V[], int NZidx[])
 {
 #ifdef DoTraceL0
   REAL    TEMP;
 #endif
   int     K, L, L1, L2, LEN, LENL, LENL0, NUML0;
   REAL    SMALL;
-  register REALXP SUM;
-  register REAL HOLD;
+   REALXP SUM;
+   REAL HOLD;
 #if (defined LUSOLFastSolve) && !(defined DoTraceL0)
   REAL    *aptr;
   int     *iptr, *jptr;
 #else
   int     I, J;
 #endif
 
@@ -646,15 +646,15 @@
      ((LUSOL->luparm[LUSOL_IP_FTRANCOUNT] == 0) && LU1U0(LUSOL, &(LUSOL->U), INFORM))) {
     LU6U0_v(LUSOL, LUSOL->U, V, W, NZidx, INFORM);
   }
   /* Alternatively, do the standard column-based L0 version */
   else {
     int  I, J, K, KLAST, L, L1, L2, L3, NRANK, NRANK1;
     REAL SMALL;
-    register REALXP T;
+     REALXP T;
 #ifdef LUSOLFastSolve
     REAL *aptr;
     int  *jptr;
 #endif
     NRANK = LUSOL->luparm[LUSOL_IP_RANK_U];
     SMALL = LUSOL->parmlu[LUSOL_RP_ZEROTOLERANCE];
     *INFORM = LUSOL_INFORM_LUSUCCESS;
@@ -721,15 +721,15 @@
    15 Dec 2002: Current version.
    ================================================================== */
 void LU6UT(LUSOLrec *LUSOL, int *INFORM, REAL V[], REAL W[], int NZidx[])
 {
   int  I, J, K, L, L1, L2, NRANK, NRANK1,
        *ip = LUSOL->ip + 1, *iq = LUSOL->iq + 1;
   REAL SMALL;
-  register REAL T;
+   REAL T;
 #ifdef LUSOLFastSolve
   REAL *aptr;
   int  *jptr;
 #endif
 
   NRANK = LUSOL->luparm[LUSOL_IP_RANK_U];
   SMALL = LUSOL->parmlu[LUSOL_RP_ZEROTOLERANCE];
```

### Comparing `pyfmtools-0.81/src/lusol6l0.h` & `pyfmtools-5.1/src/lusol6l0.h`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 void LU6L0T_v(LUSOLrec *LUSOL, LUSOLmat *mat, REAL V[], int NZidx[], int *INFORM)
 {
 #ifdef DoTraceL0
   REAL TEMP;
 #endif
   int  LEN, K, KK, L, L1, NUML0;
   REAL SMALL;
-  register REAL VPIV;
+   REAL VPIV;
 #if (defined LUSOLFastSolve) && !(defined DoTraceL0)
   REAL *aptr;
   int  *jptr;
 #else
   int  J;
 #endif
```

### Comparing `pyfmtools-0.81/src/lusol6u.h` & `pyfmtools-5.1/src/lusol6u.h`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 void LU6U0_v(LUSOLrec *LUSOL, LUSOLmat *mat, REAL V[], REAL W[], int NZidx[], int *INFORM)
 {
 #ifdef DoTraceU0
   REAL TEMP;
 #endif
   int  LEN, I, K, L, L1, NRANK, NRANK1, KLAST;
   REAL SMALL;
-  register REAL T;
+   REAL T;
 #if (defined xxLUSOLFastSolve) && !(defined DoTraceU0)
   REAL *aptr;
   int  *jptr;
 #else
   int  J;
 #endif
```

### Comparing `pyfmtools-0.81/src/lusol7a.h` & `pyfmtools-5.1/src/lusol7a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusol8a.h` & `pyfmtools-5.1/src/lusol8a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusolio.c` & `pyfmtools-5.1/src/lusolio.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/lusolio.h` & `pyfmtools-5.1/src/lusolio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/minimalsplus.h` & `pyfmtools-5.1/src/minimalsplus.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/mmio.c` & `pyfmtools-5.1/src/mmio.c`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 #include <R.h>
 #include <R_ext/Print.h>
 #else
 #define REprintf printf
 #define Rprintf printf
 #endif
 
+int mysprintf(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf
+
 int mm_read_unsymmetric_sparse(const char *fname, int *M_, int *N_, int *nz_,
                 double **val_, int **I_, int **J_)
 {
     FILE *f;
     MM_typecode matcode;
     int M, N, nz;
 #ifdef ORIG
```

### Comparing `pyfmtools-0.81/src/mmio.h` & `pyfmtools-5.1/src/mmio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/myblas.c` & `pyfmtools-5.1/src/myblas.c`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
    jack dongarra, linpack, 3/11/78.
    modified 12/3/93, array[1] declarations changed to array[*] */
 
   int      i, ix, iy; 
 #ifndef DOFASTMATH
   int      m, mp1;
 #endif
-  register REAL rda;
+   REAL rda;
   REAL     da = *_da;
   int      n = *_n, incx = *_incx, incy = *_incy;
 
   if (n <= 0) return;
   if (da == 0.0) return;
 
   dx--;
@@ -324,15 +324,15 @@
      For I = 0 to N-1, replace DX(IX+I*INCX) with  DA * DX(IX+I*INCX),
      where IX = 1 if INCX .GE. 0, else IX = 1+(1-N)*INCX. */
 
   int      i;
 #ifndef DOFASTMATH
   int      m, mp1, ix;
 #endif
-  register REAL rda;
+   REAL rda;
   REAL      da = *_da;
   int      n = *_n, incx = *_incx;
 
   if (n <= 0)
     return;
   rda = da;  
   
@@ -393,15 +393,15 @@
 {
 
 /* forms the dot product of two vectors.
    uses unrolled loops for increments equal to one.
    jack dongarra, linpack, 3/11/78.
    modified 12/3/93, array[1] declarations changed to array[*] */
 
-  register REAL dtemp;
+   REAL dtemp;
   int      i, ix, iy;
 #ifndef DOFASTMATH
   int      m, mp1;
 #endif
   int      n = *_n, incx = *_incx, incy = *_incy;
 
   dtemp = 0.0;
@@ -474,15 +474,15 @@
 void BLAS_CALLMODEL my_dswap( int *_n, REAL *dx, int *_incx, REAL *dy, int *_incy )
 {
   int   i, ix, iy;
 #ifndef DOFASTMATH
   int   m, mp1, ns;
   REAL  dtemp2, dtemp3;
 #endif
-  register REAL  dtemp1;
+   REAL  dtemp1;
   int   n = *_n, incx = *_incx, incy = *_incy;
 
   if (n <= 0) return;
 
   dx--;
   dy--;
   ix = 1;
@@ -642,15 +642,15 @@
 {
   x++;
   return ( BLAS_idamin( &n, x, &is ) );
 }
 
 int BLAS_CALLMODEL my_idamax( int *_n, REAL *x, int *_is )
 {
-  register REAL xmax, xtest;
+   REAL xmax, xtest;
   int    i, imax = 0;
 #if !defined DOFASTMATH
   int    ii;
 #endif
   int    n = *_n, is = *_is;
 
   if((n < 1) || (is <= 0))
@@ -681,15 +681,15 @@
   }
 #endif  
   return(imax);
 }
 
 int BLAS_CALLMODEL my_idamin( int *_n, REAL *x, int *_is )
 {
-  register REAL xmin, xtest;
+   REAL xmin, xtest;
   int    i, imin = 0;
 #if !defined DOFASTMATH
   int    ii;
 #endif
   int    n = *_n, is = *_is;
 
   if((n < 1) || (is <= 0))
@@ -731,15 +731,15 @@
 
 REAL BLAS_CALLMODEL my_dnormi( int *_n, REAL *x )
 {
 /* ===============================================================
    dnormi  returns the infinity-norm of the vector x.
    =============================================================== */
    int      j;
-   register REAL hold, absval;
+    REAL hold, absval;
    int      n = *_n;
 
    x--;
    hold = 0.0;
 /*   for(j = 1; j <= n; j++) */
    for(j = n; j > 0; j--) {
      absval = fabs(x[j]);
```

### Comparing `pyfmtools-0.81/src/myblas.h` & `pyfmtools-5.1/src/myblas.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/pyfmtools.egg-info/PKG-INFO` & `pyfmtools-5.1/src/pyfmtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 0.81
+Version: 5.1
 Summary: Library for handling and fitting fuzzy measures
-Home-page: UNKNOWN
+Home-page: 
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: cffi>=1.0.0
 
 # Pyfmtools    
 Pyfmtools provides various tools for handling fuzzy measures, calculating various indices, Choquet and Sugeno integrals, as well as fitting fuzzy measures to empirical data. This package is designed for Python , but it also includes the C++ source files and a user manual.
 Chapter 2 of the user manual provides some background on fuzzy measures. A more detailed overview can be found in [4, 5, 12, 16] and references therein. Chapter 3 of the user manual outlines computational methods used to fit fuzzy measures to empirical data. The description of the programming library pyfmtools is given in Chapter 4. Examples of its usage are provided in Section 4.6.
 To cite pyfmtools package, use references [2–6,21–24]. 
 ### New in version 4
 Random generation of fuzzy measures of different types, including k-additive, k-interactive, supermodular and submodular, sparse representation of k- additive fuzzy measures.<br>
@@ -149,8 +148,7 @@
 
 
 ### Test
 To unit test type:
 ```python
 $ test/test_no_wrapper.py
 ```
-
```

### Comparing `pyfmtools-0.81/src/pyfmtools.egg-info/SOURCES.txt` & `pyfmtools-5.1/src/pyfmtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
-dist/pyfmtools-0.81-cp39-cp39-macosx_10_9_x86_64.whl
+dist/pyfmtools-5.1-cp312-cp312-macosx_14_0_arm64.whl
 src/binarylattice.h
 src/buildPyfmtools.py
 src/colamd.c
 src/colamd.h
 src/commonlib.c
 src/commonlib.h
 src/declare.h
 src/fmrandom.cpp
 src/fmrandom.h
+src/fmrandomsort.inc
 src/fortify.h
 src/fuzzymeasurefit.cpp
 src/fuzzymeasurefit.h
 src/fuzzymeasurefit3.cpp
 src/fuzzymeasuretools.bak.cpp
 src/fuzzymeasuretools.bak.h
 src/fuzzymeasuretools.cpp
 src/fuzzymeasuretools.h
+src/gbrealloc.c
 src/generaldefs.h
 src/hbio.h
 src/ini.c
 src/ini.h
 src/isfixedvar.c
 src/lp_BFP.h
 src/lp_BFP1.h
```

### Comparing `pyfmtools-0.81/src/pyfmtools.py` & `pyfmtools-5.1/src/pyfmtools.py`

 * *Files 16% similar despite different names*

```diff
@@ -138,14 +138,39 @@
 import sys
 import numpy as np
 import types
 import math
 import re
 from  _pyfmtools import ffi, lib as fm
 
+
+CB = None
+# call-back function
+@ffi.def_extern()
+def py_user_defined_measurecheck(  n, x):
+    # print( "py_user_defined")
+    # User defined python function
+    return CB( n, x)
+
+# Retrieve C call-back function based on Python call-back function
+def get_c_callback_function( py_cb):
+    try:
+        # check if this is a function
+        if not( isinstance( py_cb, types.FunctionType)): raise ValueError( "no call-back function")
+
+        # Check if Python call-back function is one of the pre-defined call-backs
+        if( py_cb == py_user_defined_measurecheck): p_c_cb = fm.py_user_defined_measurecheck
+        else: raise ValueError( "undefined call-back function")
+
+        return p_c_cb
+    except ValueError:
+        raise
+        
+        
+
 ###
 # Helper functions
 ###
 
 # global variable to support trace-info while testing
 isTest = False
 
@@ -158,21 +183,21 @@
 def convert_float_to_CFFI_double( x):
     if x.dtype != "float64": x = x.astype(float)
     px = ffi.cast( "double *", x.ctypes.data)
     return px
 
 # use numpy to create an intc array with n zeros and cast to CFFI 
 def create_intc_zeros_as_CFFI_int( n):
-    x = np.zeros( n, np.intc)
+    x = np.zeros( int(n), np.intc)
     px = ffi.cast( "int *", x.ctypes.data)
     return x, px
 
 # use numpy to create an float array with n zeros and cast to CFFI 
 def create_float_zeros_as_CFFI_double( n):
-    x = np.zeros( n, float)
+    x = np.zeros( int(n), dtype=np.float64)
     px = ffi.cast( "double *", x.ctypes.data)
     return x, px
 
 
 # version of the function using np.ascontiguousarray() 
 def convert_py_float_to_cffi_cont( x):
     if x is not None:
@@ -245,14 +270,15 @@
 
 # void py_fm_free( struct fm_env* env)
 def fm_free( env):
     try:
         trace( "py_fm_free")
         if( env == None): raise ValueError( "Env not initialised") 
         fm.py_fm_free( env)
+        return None
     except ValueError:
         raise
 
 # void py_ShowCoalitions(int* coalition, struct fm_env* env)
 def ShowCoalitions( env):
     trace( "py_ShowCoalitions")
     A, pA = create_intc_zeros_as_CFFI_int( env.m) 
@@ -720,20 +746,20 @@
     pvnp, pv = convert_py_float_to_cffi( v)
     pout_wnp, pout_w = create_float_zeros_as_CFFI_double( env.m)
     fm.py_BipartitionBanzhafIndex( pv, pout_w, env)
     return pout_wnp
 
 
 
-#    void py_BNonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)
-def BNonadditivityIndexMob(Mob, env):
-    trace( "void py_BNonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)")
+#    void py_NonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)
+def NonadditivityIndexMob(Mob, env):
+    trace( "void py_NonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)")
     pMobnp, pMob = convert_py_float_to_cffi( Mob)
     pout_wnp, pout_w = create_float_zeros_as_CFFI_double( env.m)
-    fm.py_BNonadditivityIndexMob( pMob, pout_w, env)
+    fm.py_NonadditivityIndexMob( pMob, pout_w, env)
     return pout_wnp
 
 
 
 #    void py_NonadditivityIndex(double* v, double* out_w, struct fm_env* env)
 def NonadditivityIndex(v, env):
     trace( "void py_NonadditivityIndex(double* v, double* out_w, struct fm_env* env)")
@@ -978,15 +1004,15 @@
 
 
 #    void py_dualMobKadd(int m, int length, int k, double* src, double* out_dest, struct fm_env* env)
 def dualMobKadd(k, src, env):
     trace( "void py_dualMobKadd(int m, int length, int k, double* src, double* out_dest, struct fm_env* env)")
     psrcnp, psrc = convert_py_float_to_cffi( src)
     pout_destnp, pout_dest = create_float_zeros_as_CFFI_double( env.m)
-    length = fm.py_fm_arraysize( env.n, k, env)
+    length = fm.py_fm_arraysize_kadd( env.n, k, env)
     fm.py_dualMobKadd( env.m, length, k, psrc, pout_dest, env)
     return pout_destnp, length
 
 
 
 #    void py_Shapley2addMob(double* v, double* out_x, int n)
 def Shapley2addMob(v, n):
@@ -1020,41 +1046,44 @@
 
 #    int py_fm_arraysize(int n, int kint, struct fm_env* env)
 def fm_arraysize(n, kint, env):
     trace( "int py_fm_arraysize(int n, int kint, struct fm_env* env)")
     yy = fm.py_fm_arraysize( n, kint, env)
     return yy
 
-
+def fm_arraysize_kadd(n, kint, env):
+    trace( "int py_fm_arraysize(int n, int kint, struct fm_env* env)")
+    yy = fm.py_fm_arraysize_kadd( n, kint, env)
+    return yy
 
 #    int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double* out_vv, struct fm_env* env)
 def generate_fm_minplus(num, n, kint, markov, option, K, env):
     trace( "int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double* out_vv, struct fm_env* env)")
     length = fm.py_fm_arraysize(n, kint, env)
     pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
     yy = fm.py_generate_fm_minplus( num, n, kint, markov, option, K, pout_vv, env)
     return yy, pout_vvnp, length
 
 
 
 #    int py_generate_fm_2additive_convex(int num, int n,  double* out_vv)
 def generate_fm_2additive_convex(num, n):
     trace( "int py_generate_fm_2additive_convex(int num, int n,  double* vv)")
-    length = num * n * n
-    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( length)
+    length = n * n
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
     yy = fm.py_generate_fm_2additive_convex( num, n, pout_vv)
     return yy, pout_vvnp, length
 
 
 
 #    int py_generate_fm_2additive_convex_withsomeindependent(int num, int n, double* out_vv)
 def generate_fm_2additive_convex_withsomeindependent(num, n):
     trace( "int py_generate_fm_2additive_convex_withsomeindependent(int num, int n, double* vv)")
-    length = num * n * n
-    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( length)
+    length = n * n
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
     yy = fm.py_generate_fm_2additive_convex_withsomeindependent( num, n, pout_vv)
     return yy, pout_vvnp, length
 
 
 
 #    void py_prepare_fm_sparse(int n, int tupsize, int* tuples, struct fm_env_sparse* out_env)
 def prepare_fm_sparse( n, tupsize):
@@ -1071,14 +1100,15 @@
 
 #    void py_free_fm_sparse( struct fm_env_sparse* env)
 def free_fm_sparse(env_sparse):
     try:
         trace( "void py_free_fm_sparse( struct fm_env_sparse* env)")
         if( env_sparse == None): raise ValueError( "Env sparse not initialised") 
         fm.py_free_fm_sparse( env_sparse)
+        return None
     except ValueError:
         raise
 
 
 #    int py_tuple_cardinality_sparse(int i, struct fm_env_sparse* env)
 def tuple_cardinality_sparse(i, env):
     trace( "int py_tuple_cardinality_sparse(int i, struct fm_env_sparse* env)")
@@ -1268,7 +1298,239 @@
 
 #    void py_Nonmodularityindex_sparse(double* out_w, int n, struct fm_env_sparse* env)
 def Nonmodularityindex_sparse(n, env):
     trace( "void py_Nonmodularityindex_sparse(double* out_w, int n, struct fm_env_sparse* env)")
     pout_wnp, pout_w = create_float_zeros_as_CFFI_double( 2 ** n)
     fm.py_Nonmodularityindex_sparse( pout_w, n, env)
     return pout_wnp
+    
+    
+# from version 5
+
+def generate_fm_randomwalk( num, n , kint, markov, option, step, env, F):
+    trace( "generate_fm_randomwalk( num, n , kint, markov, option, step, env, F)")
+    try:
+        global CB
+        if (F != None) :
+            CB = F
+            F =  py_user_defined_measurecheck
+            p_c_cb =  get_c_callback_function( F)
+        else:
+            p_c_cb = ffi.cast( "void *", 0)
+            
+               # Use CFFI type conversion
+        # Retrieve C call-back function
+        if ((option & 127) ==3) or ((option & 127)==5):
+            length = fm.py_fm_arraysize_kadd(n, kint, env)
+        else:
+            length=pow(2,n)
+        
+        pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
+
+        yy = fm.py_generate_fm_randomwalk(num, n, kint, markov, option, step, pout_vv, env, p_c_cb)
+        return yy, pout_vvnp, length
+        
+    except ValueError:
+        raise
+        
+def generate_fm_kinteractivedualconvex( num, n , kint, markov, step, env, F):
+    trace( "generate_fm_kinteractivedualconvex( num, n , kint, markov, step, env, F)")
+    try:
+        global CB
+        if (F != None) :
+            CB = F
+            F =  py_user_defined_measurecheck
+            p_c_cb =  get_c_callback_function( F)
+        else:
+            p_c_cb = ffi.cast( "void *", 0)
+            
+               # Use CFFI type conversion
+        # Retrieve C call-back function
+        length = fm.py_fm_arraysize_kadd(n, kint, env)+n
+
+        pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
+        if(kint>n-2) :
+            print("kint must be at most n-2")
+            return 0, pout_vvnp, 0
+
+        yy = fm.py_generate_fm_kinteractivedualconvex(num, n, kint, markov, length, step, pout_vv, env, p_c_cb)
+        return yy, pout_vvnp, length
+        
+    except ValueError:
+        raise
+
+
+def generate_fm_kinteractivedualconcave( num, n , kint, markov, step, env, F):
+    trace( "generate_fm_kinteractivedualconcave( num, n , kint, markov, step, env, F)")
+    try:
+        global CB
+        if (F != None) :
+            CB = F
+            F =  py_user_defined_measurecheck
+            p_c_cb =  get_c_callback_function( F)
+        else:
+            p_c_cb = ffi.cast( "void *", 0)
+            
+               # Use CFFI type conversion
+        # Retrieve C call-back function
+        
+
+        length = fm.py_fm_arraysize_kadd(n, kint, env)+n
+
+        pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
+        if(kint>n-2) :
+            print("kint must be at most n-2")
+            return 0, pout_vvnp, 0
+
+        yy = fm.py_generate_fm_kinteractivedualconcave(num, n, kint, markov, length, step, pout_vv, env, p_c_cb)
+        return yy, pout_vvnp, length
+        
+    except ValueError:
+        raise
+        
+def generate_fm_2additive_randomwalk2( num, n ,markov, option, step, F):
+    trace( "generate_fm_2additive_randomwalk2( num, n ,markov, option, step, F)")
+    try:
+        global CB
+        if (F != None) :
+            CB = F
+            F =  py_user_defined_measurecheck
+            p_c_cb =  get_c_callback_function( F)
+        else:
+            p_c_cb = ffi.cast( "void *", 0)
+            
+               # Use CFFI type conversion
+        # Retrieve C call-back function
+        length = n*(n-1)/2+n
+
+        pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
+
+        yy = fm.py_generate_fm_2additive_randomwalk2(num, n, markov, option, step, pout_vv,  p_c_cb)
+        return yy, pout_vvnp, int(length)
+        
+    except ValueError:
+        raise
+
+
+
+def generate_fm_2additive(num , n):
+    trace( "int py_generate_fm_2additive(int num, int n,  double* vv)")
+    length = (n * (n-1)/2+n)
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double(num* length)
+    yy = fm.py_generate_fm_2additive( num, n, pout_vv)
+    return yy, pout_vvnp, int(length)
+
+
+def generateAntibuoyant(n, env):
+    trace( "int py_GenerateAntibuoyant( int n,  double* vv)")
+    length = pow(2,n)
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( length)
+    fm.py_GenerateAntibuoyant( pout_vv, env )
+    return pout_vvnp
+    
+def generate_fm_belief(num, n, kadd, env):
+    trace( "int py_generate_fm_belief(int num, int n,  double* vv)")
+    length = py_fm_arraysize_kadd(n,kadd)
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double(num* length)
+    yy=fm.py_generate_fm_belief( num, n, kadd, pout_vv,env)
+    return yy,pout_vvnp,length
+    
+
+def generate_fm_balanced(num, n,  env):
+    trace( "int py_generate_fm_balanced(int num, int n,  double* vv)")
+    length = pow(2,n)
+    pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double(num* length)
+    yy=fm.py_generate_fm_balanced( num, n,  pout_vv, env)
+    return yy,pout_vvnp,length
+    
+
+
+def generate_fm_sorting( num, n , markov, option,  env):
+    trace( "int py_generate_fm_sorting( num, n , markov, option,  env)")
+    try:
+        length = pow(2,n)
+        pout_vvnp, pout_vv = create_float_zeros_as_CFFI_double( num * length)
+
+        fm.py_generate_fm_sorting(num, n, markov, option,  pout_vv, env)
+        return  pout_vvnp
+        
+    except ValueError:
+        raise
+        
+        
+        
+def CheckMonotonicitySortMerge(n, v, env):
+    trace( "int CheckMonotonicitySortMerge(n, v, indices, env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    pout_indicesnp, pout_indices = create_float_zeros_as_CFFI_double(pow(2,n))
+    yy = fm.py_CheckMonotonicitySortMerge( pMob,pout_indices, env)
+    return yy, pout_indicesnp
+    
+    
+def CheckMonotonicitySortInsert(n, v, indices, env):
+    trace( "int py_CheckMonotonicitySortInsert(n, v, indices, env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    pout_indicesnp, pout_indices = convert_py_float_to_cffi( indices )
+    yy = fm.py_CheckMonotonicitySortInsert( pMob, pout_indices, env)
+    return yy, pout_indicesnp
+   
+   
+def CheckMonotonicitySimple(v, env):
+    trace( "int py_CheckMonotonicitySimple(double* v, struct fm_env* env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    yy = fm.py_CheckMonotonicitySimple( pMob,  env)
+    return yy
+
+def CheckMonMob2additive2(v, n):
+    trace( "int py_CheckMonMob2additive2(double* v, struct fm_env* env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    length=n*(n-1)+n
+    out_indicesnp, temp = create_float_zeros_as_CFFI_double(length+1)
+    yy = fm.py_CheckMonMob2additive2( pMob, n, length, temp)
+    return yy
+
+def CheckMonotonicityMob(v, len,  env):
+    trace( "int py_CheckMonotonicityMob(double* Mob, len, struct fm_env* env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    yy = fm.py_CheckMonotonicityMob( pMob, len,  env)
+    return yy
+
+def CheckConvexityMonMob(v,  len, env):
+    trace( "int py_CheckConvexityMonMob(double* Mob, len , struct fm_env* env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    yy = fm.py_CheckConvexityMonMob( pMob, len, env)
+    return yy
+
+
+def ConvertCoMob2Kinter(n, kint, len, v, fullmu, env):
+    trace( "int py_ConvertCoMob2KinterCall(n, kint, len, v, fullmu, env)")
+    pMobnp, pMob = convert_py_float_to_cffi( v)
+    pout_munp, pout_mu= create_float_zeros_as_CFFI_double(n*n)
+    fm.py_ConvertCoMob2KinterCall( n, kint, len, pout_mu, pMob, fullmu, env)
+    return pout_munp
+
+
+   
+def ChoquetCoMobKInter(x, Mob, kint, len, env):
+    trace( "double py_ChoquetCoMobKInter(double* x, double* Mob, int n)")
+    pxnp, px = convert_py_float_to_cffi( x)
+    pMobnp, pMob = convert_py_float_to_cffi( Mob)
+    yy = fm.py_ChoquetCoMobKInter( px, pMob, kint, len, env)
+    return yy
+
+
+def FuzzyMeasureFit2Additive(datanum, n, options, indexlow, indexhihg, option1, orness, dataset):
+    trace( "void FuzzyMeasureFit2Additive( datanum, n, options, indexlow, indexhihg, option1, orness, dataset)")
+    len=n*(n-1)/2+n
+    pout_vnp, pout_v = create_float_zeros_as_CFFI_double( len)
+    pdatasetnp, pdataset = convert_py_float_to_cffi_cont( dataset)
+    #poptionsnp, poptions = convert_py_int_to_cffi_cont( options)
+    pindexlownp, pindexlow = convert_py_float_to_cffi_cont( indexlow)
+    pindexhihgnp, pindexhihg = convert_py_float_to_cffi_cont( indexhihg)
+   # poption1np, poption1 = convert_py_int_to_cffi_cont( option1)
+    pornessnp, porness = convert_py_float_to_cffi_cont( orness)
+    fm.py_fitting2additive( int(datanum), int(n), int(len),  pout_v, pdataset, int(options), pindexlow, pindexhihg, int(option1), porness)
+    return pout_vnp
+
+
+
+
```

### Comparing `pyfmtools-0.81/src/sparselib.c` & `pyfmtools-5.1/src/sparselib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/sparselib.h` & `pyfmtools-5.1/src/sparselib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/ufortify.h` & `pyfmtools-5.1/src/ufortify.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/src/wrapperpy.cpp` & `pyfmtools-5.1/src/wrapperpy.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,79 @@
 //
 /* This is a C-wrapper for fmtools library 
 
    Gleb Beliakov, 2020
 */
-#include "generaldefs.h" //NH
+
 #define R_NO_REMAP
 
-#undef __R
-// #define __R //NH
+#define PYTHON_
+
+#include <stdlib.h>
+
+//#define PYTHON_
+#include "generaldefs.h"
+
+
+typedef unsigned long long int_64;
+
+
+#ifdef __cplusplus
+
+#include "fuzzymeasuretools.h"
+#include "fuzzymeasurefit.h"
+
+#endif
+
+
+
+
+struct  fm_env {
+    int n;
+    int m;
+    int* card;
+    int* cardpos;
+    double* bit2card;
+    double* card2bit;
+    double* factorials;
+
+};
+
+
+
+struct  fm_env_sparse { // to use in wrappers, just to keep pointers. pointers might change when vectors are growing, but steady afterwards
+    int n;
+    double *m_singletons;
+    double* m_pairs;
+    double* m_tuples;
+    int* m_pair_index;
+    int* m_tuple_start;
+    int* m_tuple_content;
+};
+
+
+
+//#define __R
 #ifdef __R
 //#include "cpp11.hpp"
 
 
 
 #include <R.h>
 #include <Rdefines.h>
 #include <Rinternals.h>
 #endif
 //#include <Rcpp.h>
 
 
+
 #include <stdlib.h>
-#include "wrapperpy.h"
 
-#ifdef PYTHON_
-#define LIBEXP
-#endif
+//#include "wrapperpy.h"
 
-#ifdef __R
 //#if (defined(__clang__) || defined(__APPLE__) || defined(__arm64__)) && defined(_LIBCPP_VERSION)
 //#if (defined(__clang__) ||  defined(__arm64__)) && defined(_LIBCPP_VERSION)	
 #if  defined(_LIBCPP_VERSION)	// may be just detect libc++
 
 #if (_LIBCPP_VERSION < 14000)
 template <class T>
 void wrapArrayInVector( T *sourceArray, size_t arraySize, std::vector<T,  std::allocator<T> > volatile &targetVector ) {
@@ -77,33 +119,14 @@
 template <class T>
 void releaseVectorWrapper( std::vector<T,  std::allocator<T> > volatile &targetVector )
 {
 	// do nothing 
 	return ;
 }
 
-/* Can also do this way
-template <class _Allocator>
-class  myvector<bool, _Allocator>
-{
-	public:
-	    __storage_pointer                                      __begin_;
-    size_type                                              __size_;
-    __compressed_pair<size_type, __storage_allocator> __cap_alloc_;
-
-}
-myvector *b = reinterpret_cast<myvector *> &targetVector; 
-
-//now you can use b to access members of vector 
-
-		b->__begin_ = sourceArray;
-		b->__end_ =  b-> __end_cap() = b->__begin_ + arraySize;	
-*/
-
-
 /*
 	template <class T>
 void wrapArrayInVector( T *sourceArray, size_t arraySize, std::vector<T,  std::allocator<T> > volatile &targetVector ) {
   typename std::vector<T, std::allocator<T> > *vectorPtr =
     (typename std::vector<T, std::allocator<T> > *)((void *) &targetVector);
 	
     class MyDerivedClass : public std::vector<T, std::allocator<T> > {
@@ -148,33 +171,29 @@
   typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *vectorPtr =
         (typename std::_Vector_base<T, std::allocator<T> >::_Vector_impl *)((void *) &targetVector);
   vectorPtr->_M_start = vectorPtr->_M_finish = vectorPtr->_M_end_of_storage = NULL;
 }
 #endif
 
 
-#endif
-// #undef PYTHON_ commented out by NH
+
+//#undef PYTHON_
 
 extern "C" {
 
 // todo: add cases i==3,4 explicit formulas
 inline int_64 choose(int i, int n, struct fm_env* env)
 {
-	 if (i == 1) return n;
-    if (i == 2) return (int_64)(n*(n - 1)) / 2;
-    if (i == 3) return (int_64)(n*(n - 1)*(n - 2)) / 6;
-    if (i == 4) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)) / 24;
-    if (i == 5) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)) / 120;
-    if (i == 6) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)) / 120 / 6;
-    if (i == 7) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)*(n - 6)) / 120 / 42;
-    if (i == 8) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)*(n - 6)*(n - 7)) / 120 / 42 / 8;
-    if (i == 9) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)*(n - 5)*(n - 6)*(n - 7)*(n - 8)) / 120 / 42 / 72;
+	if (i == 1) return n;
+	if (i == 2) return (int_64)(n*(n - 1)) / 2;
+	if (i == 3) return (int_64)(n*(n - 1)*(n - 2)) / 6;
+	if (i == 4) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)) / 24;
+	if (i == 5) return (int_64)(n*(n - 1)*(n - 2)*(n - 3)*(n - 4)) / 120;
 
-    return (int_64)(env->factorials[n] / env->factorials[i] / env->factorials[n - i]);
+	return (int_64)(env->factorials[n] / env->factorials[i] / env->factorials[n - i]);
 }
 
 #ifdef PYTHON_
 LIBEXP double py_min_subset(double* x, int n, int_64 S)
 	{
 		return min_subset(x, n, S);
 	}
@@ -1462,19 +1481,21 @@
 	env->factorials=(double* ) malloc((n+1)*sizeof(double));
 	
 	Preparations_FMCall(&n,&(env->m),env->card,env->cardpos, env->bit2card, env->card2bit,env->factorials );
 
 }
 LIBEXP void py_fm_free( struct fm_env* env)
 {
-	free(env->card);
-	free(env->cardpos);
-	free(env->bit2card);
-	free(env->card2bit);
-	free(env->factorials);
+    if(env->n>0) {
+        free(env->card);
+        free(env->cardpos);
+        free(env->bit2card);
+        free(env->card2bit);
+        free(env->factorials);
+    }
 	env->n=0;
 	env->m=0;
 }
 LIBEXP void py_ExpandKinteractive2Bit(double* dest, double* src, struct fm_env* env, int kint, int arraysize) {
 
 	 ExpandKinteractive2Bit( dest,  src, env-> n,env-> m,  kint,  arraysize);
 	 
@@ -1665,15 +1686,15 @@
 
 LIBEXP void py_BipartitionBanzhafIndex(double* v, double* w, struct fm_env* env)
 {
 	// Calculates an array of BipartitionBanzhafIndex indices
 	BipartitionBanzhafCall(v, w, &(env->n), &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
 }
 
-LIBEXP void py_BNonadditivityIndexMob(double* Mob, double* w, struct fm_env* env)
+LIBEXP void py_NonadditivityIndexMob(double* Mob, double* w, struct fm_env* env)
 {
 	// Calculates an array of NonadditivityIndexMob indices
 	NonadditivityIndexMobCall(Mob, w, &(env->n),  &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
 }
 
 LIBEXP void py_NonadditivityIndex(double* v, double* w, struct fm_env* env)
 {
@@ -1955,86 +1976,35 @@
 
 void Choquet2addMobCall(double* v, double* x, double* out, int *n)
 // calculates the array x of Banzhaf indices for 2 additive fm in compact representation (cardinality based)
 {
 	*out= Choquet2add(x, v, *n);// Note it is x,v in that order here
 }
 int fm_arraysizeCall(int* n, int_64* m, int* kint,  double* Rfactorials)
-// calculates the size of the array to store one k-interctive fuzzy measure
+// calculates the size of the array to store one k-interactive fuzzy measure
 {
 	m_factorials = Rfactorials;
 	int_64 m1=*m;
 	return fm_arraysize(*n, m1, *kint);
 }
-
+int fm_arraysizekaddCall(int* n, int_64* m, int* kint,  double* Rfactorials)
+// calculates the size of the array to store one k-additive fuzzy measure
+{
+    m_factorials = Rfactorials;
+    int_64 m1=*m;
+    return fm_arraysize_kadd(*n, *kint);
+}
 void fm_arraysizeCallR(int* n, int* m, int* kint, int* out, double* Rfactorials)
 // calculates the size of the array to store one k-interctive fuzzy measure
 {
 	m_factorials = Rfactorials;
 	int_64 m1=*m;
 	*out= fm_arraysize(*n, m1, *kint);
 }
 
-// generate fuzzy measures randomly using topological sort
-int generate_fm_tsortCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials)
-{
-    card = Rcard;
-    cardpos = Rcardpos;
-    bit2card = (int_64*)Rbit2card;
-    card2bit = (int_64*)Rcard2bit;
-    m_factorials = Rfactorials;
-    return generate_fm_tsort(*num, *n, *kint, *markov, *option, *K, vv);
-}
-
-
-
-// generate convex (supermodular)  fuzzy measures randomly using topological sort
-int generate_fmconvex_tsortCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials)
-{
-    card = Rcard;
-    cardpos = Rcardpos;
-    bit2card = (int_64*)Rbit2card;
-    card2bit = (int_64*)Rcard2bit;
-    m_factorials = Rfactorials;
-    int opt = (*option) | 8; // means we do rejections inside for 1000 steps
-    return generate_fmconvex_tsort(*num, *n, *kint, *markov, opt, *K,  vv);
-}
-
-// generate fuzzy measures randomly using MinimalsPlus method
-int generate_fm_minplusCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials)
-{
-    card = Rcard;
-    cardpos = Rcardpos;
-    bit2card = (int_64*)Rbit2card;
-    card2bit = (int_64*)Rcard2bit;
-    m_factorials = Rfactorials;
-    return generate_fm_minplus(*num, *n, *kint, *markov, *option, *K, vv);
-}
-
-// generate simple 2 additive supermodular (convex) and submodular capacities
-// size is the returned size of each vector in compact representation (singletons and pairs only
-int generate_fm_2additive_convexCall(int_64* num, int* n, int * size, double * vv)
-{
-    return  generate_fm_2additive_convex(*num, *n,  size,  vv);
-}
-
-int generate_fm_2additive_concaveCall(int_64* num, int* n, int * size, double * vv)
-{
-    return  generate_fm_2additive_concave(*num, *n, size, vv);
-}
-
-int generate_fm_2additive_convex_withsomeindependentCall(int_64* num, int* n, int * size, double * vv)
-// as above, but resets randomly some interactions to 0
-{
-    return generate_fm_2additive_convex_withsomeindependent(*num, *n, size, vv);
-}
-
-
-
-#ifdef NH_USED_IN_R_INTERFACE 
 
 // generate fuzzy measures randomly using topological sort
 void generate_fm_tsortCall(int* num1, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials)
 {
 	card = Rcard;
 	cardpos = Rcardpos;
 	bit2card = (int_64*)Rbit2card;
@@ -2088,29 +2058,202 @@
 void generate_fm_2additive_convex_withsomeindependentCall(int* num1, int* n, int * size, double * vv)
 // as above, but resets randomly some interactions to 0
 {
 			int_64 num=*num1;
 	 generate_fm_2additive_convex_withsomeindependent(num, *n, size, vv);
 }
 
-#endif // NH_USED_IN_R_INTERFACE
 
 void export_maximal_chainsCall(int* n,  double * v, double * mc, double* Rfactorials)
 {
 	m_factorials = Rfactorials;
 	int_64 m = (int_64)1 << (*n);
 	export_maximal_chains(*n, m, v, mc);
 }
 void export_maximal_chainsCall1(int* n, int_64* m, double * v, double * mc, double* Rfactorials)
 {
 	m_factorials = Rfactorials;
-	export_maximal_chains(*n, *m, v, mc);
+	int_64 m1=*m;
+	export_maximal_chains(*n, m1, v, mc);
+}
+
+
+
+/* ================== new version 5 ======================== */
+
+
+
+ void generate_fm_sortingCall(int* num, int* n, int* markov, int* option, double* vv,
+ int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	//int_64 mm = (int_64)*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+ 
+	 int_64 num1=*num;	 
+	 generate_fm_sorting01(num1, *n, *markov, *option, vv);
+ }
+
+
+ void CheckMonotonicitySortMergeCall(double* v, double* indices, int* m, int* n, int* out)
+  {
+	 int_64 m1=*m;	 
+	 int_64* 	Indices = (int_64*)indices; // casting
+     for(int_64 i=0;i<m1;i++) Indices[i]=i; // initialise
+	  *out=  CheckMonotonicitySortMerge(v,Indices, m1, *n);
+ }
+ void CheckMonotonicitySortInsertCall(double* v, double* indices, int* m, int* n, int* out)
+  {
+	 int_64 m1=*m;	 
+	 int_64* 	Indices = (int_64*)indices;
+	  *out=  CheckMonotonicitySortInsert(v,Indices, m1, *n);
+ }
+ void CheckMonotonicitySimpleCall(double* v, int* m, int* n, int* out)
+  {
+	 int_64 m1=*m;	 	 
+	 *out= CheckMonotonicitySimple(v, m1, *n);
+ }
+
+
+  void GenerateAntibuoyantCall( int* n,  double* out	,
+  int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+   
+	 int_64 m1=*m;	 
+	 GenerateAntibuoyant( *n, m1, out);
+ }
+//LIBDLL_API int generate_fm_simple_randomwalk(int_64 num, int n, int markov, int option, double noise, double* vv, void* extrachecks);
+//LIBDLL_API int generate_fm_convex_randomwalk(int_64 num, int n, int markov, int option, double noise, double* vv, void* extrachecks);
+
+
+ void CheckMonotonicityMobCall(double* Mob, int* n, int* m, int* len, int* out,
+  int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+  {
+	 int_64 len1=*len;	 
+	 
+	 int_64 mm = (int_64)*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+	 
+	 *out= CheckMonotonicityMob(Mob, *n, mm, len1);
+ }
+ void CheckConvexityMonMobCall(double* Mob, int* n, int* m, int* len, int* out,
+int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+  {
+
+	 int_64 len1=*len;	 
+	 
+	 int_64 mm = (int_64)*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+	 
+	 *out= CheckConvexityMonMob(Mob, *n, mm, len1);
+ }
+
+//LIBDLL_API int generate_fm_kadditive_randomwalk(int_64 num, int n, int kadd, int markov, int option, double noise, double* vv, void* extrachecks);
+//LIBDLL_API int generate_fm_kadditiveconvex_randomwalk(int_64 num, int n, int kadd, int markov, int option, double noise, double* vv, void* extrachecks);
+ void generate_fm_beliefCall(int* num, int* n, int* kadd,  double* vv, int* out,
+ int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	//int_64 mm = (int_64)*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+   // return length
+	 int_64 num1=*num;	
+	 int_64 len1;	
+	 generate_fm_belief(num1, *n, *kadd, &len1,  vv);
+	 *out= (int)len1;
+ }
+ void generate_fm_balancedCall(int* num, int* n, double* vv, int* out,
+ 	int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	//int_64 mm = (int_64)*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+  
+	 int_64 num1=*num;		
+	 *out= generate_fm_balanced(num1, *n,  vv);
+ }
+
+
+// 2 additive
+ void generate_fm_2additiveCall(int* num, int* n,  double* vv, int* out)
+  {
+	 int_64 num1=*num;		
+	 *out= generate_fm_2additive(num1, *n,  0, vv);
+ }
+
+  void CheckMonMob2additive2Call(double* Mob, int* n, int* length, double* temp, int* out)
+   {
+	 *out= CheckMonMob2additive2(Mob, *n,  *length, temp);
+  }
+
+
+int  fitting2additive(int *n, int* datanum, int* len, int* options, double* indexlow, double* indexhigh, int* option1, double* orness, double *v, double *Dataset)
+{
+	// returns Mobius in cardinality ordering
+	int res;
+	int nn = *n;
+	int datanums = *datanum;
+	int length = *len;
+	
+	res = FuzzyMeasureFit2additive(nn,  datanums,  length, *options, indexlow, indexhigh, *option1, orness,
+	v,  Dataset);
+
+	return res;
+}
+
+void ConvertCoMob2KinterCall(int* n,  int* kadd, int* len, double* mu, double* Mob, int* fulmu,
+	int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	int_64 mm=*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+	ConvertCoMob2Kinter(mu, Mob, *n, mm, *kadd, *len, *fulmu);
+}
+void ChoquetCoMobKInterCall(double*x, double* Mob, int *n, int* kadd, int* len, double& choMob,  
+	int* m, int* Rcard, int* Rcardpos, double* Rbit2card, double* Rcard2bit, double* Rfactorials)
+{
+	int_64 mm=*m;
+	card = Rcard;
+	cardpos = Rcardpos;
+	bit2card = (int_64*)Rbit2card;
+	card2bit = (int_64*)Rcard2bit;
+	m_factorials = Rfactorials;
+	choMob=ChoquetCoMobKInter(x, Mob, *n, mm, *kadd, *len );
 }
 
 
+
+/* ================== end new version 5 ======================== */
+
+
 #ifdef PYTHON_
 
 // python wrapper
 LIBEXP void py_export_maximal_chains(int n, double* v, double* mc, struct fm_env* env)
 {
 	int_64 m = (int_64)1 << (n);
 	export_maximal_chainsCall1(&n, &m, v, mc, env->factorials);
@@ -2135,96 +2278,235 @@
 
 
 LIBEXP int py_fm_arraysize(int n, int kint, struct fm_env* env)
 {
 	int_64 m = (int_64)1 << (n);
 	return fm_arraysizeCall(&n, &m, &kint, env->factorials);
 }
+LIBEXP int py_fm_arraysize_kadd(int n, int kint, struct fm_env* env)
+{
+    int_64 m = (int_64)1 << (n);
+    return fm_arraysizekaddCall(&n, &m, &kint, env->factorials);
+}
 
 LIBEXP int py_generate_fm_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env)
 {
-	int_64 num1 = num;
-	// NH: change num to num1 in parameter list
-	generate_fm_tsortCall(&num1, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
-	return num;
+	//int_64 num1 = num;
+	 generate_fm_tsortCall(&num, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+    return 0;
 }
-
 LIBEXP int py_generate_fmconvex_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env)
 {
-	int_64 num1 = num;
-	// NH: change num to num1 in parameter list
-	return generate_fmconvex_tsortCall(&num1, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	 generate_fmconvex_tsortCall(&num, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+    return 0;
 }
 LIBEXP int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env)
 {
-	int_64 num1 = num;
-	// NH: change num to num1 in parameter list
-	return generate_fm_minplusCall(&num1, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	 generate_fm_minplusCall(&num, &n, &kint, &markov, &option, &K, vv, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+    return 0;
 }
 
 LIBEXP int py_generate_fm_2additive_convex(int num, int n,  double * vv)
 {
-	int_64 num1 = num;
+	//int_64 num1 = num;
 	int size;
-	// NH: change num to num1 in parameter list
-	generate_fm_2additive_convexCall(&num1, &n, &size, vv);
+	generate_fm_2additive_convexCall(&num, &n, &size, vv);
 	return size;
 }
 
 LIBEXP int py_generate_fm_2additive_concave(int num, int n, double * vv)
 {
-	int_64 num1 = num;
+	//int_64 num1 = num;
 	int size;
-	// NH: change num to num1 in parameter list
-	generate_fm_2additive_concaveCall(&num1, &n, &size, vv);
+	generate_fm_2additive_concaveCall(&num, &n, &size, vv);
 	return size;
 }
 
 LIBEXP int py_generate_fm_2additive_convex_withsomeindependent(int num, int n,  double * vv)
 {
-	int_64 num1 = num;
+	//int_64 num1 = num;
 	int size;
-	// NH: change num to num1 in parameter list
-	generate_fm_2additive_convex_withsomeindependentCall(&num1, &n, &size, vv);
+	generate_fm_2additive_convex_withsomeindependentCall(&num, &n, &size, vv);
 	return size;
 }
 
+// ====  new version 5 ======
+
+LIBEXP void py_generate_fm_sorting(int num, int n, int markov, int option, double * vv, struct fm_env* env)
+{
+	generate_fm_sortingCall(&num, &n, &markov, &option, vv,  &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+}
+
+LIBEXP int py_CheckMonotonicitySortMerge(double * vv, double* indices, struct fm_env* env)
+{
+	int out;
+	CheckMonotonicitySortMergeCall( vv, indices, &(env->m), &(env->n), &out);
+	return out;
+}
+
+LIBEXP int py_CheckMonotonicitySortInsert(double * vv, double* indices, struct fm_env* env)
+{
+	int out;
+	CheckMonotonicitySortInsertCall( vv, indices, &(env->m), &(env->n), &out);
+	return out;
+}
+
+LIBEXP int py_CheckMonotonicitySimple(double * vv,struct fm_env* env)
+{
+	int out;
+	CheckMonotonicitySimpleCall( vv,  &(env->m), &(env->n), &out);
+	return out;
+}
+
+LIBEXP void py_GenerateAntibuoyant( double * vv, struct fm_env* env)
+{
+	GenerateAntibuoyantCall(&(env->n), vv, &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+}
+LIBEXP int py_generate_fm_belief(int num, int n, int kadd, double * vv, struct fm_env* env)
+{
+	int out; //length, or not needed?
+	generate_fm_beliefCall(&num, &n, &kadd, vv, &out, &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	return out;
+}
+LIBEXP int py_generate_fm_balanced(int num, int n,  double * vv, struct fm_env* env)
+{
+	int out; //length, or not needed?
+	generate_fm_balancedCall(&num, &n,  vv, &out, &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	return out;
+}
+
+LIBEXP int py_generate_fm_2additive(int num, int n,  double * vv)
+{
+	int out; //length, or not needed?
+	generate_fm_2additiveCall(&num, &n,  vv, &out);
+	return out;
+}
+
+LIBEXP int py_CheckMonMob2additive2(double * vv, int n, int length, double* temp)
+{
+	int out; 
+	CheckMonMob2additive2Call(vv, &n,  &length, temp, &out);
+	return out;
+}
+
+LIBEXP int py_CheckMonotonicityMob(double * vv, int len, struct fm_env* env)
+{
+	int out; 
+	CheckMonotonicityMobCall(vv, &(env->n),  &(env->m), &len, &out, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	return out;
+}
+LIBEXP int py_CheckConvexityMonMob(double * vv, int len, struct fm_env* env)
+{
+	int out; 
+	CheckConvexityMonMobCall(vv, &(env->n),  &(env->m), &len, &out, env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	return out;
+}
+
+
+LIBEXP void py_ConvertCoMob2KinterCall(int n, int kint, int len, double* mu, double * vv, int fullmu, struct fm_env* env)
+{
+	ConvertCoMob2KinterCall( &n, &kint, &len, mu, vv, &fullmu, &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+}
+
+
+LIBEXP double py_ChoquetCoMobKInter(double* x, double* Mob, int kadd, int len, struct fm_env* env)
+{
+	// Calculates ChoquetMob integral
+	double c;
+	ChoquetCoMobKInterCall(x, Mob, &(env->n), &kadd, &len, c, &(env->m), env->card, env->cardpos, env->bit2card, env->card2bit, env->factorials);
+	return c;
+}
+
+LIBEXP void py_fitting2additive(int datanum, int n, int len,
+                        double* v, double* dataset, int  options, double* indexlow, double* indexhi, int option1, double* orness)
+{
+	int res=fitting2additive(&n, &datanum,  &len,  &options, indexlow,indexhi , &option1,orness,        v, dataset);
+
+}
 
+LIBEXP int py_generate_fm_randomwalk(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks)
+{
+    struct  fm_env* env1 = (struct  fm_env*)env;
+    //fm_env* env=as<fm_env*>(env);
+  card=env1->card;
+  cardpos=env1->cardpos;
+  bit2card=(int_64*)env1->bit2card;
+  card2bit=(int_64*)env1->card2bit;
+  m_factorials=env1->factorials;
+    
+    int len;
+    int out;
+    if(extrachecks==NULL) out = generate_fm_randomwalk(num, n, kint, markov, option, step, vv, &len, NULL);
+        else out = generate_fm_randomwalk(num, n, kint, markov, option, step, vv, &len, extrachecks);
+    
+    return out;
+}
+
+LIBEXP int py_generate_fm_kinteractivedualconvex(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks)
+{
+    struct  fm_env* env1 = (struct  fm_env*)env;
+    //fm_env* env=as<fm_env*>(env);
+  card=env1->card;
+  cardpos=env1->cardpos;
+  bit2card=(int_64*)env1->bit2card;
+  card2bit=(int_64*)env1->card2bit;
+  m_factorials=env1->factorials;
+    int_64 num1=num;
+    int_64 len=option;
+    int out;
+    if(extrachecks==NULL) out = generate_fm_kinteractivedualconvex(num1, n, kint, markov, &len, step, vv,  NULL);
+        else out = generate_fm_kinteractivedualconvex(num1, n, kint, markov, &len, step, vv,  extrachecks);
+    
+    return out;
+}
+LIBEXP int py_generate_fm_kinteractivedualconcave(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks)
+{
+    struct  fm_env* env1 = (struct  fm_env*)env;
+    //fm_env* env=as<fm_env*>(env);
+  card=env1->card;
+  cardpos=env1->cardpos;
+  bit2card=(int_64*)env1->bit2card;
+  card2bit=(int_64*)env1->card2bit;
+  m_factorials=env1->factorials;
+    int_64 num1=num;
+    
+    int_64 len=option;
+    int out;
+    if(extrachecks==NULL) out = generate_fm_kinteractivedualconcave(num1, n, kint, markov, &len, step, vv,  NULL);
+        else out = generate_fm_kinteractivedualconcave(num1, n, kint, markov, &len, step, vv,  extrachecks);
+    
+    return out;
+}
+
+
+LIBEXP int py_generate_fm_2additive_randomwalk2(int num, int n, int markov, int option, double step,  double * vv, void* extrachecks)
+{
+    int out;
+    if(extrachecks==NULL) out = generate_fm_2additive_randomwalk2(num, n,  markov, option, step, vv,  NULL);
+        else out = generate_fm_2additive_randomwalk2(num, n,  markov, option, step, vv,  extrachecks);
+    
+    return out;
+}
 
+// ==== end new version 5 ======
 
 /*
 Sparse representation of k-additive capacities. Thre representation is in the form of singletons, pairs and tuples with nonzero values, stored and indexed in the respective
 arrays (see above in this file)
 
  Prepares an empty structure, given the list of cardinalities of the nonzero tuples (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
 
  It is used to allocate storage and later populate these values
 */
-
-// SparseFM::SparseFM() {}
-// SparseFM::SparseFM( struct  fm_env_sparse* penv): 
-// 	   n(penv->n),
-//     m_singletons( penv->m_singletons, penv->m_singletons + penv->n),
-//     m_pairs( penv->m_pairs, penv->m_pairs + penv->n),
-//     m_tuples( penv->m_tuples, penv->m_tuples + penv->n),
-//     m_pair_index( penv->m_pair_index, penv->m_pair_index + penv->n),
-//     m_tuple_start( penv->m_tuple_start, penv->m_tuple_start + penv->n),
-//     m_tuple_content( penv->m_tuple_content, penv->m_tuple_content + penv->n) {}
-
 LIBEXP void py_prepare_fm_sparse( int n, int tupsize, int* tuples, struct fm_env_sparse* env)
 {
-	// SparseFM* psFM = new SparseFM( env); 
-	// Prepare_FM_sparse0(n, tupsize, tuples, psFM);
-	// env->m_sparce_fm = psFM;
-
-	Prepare_FM_sparse0(n, tupsize, tuples, (SparseFM*)env);
+	 Prepare_FM_sparse0(n, tupsize, tuples, (SparseFM*)env);
 }
 LIBEXP void py_free_fm_sparse(struct fm_env_sparse* env) {
 	Free_FM_sparse((SparseFM*)env);
-	// delete( (SparseFM*)env->m_sparce_fm);
 }
 
 /*  Returns the cardinality of the tuple numbered i in the list of tuples */
 LIBEXP int py_tuple_cardinality_sparse(int i, struct fm_env_sparse* env)
 {
 	return TupleCardinalitySparse(i, (SparseFM*)env);
 }
@@ -2357,15 +2639,14 @@
 #endif
 
 
 //}  // end extern "C"
 
 
 
-#ifdef __R
 
 void copycontent(struct SparseFM* env, double* singletons, double* pairs, double* tuples, int* pairsidx, int* tuplesidx, int* tuplescon, int* dims)
 {
 	dims[0]=env->m_pairs.size();
 	dims[1]=env->m_tuples.size();
 	dims[2]=env->m_tuple_start.size();
 	dims[3]=env->m_tuple_content.size();	
@@ -2424,14 +2705,15 @@
 
  
  
 
  
 
 
+#ifdef __R
 #include <R_ext/Rdynload.h>    
 #include <R_ext/Visibility.h>
 
 #include <Rdefines.h>
 
 /*
 static void _finalizer(SEXP ext)
@@ -2465,15 +2747,14 @@
 	//struct SparseFM *envsp = (struct SparseFM*) R_ExternalPtrAddr(ext);
 	void* envsp = (void*) (R_ExternalPtrAddr(ext));
 
 	return (void*) envsp;
 }
 
 
-
  
  
  
  
 void Prepare_FM_sparseCall(int*   n, int* tupsz, double* tup, int*  tupidx,
 double* singletons, double* pairs, double* tuples, int* pairsidx, int* tuplesidx, int* tuplescon, int* dims 
 )
```

### Comparing `pyfmtools-0.81/src/wrapperpy.h` & `pyfmtools-5.1/src/wrapperpy.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,376 +1,435 @@
-//
-/* This is a C-wrapper for fmtools library for python
-
-   Gleb Beliakov, 2020
-*/
-
-
-
-#include <stdlib.h>
-
-#define PYTHON_
-#include "generaldefs.h"
-
-#ifdef __cplusplus
-
-#include "fuzzymeasuretools.h"
-#include "fuzzymeasurefit.h"
-
-
-#if defined  (_WIN32)
-#define LIBEXP 	__declspec(dllexport)  
-#else
-#define LIBEXP 
-#endif
-
-extern "C" {
-#endif
-
-//NH
-#define LIBEXP extern
-
-	typedef unsigned long long int_64; 
-
-	struct  fm_env {
-		int n;
-		int m;
-		int* card;
-		int* cardpos;
-		double* bit2card;
-		double* card2bit;
-		double* factorials;
-
-	};
-
-
-
-	struct  fm_env_sparse { // to use in wrappers, just to keep pointers. pointers might change when vectors are growing, but steady afterwards
-		int xx[40]; // Dummy value to allocate memory and avoid segmentation fault in py_prepare_fm_sparse
-	};
-
-
-
-	LIBEXP double py_min_subset(double* x, int n, int_64 S);
-	LIBEXP double py_max_subset(double* x, int n, int_64 S);
-
-	LIBEXP void py_ConvertCard2Bit(double* dest, double* src, struct fm_env* env);
-
-	LIBEXP double py_min_subsetC(double* x, int n, int_64 S, struct fm_env* env);
-	LIBEXP double py_max_subsetNegC(double* x, int n, int_64 S, struct fm_env* env);
-
-	LIBEXP int py_SizeArraykinteractive(int n, int k, struct fm_env* env);
-	LIBEXP int py_IsSubsetC(int i, int j, struct fm_env* env); // is i subset j?
-	LIBEXP int py_IsElementC(int i, int j, struct fm_env* env);  // is i an element of j?
-
-	LIBEXP void py_ExpandKinteractive2Bit(double* dest, double* src, struct fm_env* env, int kint, int arraysize);
-	LIBEXP void py_ExpandKinteractive2Bit_m(double* dest, double* src, struct fm_env* env, int kint, int arraysize, double* VVC);
-	/* Python interface call these two methods to allocate/deallocate memory */
-
-	LIBEXP void py_fm_init(int n, struct fm_env* env);
-	LIBEXP void py_fm_free(struct fm_env* env);
-
-
-	//inline?
-	LIBEXP void py_Shapley(double* v, double* x, struct fm_env* env);
-	LIBEXP void py_Banzhaf(double* v, double* B, struct fm_env* env);
-
-	LIBEXP void py_ShapleyMob(double* Mob, double* B, struct fm_env* env);
-	LIBEXP void py_BanzhafMob(double* Mob, double* B, struct fm_env* env);
-
-	LIBEXP double py_Choquet(double* x, double* v, struct fm_env* env);
-
-	LIBEXP double py_ChoquetKinter(double* x, double* v, int kint, struct fm_env* env);
-
-
-	/*  Add here the rest of the C calls for all the functions */
-	LIBEXP double py_ChoquetMob(double* x, double* Mob, struct fm_env* env);
-
-
-	LIBEXP void py_ConstructLambdaMeasure(double* singletons, double* lambda, double* v, struct fm_env* env);
-
-	LIBEXP void py_ConstructLambdaMeasureMob(double* singletons, double* lambda, double* Mob, struct fm_env* env); // jb
-
-
-	LIBEXP void py_dualm(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_dualmMob(double* v, double* w, struct fm_env* env);
-
-
-	LIBEXP double py_Entropy(double* v, struct fm_env* env);
-
-
-	LIBEXP void py_FuzzyMeasureFit(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
-
-	LIBEXP void py_FuzzyMeasureFitMob(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
-
-
-	LIBEXP void py_FuzzyMeasureFitKtolerant(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKmaxitive(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKinteractive(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMaxChains(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKinteractiveAutoK(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int* maxiters);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMarginal(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int submod);
-
-
-	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMarginalMaxChain(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int* maxiters, int submod);
-
-
-	LIBEXP void py_FuzzyMeasureFitLP(int datanum, int additive, struct fm_env* env, double* v, double* dataset, int * options, double* indexlow, double* indexhihg, int* option1, double* orness);
-
-	LIBEXP void py_FuzzyMeasureFitLPMob(int datanum, int additive, struct fm_env* env, double* v, double* dataset, int * options, double* indexlow, double* indexhihg, int* option1, double* orness);
-
-
-	LIBEXP void py_fittingOWA(int datanum, struct fm_env* env, double* v, double* dataset);
-
-	LIBEXP void py_fittingWAM(int datanum, struct fm_env* env, double* v, double* dataset);
-
-	LIBEXP void py_Interaction(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_InteractionB(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_InteractionMob(double* Mob, double* w, struct fm_env* env); // jb
-
-	LIBEXP void py_InteractionBMob(double* Mob, double* w, struct fm_env* env); // jb
-
-
-	LIBEXP void py_BipartitionShapleyIndex(double* v, double* w, struct fm_env* env);
-
-
-	LIBEXP void py_BipartitionBanzhafIndex(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_BNonadditivityIndexMob(double* Mob, double* w, struct fm_env* env);
-	       
-
-	LIBEXP void py_NonadditivityIndex(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_NonmodularityIndex(double* v, double* w, struct fm_env* env);
-
-	LIBEXP void py_NonmodularityIndexMob(double* Mob, double* w, struct fm_env* env);	
-	
-	LIBEXP void py_NonmodularityIndexKinteractive(double* v, double* w, int kint,  struct fm_env* env);
-
-	LIBEXP void py_NonmodularityIndexMobkadditive(double* Mob, double* w, int k, struct fm_env* env);
-
-
-
-	/*For small n returns the names of the coalitions as decimal strings in the binary and cardinality ordering, like 0,1,2,12,3,13,23,123 , for printing */
-	LIBEXP void py_ShowCoalitions(int* coalition, struct fm_env* env);
-	LIBEXP void py_ShowCoalitionsCard(int* coalition, struct fm_env* env);
-
-	LIBEXP int py_IsMeasureAdditive(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureBalanced(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSelfdual(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSubadditive(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSubmodular(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSuperadditive(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSupermodular(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureSymmetric(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureKMaxitive(double* v, struct fm_env* env);
-
-
-	LIBEXP int py_IsMeasureAdditiveMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureBalancedMob(double* Mob, struct fm_env* env); // jb
-
-
-
-	LIBEXP int py_IsMeasureSelfdualMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureSubadditiveMob(double* Mob, struct fm_env* env); // jb
-	
-	LIBEXP int py_IsMeasureSubmodularMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureSuperadditiveMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureSupermodularMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureSymmetricMob(double* Mob, struct fm_env* env); // jb
-
-	LIBEXP int py_IsMeasureKMaxitiveMob(double* Mob, struct fm_env* env); // jb
-
-
-
-
-	LIBEXP void py_Mobius(double* v, double* MobVal, struct fm_env* env);
-
-	LIBEXP double py_Orness(double* Mob, struct fm_env* env);
-
-
-	LIBEXP double py_OWA(double* x, double* v, struct fm_env* env);
-
-
-
-
-	LIBEXP double py_Sugeno(double* x, double* v, struct fm_env* env);
-
-
-	LIBEXP double py_WAM(double* x, double* v, struct fm_env* env);
-
-
-	LIBEXP void py_Zeta(double* Mob, double* v, struct fm_env* env);
-
-
-	// random generation and other functions
-
-
-	LIBEXP void py_dualMobKadd(int m, int length, int k, double* src, double* dest, struct fm_env* env);
-
-	LIBEXP void py_Shapley2addMob(double* v, double* x, int n);
-
-	LIBEXP void py_Banzhaf2addMob(double* v, double* x, int n);
-
-	LIBEXP double py_Choquet2addMob(double*x, double* Mob, int n);
-
-
-
-	LIBEXP int py_fm_arraysize(int n, int kint, struct fm_env* env);
-
-
-	LIBEXP int generate_fm_tsortCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials);
-	LIBEXP int generate_fmconvex_tsortCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials);	
-	LIBEXP int generate_fm_minplusCall(int_64* num, int* n, int* kint, int* markov, int* option, double* K, double * vv, int* Rcard, int*  Rcardpos, double*  Rbit2card, double*  Rcard2bit, double* Rfactorials);
-	LIBEXP int generate_fm_2additive_convexCall(int_64* num, int* n, int * size, double * vv);
-	LIBEXP int generate_fm_2additive_concaveCall(int_64* num, int* n, int * size, double * vv);
-	LIBEXP int generate_fm_2additive_convex_withsomeindependentCall(int_64* num, int* n, int * size, double * vv);
-
-	#ifdef NH_USED_IN_R_INTERFACE
-	LIBEXP int py_generate_fm_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-	LIBEXP int py_generate_fmconvex_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-	LIBEXP int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-
-	LIBEXP int py_generate_fm_2additive_convex(int num, int n, double * vv);
-
-
-	LIBEXP int py_generate_fm_2additive_concave(int num, int n,  double * vv);
-
-
-	LIBEXP int py_generate_fm_2additive_convex_withsomeindependent(int num, int n,  double * vv);
-
-	#else
-
-    int py_generate_fm_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-	int py_generate_fmconvex_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-	int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
-
-
-	int py_generate_fm_2additive_convex(int num, int n, double * vv);
-
-
-	int py_generate_fm_2additive_concave(int num, int n,  double * vv);
-
-
-	int py_generate_fm_2additive_convex_withsomeindependent(int num, int n,  double * vv);
-
-	#endif // NH_USED_IN_R_INTERFACE
-
-
-
-	LIBEXP void py_export_maximal_chains(int n, double* v, double* mc, struct fm_env* env);
-	/*
-	Sparse representation of k-additive capacities. Thre representation is in the form of singletons, pairs and tuples with nonzero values, stored and indexed in the respective
-	arrays (see above in this file)
-
-	 Prepares an empty structure, given the list of cardinalities of the nonzero tuples (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
-
-	 It is used to allocate storage and later populate these values
-	*/
-	LIBEXP void py_prepare_fm_sparse(int n, int tupsize, int* tuples, struct fm_env_sparse* env);
-	LIBEXP void py_free_fm_sparse( struct fm_env_sparse* env);
-
-	/*  Returns the cardinality of the tuple numbered i in the list of tuples */
-	LIBEXP int py_tuple_cardinality_sparse(int i, struct fm_env_sparse* env);
-
-	LIBEXP int py_get_num_tuples(struct fm_env_sparse* env);
-	LIBEXP int py_get_sizearray_tuples(struct fm_env_sparse* env);
-
-	/* checks if element i (1-based!!!) belongs to the tuple indexed A (whose cardinality can be 1,2, other (automatically determined) */
-	LIBEXP int py_is_inset_sparse(int A, int card, int i, struct fm_env_sparse* env);
-
-	/* checks if tuple B is a subset of A */
-	LIBEXP int py_is_subset_sparse(int A, int cardA, int B, int cardB, struct fm_env_sparse* env);
-
-	/* calculates minimum (maximum) of (x_i) with the indices belonging to tuple indexed as S (its cardinality cardS can be 1,2, other( put 3, will be determined automatically)
-	note that x is 0-based, tuples are 1-based */
-	LIBEXP double py_min_subset_sparse(double* x, int n, int S, int cardS, struct fm_env_sparse* env);
-	LIBEXP double py_max_subset_sparse(double* x, int n, int S, int cardS, struct fm_env_sparse* env);
-
-	/* calculates the Choquet integral in Mobius representation */
-	LIBEXP double py_ChoquetMob_sparse(double* x, int n, struct fm_env_sparse* env);
-
-
-	/* Shapley and Banzhaf values vector of a capacity */
-	LIBEXP void py_ShapleyMob_sparse(double* v, int n, struct fm_env_sparse* env);
-	LIBEXP void py_BanzhafMob_sparse(double* v, int n, struct fm_env_sparse* env);
-
-	/* populates 2-additive sparse capacity with nonzero values using the singletons and two arrays of indices (of size numpairs) . Indices need to be 1-based. Singletons 0-based */
-	LIBEXP void py_populate_fm_2add_sparse(double* singletons, int numpairs, double* pairs, int* indicesp1, int* indicesp2, struct fm_env_sparse* env);
-
-	/* for populating capacities. Add pair (v_ij) to the structure. indices are 1-based */
-	LIBEXP void py_add_pair_sparse(int i, int j, double v, struct fm_env_sparse* env);
-
-	/* for populating capacities, adds a tuple of size tupsize whose 1-based indices are in tuple */
-	LIBEXP void py_add_tuple_sparse(int tupsize, int* tuple, double v, struct fm_env_sparse* env);
-
-	/* Given 2-additive capacity singletons=pairs in one array v , selects nonzero pairs */
-	LIBEXP void py_populate_fm_2add_sparse_from2add(int n, double * v, struct fm_env_sparse* env);
-
-	/* from sparse to full representaiotn of 2-additive capacity (singletons and paits, augmented with 0 ) Vector v has to be allocated, size is n+ n(n-1)/2 */
-	LIBEXP void py_expand_2add_full(double* v, struct fm_env_sparse* env);
-
-	/* from sparse to full capacity (vector v, size 2^n has to be preallocated) */
-	LIBEXP void py_expand_sparse_full(double* v, struct fm_env_sparse* env);
-
-	LIBEXP void py_sparse_get_singletons(int n, double* v, struct fm_env_sparse* env);
-
-	LIBEXP int py_sparse_get_pairs(int* pairs, double* v, struct fm_env_sparse* env);
-
-	LIBEXP int py_sparse_get_tuples(int* tuples, double* v, struct fm_env_sparse* env);
-
-
-	/* random generation of  sparse supermodular capacities */
-	LIBEXP int   py_generate_fm_2additive_convex_sparse(int n, struct fm_env_sparse* env);
-
-	LIBEXP int   py_generate_fm_kadditive_convex_sparse(int n, int k, int nonzero, struct fm_env_sparse* env);
-
-	LIBEXP void py_Nonmodularityindex_sparse(double* w, int n, struct fm_env_sparse* env);
-
-#ifdef __cplusplus
-} 
-#endif
-
-
-
-
-
-
+//
+/* This is a C-wrapper for fmtools library for python
+
+   Gleb Beliakov, 2020
+*/
+
+
+
+#include <stdlib.h>
+
+#define PYTHON_
+#include "generaldefs.h"
+
+#ifdef __cplusplus
+
+#include "fuzzymeasuretools.h"
+#include "fuzzymeasurefit.h"
+
+
+#if defined  (_WIN32)
+#define LIBEXP 	__declspec(dllexport)  
+#else
+#define LIBEXP 
+#define LIBEXP extern
+#endif
+
+extern "C" {
+#endif
+
+
+	typedef unsigned long long int_64;
+
+	struct  fm_env {
+		int n;
+		int m;
+		int* card;
+		int* cardpos;
+		double* bit2card;
+		double* card2bit;
+		double* factorials;
+
+	};
+
+
+struct  fm_env_sparse { // to use in wrappers, just to keep pointers. pointers might change when vectors are growing, but steady afterwards
+    int xx[44]; // Dummy value to allocate memory and avoid segmentation fault in py_prepare_fm_sparse
+};
+
+/*
+	struct  fm_env_sparse { // to use in wrappers, just to keep pointers. pointers might change when vectors are growing, but steady afterwards
+		int n;		
+//		double *m_singletons;
+//		double* m_pairs;
+//		double* m_tuples;
+//		int* m_pair_index;
+//		int* m_tuple_start;
+//		int* m_tuple_content;
+		double* m_parentref;
+	};
+*/
+
+
+	LIBEXP double py_min_subset(double* x, int n, int_64 S);
+	LIBEXP double py_max_subset(double* x, int n, int_64 S);
+
+	LIBEXP void py_ConvertCard2Bit(double* dest, double* src, struct fm_env* env);
+
+	LIBEXP double py_min_subsetC(double* x, int n, int_64 S, struct fm_env* env);
+	LIBEXP double py_max_subsetNegC(double* x, int n, int_64 S, struct fm_env* env);
+
+	LIBEXP int py_SizeArraykinteractive(int n, int k, struct fm_env* env);
+	LIBEXP int py_IsSubsetC(int i, int j, struct fm_env* env); // is i subset j?
+	LIBEXP int py_IsElementC(int i, int j, struct fm_env* env);  // is i an element of j?
+
+	LIBEXP void py_ExpandKinteractive2Bit(double* dest, double* src, struct fm_env* env, int kint, int arraysize);
+	LIBEXP void py_ExpandKinteractive2Bit_m(double* dest, double* src, struct fm_env* env, int kint, int arraysize, double* VVC);
+	/* Python interface call these two methods to allocate/deallocate memory */
+
+	LIBEXP void py_fm_init(int n, struct fm_env* env);
+	LIBEXP void py_fm_free(struct fm_env* env);
+
+
+	//inline?
+	LIBEXP void py_Shapley(double* v, double* x, struct fm_env* env);
+	LIBEXP void py_Banzhaf(double* v, double* B, struct fm_env* env);
+
+	LIBEXP void py_ShapleyMob(double* Mob, double* B, struct fm_env* env);
+	LIBEXP void py_BanzhafMob(double* Mob, double* B, struct fm_env* env);
+
+	LIBEXP double py_Choquet(double* x, double* v, struct fm_env* env);
+
+	LIBEXP double py_ChoquetKinter(double* x, double* v, int kint, struct fm_env* env);
+
+
+	/*  Add here the rest of the C calls for all the functions */
+	LIBEXP double py_ChoquetMob(double* x, double* Mob, struct fm_env* env);
+
+
+	LIBEXP void py_ConstructLambdaMeasure(double* singletons, double* lambda, double* v, struct fm_env* env);
+
+	LIBEXP void py_ConstructLambdaMeasureMob(double* singletons, double* lambda, double* Mob, struct fm_env* env); // jb
+
+
+	LIBEXP void py_dualm(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_dualmMob(double* v, double* w, struct fm_env* env);
+
+
+	LIBEXP double py_Entropy(double* v, struct fm_env* env);
+
+
+	LIBEXP void py_FuzzyMeasureFit(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
+
+	LIBEXP void py_FuzzyMeasureFitMob(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
+
+
+	LIBEXP void py_FuzzyMeasureFitKtolerant(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKmaxitive(int datanum, int additive, struct fm_env* env, double* v, double* dataset);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKinteractive(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMaxChains(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKinteractiveAutoK(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int* maxiters);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMarginal(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int submod);
+
+
+	LIBEXP void py_FuzzyMeasureFitLPKinteractiveMarginalMaxChain(int datanum, int additive, struct fm_env* env, double* v, double* dataset, double* K, int* maxiters, int submod);
+
+
+	LIBEXP void py_FuzzyMeasureFitLP(int datanum, int additive, struct fm_env* env, double* v, double* dataset, int * options, double* indexlow, double* indexhihg, int* option1, double* orness);
+
+	LIBEXP void py_FuzzyMeasureFitLPMob(int datanum, int additive, struct fm_env* env, double* v, double* dataset, int * options, double* indexlow, double* indexhihg, int* option1, double* orness);
+
+
+	LIBEXP void py_fittingOWA(int datanum, struct fm_env* env, double* v, double* dataset);
+
+	LIBEXP void py_fittingWAM(int datanum, struct fm_env* env, double* v, double* dataset);
+
+	LIBEXP void py_Interaction(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_InteractionB(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_InteractionMob(double* Mob, double* w, struct fm_env* env); // jb
+
+	LIBEXP void py_InteractionBMob(double* Mob, double* w, struct fm_env* env); // jb
+
+
+	LIBEXP void py_BipartitionShapleyIndex(double* v, double* w, struct fm_env* env);
+
+
+	LIBEXP void py_BipartitionBanzhafIndex(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_NonadditivityIndexMob(double* Mob, double* w, struct fm_env* env);
+
+
+	LIBEXP void py_NonadditivityIndex(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_NonmodularityIndex(double* v, double* w, struct fm_env* env);
+
+	LIBEXP void py_NonmodularityIndexMob(double* Mob, double* w, struct fm_env* env);	
+	
+	LIBEXP void py_NonmodularityIndexKinteractive(double* v, double* w, int kint,  struct fm_env* env);
+
+	LIBEXP void py_NonmodularityIndexMobkadditive(double* Mob, double* w, int k, struct fm_env* env);
+
+
+
+	/*For small n returns the names of the coalitions as decimal strings in the binary and cardinality ordering, like 0,1,2,12,3,13,23,123 , for printing */
+	LIBEXP void py_ShowCoalitions(int* coalition, struct fm_env* env);
+	LIBEXP void py_ShowCoalitionsCard(int* coalition, struct fm_env* env);
+
+	LIBEXP int py_IsMeasureAdditive(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureBalanced(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSelfdual(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSubadditive(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSubmodular(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSuperadditive(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSupermodular(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureSymmetric(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureKMaxitive(double* v, struct fm_env* env);
+
+
+	LIBEXP int py_IsMeasureAdditiveMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureBalancedMob(double* Mob, struct fm_env* env); // jb
+
+
+
+	LIBEXP int py_IsMeasureSelfdualMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureSubadditiveMob(double* Mob, struct fm_env* env); // jb
+	
+	LIBEXP int py_IsMeasureSubmodularMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureSuperadditiveMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureSupermodularMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureSymmetricMob(double* Mob, struct fm_env* env); // jb
+
+	LIBEXP int py_IsMeasureKMaxitiveMob(double* Mob, struct fm_env* env); // jb
+
+
+
+
+	LIBEXP void py_Mobius(double* v, double* MobVal, struct fm_env* env);
+
+	LIBEXP double py_Orness(double* Mob, struct fm_env* env);
+
+
+    LIBEXP double py_OWA(double* x, double* v, struct fm_env* env);
+
+
+
+
+	LIBEXP double py_Sugeno(double* x, double* v, struct fm_env* env);
+
+
+    LIBEXP double py_WAM(double* x, double* v, struct fm_env* env);
+
+
+	LIBEXP void py_Zeta(double* Mob, double* v, struct fm_env* env);
+
+
+	// random generation and other functions
+
+
+	LIBEXP void py_dualMobKadd(int m, int length, int k, double* src, double* dest, struct fm_env* env);
+
+	LIBEXP void py_Shapley2addMob(double* v, double* x, int n);
+
+	LIBEXP void py_Banzhaf2addMob(double* v, double* x, int n);
+
+	LIBEXP double py_Choquet2addMob(double*x, double* Mob, int n);
+
+
+
+	LIBEXP int py_fm_arraysize(int n, int kint, struct fm_env* env);
+    LIBEXP int py_fm_arraysize_kadd(int n, int kint, struct fm_env* env);
+
+	LIBEXP int py_generate_fm_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
+
+	LIBEXP int py_generate_fmconvex_tsort(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
+
+	LIBEXP int py_generate_fm_minplus(int num, int n, int kint, int markov, int option, double K, double * vv, struct fm_env* env);
+
+
+	LIBEXP int py_generate_fm_2additive_convex(int num, int n, double * vv);
+
+
+	LIBEXP int py_generate_fm_2additive_concave(int num, int n,  double * vv);
+
+
+	LIBEXP int py_generate_fm_2additive_convex_withsomeindependent(int num, int n,  double * vv);
+
+	LIBEXP void py_export_maximal_chains(int n, double* v, double* mc, struct fm_env* env);
+
+
+
+
+
+
+	/*
+	Sparse representation of k-additive capacities. Thre representation is in the form of singletons, pairs and tuples with nonzero values, stored and indexed in the respective
+	arrays (see above in this file)
+
+	 Prepares an empty structure, given the list of cardinalities of the nonzero tuples (cardinality, tuple composition) like this 2 pairs 4-tuple and a triple:  (2,1,2,  2, 3,1,   4, 1,2,3,4,  3,3,2,1...)
+
+	 It is used to allocate storage and later populate these values
+	*/
+	LIBEXP void py_prepare_fm_sparse(int n, int tupsize, int* tuples, struct fm_env_sparse* env);
+	LIBEXP void py_free_fm_sparse( struct fm_env_sparse* env);
+
+	/*  Returns the cardinality of the tuple numbered i in the list of tuples */
+	LIBEXP int py_tuple_cardinality_sparse(int i, struct fm_env_sparse* env);
+
+	LIBEXP int py_get_num_tuples(struct fm_env_sparse* env);
+	LIBEXP int py_get_sizearray_tuples(struct fm_env_sparse* env);
+
+	/* checks if element i (1-based!!!) belongs to the tuple indexed A (whose cardinality can be 1,2, other (automatically determined) */
+	LIBEXP int py_is_inset_sparse(int A, int card, int i, struct fm_env_sparse* env);
+
+	/* checks if tuple B is a subset of A */
+	LIBEXP int py_is_subset_sparse(int A, int cardA, int B, int cardB, struct fm_env_sparse* env);
+
+	/* calculates minimum (maximum) of (x_i) with the indices belonging to tuple indexed as S (its cardinality cardS can be 1,2, other( put 3, will be determined automatically)
+	note that x is 0-based, tuples are 1-based */
+	LIBEXP double py_min_subset_sparse(double* x, int n, int S, int cardS, struct fm_env_sparse* env);
+	LIBEXP double py_max_subset_sparse(double* x, int n, int S, int cardS, struct fm_env_sparse* env);
+
+	/* calculates the Choquet integral in Mobius representation */
+	LIBEXP double py_ChoquetMob_sparse(double* x, int n, struct fm_env_sparse* env);
+
+
+	/* Shapley and Banzhaf values vector of a capacity */
+	LIBEXP void py_ShapleyMob_sparse(double* v, int n, struct fm_env_sparse* env);
+	LIBEXP void py_BanzhafMob_sparse(double* v, int n, struct fm_env_sparse* env);
+
+	/* populates 2-additive sparse capacity with nonzero values using the singletons and two arrays of indices (of size numpairs) . Indices need to be 1-based. Singletons 0-based */
+	LIBEXP void py_populate_fm_2add_sparse(double* singletons, int numpairs, double* pairs, int* indicesp1, int* indicesp2, struct fm_env_sparse* env);
+
+	/* for populating capacities. Add pair (v_ij) to the structure. indices are 1-based */
+	LIBEXP void py_add_pair_sparse(int i, int j, double v, struct fm_env_sparse* env);
+
+	/* for populating capacities, adds a tuple of size tupsize whose 1-based indices are in tuple */
+	LIBEXP void py_add_tuple_sparse(int tupsize, int* tuple, double v, struct fm_env_sparse* env);
+
+	/* Given 2-additive capacity singletons=pairs in one array v , selects nonzero pairs */
+	LIBEXP void py_populate_fm_2add_sparse_from2add(int n, double * v, struct fm_env_sparse* env);
+
+	/* from sparse to full representaiotn of 2-additive capacity (singletons and paits, augmented with 0 ) Vector v has to be allocated, size is n+ n(n-1)/2 */
+	LIBEXP void py_expand_2add_full(double* v, struct fm_env_sparse* env);
+
+	/* from sparse to full capacity (vector v, size 2^n has to be preallocated) */
+	LIBEXP void py_expand_sparse_full(double* v, struct fm_env_sparse* env);
+
+	LIBEXP void py_sparse_get_singletons(int n, double* v, struct fm_env_sparse* env);
+
+	LIBEXP int py_sparse_get_pairs(int* pairs, double* v, struct fm_env_sparse* env);
+
+	LIBEXP int py_sparse_get_tuples(int* tuples, double* v, struct fm_env_sparse* env);
+
+
+	/* random generation of  sparse supermodular capacities */
+	LIBEXP int   py_generate_fm_2additive_convex_sparse(int n, struct fm_env_sparse* env);
+
+	LIBEXP int   py_generate_fm_kadditive_convex_sparse(int n, int k, int nonzero, struct fm_env_sparse* env);
+
+	LIBEXP void py_Nonmodularityindex_sparse(double* w, int n, struct fm_env_sparse* env);
+
+//	LIBEXP void py_add_singletons_sparse(double* v, struct fm_env_sparse* env);
+
+
+
+/* ================== new version 5 ======================== */
+
+
+LIBEXP void py_generate_fm_sorting(int num, int n, int markov, int option, double * vv, struct fm_env* env);
+
+LIBEXP int py_CheckMonotonicitySortMerge(double * vv, double* indices, struct fm_env* env);
+
+LIBEXP int py_CheckMonotonicitySortInsert(double * vv, double* indices, struct fm_env* env);
+
+LIBEXP int py_CheckMonotonicitySimple(double * vv,struct fm_env* env);
+
+LIBEXP void py_GenerateAntibuoyant( double * vv, struct fm_env* env);
+LIBEXP int py_generate_fm_belief(int num, int n, int kadd, double * vv, struct fm_env* env);
+LIBEXP int py_generate_fm_balanced(int num, int n,  double * vv, struct fm_env* env);
+
+LIBEXP int py_generate_fm_2additive(int num, int n,  double * vv);
+
+LIBEXP int py_CheckMonMob2additive2(double * vv, int n, int length, double* temp);
+
+LIBEXP int py_CheckMonotonicityMob(double * vv, int len, struct fm_env* env);
+LIBEXP int py_CheckConvexityMonMob(double * vv, int len, struct fm_env* env);
+
+
+LIBEXP void py_ConvertCoMob2KinterCall(int n, int kint, int len, double* mu, double * vv, int fullmu, struct fm_env* env);
+
+
+LIBEXP double py_ChoquetCoMobKInter(double* x, double* Mob, int kadd, int len, struct fm_env* env);
+
+LIBEXP void py_fitting2additive(int datanum, int n, int len,
+                        double* v, double* dataset, int  options, double* indexlow, double* indexhi, int option1, double* orness);
+
+
+LIBEXP int py_generate_fm_randomwalk(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+
+LIBEXP int py_generate_fm_kinteractivedualconvex(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+LIBEXP int py_generate_fm_kinteractivedualconcave(int num, int n, int kint, int markov, int option, double step,  double * vv, struct fm_env* env, void* extrachecks);
+
+
+LIBEXP int py_generate_fm_2additive_randomwalk2(int num, int n, int markov, int option, double step,  double * vv, void* extrachecks);
+
+
+
+#ifdef __cplusplus
+}
+#endif
+
+
+
+
+
+
+#ifdef __R
+#include <R_ext/Rdynload.h>    
+#include <R_ext/Visibility.h>
+
+
+static const R_CallMethodDef callMethods[]  = {
+  {NULL, NULL, 0}
+};
+
+static R_NativePrimitiveArgType myC_t[] = {
+    INTSXP, INTSXP, INTSXP, INTSXP, INTSXP, INTSXP, REALSXP
+};
+
+static const R_CMethodDef cMethods[] = {
+   {"Preparations_FMCall", (DL_FUNC) &Preparations_FMCall, 7, myC_t},
+   {NULL, NULL, 0, NULL}
+};
+
+//Rfmtool
+void
+R_init_Rfmtool(DllInfo *info)
+{
+   R_registerRoutines(info, cMethods, callMethods, NULL, NULL);
+   R_useDynamicSymbols(info, TRUE); 
+}
+#endif
```

### Comparing `pyfmtools-0.81/src/yacc_read.c` & `pyfmtools-5.1/src/yacc_read.c`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,24 @@
 #endif
 
 #ifdef FORTIFY
 # include "lp_fortify.h"
 #endif
 
 
+
+int mysprintf5(char *str, const char *format, ...){
+	// do nothing
+	return 0;
+}
+#ifdef sprintf
+#undef sprintf
+#endif
+#define sprintf mysprintf5
+
 #define tol 1.0e-10
 #define coldatastep 100
 
 #define HASHSIZE       10007  /* A prime number! */
 
 static short      Maximise;
 static short      Ignore_int_decl;
@@ -140,15 +150,15 @@
 /* called when lex gets a fatal error */
 void lex_fatal_error(char *msg)
 {
   read_error(msg);
   longjmp(jump_buf, 1);
 }
 
-void add_row()
+void add_row(void)
 {
   Rows++;
   rs = NULL;
   Lin_term_count = 0;
 }
 
 void check_int_sec_sos_decl(int within_int_decl, int within_sec_decl, int sos_decl0)
@@ -548,15 +558,15 @@
   }
   else /* could be a bound */
     tmp_store.relat = tmp_relat;
 
   return(TRUE);
 } /* store_re_op */
 
-int negate_constraint()
+int negate_constraint(void)
 {
     if(rs != NULL)
       rs->negate = TRUE;
 
     return(TRUE);
 }
```

### Comparing `pyfmtools-0.81/src/yacc_read.h` & `pyfmtools-5.1/src/yacc_read.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/tests/test_no_wrapper.py` & `pyfmtools-5.1/tests/test_no_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.81/tests/test_wrapper.py` & `pyfmtools-5.1/tests/test_wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pyfmtools as pyfm
 import random
 import sys
 
 
 r=3
 n=3
@@ -467,18 +468,18 @@
 # not documented in R or Python user guide
 v = [0.0, 0.3, 0.5, -0.2, 0.4, 0.1]
 s = pyfm.BipartitionBanzhafIndex(v, env)
 print( "v: ", v)
 print( "s: ", s)
 
 # Test wrapper for:
-#    void py_BNonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)
+#    void py_NonadditivityIndexMob(double* Mob, double* out_w, struct fm_env* env)
 # not documented in R or Python user guide
 Mob = [0.2, 0.3, 0.5, -0.2, 0.4, 0.1]
-s = pyfm.BNonadditivityIndexMob(Mob, env)
+s = pyfm.NonadditivityIndexMob(Mob, env)
 print( "v: ", v)
 print( "s: ", s)
 
 # Test wrapper for:
 #    void py_NonadditivityIndex(double* v, double* out_w, struct fm_env* env)
 v = [0,0.3,0.5,0.6,0.4,0.8,0.7,1]
 w = pyfm.NonadditivityIndex(v, env)
@@ -932,14 +933,15 @@
 c_i = pyfm.ChoquetMob_sparse(x, env_sparse)
 print( "x: ", x)
 print( "Choquet integral: ", c_i)
 
 # Test wrapper for:
 #    void py_free_fm_sparse( struct fm_env_sparse* env)
 pyfm.free_fm_sparse( env_sparse)
+pyfm.fm_free(env)
 
 #
 # --- new env sparse for n = 5 ---
 #
 n = 5
 tupsize = 0
 env_sparse = pyfm.prepare_fm_sparse( n, tupsize)
@@ -963,10 +965,215 @@
 #
 # --- free env sparse for n = 5 ---
 #
 pyfm.free_fm_sparse( env_sparse)
 
 
 
+############# FUNCTIONS VERSION 5 #######
 
+#New Functions Pytmtools 5
+fm=pyfm
+#alias
+
+#fm.generate_fm_2additive(num, n)
+num=3
+n=5
+ret_code, v, len = fm.generate_fm_2additive(num, n)
+print(v)
+print(ret_code)
+print(len)
+
+#fm.CheckMonMob2additive2(v, n)
+ret_code, v, len =fm.generate_fm_2additive(1, 10)
+n=10
+check = fm.CheckMonMob2additive2(v, n)
+print(check)
+
+
+#fm.generate_fm_2additive_randomwalk2(num, n, markov, option, step, Fn)
+num=2
+n=5
+ret_code, v, len = fm.generate_fm_2additive_randomwalk2(num, n, 1000, 0, 0.001, None)
+print(v)
+print(ret_code)
+print(len)
+
+#fm.generate_fm_sorting(num, n, markov, option, env)
+env=fm.fm_init(3)
+markovsteps=100
+fuzzymeasures = fm.generate_fm_sorting(num, 3, markovsteps, 0, env)
+print(fuzzymeasures)
+
+#fm.generate_fm_balanced(num, n, env)
+#env=fm.fm_init(3)
+ret_code, v, len = fm.generate_fm_balanced(num, 3, env)
+print(v)
+print(ret_code)
+print(len)
+
+#fm.generateAntibuoyant(n, env)
+#env=fm.fm_init(3)
+antibuoyant = fm.generateAntibuoyant(3, env)
+print(antibuoyant)
+
+#fm.generate_fm_randomwalk(num, n, kadd, markov, option, step, env, Fn)
+def Fn(n, v):
+   out = 0.0
+   for i in range(n[0]):
+     out += v[i]
+   #print(out,n[0],v[1])
+   if out > 1:
+      return 0
+   else:
+      return 1
+#env=fm.fm_init(3)
+step=0.0010
+Option=3
+n=3
+ret_code, v,len= fm.generate_fm_randomwalk(num, n, 2, 10, Option, step, env, Fn)
+print(v)
+print(ret_code)
+print(len)
+
+#fm.CheckMonotonicitySortMerge(n, v, env)
+#env=fm.fm_init(3)
+n=3
+v=fm.generate_fm_sorting(1, 3, 1000, 0, env)
+print(v)
+ret_code, index = fm.CheckMonotonicitySortMerge(n, v, env)
+
+print(ret_code)
+#print(index)
+
+#fm.CheckMonotonicitySortInsert(v, indices, env)
+
+n=3
+# already initialised above
+#env=fm.fm_init(n)
+v=fm.generate_fm_sorting(1, n, 1000, 0, env)
+ret_code, index=fm.CheckMonotonicitySortMerge(n, v, env)
+v[1] *= 1.1
+ret_code, index=fm.CheckMonotonicitySortInsert(n, v, index, env)
+
+print(ret_code)
+#print(index)
+
+#fm.CheckMonotonicitySimple(v, env)
+
+#env=fm.fm_init(3)
+v=fm.generate_fm_sorting(1, 3, 1000, 0, env)
+monotonicity=fm.CheckMonotonicitySimple(v, env)
+
+print(monotonicity)
+
+#fm.CheckMonotonicityMob(Mob, len, env)
+
+#env=fm.fm_init(3)
+step=0.001
+Fn=None
+Option=3
+ret_code, Mob, len = fm.generate_fm_randomwalk(1, 3, 2, 1000, Option, step, env, Fn)
+print(len)
+check=fm.CheckMonotonicityMob(Mob, len, env)
+print(Mob)
+print(check)
+
+
+#fm.CheckConvexityMonMob(Mob, len, env)
+#env=fm.fm_init(3)
+step=0.001
+Fn=None
+Option=5
+#5 means convex kadditive
+ret_code, Mob, len = fm.generate_fm_randomwalk(1, 3, 2, 1000, Option, step, env, Fn)
+
+check=fm.CheckConvexityMonMob(Mob, len, env)
+print(Mob)
+print(check)
+
+fm.fm_free(env)
+
+#fm.generate_fm_kinteractivedualconvex(num, n, kadd, markov,  step, env, Fn)
+n=4
+env=fm.fm_init(n)
+step=0.001
+Fn=None
+ret_code, Mob, len = fm.generate_fm_kinteractivedualconvex(num, n, 2, 1000, step, env, Fn)
+print(Mob)
+print(ret_code)
+print(len)
+
+#fm.generate_fm_kinteractivedualconcave(num, n, kadd, markov,  step, env, Fn)
+#env=fm.fm_init(3)
+step=0.001
+Fn=None
+ret_code, Mob, len = fm.generate_fm_kinteractivedualconcave(num, n, 2, 1000, step, env, Fn)
+print(Mob)
+print(ret_code)
+print(len)
 
 
+
+
+#fm.ConvertCoMob2KinterCall(n, kadd, len, Mob, fullmu, env)
+
+n=4
+env=fm.fm_init(n)
+num=1
+fullmu=0
+step= 0.001
+Fn=None
+ret_code, Mob, len = fm.generate_fm_kinteractivedualconvex(num, n, 2, 1000,  step, env, Fn)
+print(Mob,len)
+v=fm.ConvertCoMob2Kinter(n, 2, len, Mob, fullmu, env)
+print(v)
+v=fm.ConvertCoMob2Kinter(n, 2, len, Mob, 1, env)
+print(v)
+#fm.ChoquetCoMobKInter(x, Mob, kadd, len, env)
+
+#env=fm.fm_init(3)
+step= 0.001
+Fn=None
+ret_code, Mob, len= fm.generate_fm_kinteractivedualconvex(1, n, 2, 1000,  step, env, Fn)
+x=[0.2,0.5,0.4,0.1]
+print(Mob,len)
+ChoquetCoMobKInter=fm.ChoquetCoMobKInter(x, Mob, 2, len, env)
+print(ChoquetCoMobKInter)
+
+fm.fm_free(env)
+
+
+
+#fm.FuzzyMeasureFit2Additive(num, n, options, indexlow, indexhigh, option1, orness, data)
+#env=fm.fm_init(3)
+num=20
+n=3
+d = np.array([0.00125122, 0.563568, 0.193298, 0.164338,
+            0.808716, 0.584991, 0.479858, 0.544309,
+            0.350281, 0.895935, 0.822815, 0.625868,
+            0.746582, 0.174103, 0.858917, 0.480347,
+            0.71048, 0.513519, 0.303986, 0.387631,
+            0.0149841, 0.0914001, 0.364441, 0.134229,
+            0.147308, 0.165894, 0.988495, 0.388044,
+            0.445679, 0.11908, 0.00466919, 0.0897714,
+            0.00891113, 0.377869, 0.531647, 0.258585,
+            0.571167, 0.601746, 0.607147, 0.589803,
+            0.166229, 0.663025, 0.450775, 0.357412,
+            0.352112, 0.0570374, 0.607666, 0.270228,
+            0.783295, 0.802582, 0.519867, 0.583348,
+            0.301941, 0.875946, 0.726654, 0.562174,
+            0.955872, 0.92569, 0.539337, 0.633631,
+            0.142334, 0.462067, 0.235321, 0.228419,
+            0.862213, 0.209595, 0.779633, 0.498077,
+            0.843628, 0.996765, 0.999664, 0.930197,
+            0.611481, 0.92426, 0.266205, 0.334666,
+            0.297272, 0.840118, 0.0237427, 0.168081]).reshape(num, 4)
+indexlow=[0.1,0.1,0.2]
+indexhigh=[0.9,0.9,0.5]
+options=3
+option1=1
+orness=[0.1,0.7]
+v = fm.FuzzyMeasureFit2Additive(num, 3, options, indexlow, indexhigh, option1, orness, d)
+print(v)
+
+fm.fm_free(env)
```

