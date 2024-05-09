# Comparing `tmp/apex_flow-1.2.0.tar.gz` & `tmp/apex_flow-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apex_flow-1.2.0.tar", last modified: Mon May  6 09:43:56 2024, max compression
+gzip compressed data, was "apex_flow-1.2.1.tar", last modified: Thu May  9 04:21:31 2024, max compression
```

## Comparing `apex_flow-1.2.0.tar` & `apex_flow-1.2.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064822 apex_flow-1.2.0/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.0/LICENSE
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-06 09:43:56.064569 apex_flow-1.2.0/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-06 09:26:48.000000 apex_flow-1.2.0/README.md
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.045407 apex_flow-1.2.0/apex/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-04-30 08:46:56.000000 apex_flow-1.2.0/apex/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/__main__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.0/apex/archive.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10465 2024-04-24 07:51:37.000000 apex_flow-1.2.0/apex/config.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.047498 apex_flow-1.2.0/apex/core/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/__init__.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.049057 apex_flow-1.2.0/apex/core/calculator/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-04-11 09:05:32.000000 apex_flow-1.2.0/apex/core/calculator/ABACUS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/Lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/Task.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.0/apex/core/calculator/VASP.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/calculator.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.050340 apex_flow-1.2.0/apex/core/calculator/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/calculator/lib/abacus_scf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.0/apex/core/calculator/lib/abacus_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/core/calculator/lib/lammps_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/calculator/lib/vasp_utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7850 2024-04-11 09:57:42.000000 apex_flow-1.2.0/apex/core/common_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/common_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/gen_confs.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.053355 apex_flow-1.2.0/apex/core/lib/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/crys.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/dispatcher.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/lmp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/mfp_eosfit.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/pwscf.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/siesta.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/slab_orientation.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/trans_tools.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/lib/util.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/lib/utils.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/mpdb.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.056024 apex_flow-1.2.0/apex/core/property/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10390 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/EOS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    11811 2024-04-24 15:53:23.000000 apex_flow-1.2.0/apex/core/property/Elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    27104 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    24024 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    26343 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/property/Property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10716 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9520 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/property/Vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/property/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/core/reproduce.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/core/structure.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.056948 apex_flow-1.2.0/apex/database/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/DatabaseFactory.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/DynamoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/MongoDB.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/StorageBase.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/database/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-04-24 08:51:43.000000 apex_flow-1.2.0/apex/flow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.0/apex/main.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.057641 apex_flow-1.2.0/apex/op/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/op/RunLAMMPS.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/op/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/op/property_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/op/relaxation_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2622 2024-04-26 16:57:00.000000 apex_flow-1.2.0/apex/report.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.058784 apex_flow-1.2.0/apex/reporter/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13848 2024-04-26 16:49:10.000000 apex_flow-1.2.0/apex/reporter/DashReportApp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/reporter/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/reporter/property_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/reporter/relaxation_report.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.0/apex/step.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-04-28 05:07:13.000000 apex_flow-1.2.0/apex/submit.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.059403 apex_flow-1.2.0/apex/superop/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/RelaxationFlow.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/SimplePropertySteps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/apex/superop/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.0/apex/utils.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064218 apex_flow-1.2.0/apex_flow.egg-info/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/PKG-INFO
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/entry_points.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/requires.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-06 09:43:56.000000 apex_flow-1.2.0/apex_flow.egg-info/top_level.txt
--rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-06 09:43:56.064881 apex_flow-1.2.0/setup.cfg
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-03-21 06:51:12.000000 apex_flow-1.2.0/setup.py
-drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-06 09:43:56.064019 apex_flow-1.2.0/tests/
--rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/__init__.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/context.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_abacus_property.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_elastic.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_eos.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_gamma.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_interstitial.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_lammps.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_make_prop.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_mpdb.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_ops.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_phonon.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_refine.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_surface.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vacancy.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_equi.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_equi_std.py
--rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.0/tests/test_vasp_kspacing.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.970988 apex_flow-1.2.1/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7650 2024-03-02 05:00:30.000000 apex_flow-1.2.1/LICENSE
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-09 04:21:31.970086 apex_flow-1.2.1/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    42506 2024-05-09 04:19:27.000000 apex_flow-1.2.1/README.md
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.914918 apex_flow-1.2.1/apex/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3737 2024-05-09 04:20:18.000000 apex_flow-1.2.1/apex/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       88 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/__main__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10185 2024-04-17 09:34:08.000000 apex_flow-1.2.1/apex/archive.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10465 2024-04-24 07:51:37.000000 apex_flow-1.2.1/apex/config.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.920537 apex_flow-1.2.1/apex/core/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/__init__.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.932403 apex_flow-1.2.1/apex/core/calculator/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9940 2024-04-11 09:05:32.000000 apex_flow-1.2.1/apex/core/calculator/ABACUS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    21684 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/Lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3058 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/Task.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10665 2024-04-16 13:06:19.000000 apex_flow-1.2.1/apex/core/calculator/VASP.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      147 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      845 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/calculator.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.946681 apex_flow-1.2.1/apex/core/calculator/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    17254 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/calculator/lib/abacus_scf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14014 2024-04-17 13:27:07.000000 apex_flow-1.2.1/apex/core/calculator/lib/abacus_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    20281 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/core/calculator/lib/lammps_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    14831 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/calculator/lib/vasp_utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-05-08 08:06:39.000000 apex_flow-1.2.1/apex/core/common_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8282 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/common_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4024 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/gen_confs.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.953144 apex_flow-1.2.1/apex/core/lib/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2059 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/crys.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1699 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/dispatcher.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5325 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/lmp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    46593 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/mfp_eosfit.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4428 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/pwscf.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4322 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/siesta.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8248 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/slab_orientation.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1871 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/trans_tools.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3904 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/lib/util.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2344 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/lib/utils.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/mpdb.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.957188 apex_flow-1.2.1/apex/core/property/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10390 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/EOS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    11811 2024-04-24 15:53:23.000000 apex_flow-1.2.1/apex/core/property/Elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    27104 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24024 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    26343 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3861 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/property/Property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10716 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9520 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/property/Vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/property/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2250 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6184 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/core/reproduce.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2695 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/core/structure.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.958840 apex_flow-1.2.1/apex/database/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      417 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/DatabaseFactory.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3366 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/DynamoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2080 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/MongoDB.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      533 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/StorageBase.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/database/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13130 2024-04-24 08:51:43.000000 apex_flow-1.2.1/apex/flow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    24813 2024-04-24 07:51:37.000000 apex_flow-1.2.1/apex/main.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.959615 apex_flow-1.2.1/apex/op/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1311 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/op/RunLAMMPS.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/op/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7535 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/op/property_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     5216 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/op/relaxation_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2622 2024-04-26 16:57:00.000000 apex_flow-1.2.1/apex/report.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.961653 apex_flow-1.2.1/apex/reporter/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13972 2024-05-09 04:16:06.000000 apex_flow-1.2.1/apex/reporter/DashReportApp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/reporter/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    18716 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/reporter/property_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2909 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/reporter/relaxation_report.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2824 2024-04-11 02:59:58.000000 apex_flow-1.2.1/apex/step.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10455 2024-05-09 04:19:27.000000 apex_flow-1.2.1/apex/submit.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.962479 apex_flow-1.2.1/apex/superop/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     7985 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/RelaxationFlow.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     8409 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/SimplePropertySteps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/apex/superop/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    10133 2024-04-27 08:56:06.000000 apex_flow-1.2.1/apex/utils.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.969684 apex_flow-1.2.1/apex_flow.egg-info/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    43373 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2401 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        1 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       44 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/entry_points.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      182 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/requires.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       11 2024-05-09 04:21:31.000000 apex_flow-1.2.1/apex_flow.egg-info/top_level.txt
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)       38 2024-05-09 04:21:31.971043 apex_flow-1.2.1/setup.cfg
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1145 2024-05-09 04:20:18.000000 apex_flow-1.2.1/setup.py
+drwxr-xr-x   0 zhuoyuan   (501) staff       (20)        0 2024-05-09 04:21:31.969367 apex_flow-1.2.1/tests/
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)        0 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/__init__.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1735 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/context.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     9820 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3720 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)    13373 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_abacus_property.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3131 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_elastic.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3776 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_eos.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4300 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_gamma.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     4017 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_interstitial.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3769 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_lammps.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3488 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_make_prop.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     1251 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_mpdb.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6121 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_ops.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2902 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_phonon.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3584 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_refine.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3863 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_surface.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3430 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vacancy.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     6164 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     3142 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_equi.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)     2503 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_equi_std.py
+-rw-r--r--   0 zhuoyuan   (501) staff       (20)      806 2024-03-02 05:00:30.000000 apex_flow-1.2.1/tests/test_vasp_kspacing.py
```

### Comparing `apex_flow-1.2.0/LICENSE` & `apex_flow-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/PKG-INFO` & `apex_flow-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.0/README.md` & `apex_flow-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/__init__.py` & `apex_flow-1.2.1/apex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 LOCAL_PATH = os.getcwd()
 
 
 def header():
     header_str = ""
     header_str += "---------------------------------------------------------------\n"
     header_str += "░░░░░░█▐▓▓░████▄▄▄█▀▄▓▓▓▌█░░░░░░░░░░█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█░░░░░\n"
```

### Comparing `apex_flow-1.2.0/apex/archive.py` & `apex_flow-1.2.1/apex/archive.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/config.py` & `apex_flow-1.2.1/apex/config.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/ABACUS.py` & `apex_flow-1.2.1/apex/core/calculator/ABACUS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/Lammps.py` & `apex_flow-1.2.1/apex/core/calculator/Lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/Task.py` & `apex_flow-1.2.1/apex/core/calculator/Task.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/VASP.py` & `apex_flow-1.2.1/apex/core/calculator/VASP.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/calculator.py` & `apex_flow-1.2.1/apex/core/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/lib/abacus_scf.py` & `apex_flow-1.2.1/apex/core/calculator/lib/abacus_scf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/lib/abacus_utils.py` & `apex_flow-1.2.1/apex/core/calculator/lib/abacus_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/lib/lammps_utils.py` & `apex_flow-1.2.1/apex/core/calculator/lib/lammps_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/calculator/lib/vasp_utils.py` & `apex_flow-1.2.1/apex/core/calculator/lib/vasp_utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/common_equi.py` & `apex_flow-1.2.1/apex/core/common_equi.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,19 @@
     # generate a list of task names like mp-xxx/relaxation
     # dump the relaxation result.
     for ii in task_dirs:
         poscar = os.path.join(ii, "POSCAR")
         inter = make_calculator(inter_param, poscar)
         res = inter.compute(ii)
         contcar = os.path.join(ii, "CONTCAR")
-        ss = Structure.from_file(contcar)
+        try:
+            ss = Structure.from_file(contcar)
+        except FileNotFoundError:
+            logging.warning(f"No CONTCAR found in {ii}, skip")
+            continue
         st = StructureInfo(ss)
         struct_info_dict = {
             "space_group_symbol": st.space_group_symbol,
             "space_group_number": st.space_group_number,
             "point_group_symbol": st.point_group_symbol,
             "crystal_system": st.crystal_system,
             "lattice_type": st.lattice_type,
```

### Comparing `apex_flow-1.2.0/apex/core/common_prop.py` & `apex_flow-1.2.1/apex/core/common_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/gen_confs.py` & `apex_flow-1.2.1/apex/core/gen_confs.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/crys.py` & `apex_flow-1.2.1/apex/core/lib/crys.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/dispatcher.py` & `apex_flow-1.2.1/apex/core/lib/dispatcher.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/lmp.py` & `apex_flow-1.2.1/apex/core/lib/lmp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/mfp_eosfit.py` & `apex_flow-1.2.1/apex/core/lib/mfp_eosfit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/pwscf.py` & `apex_flow-1.2.1/apex/core/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/siesta.py` & `apex_flow-1.2.1/apex/core/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/slab_orientation.py` & `apex_flow-1.2.1/apex/core/lib/slab_orientation.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/trans_tools.py` & `apex_flow-1.2.1/apex/core/lib/trans_tools.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/util.py` & `apex_flow-1.2.1/apex/core/lib/util.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/lib/utils.py` & `apex_flow-1.2.1/apex/core/lib/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/mpdb.py` & `apex_flow-1.2.1/apex/core/mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/EOS.py` & `apex_flow-1.2.1/apex/core/property/EOS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Elastic.py` & `apex_flow-1.2.1/apex/core/property/Elastic.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Gamma.py` & `apex_flow-1.2.1/apex/core/property/Gamma.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Interstitial.py` & `apex_flow-1.2.1/apex/core/property/Interstitial.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Phonon.py` & `apex_flow-1.2.1/apex/core/property/Phonon.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Property.py` & `apex_flow-1.2.1/apex/core/property/Property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Surface.py` & `apex_flow-1.2.1/apex/core/property/Surface.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/property/Vacancy.py` & `apex_flow-1.2.1/apex/core/property/Vacancy.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/refine.py` & `apex_flow-1.2.1/apex/core/refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/reproduce.py` & `apex_flow-1.2.1/apex/core/reproduce.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/core/structure.py` & `apex_flow-1.2.1/apex/core/structure.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/database/DynamoDB.py` & `apex_flow-1.2.1/apex/database/DynamoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/database/MongoDB.py` & `apex_flow-1.2.1/apex/database/MongoDB.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/database/StorageBase.py` & `apex_flow-1.2.1/apex/database/StorageBase.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/flow.py` & `apex_flow-1.2.1/apex/flow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/main.py` & `apex_flow-1.2.1/apex/main.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/op/RunLAMMPS.py` & `apex_flow-1.2.1/apex/op/RunLAMMPS.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/op/property_ops.py` & `apex_flow-1.2.1/apex/op/property_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/op/relaxation_ops.py` & `apex_flow-1.2.1/apex/op/relaxation_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/report.py` & `apex_flow-1.2.1/apex/report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/reporter/DashReportApp.py` & `apex_flow-1.2.1/apex/reporter/DashReportApp.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,22 +136,25 @@
                 if d:
                     default_dimension = d_key
                     default_dataset = next(iter(d.keys()))
                     break
             if default_dataset:
                 break
 
+        radio_inline = False
+        if len(self.all_dimensions) > 10:
+            radio_inline = True
         layout = html.Div(
             [
                 html.H1("APEX Results Visualization Report", style={'textAlign': 'center'}),
                 html.Label('Configuration:', style={'font-weight': 'bold', "fontSize": UI_FRONTSIZE}),
                 dcc.RadioItems(
                     id='confs-radio',
                     options=[{'label': name, 'value': name} for name in self.all_dimensions],
-                    value=default_dimension,
+                    value=default_dimension, inline=radio_inline,
                     style={"fontSize": UI_FRONTSIZE}
                 ),
                 html.Br(),
                 html.Label('Property:', style={'font-weight': 'bold', "fontSize": UI_FRONTSIZE}),
                 dcc.Dropdown(
                     id='props-dropdown',
                     options=[{'label': name, 'value': name} for name in self.all_datasets],
```

### Comparing `apex_flow-1.2.0/apex/reporter/property_report.py` & `apex_flow-1.2.1/apex/reporter/property_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/reporter/relaxation_report.py` & `apex_flow-1.2.1/apex/reporter/relaxation_report.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/step.py` & `apex_flow-1.2.1/apex/step.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/submit.py` & `apex_flow-1.2.1/apex/submit.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/superop/RelaxationFlow.py` & `apex_flow-1.2.1/apex/superop/RelaxationFlow.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/superop/SimplePropertySteps.py` & `apex_flow-1.2.1/apex/superop/SimplePropertySteps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex/utils.py` & `apex_flow-1.2.1/apex/utils.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/apex_flow.egg-info/PKG-INFO` & `apex_flow-1.2.1/apex_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apex-flow
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alloy Properties EXplorer using simulations
 Home-page: https://github.com/deepmodeling/APEX.git
 Author: Zhuoyuan Li, Tongqi Wen
 Author-email: zhuoyli@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `apex_flow-1.2.0/apex_flow.egg-info/SOURCES.txt` & `apex_flow-1.2.1/apex_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/setup.py` & `apex_flow-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apex-flow",
-    version="1.2.0",
+    version="1.2.1",
     author="Zhuoyuan Li, Tongqi Wen",
     author_email="zhuoyli@outlook.com",
     description="Alloy Properties EXplorer using simulations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/APEX.git",
     packages=setuptools.find_packages(),
```

### Comparing `apex_flow-1.2.0/tests/context.py` & `apex_flow-1.2.1/tests/context.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_abacus.py` & `apex_flow-1.2.1/tests/test_abacus.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_abacus_equi.py` & `apex_flow-1.2.1/tests/test_abacus_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_abacus_property.py` & `apex_flow-1.2.1/tests/test_abacus_property.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_elastic.py` & `apex_flow-1.2.1/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_eos.py` & `apex_flow-1.2.1/tests/test_eos.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_gamma.py` & `apex_flow-1.2.1/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_interstitial.py` & `apex_flow-1.2.1/tests/test_interstitial.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_lammps.py` & `apex_flow-1.2.1/tests/test_lammps.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_make_prop.py` & `apex_flow-1.2.1/tests/test_make_prop.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_mpdb.py` & `apex_flow-1.2.1/tests/test_mpdb.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_ops.py` & `apex_flow-1.2.1/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_phonon.py` & `apex_flow-1.2.1/tests/test_phonon.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_refine.py` & `apex_flow-1.2.1/tests/test_refine.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_surface.py` & `apex_flow-1.2.1/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_vacancy.py` & `apex_flow-1.2.1/tests/test_vacancy.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_vasp.py` & `apex_flow-1.2.1/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_vasp_equi.py` & `apex_flow-1.2.1/tests/test_vasp_equi.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_vasp_equi_std.py` & `apex_flow-1.2.1/tests/test_vasp_equi_std.py`

 * *Files identical despite different names*

### Comparing `apex_flow-1.2.0/tests/test_vasp_kspacing.py` & `apex_flow-1.2.1/tests/test_vasp_kspacing.py`

 * *Files identical despite different names*

