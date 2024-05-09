# Comparing `tmp/sage_lib-0.1.4.9.tar.gz` & `tmp/sage_lib-0.1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sage_lib-0.1.4.9.tar", last modified: Thu Feb 29 10:29:26 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.0.tar", last modified: Thu May  9 09:43:00 2024, max compression
```

## Comparing `sage_lib-0.1.4.9.tar` & `sage_lib-0.1.5.0.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.4.9/README.md
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)       45 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/entry_points.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)       23 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/requires.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        9 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/top_level.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      184 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/PKG-INFO
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        1 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/dependency_links.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3566 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 akaris    (1000) akaris    (1000)       38 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/setup.cfg
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      394 2024-02-29 10:29:01.000000 sage_lib-0.1.4.9/setup.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)      184 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/PKG-INFO
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/descriptor/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/descriptor/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.4.9/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.4.9/sage_lib/descriptor/MDTR_rev.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.4.9/sage_lib/IO/EigenvalueFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.4.9/sage_lib/IO/KPointsManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    16921 2024-01-17 11:53:21.000000 sage_lib-0.1.4.9/sage_lib/IO/OutFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.4.9/sage_lib/IO/DOSManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.4.9/sage_lib/IO/PotentialManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputDFT.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputClassic.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFile.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.4.9/sage_lib/IO/BinaryDataHandler.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.4.9/sage_lib/IO/PROFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.4.9/sage_lib/IO/WaveFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.4.9/sage_lib/IO/BashScriptManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    31331 2024-01-31 13:09:07.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    39615 2024-02-28 10:38:59.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    21127 2024-02-27 16:53:39.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPosition.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4854 2024-01-17 15:22:16.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8624 2024-02-08 11:15:50.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10566 2024-02-27 17:11:40.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/plot.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.4.9/sage_lib/IO/ForceFieldManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.4.9/sage_lib/IO/ChargeFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.4.9/sage_lib/__init__.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/single_run/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/single_run/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRun.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.4.9/sage_lib/single_run/FF_Gap.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14547 2024-01-17 14:56:21.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRunDFT.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRunManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/ensemble/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/ensemble/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.4.9/sage_lib/ensemble/FFEnsembleManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.4.9/sage_lib/ensemble/DFTEnsemble.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/master/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.4.9/sage_lib/master/FileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/master/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    53348 2024-01-26 15:57:17.000000 sage_lib-0.1.4.9/sage_lib/master/AtomicProperties.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    56357 2024-02-28 10:38:17.000000 sage_lib-0.1.4.9/sage_lib/main.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/periodic_kdtree.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/BandPathGenerator.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/partition/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/partition/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14976 2024-02-27 15:30:04.000000 sage_lib-0.1.4.9/sage_lib/partition/Partition.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    22631 2024-02-28 09:20:51.000000 sage_lib-0.1.4.9/sage_lib/partition/PartitionManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12099 2024-01-31 09:40:59.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Crystal_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Filter_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6705 2023-12-26 16:23:08.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Config_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    35959 2024-02-28 10:59:55.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2873 2024-01-30 12:38:27.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Molecule_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Dataset_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910612 sage_lib-0.1.5.0/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-09 09:43:00.910410 sage_lib-0.1.5.0/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.0/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.889206 sage_lib-0.1.5.0/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.892930 sage_lib-0.1.5.0/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.0/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.0/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.0/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.0/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.0/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.0/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.0/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    15441 2024-05-09 06:44:19.000000 sage_lib-0.1.5.0/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.0/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.0/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.0/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.894307 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.896957 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    21571 2024-04-29 15:23:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.899271 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4892 2024-04-29 15:21:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.0/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.900907 sage_lib-0.1.5.0/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.0/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.0/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.901687 sage_lib-0.1.5.0/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.0/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.0/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60962 2024-05-02 06:53:44.000000 sage_lib-0.1.5.0/sage_lib/main.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.902971 sage_lib-0.1.5.0/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56677 2024-04-03 13:00:04.000000 sage_lib-0.1.5.0/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.5.0/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.903800 sage_lib-0.1.5.0/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.904559 sage_lib-0.1.5.0/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.0/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    25994 2024-04-29 15:00:22.000000 sage_lib-0.1.5.0/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.908903 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910049 sage_lib-0.1.5.0/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.0/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910193 sage_lib-0.1.5.0/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3657 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-09 09:43:00.910658 sage_lib-0.1.5.0/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-09 09:42:07.000000 sage_lib-0.1.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sage_lib-0.1.4.9/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.0/sage_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,23 @@
 sage_lib/ensemble/DFTEnsemble.py
 sage_lib/ensemble/FFEnsembleManager.py
 sage_lib/ensemble/__init__.py
 sage_lib/master/AtomicProperties.py
 sage_lib/master/FileManager.py
 sage_lib/master/__init__.py
 sage_lib/miscellaneous/BandPathGenerator.py
+sage_lib/miscellaneous/MD_tools.py
 sage_lib/miscellaneous/__init__.py
 sage_lib/miscellaneous/periodic_kdtree.py
 sage_lib/partition/Partition.py
 sage_lib/partition/PartitionManager.py
 sage_lib/partition/__init__.py
 sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
 sage_lib/partition/partition_builder/BandStructure_builder.py
+sage_lib/partition/partition_builder/Blender_builder.py
 sage_lib/partition/partition_builder/Config_builder.py
 sage_lib/partition/partition_builder/CrystalDefect_builder.py
 sage_lib/partition/partition_builder/Crystal_builder.py
 sage_lib/partition/partition_builder/Dataset_builder.py
 sage_lib/partition/partition_builder/Filter_builder.py
 sage_lib/partition/partition_builder/MolecularDynamic_builder.py
 sage_lib/partition/partition_builder/MoleculeCluster_builder.py
```

### Comparing `sage_lib-0.1.4.9/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.0/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.0/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/OutFileManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             if i > 0 and not self.is_number(t): 
                 break
             processed.append(token_value)
 
         # Join the processed tokens into a string if there are multiple, otherwise return the single token
         return ' '.join(processed) if len(processed) > 1 else processed[0]
 
-    def readOUTCAR(self, file_location: str = None):
+    def readOUTCAR(self, file_location: str = None, **kwargs):
         """
         Parses the OUTCAR file from a VASP simulation to extract various parameters and atom positions.
 
         This method processes the OUTCAR file line by line, extracting parameters like Fermi energy, 
         dispersion energy, lattice vectors, charges, magnetizations, total forces, and atom positions. 
         The information is stored in an AtomPosition object.
 
@@ -319,46 +319,7 @@
             
         # The following block seems incomplete and might need additional implementation
         elif 'total charge' in line and not 'charge-density' in line: 
             TC = self.NIONS+4
             total_charge = np.zeros((self.NIONS,4))
             TC_counter = 0 
 
-    def export_configXYZ(self, file_location:str=None, save_to_file:str='w', verbose:bool=False):
-        """
-        Exports configuration in XYZ format.
-
-        This method goes through the AtomPositionManager and exports the atomic configurations
-        in XYZ format. The output can be directed to a specified file.
-
-        Parameters:
-        file_location (str, optional): The path to save the XYZ file. 
-                                       Defaults to self.file_location+'_config.xyz'.
-        save_to_file (str): The file mode for opening the file. Default is 'w' (write).
-        verbose (bool): If True, prints out a message upon successful saving.
-        """
-        file_location  = file_location if file_location else self.file_location+'_config.xyz'
-
-        with open(file_location, save_to_file) as f:
-            for APM in self.AtomPositionManager:
-                # Write each AtomPosition's data to the file in XYZ format
-                f.write( APM.export_as_xyz(file_location, save_to_file=False, verbose=False) )
-
-        if verbose:
-            print(f"XYZ content has been saved to {file_location}")
-
-'''
-print(123)
-
-o = OutFileManager('/home/akaris/Documents/code/Physics/VASP/v6.1/files/OUTCAR/OUTCAR')
-o.readOUTCAR()
-o.export_configXYZ(filter_by_forces=True)
-
-#print( o.InputFileManager.exportAsINCAR() )
-
-
-print(o.AtomPositionManager)
-#print( [ APM.E for APM in o._AtomPositionManager ])
-for n in o.AtomPositionManager:
-    print(n.total_force[0])
-
-'''
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.0/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,16 +307,14 @@
         return np.dot(self.get_fractional_coordinates(r), self.latticeVectors)
 
     def get_fractional_coordinates(self, r):
         return np.dot(r, self.latticeVectors_inv) % 1.0
 
     def get_pbc(self): return self.pbc
 
-    def get_atomic_numbers(self): return np.array([self.atomic_numbers[label] for label in self.atomLabelsList])
-
     def get_cell(self): return np.array(self.latticeVectors)
 
     def get_positions(self): return np.array(self.atomPositions)
 
     def get_normal_vector_to_lattice_plane(self, ):
         """
         Calculate the normal vectors to the lattice planes.
@@ -389,15 +387,15 @@
         self.pack_to_unit_cell()
         
     def pack_to_unit_cell(self, ):
         # Apply minimum image convention
         self._atomPositions_fractional = self.atomPositions_fractional%1.0
         
         # Convert back to Cartesian coordinates
-        self._atomPositions = np.dot(self.atomPositions_fractional, self.latticeVectors)
+        self._atomPositions = None # np.dot(self.atomPositions_fractional, self.latticeVectors)
 
     def minimum_image_interpolation(self, r1, r2, n:int=2, n_max=1):
         """
 
         """
         
         # Generar todas las combinaciones de índices de celda
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files 17% similar despite different names*

```diff
@@ -85,47 +85,53 @@
             edit_positions (bool): If True, atom positions will be reset; otherwise, they will be retained.
 
         This method updates the lattice vectors and invalidates any cached inverse lattice vectors and distance matrices.
         """
         self._latticeVectors = new_latticeVectors
         self._latticeVectors_inv = None
 
+        self.atomPositions, self.atomPositions_fractional
+        self._atomPositions_fractional = None if not edit_positions else self._atomPositions_fractional
         self._atomPositions = None if edit_positions else self._atomPositions
+
         self._distance_matrix = None if edit_positions else self._distance_matrix
         self._kdtree = None if edit_positions else self._kdtree
 
-        self._atomPositions_fractional = None if not edit_positions else self._atomPositions_fractional
  
     def remove_atom(self, atom_index:np.array):
         """
         Removes one or more atoms from the molecule.
 
         Args:
             atom_index (np.array): An array of indices of atoms to remove.
 
         This method updates various properties of the molecule, including atomic constraints, positions, labels, charges, magnetization, and forces. It also adjusts the count of atoms and recalculates any necessary properties.
         """
-        atom_index = np.array(atom_index, dtype=np.int64)
+        if isinstance(atom_index, int):
+            atom_index = np.array([atom_index], dtype=np.int64)
+        else:
+            atom_index = np.array(atom_index, dtype=np.int64)
+    
         """Remove an atom at the given index."""
         self._atomicConstraints = np.delete(self.atomicConstraints, atom_index, axis=0)
         self._atomPositions = np.delete(self.atomPositions, atom_index, axis=0)
-        self._atomPositions_fractional = np.delete(self.atomPositions_fractional, atom_index, axis=0)
+        self._atomPositions_fractional = None
         self._atomLabelsList = np.delete(self.atomLabelsList, atom_index)
         self._total_charge = np.delete(self.total_charge, atom_index,  axis=0) if self._total_charge is not None else self._total_charge
         self._magnetization = np.delete(self.magnetization, atom_index,  axis=0) if self._magnetization is not None else self._magnetization
         self._total_force = np.delete(self.total_force, atom_index,  axis=0) if self._total_force is not None else self._total_force
-        
-        self._atomCount -= atom_index.shape[0]
+
+        self._atomCount = None
         self._atomCountByType = None
         self._fullAtomLabelString = None
         self._uniqueAtomLabels = None
 
         if self._distance_matrix is not None:
-            self._distance_matrix = np.delete(self._distance_matrix, var, axis=0)  # Eliminar fila
-            self._distance_matrix = np.delete(self._distance_matrix, var, axis=1)  # Eliminar columna
+            self._distance_matrix = np.delete(self._distance_matrix, atom_index, axis=0)  # Eliminar fila
+            self._distance_matrix = np.delete(self._distance_matrix, atom_index, axis=1)  # Eliminar columna
         self._kdtree = None
 
     def add_atom(self, atomLabels: str, atomPosition: np.array, atomicConstraints: np.array = None) -> bool:
         """
         Adds an atom to the AtomContainer.
 
         :param atomLabels: Label for the new atom.
@@ -394,14 +400,17 @@
         for atom_index_i in range(self.atomCount):
             for atom_index_j in range(atom_index_i, self.atomCount):
                 distance_matrix[atom_index_i, atom_index_j] = self.minimum_image_distance(
                     self.atomPositions[atom_index_i], self.atomPositions[atom_index_j])
 
         return distance_matrix
 
+    def is_bond(self, n1:int, n2:int, sigma:float=1.2, periodic:bool=None) -> bool:
+        return self.distance( self.atomPositions[n1], self.atomPositions[n2], periodic=periodic) < (self.covalent_radii[self.atomLabelsList[n1]]+self.covalent_radii[self.atomLabelsList[n2]])*sigma
+
     # ====== KDTREE ======
     def count_neighbors(self, other, r, p=2.):
         """
         Count the number of neighbors each point in 'other' has within distance 'r'.
 
         Parameters:
         other: PeriodicCKDTree or cKDTree
@@ -546,14 +555,128 @@
                 grupo_actual = {atomo}
                 dfs(atomo, grupo_actual)
                 graph_representation.append(grupo_actual)
 
         self._graph_representation = graph_representation
         return self._graph_representation
 
+    def search_molecular_subgraph(self, sigma:float=1.2, id_filter:bool=True, pattern:dict=None, 
+                                  prevent_overlapping:bool=True, prevent_shared_nodes:bool=True,
+                                  prevent_repeating:bool=True, verbose:bool=False):
+        '''
+        Searches for subgraphs within a molecular graph that match a specified pattern.
+
+        Parameters:
+        - sigma (float): Multiplier for the bond length to define the search radius. Defaults to 1.2.
+        - id_filter (bool): Filters atoms by IDs in the pattern. Defaults to True.
+        - pattern (dict): Dictionary representing the search pattern.
+        - prevent_overlapping (bool): Prevents overlapping of search results. Defaults to True.
+        - prevent_shared_nodes (bool): Prevents shared nodes between different search results. Defaults to True.
+        - prevent_repeating (bool): Prevents repeating groups in the results. Defaults to True.
+        - verbose (bool): If True, prints additional information during the search. Defaults to False.
+        
+        Returns:
+        - List of groups (subgraphs) matching the search pattern.
+        '''
+
+        # Initialize necessary variables from the class attributes
+        atom_count = self.atomCount
+        atom_positions = self.atomPositions
+        atom_labels_list = self.atomLabelsList
+        covalent_radii = self.covalent_radii
+        unique_atom_labels = self.uniqueAtomLabels
+        distance_function = self.distance
+        find_all_neighbors_radius = self.find_all_neighbors_radius
+
+        # Arrays to keep track of visited atoms to prevent overlapping and shared node searches
+        visited_by_same_graph = np.zeros(atom_count, dtype=bool)
+        visited_by_other_graph = np.zeros(atom_count, dtype=bool)
+ 
+        # Initialize containers for the results
+        subgraphs = []
+        subgraphs_sorted = []
+        
+        # Calculate the maximum possible bond length based on the sigma and maximum covalent radius
+        r_max = max(covalent_radii[a] for a in unique_atom_labels)
+        
+        def depth_first_search(atom, current_group, position, id_mapping, reverse_id_mapping):
+            """Performs depth-first search to find matching subgraphs."""
+            # Determine the maximum bond length for the current atom
+            max_bond_length = (covalent_radii[atom_labels_list[atom]] + r_max) * sigma
+            # Find all neighbors within the calculated max bond length
+            for neighbor in find_all_neighbors_radius(atom_positions[atom], max_bond_length):
+                # Skip neighbor if overlapping or shared nodes are not allowed and the neighbor is already visited
+                if (prevent_overlapping and visited_by_same_graph[neighbor]) or \
+                   (prevent_shared_nodes and visited_by_other_graph[neighbor]):
+                    continue
+
+                # Check if the neighbor is within the actual bond length after applying the sigma multiplier
+                if distance_function(atom_positions[atom], atom_positions[neighbor]) < \
+                   (covalent_radii[atom_labels_list[atom]] + covalent_radii[atom_labels_list[neighbor]]) * sigma:
+                    # Process this neighbor as part of the current group
+                    process_neighbor(neighbor, position, id_mapping, reverse_id_mapping, current_group)
+
+        def process_neighbor(neighbor, position, id_mapping, reverse_id_mapping, current_group):
+            """Processes each neighboring atom according to search criteria."""
+            # If id_filter is True, only process neighbors that match the pattern
+            if id_filter and atom_labels_list[neighbor] == pattern[position][0]:
+                id_num = pattern[position][1]
+                # Ensure that the neighbor matches the pattern's ID requirements
+                if (id_mapping.get(id_num, -1) == -1 or id_mapping[id_num] == neighbor) and \
+                   (reverse_id_mapping.get(neighbor, -1) == -1 or reverse_id_mapping[neighbor] == id_num):
+                    # Update mappings to include this neighbor
+                    id_mapping[id_num] = neighbor
+                    reverse_id_mapping[neighbor] = id_num
+                    # Mark as visited
+                    visited_by_same_graph[neighbor] = True
+                    visited_by_other_graph[neighbor] = True
+                    # Add neighbor to the current group
+                    current_group.append(neighbor)
+                    # Continue the search if there are more positions in the pattern
+                    if position + 1 < len(pattern):
+                        depth_first_search(neighbor, current_group, position + 1, id_mapping, reverse_id_mapping)
+                    # If this is the last position, handle prevent_repeating logic
+                    elif prevent_repeating:
+                        # Sort and de-duplicate groups if needed
+                        current_group_sorted = sorted(current_group)
+                        if current_group_sorted not in subgraphs_sorted:
+                            subgraphs_sorted.append(current_group_sorted)
+                            subgraphs.append(current_group)
+                    else:
+                        subgraphs.append(current_group)
+            elif not id_filter:
+                # If id_filter is False, process all neighbors
+                visited_by_same_graph[neighbor] = True
+                visited_by_other_graph[neighbor] = True
+                current_group.append(neighbor)
+                # Continue search without ID filtering
+                depth_first_search(neighbor, current_group, position + 1, id_mapping, reverse_id_mapping)
+
+        # Main loop to start the search from each atom
+        for atom in range(atom_count):
+            # Only start a new search if the atom has not been visited or matches the pattern's first position
+            if (not prevent_shared_nodes or not visited_by_other_graph[atom]) and \
+                (not id_filter or (pattern and atom_labels_list[atom] == pattern[0][0])):
+                visited_by_same_graph.fill(False)  # Reset visited flags for a new search
+                visited_by_same_graph[atom] = True
+                visited_by_other_graph[atom] = True
+                current_group = [atom]
+                # Initialize mappings with the first atom of the pattern
+                depth_first_search(atom, current_group, 1, {pattern[0][1]: atom}, {atom: pattern[0][1]})
+
+        # Remove repeating subgraphs if required
+        if prevent_repeating:
+            subgraphs = [list(subgroup) for subgroup in set(tuple(sorted(subgroup)) for subgroup in subgraphs)]
+
+        # Optionally print the found groups for debugging
+        if verbose:
+            print("Found groups:", subgraphs)
+
+        return subgraphs
+
     def count_species(self, sigma:float=1.2):
         self.get_molecular_graph(sigma=sigma)
 
         count_dict = {}
         for n in self.graph_representation:
 
             label_list = sorted([self.atomLabelsList[l] for l in n ])
@@ -571,14 +694,29 @@
             if type(specie) == str:
                 return np.max( [self.covalent_radii[a] for a in self.uniqueAtomLabels] ) + self.covalent_radii[specie]
             else:
                 return np.max( [self.covalent_radii[a] for a in self.uniqueAtomLabels] ) * 2
 
         return None
 
+    def get_connection_list(self, sigma:float=1.2, metric:str='covalent_radii', periodic:bool=None ) -> list:
+        connection_list = []
+        max_bond_lenth = np.max( [self.covalent_radii[a] for a in self.uniqueAtomLabels] )
+        for A, position_A in enumerate(self.atomPositions):       #loop over different atoms
+            bonded = self.find_all_neighbors_radius(position_A, (max_bond_lenth+self.covalent_radii[self.atomLabelsList[A]])*sigma )
+
+            for B_index, B in enumerate(bonded):
+                AB_bond_distance = (self.covalent_radii[ self.atomLabelsList[A] ] + self.covalent_radii[ self.atomLabelsList[B] ] ) * sigma
+
+                if  B>A and (periodic or np.linalg.norm( (position_A-self.atomPositions[B]) ) < AB_bond_distance):
+                    connection_list.append([A, B])
+        
+        return connection_list
+        #[(n1, n2) for n1 in range(self.atomCount) for n2 in range(n1 + 1, self.atomCount) if self.is_bond(n1, n2, periodic=periodic)]
+
     # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # # =========== NEIGHBORS =========== # 
 
     # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # # =========== OPERATIONS =========== # 
     def get_plane(self, atom1, atom2, atom3):
         v1 = self.atomPositions[atom1, :] - self.atomPositions[atom2, :]
         v2 = self.atomPositions[atom2, :] - self.atomPositions[atom3, :]
         # | i        j     k   | #
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,17 @@
         self._E = None  # Total energy. Type: float or None
         self._Edisp = None  # Dispersion energy. Type: float or None
         self._IRdisplacement = None  # IR displacement. Type: np.array or None
 
         self._mass = None # 
         self._mass_list = None # 
 
+        self.info_system = {}
+        self.info_atoms = {}
+        
     @property
     def distance_matrix(self):
         """
         Calculates and returns the distance matrix between atoms.
 
         The distance matrix is calculated using Euclidean distances. It is computed only if not already available.
 
@@ -381,21 +384,32 @@
         (indicating no constraints). Otherwise, it returns the set constraints.
 
         Returns:
             np.array: Array of atomic constraints.
         """
         if self._atomicConstraints is list:
             return np.array(self._atomicConstraints)
-        elif self._atomPositions is not None:
-            self._atomicConstraints = np.ones_like(self._atomPositions) 
+        elif self._atomicConstraints is None:
+            self._atomicConstraints = np.ones_like(self.atomPositions) 
             return self._atomicConstraints
         else:
             return self._atomicConstraints
 
     @property
+    def selectiveDynamics(self):
+        """
+        """
+        if self._selectiveDynamics:
+            return True        
+        if not self._atomicConstraints is None:
+            return True
+        else:
+            return False
+
+    @property
     def mass_list(self):
         """
 
         """
         if self._mass_list is list:
             return np.array(self._mass_list)
         else:
@@ -442,14 +456,20 @@
         """
         if self._graph_representation is None:
             self._graph_representation = self.find_related_atoms_groups()
             return self._graph_representation
         else:
             return self._graph_representation
 
+    def get_atomic_numbers(self, ):
+        return self.atomLabelsList
+    
+    def get_cell(self, ):
+        return self.la
+
     def get_MBTR_representation(self, grid:int=500, get_dev:bool=True):
         md = MBTR.MDTR( lattice_vectors =   self.latticeVectors, 
                         atomLabelsList  =   self.atomLabelsList, 
                         atomPositions   =   self.atomPositions , )
 
         self._MBTR_representation, self._MBTR_representation_dev = md.get_mdtr()
         self._MBTR = md
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,23 @@
                 file.write('{:>18.15f}\t{:>18.15f}\t{:>18.15f}\n'.format(*lv))
 
             # Tipos de átomos y sus números
             file.write('    '.join(self.uniqueAtomLabels) + '\n')
             file.write('    '.join(map(str, self.atomCountByType)) + '\n')
 
             # Opción para dinámica selectiva (opcional)
-            if self._selectiveDynamics:     file.write('Selective dynamics\n')
+            if self.selectiveDynamics:     file.write('Selective dynamics\n')
             # Tipo de coordenadas (Direct o Cartesian)
             aCT = 'Cartesian' if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else 'Direct'
             file.write(f'{aCT}\n')
 
             # Coordenadas atómicas y sus restricciones
             for i, atom in enumerate(self.atomPositions if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else self.atomPositions_fractional):
                 coords = '\t'.join(['{:>18.15f}'.format(n) for n in atom])
-                constr = '\tT\tT\tT' if self.atomicConstraints is None else '\t'.join(['T' if n else 'F' for n in self.atomicConstraints[i]]) 
+                constr = '\t'.join(['T' if n else 'F' for n in self.atomicConstraints[i]]) if self.selectiveDynamics else ''
                 file.write(f'\t{coords}\t{constr}\n')
 
             # Comentario final (opcional)
             file.write('Comment_line\n')
 
     def read_POSCAR(self, file_location:str=None):
         file_location = file_location if type(file_location) == str else self.file_location
@@ -105,14 +105,14 @@
         # Ion positions
         self._atomCount = np.array(sum(self._atomCountByType))
         if self._atomCoordinateType == 'cartesian':
             self._atomPositions = np.array([list(map(float, line.strip().split()[:3])) for line in lines[7+offset:7+offset+self._atomCount]])
         else:
             self._atomPositions_fractional = np.array([list(map(float, line.strip().split()[:3])) for line in lines[7+offset:7+offset+self._atomCount]])
 
-        self._atomicConstraints = np.array([list(map(str, line.strip().split()[3:])) for line in lines[7+offset:7+offset+self._atomCount]])
+        self._atomicConstraints = (np.array([list(map(str, line.strip().split()[3:])) for line in lines[7+offset:7+offset+self._atomCount]]) == 'T').astype(int) if self.selectiveDynamics else None
         # Check for lattice velocities
         # Check for ion velocities
 
     def read_CONTCAR(self, file_location:str=None):
         self.read_POSCAR(file_location)
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files 13% similar despite different names*

```diff
@@ -153,23 +153,16 @@
         self.atomPositions = self.atomPositions - np.min( self.atomPositions, axis=0 ) 
         if verbose: print(f' >> Export as PDB >> {file_location}')
 
         pdb_str = ''
         for A, position_A in enumerate(self.atomPositions):     #loop over different atoms
             pdb_str += "ATOM  %5d %2s   MOL     1  %8.3f%8.3f%8.3f  1.00  0.00\n" % (int(A+1), self.atomLabelsList[A], position_A[0], position_A[1], position_A[2])
 
-        max_bond_lenth = np.max( [self.covalent_radii[a] for a in self.uniqueAtomLabels] )
-        for A, position_A in enumerate(self.atomPositions):       #loop over different atoms
-            bonded = self.find_all_neighbors_radius(position_A, (max_bond_lenth+self.covalent_radii[self.atomLabelsList[A]])*bond_factor )
-
-            for B_index, B in enumerate(bonded):
-                AB_bond_distance = (self.covalent_radii[ self.atomLabelsList[A] ] + self.covalent_radii[ self.atomLabelsList[B] ] ) * bond_factor
-                #if  B>A and self.distance(position_A, self.atomPositions[B]) < AB_bond_distance:
-                if  B>A and np.linalg.norm( (position_A-self.atomPositions[B]) ) < AB_bond_distance:
-                    pdb_str += f'CONECT{int(A+1):>5}{int(B+1):>5}\n'
+        for A, B in self.get_connection_list(periodic=False):
+            pdb_str += f'CONECT{int(A+1):>5}{int(B+1):>5}\n'
                    
         # Save the generated XYZ content to a file if file_location is specified and save_to_file is True
         if file_location and save_to_file:
             with open(file_location, save_to_file) as f:
                 f.write(pdb_str)
             if verbose:
                 print(f"XYZ content has been saved to {file_location}")
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     del sys
 
 class XYZ(FileManager):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         super().__init__(name=name, file_location=file_location)
 
     def export_as_xyz(self, file_location:str=None, save_to_file:str='w', verbose:bool=False,
-                            species:bool=True, position:bool=True, energy:bool=True, forces:bool=True, charge:bool=True, magnetization:bool=True, lattice:bool=True, pbc:bool=True, time:bool=True,
-                            position_tag:str='pos', forces_tag:str='forces', charge_tag:str='charge', magnetization_tag:str='magnetization', energy_tag:str='E',
+                            species:bool=True, position:bool=True, energy:bool=True, forces:bool=True, charge:bool=True, magnetization:bool=True, lattice:bool=True, pbc:bool=True, time:bool=True, fixed:bool=True,
+                            position_tag:str='pos', forces_tag:str='forces', charge_tag:str='charge', magnetization_tag:str='magnetization', energy_tag:str='energy', fixed_tag:str='fixed',
                             time_tag:str='time', pbc_tag:str='pbc') -> str:
         """
         Export atomistic information in the XYZ format.
 
         Parameters:
             file_location (str): The location where the XYZ file will be saved. Ignored if save_to_file is False.
             save_to_file (bool): Flag to control whether to save the XYZ content to a file.
@@ -37,40 +37,45 @@
 
         Returns:
             str: The generated XYZ content.
         """
         file_location  = file_location  if not file_location  is None else self.file_location+'config.xyz' if self.file_location is str else self.file_location
         self.group_elements_and_positions()
 
-        # Ensuring no property is included if its value is None
-        lattice = hasattr(self, 'latticeVectors') and self.latticeVectors is not None and lattice
-        species = hasattr(self, 'atomLabelsList' ) and self.atomLabelsList is not None and species 
-        position = hasattr(self, 'atomPositions') and self.atomPositions is not None and position
-        forces = hasattr(self, 'total_force') and self.total_force is not None and forces
-        charge = hasattr(self, 'charge') and self.charge is not None and charge
-        magnetization = hasattr(self, 'magnetization') and self.magnetization is not None and magnetization
-        energy = hasattr(self, 'E') and energy and self.E is not None and energy
-        pbc = hasattr(self, 'latticeVectors') and self.latticeVectors is not None and pbc
-        time = hasattr(self, 'time') and self.time is not None and time 
+        # Dynamically determine which properties to include based on their presence and non-None status
+        include_lattice = hasattr(self, 'latticeVectors') and self.latticeVectors is not None and lattice
+        include_species = hasattr(self, 'atomLabelsList' ) and self.atomLabelsList is not None and species 
+        include_position = hasattr(self, 'atomPositions') and self.atomPositions is not None and position
+        include_forces = hasattr(self, 'total_force') and self.total_force is not None and forces
+        include_charge = hasattr(self, 'charge') and self.charge is not None and charge
+        include_magnetization = hasattr(self, 'magnetization') and self.magnetization is not None and magnetization
+        include_energy = hasattr(self, 'E') and energy and self.E is not None and energy
+        include_pbc = hasattr(self, 'latticeVectors') and self.latticeVectors is not None and pbc
+        include_time = hasattr(self, 'time') and self.time is not None and time 
+        include_fixed = hasattr(self, 'selectiveDynamics') and self.selectiveDynamics and fixed 
 
         # Constructing the header information dynamically
         properties_list = [
-            f'Lattice="{ " ".join(map(str, self.latticeVectors.flatten())) }"' if lattice else '',
-            f'Properties={":".join(filter(None, [f"species:S:1" if species else "", f"{position_tag}:R:3" if position else "", f"{forces_tag}:R:3" if forces else "", f"{charge_tag}:R:{self.charge.shape[1]}" if charge else "", f"{magnetization_tag}:R:{self.magnetization.shape[1]}" if magnetization else ""]))}',
-            f'{energy_tag}={self.E}' if energy else '',
-            f'{pbc_tag}="T T T"' if pbc else '',
-            f'{time_tag}={self.time}' if time else ''
+            f'Lattice="{ " ".join(map(str, self.latticeVectors.flatten())) }"' if include_lattice else '', 
+            f'Properties={":".join(filter(None, [f"species:S:1" if include_species else "",                 f"{position_tag}:R:3" if include_position else "",                 f"{forces_tag}:R:3" if include_forces else "",                 f"{charge_tag}:R:1" if include_charge and hasattr(self.charge, "shape") and len(self.charge.shape) > 1 else "",                 f"{magnetization_tag}:R:1" if include_magnetization and hasattr(self.magnetization, "shape") and len(self.magnetization.shape) > 1 else "",                f"{fixed_tag}:I:3" if include_fixed else "",                 ]))}',
+            f'{energy_tag}={self.E}' if include_energy else '',
+            f'{pbc_tag}="T T T"' if include_pbc else '',
+            f'{time_tag}={self.time}' if include_time else ''
         ]
         properties_str = ' '.join(filter(None, properties_list))
 
         # Preparing atom data lines
         atom_lines = [
-            f"{self.atomLabelsList[i]} {' '.join(map('{:12.6f}'.format, self.atomPositions[i])) if position else ''} {' '.join(map('{:14.6f}'.format, self.total_force[i])) if forces else ''}  {' '.join(map('{:14.6f}'.format, self.charge[i])) if charge else ''} {' '.join(map('{:14.6f}'.format, self.magnetization[i])) if magnetization else ''}"
+            f"{self.atomLabelsList[i]} {' '.join(map('{:13.10f}'.format, self.atomPositions[i])) if include_position else ''} \
+            {' '.join(map('{:2d}'.format, np.array(self.atomicConstraints[i], dtype=np.int32) )) if include_fixed else ''} \
+            {' '.join(map('{:14.10f}'.format, self.charge[i] if np.ndim(self.charge) == 1 else [self.charge[i, -1]])) if include_charge else ''} \
+            {' '.join(map('{:14.10f}'.format, self.magnetization[i] if np.ndim(self.magnetization) == 1 else [self.magnetization[i, -1]])) if include_magnetization else ''} \
+            {' '.join(map('{:14.10f}'.format, self.total_force[i])) if include_forces else ''} "
             for i in range(self.atomCount)
-        ] if position or forces else []
+        ]
 
         # Combining header and atom data
         xyz_content = f"{self.atomCount}\n{properties_str}\n" + "\n".join(atom_lines)+ "\n"
 
         # Saving to file if required
         if file_location and save_to_file != 'none':
             with open(file_location, save_to_file) as f:
@@ -105,14 +110,17 @@
             'forces': 'forces',
             'position': 'pos',
             'species': 'species',
             'pbc': 'pbc',
             'time': 'time',
             'Lattice': 'Lattice',
             'Properties': 'Properties',
+            'charge': 'charge',
+            'magnetization': 'magnetization',          
+            'fixed': 'fixed', 
         }
         tags = {k: tags.get(k, v) for k, v in default_tags.items()} if tags else default_tags
 
         file_location = file_location if isinstance(file_location, str) else self.file_location
 
         # Regex pattern to match property keys and values
         pattern = r'(\w+)=("[^"]+"|\S+)'
@@ -126,14 +134,15 @@
 
         # Mapping property keys to object attributes
         property_to_attr = {
             tags['forces']: "_total_force",
             tags['mass']: "_mass",
             tags['position']: "_atomPositions",
             tags['species']: "_atomLabelsList",
+            tags['fixed']: "_atomicConstraints",
         }
 
         lines = lines or list(self.read_file(file_location, strip=False))
         read_header = False
 
         for i, line in enumerate(lines):
             if read_header:
@@ -148,16 +157,17 @@
                 num_atoms = int(line.strip())
                 if num_atoms > 0:
                     self._atomCount = num_atoms
                     read_header = True 
 
         return {
                 'position':self.atomPositions,
-                'atomCount':self._atomCount,
+                'atomCount':self.atomCount,
                 'species':self.atomLabelsList, 
+                'atomicConstraints':self.atomicConstraints, 
                 }
 
     def _process_key_value(self, key, value, tags, dtype_map, property_to_attr, body):
         """
         Processes each key-value pair found in the XYZ file.
 
         Parameters:
@@ -180,15 +190,25 @@
 
         elif key == tags['pbc']:
             self._pbc = ['T' in v for v in value.split()]
 
         elif key == tags['time']:
             self._time = float(value)
 
+        elif key == tags['fixed']:
+            self._atomicConstraints = np.array(value)
+
+        elif key == tags['charge']:
+            self._charge = float(value)
+
+        elif key == tags['magnetization']:
+            self._magnetization = float(value)
+
         else:
+            self.info_system[key] = value
             setattr(self, key, value)
 
     def _parse_properties(self, properties_str, body, dtype_map, property_to_attr):
         """
         Parses the 'Properties' string to extract and assign properties to their respective attributes.
 
         Parameters:
@@ -208,14 +228,15 @@
 
             # Transform column vector to row vector if necessary, else leave matrices as is
             property_value = property_value.T[0] if property_value.shape[1] == 1 else property_value
 
             # Assign property_value to the respective attribute based on p[0]
             attr_name = property_to_attr.get(p[0], p[0])  # Fallback to p[0] if not in property_to_attr
             setattr(self, attr_name, property_value)
+            self.info_atoms[attr_name] = property_value 
 
             count_col += int(p[2])
 
     def read_file(self, file_location, strip=True):
         """
         Reads the content of a file.
```

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.0/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/__init__.py` & `sage_lib-0.1.5.0/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.0/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.0/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.0/sage_lib/single_run/SingleRunDFT.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,31 +108,14 @@
         if self.vdw_kernel_Handler and kernel:
             self._export_file(self.vdw_kernel_Handler.export_VASP_VDW_Kernel, 'vdw_kernel.bindat', file_location + '/vdw_kernel.bindat')
         if self.WaveFileManager and WAVECAR:
             self._export_file(self.WaveFileManager.exportFile, 'WAVECAR', file_location + '/WAVECAR')
         if self.ChargeFileManager and CHGCAR:
             self._export_file(self.ChargeFileManager.exportFile, 'CHGCAR', file_location + '/CHGCAR')
 
-        '''
-        if self.AtomPositionManager is not None:    
-            self.AtomPositionManager.NonPeriodic_2_Periodic()
-            self.AtomPositionManager.export_as_POSCAR(file_location+'/POSCAR')
-        if self.PotentialManager:       self.PotentialManager.exportAsPOTCAR(file_location+'/POTCAR', self.AtomPositionManager.uniqueAtomLabels )
-        if self.InputFileManager:       self.InputFileManager.exportAsINCAR(file_location+'/INCAR', self.AtomPositionManager.uniqueAtomLabels)
-        if self.KPointsManager:         self.KPointsManager.exportAsKPOINTS(file_location+'/KPOINTS')
-
-        if self.BashScriptManager:      self.BashScriptManager.exportAsBash(file_location+'/RUNscript.sh')
-        if self.vdw_kernel_Handler and kernel:     
-                                        self.vdw_kernel_Handler.export_VASP_VDW_Kernel(file_location+'/vdw_kernel.bindat')
-        if self.WaveFileManager and WAVECAR:     
-                                        self.WaveFileManager.exportFile(file_location+'/WAVECAR')
-        if self.ChargeFileManager and CHGCAR:     
-                                        self.ChargeFileManager.exportFile(file_location+'/CHGCAR')
-        '''
-
     def recommend_vasp_parameters(self, num_cores, num_nodes, num_atoms:int=None, system_type:str="multi-core", network_type:str="fast"):
         """
         Recommends optimal VASP parameters based on the number of cores, nodes, and system type.
 
         Parameters:
             num_cores (int): Total number of compute cores available.
             num_nodes (int): Total number of nodes in the cluster.
```

### Comparing `sage_lib-0.1.4.9/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.0/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.0/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.0/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.0/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.0/sage_lib/master/AtomicProperties.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,25 +178,68 @@
             'W' : 1.62, 'Re': 1.51, 'Os': 1.44, 'Ir': 1.41, 'Pt': 1.36, 'Au': 1.36, 'Hg': 1.32, 'Tl': 1.45,
             'Pb': 1.46, 'Bi': 1.48, 'Th': 1.79, 'Pa': 1.63, 'U' : 1.56, 'Np': 1.55, 'Pu': 1.53, 'Am': 1.51,
             'Cm': 1.50, 'Bk': 1.50, 'Cf': 1.50, 'Es': 1.50, 'Fm': 1.50, 'Md': 1.50, 'No': 1.50, 'Lr': 1.50,
             'Rf': 1.50, 'Db': 1.50, 'Sg': 1.50, 'Bh': 1.50, 'Hs': 1.50, 'Mt': 1.50, 'Ds': 1.50, 'Rg': 1.50,
             'Cn': 1.50, 'Nh': 1.50, 'Fl': 1.50, 'Mc': 1.50, 'Lv': 1.50, 'Ts': 1.50, 'Og': 1.50
         }
 
-        self.vdw_radii = {
+        self._vdw_radii = {
             'H': 1.20, 'He': 1.40, 'Li': 1.82, 'Be': 1.53, 'B': 1.92, 'C': 1.70, 'N': 1.55, 'O': 1.52, 'F': 1.47, 'Ne': 1.54, 'Na': 2.27,
             'Mg': 1.73, 'Al': 1.84, 'Si': 2.10, 'P': 1.80, 'S': 1.80, 'Cl': 1.75, 'Ar': 1.88, 'K': 2.75, 'Ca': 2.31, 'Sc': 2.11, 'Ti': 2.00,
             'V': 1.92, 'Cr': 2.09, 'Mn': 2.09, 'Fe': 1.94, 'Co': 1.92, 'Ni': 1.63, 'Cu': 1.40, 'Zn': 1.39, 'Ga': 1.87, 'Ge': 2.11,
             'As': 1.85, 'Se': 1.90, 'Br': 1.85, 'Kr': 2.02, 'Rb': 3.03, 'Sr': 2.49, 'Y': 2.19, 'Zr': 2.11, 'Nb': 1.98, 'Mo': 2.27,
             'Tc': 2.20, 'Ru': 2.20, 'Rh': 2.18, 'Pd': 2.02, 'Ag': 1.72, 'Cd': 1.58, 'In': 1.93, 'Sn': 2.17, 'Sb': 2.06, 'Te': 2.06,
             'I': 1.98, 'Xe': 2.16, 'Cs': 3.43, 'Ba': 2.68, 'Lu': 1.75, 'Hf': 2.08, 'Ta': 2.11, 'W': 1.93, 'Re': 1.88, 'Os': 1.85,
             'Ir': 1.80, 'Pt': 1.75, 'Au': 1.66, 'Hg': 1.55, 'Tl': 1.96, 'Pb': 2.02, 'Bi': 2.07, 'Po': 1.97, 'At': 2.02, 'Rn': 2.20,
             'Fr': 3.48, 'Ra': 2.83, 'Ac': 2.60, 'Th': 2.60, 'U': 2.60, 'Np': 2.60, 'Pu': 2.60, 'X': 0.00  # Placeholder for unknown elements
         }
 
+        # Creating a dictionary for empirical atomic radii from the provided data
+        self._atomic_radii_empirical = {
+            'H': 0.25, 'He': 1.2, 'Li': 1.45, 'Be': 1.05, 'B': 0.85, 'C': 0.7,
+            'N': 0.65, 'O': 0.6, 'F': 0.5, 'Ne': 1.6, 'Na': 1.8, 'Mg': 1.5,
+            'Al': 1.25, 'Si': 1.1, 'P': 1.0, 'S': 1.0, 'Cl': 1.0, 'Ar': 0.71,
+            'K': 2.2, 'Ca': 1.8, 'Sc': 1.6, 'Ti': 1.4, 'V': 1.35, 'Cr': 1.4,
+            'Mn': 1.4, 'Fe': 1.4, 'Co': 1.35, 'Ni': 1.35, 'Cu': 1.35, 'Zn': 1.35,
+            'Ga': 1.3, 'Ge': 1.25, 'As': 1.15, 'Se': 1.15, 'Br': 1.15, 'Kr': None,  
+            'Rb': 2.35, 'Sr': 2.0, 'Y': 1.8, 'Zr': 1.55, 'Nb': 1.45, 'Mo': 1.45,
+            'Tc': 1.35, 'Ru': 1.3, 'Rh': 1.35, 'Pd': 1.4, 'Ag': 1.6, 'Cd': 1.55,
+            'In': 1.55, 'Sn': 1.45, 'Sb': 1.45, 'Te': 1.4, 'I': 1.4, 'Xe': None,  
+            'Cs': 2.6, 'Ba': 2.15, 'La': 1.95, 'Ce': 1.85, 'Pr': 1.85,
+            'Nd': 1.85, 'Pm': 1.85, 'Sm': 1.85, 'Eu': 1.85, 'Gd': 1.8,
+            'Tb': 1.75, 'Dy': 1.75, 'Ho': 1.75, 'Er': 1.75, 'Tm': 1.75,
+            'Yb': 1.75, 'Lu': 1.75, 'Hf': 1.55, 'Ta': 1.45, 'W': 1.35,
+            'Re': 1.35, 'Os': 1.3, 'Ir': 1.35, 'Pt': 1.35, 'Au': 1.35,
+            'Hg': 1.5, 'Tl': 1.9, 'Pb': 1.8, 'Bi': 1.6, 'Po': 1.9,
+            'At': None, 'Rn': None, 'Fr': None, 'Ra': 2.15, 'Ac': 1.95,
+            'Th': 1.8, 'Pa': 1.8, 'U': 1.75, 'Np': 1.75, 'Pu': 1.75,
+            'Am': 1.75, 'Cm': 1.76, 'Bk': None, 'Cf': None, 'Es': None,
+            'Fm': None, 'Md': None, 'No': None, 'Lr': None, 'Rf': None,
+            'Db': None, 'Sg': None, 'Bh': None, 'Hs': None, 'Mt': None,
+            'Ds': None, 'Rg': None, 'Cn': None, 'Nh': None, 'Fl': None,
+            'Mc': None, 'Lv': None, 'Ts': None, 'Og': None
+            }
+            
+        self._atomic_radii = {
+            'H': 0.53, 'He': 0.31, 'Li': 1.67, 'Be': 1.12, 'B': 0.87, 'C': 0.67, 'N': 0.56, 'O': 0.48, 'F': 0.42,
+            'Ne': 0.38, 'Na': 1.90, 'Mg': 1.45, 'Al': 1.18, 'Si': 1.11, 'P': 0.98, 'S': 0.88, 'Cl': 0.79,
+            'Ar': 0.71, 'K': 2.43, 'Ca': 1.94, 'Sc': 1.84, 'Ti': 1.76, 'V': 1.71, 'Cr': 1.66, 'Mn': 1.61,
+            'Fe': 1.56, 'Co': 1.52, 'Ni': 1.49, 'Cu': 1.45, 'Zn': 1.42, 'Ga': 1.36, 'Ge': 1.25, 'As': 1.14,
+            'Se': 1.03, 'Br': 0.94, 'Kr': 0.88, 'Rb': 2.65, 'Sr': 2.19, 'Y': 2.12, 'Zr': 2.06, 'Nb': 1.98,
+            'Mo': 1.90, 'Tc': 1.83, 'Ru': 1.78, 'Rh': 1.73, 'Pd': 1.69, 'Ag': 1.65, 'Cd': 1.61, 'In': 1.56,
+            'Sn': 1.45, 'Sb': 1.33, 'Te': 1.23, 'I': 1.15, 'Xe': 1.08, 'Cs': 2.98, 'Ba': 2.53, 'La': 1.95,
+            'Ce': 1.85, 'Pr': 2.47, 'Nd': 2.06, 'Pm': 2.05, 'Sm': 2.38, 'Eu': 2.31, 'Gd': 2.33, 'Tb': 2.25,
+            'Dy': 2.28, 'Ho': 2.26, 'Er': 2.26, 'Tm': 2.22, 'Yb': 2.22, 'Lu': 2.17, 'Hf': 2.08, 'Ta': 2.00,
+            'W': 1.93, 'Re': 1.88, 'Os': 1.85, 'Ir': 1.80, 'Pt': 1.77, 'Au': 1.74, 'Hg': 1.70, 'Tl': 1.55,
+            'Pb': 1.54, 'Bi': 1.43, 'Th': 1.79, 'Pa': 1.61, 'U': 1.58, 'Np': 1.55, 'Pu': 1.53, 'Am': 1.51,
+            'Cm': 1.50, 'Bk': 1.50, 'Cf': 1.50, 'Es': 1.50, 'Fm': 1.50, 'Md': 1.50, 'No': 1.50, 'Lr': 1.50,
+            'Rf': 1.50, 'Db': 1.50, 'Sg': 1.50, 'Bh': 1.50, 'Hs': 1.50, 'Mt': 1.50, 'Ds': 1.50, 'Rg': 1.50,
+            'Cn': 1.50, 'Nh': 1.50, 'Fl': 1.50, 'Mc': 1.50, 'Lv': 1.50, 'Ts': 1.50, 'Og': 1.50
+        }
+
         self.electronegativity = {
             'H': 2.2, 'He': None, 'Li': 1.0, 'Be': 1.5, 'B': 2.0, 'C': 2.5, 'N': 3.1, 'O': 3.5, 'F': 4.1, 'Ne': None, 'Na': 0.9,
             'Mg': 1.2, 'Al': 1.5, 'Si': 1.7, 'P': 2.1, 'S': 2.4, 'Cl': 2.8, 'Ar': None, 'K': 0.9, 'Ca': 1.0, 'Sc': 1.2, 'Ti': 1.3,
             'V': 1.3, 'Cr': 1.6, 'Mn': None, 'Fe': 1.6, 'Co': None, 'Ni': 1.5, 'Cu': 1.8, 'Zn': 1.4, 'Ga': 1.6, 'Ge': 1.8,
             'As': 2.0, 'Se': 2.4, 'Br': 2.7, 'Kr': None, 'Rb': 0.9, 'Sr': 1.0, 'Y': None, 'Zr': None, 'Nb': None, 'Mo': 1.3,
             'Tc': None, 'Ru': 1.4, 'Rh': 1.5, 'Pd': 1.4, 'Ag': 1.4, 'Cd': 1.4, 'In': 1.4, 'Sn': 1.4, 'Sb': 1.5, 'Te': 2.1,
             'I': 2.2, 'Xe': None, 'Cs': 0.7, 'Ba': 0.9, 'Lu': None, 'Hf': 1.3, 'Ta': 1.3, 'W': 1.3, 'Re': 1.6, 'Os': 1.6,
@@ -579,24 +622,24 @@
             "Mg": (0.4, 0.8, 0.0),  # Verde oliva
             "Al": (0.8, 0.6, 0.5),  # Rosa
             "Si": (0.5, 0.5, 1.0),  # Azul medio
             "P":  (1.0, 0.5, 0.0),  # Naranja
             "S":  (1.0, 1.0, 0.0),  # Amarillo
             "Cl": (0.0, 1.0, 0.5),  # Verde menta
             "Ar": (0.5, 0.0, 0.5),  # Púrpura
-            "K":  (0.6, 0.1, 0.7),  # 
+            "K":  (0.3, 0.0, 0.8),  # Purple
             "Ca": (0.3, 0.3, 0.3),  # Gris medio
             "Sc": (0.9, 0.6, 0.9),  # Lavanda
             "Ti": (0.3, 0.8, 0.8),  # Turquesa
-            "V":  (0.6, 0.2, 0.2),  # Marrón rojizo
+            "V":  (0.9, 1.0, 1.0),  # Marrón rojizo
             "Cr": (0.4, 0.0, 0.0),  # Rojo oscuro
             "Mn": (0.7, 0.0, 0.7),  # Magenta
             "Fe": (0.6, 0.4, 0.0),  # Naranja oscuro
             "Co": (0.0, 0.6, 0.6),  # Verde azulado
-            "Ni": (0.6, 0.6, 0.6),  # Gris plata
+            "Ni": (0.0, 0.8, 0.2),  # Gris plata
             "Cu": (0.7, 0.4, 0.2),  # Bronce
             "Zn": (0.5, 0.5, 0.5),   # Gris
 
             "Ga": (0.76, 0.56, 0.56),  # Rojo claro
             "Ge": (0.40, 0.56, 0.56),  # Verde azulado claro
             "As": (0.74, 0.50, 0.89),  # Púrpura claro
             "Se": (1.00, 0.63, 0.00),  # Naranja
```

### Comparing `sage_lib-0.1.4.9/sage_lib/main.py` & `sage_lib-0.1.5.0/sage_lib/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -259,17 +259,17 @@
         else:
             for conteiner_index, conteiner in enumerate(PT.containers):
                 file_location = output_path+f'/frame{conteiner_index}'
                 PT.create_directories_for_path(file_location)
                 conteiner.AtomPositionManager.plot_RBF(periodic_image=0, cutoff=cutoff, number_of_bins=number_of_bins, output_path=file_location,
                                                         bin_volume_normalize=True, number_of_atoms_normalize=True, density_normalize=True)
 
-def generate_MD(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
-                    plot:str=None, reference:str=None, ff_energy_tag:str=None, ff_forces_tag:str=None, sigma:float=None,
-                    verbose:bool=False, conteiner_index:int=None):
+def generate_MD(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, output_source: str = None,
+                    plot:str=None, reference:str=None, ff_energy_tag:str=None, ff_forces_tag:str=None, sigma:float=None, topology:str=None, wrap:bool=None,
+                    verbose:bool=False, conteiner_index:int=None, tranparency:bool=None, bins:int=None, save:bool=None):
     """
     Generate plots from simulation data.
 
     This function processes simulation data and generates plots, such as band structure or molecular structures, based on the data and specified plot type.
 
     Parameters:
     path (str): Path to the directory containing the simulation data files.
@@ -283,32 +283,34 @@
     Returns:
     None
     """
     # 'count_species', 'displacements', 'RBF', 'evaluate_ff', 'bond_distance_tracking', 'molecule_formation_tracking'
     output_path = output_path if output_path is not None else '.'
     PT = Partition(path)
     PT.read_files( file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
-    if plot.upper() == 'COUNT_SPECIES':
-        PT.handleMDAnalysis( values= {'COUNT_SPECIES':{'output_path':output_path, 'verbose':verbose} }  )
 
-    elif plot.upper() == 'DISPLACEMENTS':
-        PT.handleMDAnalysis( values= {'DISPLACEMENTS':{'reference':reference, 'verbose':verbose} }  )
+    if plot.upper() == 'PATH_TRACKING':
+        PT.handleMDAnalysis( values= {'PATH_TRACKING':{'wrap':wrap, 'tranparency':tranparency, 'bins':bins, 'verbose':verbose, 'save':save} }  )
 
     elif plot.upper() == 'RBF':
         PT.handleMDAnalysis( values= {'RBF':{'output_path':output_path, 'verbose':verbose} }  )
 
+    elif plot.upper() == 'COUNT_SPECIES':
+        PT.handleMDAnalysis( values= {'COUNT_SPECIES':{'output_path':output_path, 'verbose':verbose, 'sigma':sigma} }  )
+
     elif plot.upper() == 'EVALUATE_FF':
         PT.handleMDAnalysis( values= {'EVALUATE_FF':{'output_path':output_path, 'ff_energy_tag':ff_energy_tag, 'ff_forces_tag':ff_forces_tag, 'verbose':verbose} }  )
 
     elif plot.upper() == 'BOND_DISTANCE_TRACKING':
         PT.handleMDAnalysis( values= {'BOND_DISTANCE_TRACKING':{'reference':reference, 'sigma':sigma, 'output_path':output_path, 'verbose':verbose} }  )
     
     elif plot.upper() == 'MOLECULE_FORMATION_TRACKING':
-        PT.handleMDAnalysis( values= {'MOLECULE_FORMATION_TRACKING':{'sigma':sigma, 'output_path':output_path, 'verbose':verbose} }  )
-   
+        PT.handleMDAnalysis( values= {'MOLECULE_FORMATION_TRACKING':{'sigma':sigma, 'topology':topology, 'verbose':verbose} }  )
+        PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
+
 def generate_AbInitioThermodynamics(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
                 plot:str=None, reference_ID:list=None, especie:str=None, mu_max:float=None, mu_min:float=None,
                 verbose:bool=False, conteiner_index:int=None):
     """
     .
     """
     output_path = output_path if output_path is not None else '.'
@@ -318,15 +320,15 @@
     if plot.upper() == 'PHASE_DIAGRAM':
         PT.handleABITAnalysis( values= {'phase_diagram':{'reference_ID':reference_ID, 'especie':especie, 'mu_max':mu_max, 'mu_min':mu_min, 
                                                         'output_path':output_path, 'verbose':verbose} }  )
 
 def generate_edit_positions(path: str, source: str = None, forces_tag:str=None, energy_tag:str=None, subfolders: bool = False, output_path: str = None, 
                             output_source: str = None, verbose: bool = False, edit: str = None, N: int = None, direction:str=None, 
                             std: float = None, repeat: list = None, compress_min: list = None, compress_max: list = None,
-                            init_index:int=None, mid_index:int=None, end_index:int=None):
+                            init_index:int=None, mid_index:int=None, end_index:int=None, degree:int=None, first_neighbor:bool=None):
     """
     Modifies and exports atomic positions based on specified editing operations.
 
     This function applies various editing operations like 'rattle', 'supercell', or 'compress' to the atomic positions
     in the provided path and exports the modified structures.
 
     Parameters:
@@ -354,43 +356,51 @@
 
     # Apply the specified movement to the atomic positions
     if edit.lower() == 'rattle':
         # Ensure that N and std are provided for the 'rattle' move
         if N is None or std is None:
             raise ValueError("For the 'rattle' edit, both 'N' and 'std' parameters must be provided.")
         
-        PT.generate_variants('rattle', [{'N': N, 'std': [std]}])
+        values = {'N': N, 'std': [std]}
+        PT.containers = PT.handleRattle(values=values)
         PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
-    if edit.lower() == 'supercell':
+    elif edit.lower() == 'supercell':
         # Ensure that N and std are provided for the 'rattle' move
         if repeat is None:
             raise ValueError("For the 'supercell' edit, the 'repeat' parameter must be provided.") 
 
         for container in PT.containers:
             container.AtomPositionManager.generate_supercell(repeat=repeat)
             name  = '_'.join( [ str(r) for r in repeat ] )
             container.file_location += f'/{name}'
         PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
-    if edit.lower() == 'compress':
+    elif edit.lower() == 'compress':
         #
         if compress_min is None and compress_max is None:
             raise ValueError("For the 'compress' edit, the 'compress_factor' parameter must be provided.") 
 
         PT.generate_variants(parameter='compress', values={'N': N, 'compress_min': compress_min, 'compress_max': compress_max} )
         PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
-    if edit.lower() == 'widening':
+    elif edit.lower() == 'widening':
         #
         PT.containers = PT.handleWidening(values=[{'direction': direction, 'N':N, 'init_index': init_index, 'mid_index': mid_index, 'end_index': end_index}])
         PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
+    elif edit.lower() == 'interpolation':
+        ''' 
+        '''
+        value = {'images':N, 'degree':degree, 'first_neighbor':first_neighbor}
+        PT.containers = PT.handleInterpolation(values=value)
+        PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
+
 def generate_edit_configuration(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, output_path:str=None, output_source:str=None, verbose:bool=False, edit:str=None,
-                            atom_ID:list=None, new_atom_ID:list=None, weights:list=None, N:int=None):
+                            atom_index:list=None, atom_ID:list=None, new_atom_ID:list=None, weights:list=None, N:int=None, search:str=None, seed:int=None):
     """
     Edits the configuration of atomic structures by changing atomic IDs and exports the modified structures.
 
     This function changes the IDs of atoms in the provided structures based on the specified edit operations and 
     then exports these modified structures to the defined output path.
 
     Parameters:
@@ -410,22 +420,26 @@
 
     # Initialize the DFTPartition object
     PT = Partition(path)
 
     # Read files based on provided parameters
     PT.read_files( file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
 
-    if edit.upper() == 'ATOM_ID':
-        PT.generate_variants(   
-                                parameter='CHANGE_ATOM_ID', 
-                                values={    'atom_ID':atom_ID,
-                                            'new_atom_ID':new_atom_ID, 
-                                            'weights':weights,
-                                            'N':N 
-                                            }, )
+    values = {
+        'search': search,
+        'atom_index': atom_index,
+        'atom_ID': atom_ID,
+        'new_atom_ID': new_atom_ID,
+        'N': N,
+        'weights':weights,
+        'seed':seed,
+        'verbose':verbose
+                }
+
+    PT.handleAtomIDChange( values={f'{edit}':values} )
 
     # Export the edited files
     PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
 def generate_filter(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, output_path:str=None, output_source:str=None, verbose:bool=False, 
                     filter_class:str=None, container_property:str=None, filter_type:str=None, value:float=None, ID:str=None, traj:bool=False, N:int=None):
     """
@@ -470,15 +484,15 @@
     # Initialize the DFTPartition object
     PT = Partition(path)
 
     # Read files and apply filters
     PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
     if operation.upper() == 'SORT':
         PT.handleDataset( values= {'sort':{'verbose':verbose} }  )
-    print( [n.AtomPositionManager.E for n in PT.containers] )
+
     # Export the filtered files
     PT.export_files(file_location=output_path, source=source, label='enumerate', verbose=verbose)
 
 
 def generate_supercell_embedding(
                         unitcell_path:str=None,              unitcell_source:str=None, forces_tag:str=None, energy_tag:str=None,
                         relax_supercell_path:str=None,       relax_supercell_source:str=None, 
@@ -518,14 +532,15 @@
 
     # Export the embedded supercell
     PT.export_defect_supercell_unrelax_Np1(source=output_source, file_location=output_path)
 
 def generate_solvent(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, conteiner_index:int=None, output_path:str=None, output_source:str=None, verbose:bool=False, 
                     density:float=None, solvent:list=None, slab:bool=None, 
                     shape:str=None, size:list=None, vacuum_tolerance:float=None, 
+                    seed:float=None,
                     colition_tolerance:float=None, translation:list=None, wrap:bool=None):
     """
     Generates a solvent environment for molecular dynamics or quantum mechanics simulations.
 
     Parameters:
     - path (str): Path to the directory containing input files for the simulation.
     - source (str, optional): Source format of the input files (e.g., 'VASP', 'OUTCAR', etc.).
@@ -550,46 +565,73 @@
     generates variants based on these configurations, and exports the results.
     """
     # Initialize the DFTPartition object
     PT = Partition()
 
     # Read files and apply configurations
     PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
-
+    
     values = {
         'density': density,
         'solvent': solvent,
         'slab': slab,
         'shape': shape,
         'size': size,
         'vacuum_tolerance': vacuum_tolerance,
         'colition_tolerance': colition_tolerance,
         'translation': translation,
         'wrap': wrap,
+        'seed':seed,
+        'verbose':verbose
     }
-
-    PT.generate_variants(parameter='SOLVENT', values=[values])
+    PT.handleCLUSTER( values= {'ADD_SOLVENT':values}  )
 
     # Export the modified files
     PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
+def generate_BLENDER(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
+                plot:str=None, resolution:list=None, samples:int=None, fog:bool=None, render:bool=False, 
+                sigma:float=None, scale:float=None, camera:list=None, repeat:list=None, 
+                verbose:bool=False, conteiner_index:int=None):
+
+    # Initialize the DFTPartition object
+    PT = Partition()
+
+    # Read files and apply configurations
+    PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+    
+    values = {
+        'samples': samples,
+        'resolution_x': resolution[0],
+        'resolution_y': resolution[1],
+        'fog': fog,
+        'render':render,
+        'sigma': sigma,
+        'scale': scale,
+        'camera': camera,
+        'repeat': repeat,
+        'verbose': verbose,
+    }
+
+    PT.handleBLENDER( values={f'{plot}':values}  )
+
 def add_arguments(parser):
     """
     Adds common arguments to the given subparser. This includes arguments for file paths, 
     verbosity, and other common settings used across various sub-commands.
     """
     structure_list = ['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS', 'gen', 'POSCAR', 'AIMS', 'ASE', 'PDB']
     parser.add_argument('--path', type=str, default='.', help='Path to the files directory')
-    parser.add_argument('--source', type=str, choices=structure_list, default='VASP', help='Source of calculation from which the files originate: VASP, molecular_dynamics, or force_field (default: VASP)')
+    parser.add_argument('--source', type=str, choices=structure_list, help='Source of calculation from which the files originate: VASP, molecular_dynamics, or force_field (default: VASP)')
     
     parser.add_argument('--forces-tag', type=str, default='forces', help='')
     parser.add_argument('--energy-tag', type=str, default='E', help='')
 
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
-    parser.add_argument('--output_source', type=str, choices=structure_list, default='VASP', help='Source for exporting partition and scripts')
+    parser.add_argument('--output_source', type=str, choices=structure_list, help='Source for exporting partition and scripts')
 
     parser.add_argument('--verbose', default=False, action='store_true', help='Display additional information')
     parser.add_argument('--subfolders', default=False, action='store_true', help='Read from all subfolders under the specified path')    
     parser.add_argument('--conteiner_index', type=int, help='')    
 
 
 def main():
@@ -657,43 +699,54 @@
     parser_plot.add_argument('--emax', type=float, help='Specifies the maximum energy (in eV) for the plot range. Similar to --emin, it allows focusing on a specific energy interval in the plot.')
     parser_plot.add_argument('--cutoff', type=float, default=6.0, help='Defines the cutoff distance (in Ångströms) for RBF plots. This parameter is crucial for determining the extent of spatial interactions to be considered in the plot.')
     parser_plot.add_argument('--number_of_bins', type=int, default=100, help='Sets the number of bins for the histogram in RBF plots. A higher number of bins can lead to finer details in the plot, but may also increase computational load.')
 
     # =========== MD analisis ===========
     parser_MD = subparsers.add_parser('MD', help='')
     add_arguments(parser_MD)
-    parser_MD.add_argument('--plot', type=str, required=True, choices=['count_species', 'displacements', 'RBF', 'evaluate_ff', 'bond_distance_tracking', 'molecule_formation_tracking'], help='')
+    parser_MD.add_argument('--plot', type=str, required=True, choices=[
+            'path_tracking', 'count_species', 'RBF', 'evaluate_ff', 'bond_distance_tracking', 'molecule_formation_tracking'], help='')
     parser_MD.add_argument('--specie', type=str, required=False, help='')
-    parser_MD.add_argument('--sigma', type=float, required=False, help=' bonda factor')
+    parser_MD.add_argument('--sigma', type=float, required=False, default=1.2, help='bonda factor')
     parser_MD.add_argument('--reference', type=str, required=False, help='')
+    parser_MD.add_argument('--topology', type=str, required=False, help='')
     parser_MD.add_argument('--ff-forces-tag', type=str, required=False, help='')
     parser_MD.add_argument('--ff-energy-tag', type=str, required=False, help='')
-
+    parser_MD.add_argument('--wrap', default=False, action='store_true', help='.')
+    parser_MD.add_argument('--save', default=False, action='store_true', help='.')
+    parser_MD.add_argument('--tranparency', default=False, action='store_true', help='.')
+    parser_MD.add_argument('--bins', type=int, default=100, required=False, help='')
+    
     # ========== Sub-command: edit_positions ===========
     parser_edit = subparsers.add_parser('edit_positions', help='Modify atomic positions in the input files, allowing operations like "rattling" to introduce small random displacements.')
     add_arguments(parser_edit)
-    parser_edit.add_argument('--edit', type=str, choices=['rattle', 'compress', 'supercell', 'widening'], default='rattle', help='Type of modification to apply to atomic positions. E.g., "rattle" for random displacements.')
+    parser_edit.add_argument('--edit', type=str, choices=['rattle', 'compress', 'supercell', 'widening', 'interpolation'], default='rattle', help='Type of modification to apply to atomic positions. E.g., "rattle" for random displacements.')
     parser_edit.add_argument('--std', type=float, required=False, help='Standard deviation for displacement distribution in "rattle" operation, defining displacement magnitude.')
     parser_edit.add_argument('--N', type=int, required=False, help='Number of applications of the selected operation. Defaults to 1 if not specified.')
     parser_edit.add_argument('--repeat', type=int, nargs=3, default=[1, 1, 1], help='Repeat the unit cell in x, y, z dimensions respectively. Format: x y z')
     parser_edit.add_argument('--direction', type=str, choices=['x', 'y', 'z'], required=False, default='z', help='')
     parser_edit.add_argument('--compress_min', type=float, nargs=3, default=[1, 1, 1], help='Minimum compression factors in x, y, z for the "compress" operation. Format: x y z')
     parser_edit.add_argument('--compress_max', type=float, nargs=3, default=[1, 1, 1], help='Maximum compression factors in x, y, z for the "compress" operation. Format: x y z')
     parser_edit.add_argument('--init_index', type=int, required=False, help='')
     parser_edit.add_argument('--mid_index', type=int, required=False, help='')
     parser_edit.add_argument('--end_index', type=int, required=False, help='')
+    parser_edit.add_argument('--degree', type=int, required=False, default=1, help='')
+    parser_edit.add_argument('--first_neighbor', required=False, default=False, action='store_true', help='')
 
     # ========== Sub-command: edit_configuration ===========
     parser_edit_config = subparsers.add_parser('edit_configuration', help='Modify the configuration settings of your simulation or calculation process.')
     add_arguments(parser_edit_config)
-    parser_edit_config.add_argument('--edit', type=str, help='Specify the type of configuration modification.')
+    parser_edit_config.add_argument('--edit', type=str, choices=['atom_id', 'atom_index'], help='Specify the type of configuration modification.')
+    parser_edit_config.add_argument('--search', type=str, choices=['full', 'random'], required=False, help='')
+    parser_edit_config.add_argument('--index', type=int, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--ID', type=str, nargs='+', required=False, help='Identifier for the configuration element to modify.')
     parser_edit_config.add_argument('--new_ID', type=str, nargs='+', required=False, help='New identifier to assign to the configuration element.')
     parser_edit_config.add_argument('--weights', type=float, nargs='+', required=False, help='')
-    parser_edit_config.add_argument('--N', default=1, type=int, help='.')
+    parser_edit_config.add_argument('--N', default=1, type=int, required=False, help='.')
+    parser_edit_config.add_argument('--seed', default=1, type=int, required=False, help='.')
 
     # ========== Sub-command: filter ===========
     parser_filter = subparsers.add_parser('filter', help='Apply filters to select specific data based on various criteria.')
     add_arguments(parser_filter)
     parser_filter.add_argument('--filter', choices=['random', 'flat_histogram', 'binary', 'index'], type=str, help='Type of filter to apply: random, flat_histogram, or binary.')
     parser_filter.add_argument('--property', choices=['E', 'E/N', 'forces', 'has_ID', 'has_not_ID'], type=str, help='Property to use for filtering: Energy (E), forces, or atom IDs.')
     parser_filter.add_argument('--type', choices=['max', 'min', 'equipartition', 'tail', 'uniform'], type=str, help='Filter type: max (maximum value) or min (minimum value).')
@@ -717,31 +770,44 @@
     
     # ========== ADD - solvent ===========
     parser_solvent = subparsers.add_parser('solvent', help='Configure solvent environment for molecular dynamics or quantum mechanics simulations. This includes setting solvent type, density, and the geometry of the simulation environment.')
     add_arguments(parser_solvent)
     parser_solvent.add_argument('--density', type=float, default='.', help='Specify the density of the solvent in the simulation. The unit of density should align with the simulation system.')
     parser_solvent.add_argument('--solvent', type=str, nargs='+', choices=['H2O', 'H2'], default='H2O', help='Select the type of solvent to be used. Options include "H2O" for water and "H2" for hydrogen. Multiple solvents can be specified.')
     parser_solvent.add_argument('--slab', default=False, action='store_true', help='Enable this flag to indicate a slab geometry in the simulation, typically used in surface studies.')
-    parser_solvent.add_argument('--shape', type=str, choices=['box', 'sphere'], default='box', help='Define the shape of the simulation box. Options are "box" for a rectangular prism and "sphere" for spherical geometry.')
+    parser_solvent.add_argument('--shape', type=str, choices=['box', 'sphere', 'cell', 'parallelepiped'], default='cell', help='Define the shape of the simulation box. Options are "box" for a rectangular prism and "sphere" for spherical geometry.')
     parser_solvent.add_argument('--size', type=float, nargs=3, default=[10, 10, 10], help='Set the dimensions of the simulation box, specified as length, width, and height. Applicable when the shape is "box".')
     parser_solvent.add_argument('--vacuum_tolerance', type=float, default=0.0, help='Set the vacuum tolerance for the simulation, defining the minimum allowed spacing between atoms or molecules.')
     parser_solvent.add_argument('--colition_tolerance', type=float, default=1.6, help='Specify the collision tolerance, which is the minimum distance allowed between atoms or molecules to avoid overlaps.')
+    parser_solvent.add_argument('--seed', type=float, default=0, help='')
     parser_solvent.add_argument('--translation', type=float, nargs=3, default=[0, 0, 0], help='Provide a translation vector to adjust the position of the system within the simulation box. Format: x-offset y-offset z-offset.')
     parser_solvent.add_argument('--wrap', default=True, action='store_true', help='Enable or disable wrapping of atoms or molecules within the simulation box boundaries. Useful for periodic boundary conditions.')
 
     # ========== AbInitioThermodynamics ===========
-    parser_AbIT = subparsers.add_parser('Thermodynamic', help='')
+    parser_AbIT = subparsers.add_parser('thermodynamic', help='')
     add_arguments(parser_AbIT)
     parser_AbIT.add_argument('--plot', type=str, choices=['phase_diagram'], default='phase_diagram', help='')
     parser_AbIT.add_argument('--especie', type=str, default='O', help='')
     parser_AbIT.add_argument('--reference_ID', type=int, nargs='+', help='')
     parser_AbIT.add_argument('--mu_max', type=float, default=0.0, help='')
     parser_AbIT.add_argument('--mu_min', type=float, default=-10.0, help='')
 
-
+    # ========== BLENDER ===========
+    parser_blender = subparsers.add_parser('blender', help='')
+    add_arguments(parser_blender)
+    parser_blender.add_argument('--plot', type=str, choices=['render'], default='xyz', required=False, help='')
+    parser_blender.add_argument('--resolution', type=int, nargs=2, default=[1920, 1920], required=False, help='')
+    parser_blender.add_argument('--samples', type=int, default=15, required=False, help='')
+    parser_blender.add_argument('--fog', action='store_true', default=False, required=False, help='')
+    parser_blender.add_argument('--render', action='store_true', default=False, required=False, help='')
+    parser_blender.add_argument('--sigma', type=float, default=1.1, required=False, help='')
+    parser_blender.add_argument('--scale', type=float, default=1.0, required=False, help='')
+    parser_blender.add_argument('--camera', type=str, nargs='+', default=['x', 'y', 'z'], choices=['x', '-x', 'y', '-y', 'z', '-z'], required=False, help='')
+    parser_blender.add_argument('--repeat', type=int, nargs=3, default=[0,0,0], required=False, help='')
+    
     args = parser.parse_args()
 
     # Handle execution based on the specified sub-command
     if args.command == 'defect':
         generate_defects(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, 
             defect=args.defect, species=args.species, new_species=args.new_species)
@@ -776,27 +842,29 @@
     elif args.command == 'plot':
         generate_plot(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, plot=args.plot, fermi=args.fermi,
             emin=args.emin, emax=args.emax, cutoff=args.cutoff, number_of_bins=args.number_of_bins)
 
     elif args.command == 'MD':
         generate_MD(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
-            verbose=args.verbose, output_path=args.output_path, plot=args.plot,  sigma=args.sigma, 
-            reference=args.reference, ff_energy_tag=args.ff_energy_tag, ff_forces_tag=args.ff_forces_tag)
+            output_path=args.output_path, output_source=args.output_source,
+            verbose=args.verbose, plot=args.plot,  sigma=args.sigma, topology=args.topology, wrap=args.wrap,
+            reference=args.reference, ff_energy_tag=args.ff_energy_tag, ff_forces_tag=args.ff_forces_tag, 
+            tranparency=args.tranparency, save=args.save)
 
     elif args.command == 'edit_positions':
         generate_edit_positions(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, verbose=args.verbose, 
             output_path=args.output_path, output_source=args.output_source, 
             edit=args.edit, std=args.std, N=args.N, direction=args.direction, repeat=args.repeat, compress_min=args.compress_min, compress_max=args.compress_max,
-            init_index=args.init_index, mid_index=args.mid_index, end_index=args.end_index)
+            init_index=args.init_index, mid_index=args.mid_index, end_index=args.end_index, degree=args.degree, first_neighbor=args.first_neighbor)
 
     elif args.command == 'edit_configuration':
         generate_edit_configuration(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, verbose=args.verbose, 
             output_path=args.output_path, output_source=args.output_source, 
-            edit=args.edit, atom_ID=args.ID, new_atom_ID=args.new_ID, weights=args.weights, N=args.N )
+            edit=args.edit, search=args.search, atom_index=args.index, atom_ID=args.ID, new_atom_ID=args.new_ID, weights=args.weights, N=args.N, seed=args.seed)
 
     elif args.command == 'filter':
         generate_filter(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, verbose=args.verbose, output_path=args.output_path, output_source=args.output_source,
                 filter_class=args.filter, container_property=args.property, filter_type=args.type, value=args.value, traj=args.traj, N=args.N, ID=args.ID)
 
     elif args.command == 'dataset':
         generate_dataset(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
@@ -814,18 +882,26 @@
         generate_solvent(
                         path=args.path,     source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, 
                         subfolders=args.subfolders, conteiner_index=args.conteiner_index,
     
                         density=args.density, solvent=args.solvent, slab=args.slab, 
                         shape=args.shape, size=args.size, vacuum_tolerance=args.vacuum_tolerance, 
                         colition_tolerance=args.colition_tolerance, translation=args.translation, wrap=args.wrap, 
+                        seed=args.seed, 
 
                         output_path=args.output_path,       output_source=args.output_source,
                         verbose=args.verbose )
 
-    elif args.command == 'Thermodynamic':
+    elif args.command == 'thermodynamic':
         generate_AbInitioThermodynamics(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, plot=args.plot, 
             reference_ID=args.reference_ID, especie=args.especie, mu_max=args.mu_max, mu_min=args.mu_min)
 
+    elif args.command == 'blender':
+        generate_BLENDER(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
+            verbose=args.verbose, output_path=args.output_path, 
+            plot=args.plot, resolution=args.resolution, samples=args.samples, fog=args.fog, render=args.render,
+            scale=args.scale, camera=args.camera, repeat=args.repeat, 
+            sigma=args.sigma, )
+
 if __name__ == '__main__':
     main()
```

### Comparing `sage_lib-0.1.4.9/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.0/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.0/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.0/sage_lib/partition/Partition.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,33 +91,47 @@
 
 try:
     from sage_lib.partition.partition_builder.AbInitioThermodynamics_builder import AbInitioThermodynamics_builder
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing AbInitioThermodynamics_builder: {str(e)}\n")
     del sys
-    
+
+try:
+    from sage_lib.partition.partition_builder.Blender_builder import Blender_builder
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing Blender_builder: {str(e)}\n")
+    del sys
+
 try:
     from sage_lib.partition.PartitionManager import PartitionManager
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing PartitionManager: {str(e)}\n")
     del sys
 
-
 try:
     import numpy as np
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing numpy: {str(e)}\n")
     del sys
 
+try:
+    from scipy.interpolate import interp1d
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing numpy: {str(e)}\n")
+    del sys
+
 class Partition(BandStructure_builder, Config_builder, Crystal_builder, CrystalDefect_builder, Dataset_builder, 
                  Molecule_builder, PositionEditor_builder, SurfaceStates_builder, VacuumStates_builder, Filter_builder, 
-                 SupercellEmbedding_builder, MoleculeCluster_builder,MolecularDynamic_builder,AbInitioThermodynamics_builder):
+                 SupercellEmbedding_builder, MoleculeCluster_builder,MolecularDynamic_builder,AbInitioThermodynamics_builder,
+                 Blender_builder):
     """
     The Partition class is designed to handle various operations related to different types
     of crystal structure manipulations. It inherits from multiple builder classes, each
     specialized in a specific aspect of crystal structure and simulation setup.
     """
 
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
@@ -323,7 +337,69 @@
         Returns
         -------
         float
             The R^2 score as a float.
         """
         # Compute R^2 score, indicating the proportion of variance in the dependent variable predictable from the independent variable(s).
         return 1 - (np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2))
+
+    def str_to_connectivity(self, input_string:str) -> dict:
+        # Initialize variables
+        elements = {}  # To store parsed elements and their indexes
+        i = 0  # Index to iterate through the string
+        element_id_map = {}
+
+        # Iterate through the string to parse elements and indexes
+        while i < len(input_string):
+            # Detect element (considering elements can have 2 characters, e.g., 'Ni')
+            if i < len(input_string) - 1 and input_string[i:i+2] in self.atomic_numbers.keys() :
+                element = input_string[i:i+2]
+                i += 2
+
+            elif input_string[i:i+1] in self.atomic_numbers.keys() or input_string[i:i+1] == '*':
+                element = input_string[i]
+                i += 1
+
+            # If next character is a digit, it's an index for self-connection, skip it
+            if i < len(input_string) and input_string[i].isdigit():
+                if not input_string[i] in element_id_map: element_id_map[input_string[i]] = len(elements)
+                element_id = element_id_map[input_string[i]]
+                i += 1
+            
+            else:
+                element_id = len(elements)
+            
+            # Add element to list
+            elements[len(elements)] = [element, element_id] 
+
+        return elements
+
+    def interpolate_with_splines(self, data:np.array, M:int, degree='cubic'):
+        """
+        Interpolates using splines or polynomials between each pair of subsequent images.
+        
+        Parameters:
+        - data: A NumPy array of shape (N, 3, I).
+        - M: Number of points to interpolate between each pair of images.
+        - degree: Type of spline or polynomial for interpolation ('linear', 'cubic', 'quadratic', etc.).
+        
+        Returns:
+        - A new array with interpolations.
+        """
+        N, _, I = data.shape
+        # Original "x" positions (indices of the images)
+        x_orig = np.arange(I)
+        # New "x" positions where we want to interpolate
+        x_new = np.linspace(0, I - 1, I + (I - 1) * M)
+        
+        # Prepare the new array
+        new_array = np.empty((N, 3, len(x_new)))
+        
+        # Iterate over each atom and each spatial dimension
+        for n in range(N):
+            for dim in range(3):
+                # Create an interpolation function for each atom and dimension
+                f_interp = interp1d(x_orig, data[n, dim, :], kind=degree)
+                # Compute interpolated values and assign them to the new array
+                new_array[n, dim, :] = f_interp(x_new)
+        
+        return new_array
```

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.0/sage_lib/partition/PartitionManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -149,54 +149,169 @@
 
     def apply_filter_mask(self, mask:list) -> bool:
         """
 
         """
         self._containers = [conteiner for conteiner, m in zip(self.containers, mask) if m == 1]
 
-    def read_Config_Setup(self, file_location:str=None, source='VASP', verbose=False):
-        '''
-        '''
-        file_location = file_location if type(file_location) == str else self.file_location
+    def _update_container(self, container, container_setter):
+        """
+        Updates a given container with simulation parameters extracted from the simulation reader.
+
+        Parameters:
+        - container: The container to be updated with simulation settings.
+        - container_setter: The simulation reader instance containing the extracted settings.
+
+        Returns:
+        None
+        """
+
+        container.InputFileManager = container_setter.InputFileManager
+        container.KPointsManager = container_setter.KPointsManager
+        container.PotentialManager = container_setter.PotentialManager
+        container.BashScriptManager = container_setter.BashScriptManager
+        container.vdw_kernel_Handler = container_setter.vdw_kernel_Handler
+        container.WaveFileManager = container_setter.WaveFileManager
+        container.ChargeFileManager = container_setter.ChargeFileManager
+
+    def read_config_setup(self, file_location: str = None, source: str = 'VASP', verbose: bool = False):
+        """
+        Reads simulation configuration from a specified file location and updates containers with the read settings.
+
+        This method supports reading configurations specifically tailored for VASP simulations. It extracts simulation
+        parameters such as input file management, k-points, potentials, and more, and applies these configurations
+        across all containers managed by this instance.
+
+        Parameters:
+        - file_location (str, optional): The path to the directory containing the simulation files. Defaults to None,
+                                         in which case the instance's file_location attribute is used.
+        - source (str, optional): The source/format of the simulation files. Currently, only 'VASP' is supported.
+                                  Defaults to 'VASP'.
+        - verbose (bool, optional): If True, prints detailed messages during the process. Defaults to False.
 
+        Returns:
+        None
+        """
+
+        # Use instance's file_location if none provided or invalid
+        file_location = file_location if isinstance(file_location, str) else self.file_location
+
+        # Initialize simulation reader based on the source format
         if source.upper() == 'VASP':
-            SR = self.readVASPFolder(file_location=file_location, add_container=False, verbose=verbose)
-            if SR.AtomPositionManager is not None:
-                SR.InputFileManager.set_LDAU( SR.AtomPositionManager.uniqueAtomLabels )
+            container_setter = self.read_vasp_folder(file_location=file_location, add_container=False, verbose=verbose)
+            if container_setter.AtomPositionManager is not None:
+                container_setter.InputFileManager.set_ldau(container_setter.AtomPositionManager.uniqueAtomLabels)
 
-        for c_i, container in enumerate(self.containers):
-            container.InputFileManager = SR.InputFileManager
-            container.KPointsManager = SR.KPointsManager
-            container.PotentialManager = SR.PotentialManager
-            container.BashScriptManager = SR.BashScriptManager
-            container.vdw_kernel_Handler = SR.vdw_kernel_Handler
-            container.WaveFileManager = SR.WaveFileManager
-            container.ChargeFileManager = SR.ChargeFileManager
+        # Update all containers with the read configuration
+        for container in self.containers:
+            self._update_container(container, container_setter)
+
+    @staticmethod
+    def _identify_file_type(file_name: str) -> str:
+        """
+        Identifies the type of file based on common atomic input file identifiers.
+
+        The function is case-insensitive and recognizes a variety of file types commonly
+        used in computational chemistry and physics. If the file type is not recognized,
+        it returns 'Unknown File Type'.
+
+        Parameters:
+        - file_name (str): The name of the file to identify.
+
+        Returns:
+        - str: The identified file type or 'Unknown File Type' if not recognized.
+
+        Example:
+        >>> identify_file_type('sample-OUTCAR.txt')
+        'OUTCAR'
+        """
+
+        # Mapping of file identifiers to their respective types, case-insensitive
+        file_types = {
+            'poscar': 'POSCAR', 'contcar': 'POSCAR',
+            'outcar': 'OUTCAR',
+            'config': 'xyz', 'xyz': 'xyz',
+            'traj': 'traj',
+            'pdb': 'pdb',
+            'cif': 'CIF',
+            'vasp': 'VASP',
+            'chgcar': 'CHGCAR',
+            'doscar': 'DOSCAR',
+            'xdatcar': 'XDATCAR',
+            'incar': 'INCAR',
+            'procar': 'PROCAR',
+            'wavecar': 'WAVECAR',
+            'kpoints': 'KPOINTS',
+            'eigenval': 'EIGENVAL'
+        }
+
+        # Convert the file name to lowercase for case-insensitive comparison
+        file_name_lower = file_name.lower()
+
+        # Identify the file type based on the presence of identifiers in the file name
+        for identifier, file_type in file_types.items():
+            if identifier in file_name_lower:
+                return file_type
+
+        # Return a default value if no known identifier is found
+        return 'Unknown File Type'
+
+    def read_files(self, file_location: str = None, source: str = None, subfolders: bool = False,
+                   energy_tag: str = None, forces_tag: str = None, verbose: bool = False):
+        """
+        Reads simulation files from the specified location, handling both individual files and subfolders
+        containing simulation data. It supports multiple file formats and structures, adapting the reading
+        process according to the source parameter.
+
+        Parameters:
+        - file_location (str, optional): The path to the directory or file containing simulation data.
+                                         Defaults to None, which uses the instance's file_location attribute.
+        - source (str, optional): The format/source of the simulation files (e.g., 'VASP', 'TRAJ', 'XYZ', 'OUTCAR').
+                                  Defaults to None.
+        - subfolders (bool, optional): If True, reads files from subfolders under the specified location.
+                                       Defaults to False.
+        - energy_tag (str, optional): Specific tag used to identify energy data within the files, applicable for
+                                      formats like 'XYZ'. Defaults to None.
+        - forces_tag (str, optional): Specific tag used to identify forces data within the files, applicable for
+                                      formats like 'XYZ'. Defaults to None.
+        - verbose (bool, optional): If True, enables verbose output during the file reading process. Defaults to False.
+
+        Raises:
+        - ValueError: If the source format is not recognized or supported.
+
+        Returns:
+        None
+        """
+        source = self._identify_file_type(file_location) if source is None else source
 
-    def read_files(self, file_location:str=None, source:str='VASP', subfolders:bool=False, energy_tag:str=None, forces_tag:str=None, verbose:bool=False):
-        '''
-        '''
         if subfolders:
-            self.readSubFolder(file_location=file_location, source=source, verbose=verbose)
+            self.read_subfolder(file_location=file_location, source=source, verbose=verbose)
+            return
 
-        else:
-            if source.upper() == 'VASP':
-                self.readVASPFolder(file_location=file_location, add_container=True, verbose=verbose)
-            elif source.upper() == 'TRAJ':
-                self.read_traj(file_location=file_location, add_container=True, verbose=verbose)
-            elif source.upper() == 'XYZ':
-                self.read_XYZ(file_location=file_location, add_container=True, verbose=verbose, energy_tag=energy_tag, forces_tag=forces_tag)
-            elif source.upper() == 'OUTCAR':
-                self.read_OUTCAR(file_location=file_location, add_container=True, verbose=verbose)
+        # Define a strategy for each source format to simplify the conditional structure
+        source_strategy = {
+            'VASP': self.read_vasp_folder,
+            'TRAJ': self.read_traj,
+            'XYZ': self.read_XYZ,
+            'OUTCAR': self.read_OUTCAR
+        }
+
+        try:
+            # Attempt to read using a specific strategy for the source format
+            if source.upper() in source_strategy:
+                source_strategy[source.upper()](file_location=file_location, add_container=True,
+                                                verbose=verbose, energy_tag=energy_tag, forces_tag=forces_tag)
             else:
-                try:    
-                    self.read_structure(file_location=file_location, source=source, add_container=True, verbose=verbose)
-                except Exception as e:
-                    print(f'Source {source} is not compatible. {e}')
-    
+                # Fallback for other sources
+                self.read_structure(file_location=file_location, source=source, add_container=True, verbose=verbose)
+        except KeyError as e:
+            raise ValueError(f"Source {source} is not compatible. {e}")
+        except Exception as e:
+            print(f"An error occurred while reading files: {e}")
+
     def readSubFolder(self, file_location:str=None, source:str='VASP', verbose=False):
         """
         Reads files from a specified directory and its subdirectories.
 
         This function is designed to traverse through a directory (and its subdirectories) to read files 
         according to the specified source type. It handles various file-related errors gracefully, providing 
         detailed information if verbose mode is enabled.
@@ -237,14 +352,15 @@
             If available, time information is also stored.
         """
         file_location = file_location if type(file_location) == str else self.file_location
         SR = SingleRun(file_location)
         SR.read_structure(file_location=file_location, source=source) 
         self.add_container(container=SR)
 
+
     def read_traj(self, file_location:str=None, add_container:bool=True, verbose=False):
         """
         Reads a trajectory file and stores each frame along with its time information.
 
         Args:
             file_location (str, optional): The file path of the trajectory file.
             verbose (bool, optional): If True, enables verbose output.
@@ -293,63 +409,68 @@
                     # 
                     if verbose: 
                         try: 
                             print(f' >> READ xyz :: frame {len(container)} - atoms {num_atoms}')
                         except Exception as e:
                             print(f'Verbose output failed due to an error: {e}')
                             print('Skipping line due to the above error.')
+                            
         return container
 
-    def read_OUTCAR(self, file_location:str=None, add_container:bool=True,verbose=False):
+    def read_OUTCAR(self, file_location:str=None, add_container:bool=True, verbose=False, **kwargs):
         '''
         '''
         OF = OutFileManager(file_location)
         OF.readOUTCAR()
 
         for APM in OF.AtomPositionManager:
             SR = SingleRun(file_location)
             SR._AtomPositionManager = APM
             SR._InputFileManager = OF.InputFileManager
             SR._KPointsManager = OF._KPointsManager
             SR._PotentialManager = OF._PotentialManager
             if add_container and SR.AtomPositionManager is not None: 
                 self.add_container(container=SR)
 
-    def readVASPFolder(self, file_location:str=None, add_container:bool=True, verbose:bool=False):
+    def read_vasp_folder(self, file_location:str=None, add_container:bool=True, verbose:bool=False):
         '''
         '''
         file_location = file_location if type(file_location) == str else self.file_location
         SR = SingleRun(file_location)
         SR.readVASPDirectory(file_location)        
         if add_container and SR.AtomPositionManager is not None: 
             self.add_container(container=SR)
 
         return SR
 
-    def export_files(self, file_location:str=None, source:str='VASP', label:str=None, bond_factor:float=None, verbose:bool=False):
+    def export_files(self, file_location:str=None, source:str=None, label:str=None, bond_factor:float=None, verbose:bool=False):
         """
         Exports files for each container in a specified format.
 
         The function iterates over all containers and exports them according to the specified format.
         In case of an error during export, it logs the error (if verbose is True) and continues with the next container.
 
         Args:
             file_location (str): The base directory for exporting files.
             source (str): The format to export files in ('VASP', 'POSCAR', 'XYZ', 'PDB', 'ASE').
             label (str): Labeling strategy for exported files ('enumerate' or 'fixed').
             bond_factor (float): The bond factor to use for PDB export.
             verbose (bool): If True, enables verbose output including error messages.
         """
+        source = self._identify_file_type(file_location) if source is None else source
+
         label = label if isinstance(label, str) else 'fixed'
         file_locations = []
 
         for c_i, container in enumerate(self.containers):
             try:
+                num_digits = len(str(len(self.containers)))
+
                 if label == 'enumerate':
-                    file_location_edited = file_location + f'/{c_i:03d}'
+                    file_location_edited = file_location + f'/{c_i:0{num_digits}d}'
                 elif label == 'fixed':
                     file_location_edited = container.file_location
 
                 if source.upper() != 'XYZ':
                     self.create_directories_for_path(file_location_edited)
                 else:
                     self.create_directories_for_path(file_location)
@@ -496,68 +617,7 @@
             This method creates or overwrites the file at the specified path with the given script content.
         """
         for sc_index, sc in enumerate(script_content):
             with open(file_path+f"/execution_script_for_each_container_{sc_index}.py", "w") as f:
                 f.write(sc)
 
 
-
-
-'''
-DP.exportVaspPartition()
-
-print(DP.containers[0].AtomPositionManager.pbc)
-DP.generateDFTVariants('band_structure', values=[{'points':20, 'special_points':'GMLCXG'}])
-DP.exportVaspPartition()
-
-
-path = '/home/akaris/Documents/code/Physics/VASP/v6.1/files/POSCAR/Cristals/test/files'
-DP = DFTPartition(path)
-DP.readVASPSubFolder(v=False)
-DP.readConfigSetup('/home/akaris/Documents/code/Physics/VASP/v6.1/files/POSCAR/Cristals/test/config')
-DP.generate_execution_script_for_each_container([ f'{n:03d}'for n, c in enumerate(DP.containers) ], '/home/akaris/Documents/code/Physics/VASP/v6.1/files/POSCAR/Cristals/test/calcs')
-
-#DP.read_configXYZ()
-
-'''
-
-
-
-
-'''
-DP.export_configXYZ()
-
-path = '/home/akaris/Documents/code/Physics/VASP/v6.1/files/dataset/CoFeNiOOH_jingzhu/surf_CoFe_4H_4OH/MAG'
-
-DP = DFTPartition(path)
-
-DP.readVASPFolder(v=True)
-
-DP.generateDFTVariants('Vacancy', [1], is_surface=True)
-#DP.generateDFTVariants('KPOINTS', [[n,n,1] for n in range(1, 15)] ) 
-
-
-path = '/home/akaris/Documents/code/Physics/VASP/v6.1/files/dataset/CoFeNiOOH_jingzhu/surf_CoFe_4H_4OH/MAG'
-DP = DFTPartition(path)
-DP.readVASPFolder(v=True)
-DP.generateDFTVariants('NUPDOWN', [n for n in range(0, 10, 1)] )
-DP.writePartition()
-
-path = '/home/akaris/DocumeEENnts/code/Physics/VASP/v6.1/files/POSCAR/Cristals/NiOOH/*OH surface with Fe(HS)'
-path = '/home/akaris/Documents/code/Physics/VASP/v6.1/files/POSCAR/Cristals/NiOOH/*OH surface for pure NiOOH'
-#DP = DFTPartition('/home/akaris/Documents/code/Physics/VASP/v6.1/files/bulk_optimization/Pt/parametros/ENCUT_optimization_252525_FCC')
-DP = DFTPartition(path)
-#DP.readVASPSubFolder(v=True)
-DP.readVASPFolder(v=True)
-
-#DP.generateDFTVariants('Vacancy', [1], is_surface=True)
-#DP.generateDFTVariants('KPOINTS', [[n,n,1] for n in range(1, 15)] )    
-DP.generateDFTVariants('ENCUT', [n for n in range(200, 1100, 45)] )
-
-DP.writePartition()
-
-DP.generateDFTVariants('ENCUT', [ E for E in range(400,700,30)] )
-print( DP.summary() )
-
-print( DP.containers[0].AtomPositionManager.summary() )
-'''
-
```

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -187,57 +187,76 @@
             for mn in range(molecule_number):
                 if verbosity: print(f'adding solvent: {int(mn/molecule_number*100)} %')
                 if not self.add_molecule( container=container, molecule=self.molecule_template[molecule_name], translation=translation, tolerance=tolerance,
                                         shape=shape, cluster_lattice_vectors=cluster_lattice_vectors, distribution=distribution, max_iteration=max_iteration ):
                     print('Can not set cluster, try lower density. ')
                     break
         
-    def handleCLUSTER(self, container:object, values:list, container_index:int,  file_location:str=None):
+    def handleCLUSTER(self, values:dict):
         """
         Handles the creation and management of a molecular cluster within a specified container.
 
         Parameters:
             container (object): The container in which the cluster is built.
             values (list): A list of parameters defining the cluster properties.
             container_index (int): The index of the container.
             file_location (str, optional): The file location for storing cluster data.
 
         Returns:
             list: A list of containers with the created clusters.
         """
-        sub_directories, containers = [], []
- 
-        for v in values:
-            # Copy and update container for each set of k-point values
-            container_copy = self.copy_and_update_container(container, f'/solvent/', file_location)
-            
-            for s in v['solvent']:
-                molecule = AtomPosition()
-                molecule.build(s)
-                self.add_molecule_template(s, molecule)
-            
-            if v['slab']:
-                vacuum_box, vacuum_start = container_copy.AtomPositionManager.get_vacuum_box(tolerance=v['vacuum_tolerance']) 
-                shape = 'box'
-                distribution = 'random'
-            else:
-                vacuum_box, vacuum_start = v['size'], v['translation']
-                shape = v['shape']
-                distribution = v['distribution']
-
-            tolerance = v['colition_tolerance']
-            density = v['density']
-
-            self.add_solvent(container=container_copy, shape=shape, cluster_lattice_vectors=vacuum_box, 
-                        translation=vacuum_start, distribution=distribution, density=density, tolerance=tolerance)
-
-            if v['wrap']:
-                container_copy.AtomPositionManager.pack_to_unit_cell()
-
-            concatenate_solvent = '-'.join(v['solvent'])
-            sub_directories.append(f'{density}_{concatenate_solvent}')
-            containers.append(container_copy)
+        #sub_directories, containers = [], []
+        
+        containers = []
+        for container_index, container in enumerate(self.containers):
+            for v_key, v_item in values.items():
+                if isinstance(v_item['seed'], float): np.random.seed(int(v_item['seed'])) 
+
+                if v_key.upper() == 'ADD_SOLVENT':
+                    # Copy and update container for each set of k-point values
+                    container_copy = self.copy_and_update_container(container, f'/solvent/', '')
+                    
+                    for s in v_item['solvent']:
+                        molecule = AtomPosition()
+                        molecule.build(s)
+                        self.add_molecule_template(s, molecule)
+                    
+                    if v_item['slab']:
+                        vacuum_box, vacuum_start = container_copy.AtomPositionManager.get_vacuum_box(tolerance=v_item['vacuum_tolerance']) 
+                        shape = 'box'
+                        distribution = 'random'
+                    else:
+                        shape = v_item['shape']
+                        if shape.upper() == 'BOX':
+                            shape = 'box'
+                            vacuum_box, vacuum_start = np.array([[v_item['size'][0],0,0],[0,v_item['size'][1],0],[0,0,v_item['size'][2]]], dtype=np.float64), v_item['translation']
+                        elif shape.upper() == 'SPHERE':
+                            shape = 'sphere'
+                            vacuum_box, vacuum_start = float(v_item['size'][0]), v_item['translation']
+                        elif shape.upper() == 'PARALLELEPIPED':
+                            shape = 'box'
+                            vacuum_box, vacuum_start = np.array([
+                                                            [v_item['size'][0],v_item['size'][1],v_item['size'][2]],
+                                                            [v_item['size'][3],v_item['size'][4],v_item['size'][5]],
+                                                            [v_item['size'][6],v_item['size'][7],v_item['size'][8]]], 
+                                                        dtype=np.float64), v_item['translation']
+                        elif shape.upper() == 'CELL':
+                            shape = 'box'
+                            vacuum_box, vacuum_start = np.array(container_copy.AtomPositionManager.get_cell() ,dtype=np.float64), np.array([0,0,0] ,dtype=np.float64)
+
+                        distribution = 'random'
+
+                    tolerance = v_item['colition_tolerance']
+                    density = v_item['density']
+
+                    self.add_solvent(container=container_copy, shape=shape, cluster_lattice_vectors=vacuum_box, 
+                                translation=vacuum_start, distribution=distribution, density=density, tolerance=tolerance)
+
+                    if v_item['wrap']:
+                        container_copy.AtomPositionManager.pack_to_unit_cell()
+
+                    containers.append(container_copy)
+
+        self.containers = containers
 
-        # Generate execution script for each updated container
-        #self.generate_execution_script_for_each_container(sub_directories, container.file_location + '/solvent')
         return containers
```

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     import imageio
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing imageio: {str(e)}\n")
     del sys
 
 try:
-    from concurrent.futures import ProcessPoolExecutor
+    from concurrent.futures import ProcessPoolExecutor, as_completed
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing imageio: {str(e)}\n")
     del sys
     
 try:
     import matplotlib.pyplot as plt
@@ -68,28 +68,36 @@
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing itertools: {str(e)}\n")
     del sys
 
 try:
     from scipy.stats import iqr
+    from scipy.interpolate import make_interp_spline
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing itertools: {str(e)}\n")
     del sys
 
 try:
     from sage_lib.descriptor import MBTR
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing sage_lib.IO.descriptor.MBTR: {str(e)}\n")
     del sys
+'''
+try:
+    from sage_lib.miscellaneous import MD_tools
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing sage_lib.IO.descriptor.MBTR: {str(e)}\n")
+    del sys
+''' 
 
-
-class MolecularDynamic_builder(PartitionManager):
+class MolecularDynamic_builder(PartitionManager, ):
     """
     Class for building and managing molecular dynamic simulations.
     
     Inherits from PartitionManager and integrates additional functionalities
     specific to molecular dynamics, such as calculating displacement and plotting.
 
     Attributes:
@@ -109,66 +117,56 @@
         """
         super().__init__(name=name, file_location=file_location)
 
         self._molecule_template = {}
         self._density = None
         self._cluster_lattice_vectors = None
 
-    def get_count_species(self, sigma:float=None) -> list:
-        """
+    def _calculate_reference_values(self, container, reference):
         """
-        count_species = []
-        for container_i, container in enumerate(self.containers):
-            count_species.append( container.AtomPositionManager.count_species(sigma) )
-
-        return count_species
-
-    def get_molecular_graph_tracking(self, sigma:float=None ) -> list:
-        count_species = []
-        for container_i, container in enumerate(self.containers):
-            count_species.append( container.AtomPositionManager.get_molecular_graph(sigma=sigma) )
-
-        for i, n in enumerate(count_species[1:]):
-            print('iter', i)
-            for j, m in enumerate(n):
-                if len(m) < 10 and not m in count_species[i]:
-                    print('MOL', j)                    
-                    for o in count_species[i]:
-                        for p in o:
-
-                            if p in m:
-                                print( [ self.containers[0].AtomPositionManager.atomLabelsList[oo] for oo in o ], [ self.containers[0].AtomPositionManager.atomLabelsList[oo] for oo in m ] )
-                                print( o, m )
+        Calculate reference values based on the specified reference type.
 
+        Args:
+            container: The container holding atom positions and lattice vectors.
+            reference (str): The reference type ('a', 'b', 'c', 'x', 'y', 'z').
 
-        return count_species
+        Returns:
+            numpy.ndarray: Calculated reference values.
+        """
+        if type(reference) is str and reference.upper() in ['A', 'B', 'C']:
+            lv_index = {'A': 0, 'B': 1, 'C': 2}[reference.upper()]
+            lv = container.AtomPositionManager.latticeVectors[:, lv_index]
+            return np.dot(container.AtomPositionManager.atomPositions, lv / np.linalg.norm(lv))
+        
+        if type(reference) is str and reference.upper() in ['X', 'Y', 'Z']:
+            return container.AtomPositionManager.atomPositions[:, {'X': 0, 'Y': 1, 'Z': 2}[reference.upper()]]
+    
+        return np.zeros(container.AtomPositionManager.atomCount)
 
-    def get_displacement(self, reference:str=None):
+    def get_positions(self, fractional:bool=False, wrap:bool=False):
         """
-        Calculate the displacement of atoms based on a reference point.
+        """
+        if wrap:
+            for container_i, container in enumerate(self.containers):
+                container.AtomPositionManager.wrap()
 
-        Args:
-            reference (str, optional): Reference axis or lattice vector ('a', 'b', 'c', 'x', 'y', 'z').
+        if fractional:
+            return np.array([container.AtomPositionManager.atomPositions_fractional  for container_i, container in enumerate(self.containers)], dtype=np.float64)
+        else:
+            return np.array([container.AtomPositionManager.atomPositions  for container_i, container in enumerate(self.containers)], dtype=np.float64)
 
-        Returns:
-            numpy.ndarray: Array of displacement values for each atom.
+    def get_count_species(self, sigma:float=None) -> list:
         """
-
-        data_displacement = []
+        """
+        count_species = []
         for container_i, container in enumerate(self.containers):
+            count_species.append( container.AtomPositionManager.count_species(sigma) )
 
-            if container_i == 0:
-                displacement_reference_values = container.AtomPositionManager.atomPositions
-                reference_values = self._calculate_reference_values(container, reference)
-
-            displacement = np.linalg.norm(displacement_reference_values - container.AtomPositionManager.atomPositions, axis=1)
-            data_displacement.append(displacement + reference_values)
+        return count_species
 
-        return np.array(data_displacement, dtype=np.float64 )
-        
     def get_evaluation(self, ff_energy_tag:str='ff-energy', ff_forces_tag:str='ff-forces', ):
         """
         Collects and organizes energy and force data for training and validation.
 
         This method compiles energies and forces from the AtomPositionManager instances
         associated with each container in the current EvaluationManager. It organizes
         this data into a structured format suitable for comparison and further analysis.
@@ -245,15 +243,15 @@
         data['N']['validation'] = np.array( data['N']['validation'], np.float64 )
 
         return data
 
     def get_bond_tracking(self, sigma:float=1.2, reference:str='Z', verbose:bool=True):
         '''
         '''
-        if verbose: print(sigma)
+        if verbose: print(f'bond_tracking :: Sigma: {sigma} reference {reference}')
         sigma = sigma if type(sigma) in [int, float] else 1.2
         initial_bonds = []
         c0 = self.containers[0].AtomPositionManager
         r_max = np.max( [c0.covalent_radii[a] for a in c0.uniqueAtomLabels] )
         for atomo_i, atomo in enumerate(c0.atomPositions):
             max_bond_lenth = (c0.covalent_radii[c0.atomLabelsList[atomo_i]]+r_max)*sigma
             neighbors = c0.find_all_neighbors_radius(x=atomo, r=max_bond_lenth)
@@ -268,15 +266,144 @@
         for c_i, c in enumerate(self.containers):
             reference_pos = self._calculate_reference_values(c, reference='Z')
             for n_i, n in enumerate(initial_bonds):
                 data[c_i, n_i, 0] = reference_pos[n[0]]
                 data[c_i, n_i, 1] = c.AtomPositionManager.distance( c.AtomPositionManager.atomPositions[n[0]], c.AtomPositionManager.atomPositions[n[1]] )
 
         return {'initial_bonds_index':initial_bonds, 'bonds_data':data}
+
+    def config_molecular_subgraph(self, container, container_i, pattern, verbose):
+        """
+        Function to be executed in parallel. Wraps the search_molecular_subgraph method.
+        
+        Parameters:
+        - container_i (int): Index of the container in self.containers
+        
+        Returns:
+        - Tuple of (container_i, search results)
+        """
+
+        if verbose:
+            print(f'(%) >> Config {container_i} ({float(container_i)/len(self.containers)*100}%)')
+        sms = container.AtomPositionManager.search_molecular_subgraph(pattern=pattern, verbose=verbose)
+
+        return container_i, sms
+
+    def get_molecular_graph_tracking(self, sigma: float = None, id_filter: bool = True, pattern: dict = None, 
+                                     prevent_overlapping: bool = True, prevent_shared_nodes: bool = True,
+                                     prevent_repeating: bool = True, backtracking: bool = False,
+                                     parallel: bool = False, verbose: bool = True) -> list:
+        """
+        Analyzes molecular graphs to identify specific patterns, offering options for parallel processing,
+        backtracking, and other custom filters.
+
+        Parameters:
+        - sigma (float): Optional parameter for algorithm adjustment.
+        - id_filter (bool): If True, applies an identifier-based filter to the analysis.
+        - pattern (dict): A dictionary specifying the pattern to look for in the molecular graphs.
+        - prevent_overlapping (bool): If True, prevents overlapping in pattern matching.
+        - prevent_shared_nodes (bool): Prevents shared nodes in the pattern matching process.
+        - prevent_repeating (bool): If True, ensures that repeating patterns are not counted.
+        - backtracking (bool): Enables or disables backtracking in the search process.
+        - parallel (bool): If True, enables parallel processing to speed up the analysis.
+        - verbose (bool): If True, prints detailed progress and debugging information.
+
+        Returns:
+        - list: A list of results from the molecular graph tracking process.
+
+        Note:
+        The method dynamically adjusts to either parallel or sequential execution based on the `parallel` flag.
+        """
+        
+        if verbose:
+            print(f'Looking for specific pattern: {pattern}')
         
+        # Determine execution mode and containers based on input flags
+        executor_class = ProcessPoolExecutor if parallel else None  # None signifies sequential execution
+        containers_to_process = [(len(self.containers), self.containers[-1])] if backtracking else enumerate(self.containers)
+
+        # Execute the configuration for each container, either in parallel or sequentially
+        if parallel:
+            with ProcessPoolExecutor() as executor:
+                futures = [executor.submit(self.config_molecular_subgraph, container, container_i, pattern, verbose)
+                           for container_i, container in containers_to_process]
+                results = [future.result() for future in futures]
+        else:
+            # Para ejecución secuencial, simplemente iteramos sin usar 'executor'
+            results = [self.config_molecular_subgraph(container, container_i, pattern, verbose) 
+                       for container_i, container in containers_to_process]
+
+        return results
+
+    # ========== PLOTs ========== # # ========== PLOTs ========== # # ========== PLOTs ========== # # ========== PLOTs ========== # 
+    # ========== PLOTs ========== # # ========== PLOTs ========== # # ========== PLOTs ========== # # ========== PLOTs ========== # 
+    @staticmethod
+    def setup_subplot(ax, xlabel, ylabel, title):
+        """
+        Set up the subplot with labels and title.
+
+        Args:
+            ax (matplotlib.axes.Axes): The axes object to setup.
+            xlabel (str): Label for the x-axis.
+            ylabel (str): Label for the y-axis.
+            title (str): Title of the subplot.
+        """
+        ax.set_xlabel(xlabel)
+        ax.set_ylabel(ylabel)
+        ax.set_title(title)
+
+    def plot_path(self, positions, bins:int=100, output_path:str=None, transparency:bool=True, wrap:bool=False, save:bool=True, verbose:bool=True):
+        """
+        """    
+        d_name = {0:'x', 1:'y', 2:'z', }
+        for d in range(3):
+            for u in self.containers[0].AtomPositionManager.uniqueAtomLabels:
+                mask = self.containers[0].AtomPositionManager.atomLabelsList == u
+
+                fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
+                color = self.containers[0].AtomPositionManager.element_colors[u]
+
+                mark = '.' if wrap else '-'
+                ax1.plot(positions[:, mask, d], mark, ms=1, alpha=0.1, lw=0.7, color=color)
+                self.setup_subplot(ax1, 'Time', f'Path {d_name[d]}', f'Path ({d_name[d]}) for {u}')
+
+                ax2.hist(positions[:, mask, d].flatten(), bins=bins, alpha=0.7, orientation='vertical', color=color)
+                self.setup_subplot(ax2, 'Frequency', f'Path {d_name[d]}', f'Histogram ({d_name[d]}) for {u}')
+
+                plt.tight_layout()
+                if save:
+                    plt.savefig(f'{output_path}/PATH_TRACKING_{u}_{d_name[d]}.png', dpi=300, transparent=transparency)
+
+                plt.clf()
+
+                if verbose:
+                    print(f' >> Plot :: PATH_TRACKING ({u}-{d_name[d]}) - data shape {positions.shape}')
+
+                for d2 in range(d+1,3):
+                    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
+
+                    mark = '.' if wrap else '-'
+                    ax1.plot(positions[:, mask, d], positions[:, mask, d2], mark, ms=.7, color=color, alpha=0.1, lw=0.8)
+                    self.setup_subplot(ax1, f'Path {d_name[d]}', f'Path {d_name[d2]}', f'Path ({d_name[d]}-{d_name[d2]}) for {u}')
+
+                    self.setup_subplot(ax2, f'Path {d_name[d]}', f'Path {d_name[d2]}', f'Histogram ({d_name[d]}-{d_name[d2]}) for {u}')
+                    h = ax2.hist2d(positions[:, mask, d].flatten(), positions[:, mask, d2].flatten(), bins=bins, cmap='Blues')
+
+                    # Añadir barra de color con referencia al resultado de hist2d
+                    cbar = fig.colorbar(h[3], ax=ax2)  # h[3] es el QuadMesh que hist2d regresa
+                    cbar.set_label('Frecuency')
+
+                    plt.tight_layout()
+                    if save:
+                        plt.savefig(f'{output_path}/PATH_TRACKING_{u}_{d_name[d]}-{d_name[d2]}.png', dpi=300, transparent=transparency)
+
+                    plt.clf()
+
+                    if verbose:
+                        print(f' >> Plot :: PATH_TRACKING ({u}-{d_name[d]}-{d_name[d2]}) - data shape {positions.shape}')
 
     def _plot_RBF_for_container(self, container, container_i, output_path, verbose:bool=True):
         """
         Función para trazar RBF para un contenedor específico.
         """
         if verbose: print(f'Plot container {container_i}')
         output_path_container = os.path.join(output_path, f'MD_RBF/{container_i}')
@@ -297,67 +424,29 @@
 
             for future in futures:
                 # Aquí puedes manejar los resultados o excepciones si es necesario
                 result = future.result()
 
         return data_displacement
 
-    def _calculate_reference_values(self, container, reference):
+    def animated_RBF(self, output_path:str=None, duration:float=0.1, save:bool=True, verbose:bool=True):
         """
-        Calculate reference values based on the specified reference type.
-
-        Args:
-            container: The container holding atom positions and lattice vectors.
-            reference (str): The reference type ('a', 'b', 'c', 'x', 'y', 'z').
 
-        Returns:
-            numpy.ndarray: Calculated reference values.
         """
-        if type(reference) is str and reference.upper() in ['A', 'B', 'C']:
-            lv_index = {'A': 0, 'B': 1, 'C': 2}[reference.upper()]
-            lv = container.AtomPositionManager.latticeVectors[:, lv_index]
-            return np.dot(container.AtomPositionManager.atomPositions, lv / np.linalg.norm(lv))
-        
-        if type(reference) is str and reference.upper() in ['X', 'Y', 'Z']:
-            return container.AtomPositionManager.atomPositions[:, {'X': 0, 'Y': 1, 'Z': 2}[reference.upper()]]
-    
-        return np.zeros(container.AtomPositionManager.atomCount)
 
-    def plot_displacement(self, data_displacement, output_path:str=None, save:bool=True, verbose:bool=True):
-        """
-        Plot the displacement of atoms.
-
-        Args:
-            data_displacement (numpy.ndarray): Displacement data to plot.
-            save (bool, optional): Whether to save the plot as an image. Defaults to True.
-            verbose (bool, optional): Enable verbose output. Defaults to True.
-        """
         for u in self.containers[0].AtomPositionManager.uniqueAtomLabels:
-            mask = self.containers[0].AtomPositionManager.atomLabelsList == u
-
-            fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12, 6))
-            color = self.containers[0].AtomPositionManager.element_colors[u]
-
-            ax1.plot(data_displacement[:, mask], color=color, alpha=0.3, lw=0.5)
-            self.setup_subplot(ax1, 'Time', 'Displacements', f'Displacements for {u}')
-
-            avg_displacement = np.mean(data_displacement[:, mask], axis=0)
-            var_displacement = np.var(data_displacement[:, mask], axis=0)
-            avg_displacement = self._calculate_reference_values(self.containers[0], 'c')[mask]
-            ax2.plot(var_displacement, avg_displacement, 'o', label='Average', color=color)
-            self.setup_subplot(ax2, 'Variance', 'Average', f'Average and Variance for {u}')
-
-            plt.tight_layout()
+            images = []
+            #for file_name in sorted(os.listdir(file_location)):
+                #if file_name.endswith(('.png', '.jpg', '.jpeg', '.bmp', '.gif')):
+            for container_i, container in enumerate(self.containers):
+                file_path = f'MD_RBF/{container_i}/RBF_{u}.png'
+                images.append(imageio.imread(file_path))
+        
             if save:
-                plt.savefig(f'{output_path}/displacements_{u}.png', dpi=100)
-
-            plt.clf()
-
-            if verbose:
-                print(f' >> Plot :: displacements ({u}) - data shape {data_displacement.shape}')
+                imageio.mimsave( f'MD_RBF{u}.gif', images, duration=duration)
 
     def plot_count(self, count_dict, output_path:str=None, save:bool=True, verbose:bool=True ):
         diferent_species = set()
         for c in count_dict:
             for specie in c:
                 diferent_species.add(specie) 
         diferent_species = list(diferent_species)
@@ -394,15 +483,14 @@
 
         # Adding gridlines
         plt.grid(True, linestyle='--', alpha=0.7)
 
         # Fine-tuning axes
         plt.xticks(fontsize=10)
         plt.yticks(fontsize=10)
-        plt.xlim([0, len(specie_count_frame[0]) - 1])  # Adjust according to your data
         plt.ylim([0, np.max(specie_count_frame) + 1])  # Adjust according to your data
 
         plt.tight_layout()
         if save:
             plt.savefig(f'{output_path}/count_plot.png', dpi=100)
         plt.clf()
 
@@ -540,46 +628,14 @@
                 data_y=data_y, 
                 data_color=(0.2, 0.2, 0.2), 
                 data_label='E', data_output_path=output_path, data_max=np.max(data_x)*1.2, data_min=np.min(data_x)*0.8)
         if verbose:
             print(f' >> Plot :: Evaluation E - data shape: {data["E"]["train"].shape}')
             print(f' >> Plot :: Error Distribution E - data shape: {error.shape}')
 
-    def animated_RBF(self, output_path:str=None, duration:float=0.1, save:bool=True, verbose:bool=True):
-        """
-
-        """
-
-        for u in self.containers[0].AtomPositionManager.uniqueAtomLabels:
-            images = []
-            #for file_name in sorted(os.listdir(file_location)):
-                #if file_name.endswith(('.png', '.jpg', '.jpeg', '.bmp', '.gif')):
-            for container_i, container in enumerate(self.containers):
-                file_path = f'MD_RBF/{container_i}/RBF_{u}.png'
-                images.append(imageio.imread(file_path))
-        
-            if save:
-                imageio.mimsave( f'MD_RBF{u}.gif', images, duration=duration)
-
-    @staticmethod
-    def setup_subplot(ax, xlabel, ylabel, title):
-        """
-        Set up the subplot with labels and title.
-
-        Args:
-            ax (matplotlib.axes.Axes): The axes object to setup.
-            xlabel (str): Label for the x-axis.
-            ylabel (str): Label for the y-axis.
-            title (str): Title of the subplot.
-        """
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
-        ax.set_title(title)
-        #ax.legend(loc='upper right')
-
     def plot_bond_tracking(self, bond_tracking_dict, output_path:str=None, window_size:float=None, save:bool=True, verbose:bool=True):
         
         def moving_average_std(x_values, z_value, mean_x, window_size):
             """Calculate moving average and moving standard deviation."""
             # Create bins based on the range of X values and the desired window size
             bins = np.arange(min(mean_x)-window_size/2, max(mean_x) + window_size, window_size)
             bin_indices = np.digitize(mean_x, bins)  # Assign each x to a bin
@@ -644,34 +700,38 @@
             # Legend
             plt.legend()
 
             #Show plot
             if save:
                 plt.savefig(f'{output_path}/bond_tracking_{n}_plot.png', dpi=100)
 
-    def handleMDAnalysis(self, values:list, file_location:str=None):
+
+    def handleMDAnalysis(self, values:list ):
         """
         Handle molecular dynamics analysis based on specified values.
 
         Args:
             values (list): List of analysis types to perform.
-            file_location (str, optional): File location for output data.
         """
         MDA_data = {}
 
         for plot in values:
-            if plot.upper() == 'DISPLACEMENTS':
-                MDA_data['displacement'] = self.get_displacement(reference=values[plot].get('reference', None))
-                self.plot_displacement( data_displacement=MDA_data['displacement'], output_path=values[plot].get('output_path', '.'), verbose=values[plot].get('verbose', False) )
+
+            if plot.upper() == 'PATH_TRACKING':
+                MDA_data['positions'] = self.get_positions( fractional=values[plot].get('reference', False)=='fractional', wrap=values[plot].get('wrap', False) )
+                self.plot_path( positions=MDA_data['positions'], output_path=values[plot].get('output_path', '.'), transparency=values[plot].get('transparency', False), 
+                                wrap=values[plot].get('wrap', False), verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'RBF':
+                # RADIAL basis function
                 MDA_data['RBF'] = self.plot_RBF()
                 self.animated_RBF( output_path=values[plot].get('output_path', '.'), duration=0.1, save=True, verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'COUNT_SPECIES':
+                #  
                 MDA_data['count'] = self.get_count_species(sigma=values[plot].get('sigma', None))
                 self.plot_count( count_dict=MDA_data['count'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'EVALUATE_FF':
                 MDA_data['evaluation'] = self.get_evaluation(
                                                     ff_energy_tag=values[plot].get('ff_energy_tag', 'ff-energy'),
                                                     ff_forces_tag=values[plot].get('ff_forces_tag', 'ff-forces'),
@@ -679,153 +739,10 @@
                 self.plot_evaluation(data=MDA_data['evaluation'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'BOND_DISTANCE_TRACKING':
                 MDA_data['bond_tracking'] = self.get_bond_tracking(sigma=values[plot].get('sigma', None), reference=values[plot].get('reference', None))
                 self.plot_bond_tracking( bond_tracking_dict=MDA_data['bond_tracking'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'MOLECULE_FORMATION_TRACKING':
-                MDA_data['molecule_formation_tracking'] = self.get_molecular_graph_tracking(sigma=values[plot].get('sigma', None))
-                #self.plot_bond_tracking( bond_tracking_dict=MDA_data['bond_tracking'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
-
-                #self.plot_count( count_dict=MDA_data['count'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
-
-
-
-'''
-import numpy as np
-import ase.io
-from ase.build import bulk
-from dscribe.descriptors import LMBTR
-
-# Lets create iron in BCC phase
-n_z = 8
-n_xy_bcc = 10
-a_bcc = 2.866
-bcc = bulk("Fe", "bcc", a=a_bcc, cubic=True) * [n_xy_bcc, n_xy_bcc, n_z]
-
-# Lets create iron in FCC phase
-a_fcc = 3.5825
-n_xy_fcc = 8
-fcc = bulk("Fe", "fcc", a=a_fcc, cubic=True) * [n_xy_fcc, n_xy_fcc, n_z]
-
-# Setting up the descriptor
-descriptor = LMBTR(
-    grid={"min": 0, "max": 12, "sigma": 0.1, "n": 200},
-    geometry={"function": "distance"},
-    weighting={"function": "exp", "scale": 0.5, "threshold": 1e-3},
-    species=["Fe"],
-    periodic=True,
-)
-
-# Calculate feature references
-bcc_features = descriptor.create(bcc, [0])
-fcc_features = descriptor.create(fcc, [0])
-
-# Combine into one large grain boundary system with some added noise
-bcc.translate([0, 0, n_z * a_fcc])
-combined = bcc + fcc
-combined.set_cell([
-    n_xy_bcc * a_bcc,
-    n_xy_bcc * a_bcc,
-    n_z * (a_bcc + a_fcc)
-])
-combined.rattle(0.1, seed=7)
-
-# Create a measure of of how similar the atoms are to the reference. Euclidean
-# distance is used and the values are scaled between 0 and 1 from least similar
-# to identical with reference.
-def metric(values, reference):
-    dist = np.linalg.norm(values - reference, axis=1)
-    dist_max = np.max(dist)
-    return  1 - (dist / dist_max)
-
-# Create the features and metrics for all atoms in the sample.
-combined_features = descriptor.create(combined)
-fcc_metric = metric(combined_features, fcc_features)
-bcc_metric = metric(combined_features, bcc_features)
-
-# Write an image with the atoms coloured corresponding to their similarity with
-# BCC and FCC: BCC = blue, FCC = red
-n_atoms = len(combined)
-colors = np.zeros((n_atoms, 3))
-for i in range(n_atoms):
-    colors[i] = [fcc_metric[i], 0, bcc_metric[i]]
-ase.io.write(
-    f'coloured.png',
-    combined,
-    rotation='90x,20y,20x',
-    colors=colors,
-    show_unit_cell=1,
-    maxwidth=2000,
-)
-
-
-asdf
-
-import numpy as np
-from sklearn.cluster import KMeans
-from sklearn.decomposition import PCA
-import matplotlib.pyplot as plt
-
-
-
-
-def aplicar_pca_y_clasificar(datos, n_componentes=2):
-    """
-    Aplica PCA a los datos proporcionados y clasifica en el número especificado de componentes principales.
-
-    :param datos: Array de numpy con los datos (espectros de potencia).
-    :param n_componentes: Número de componentes principales para clasificar.
-    :return: Datos transformados y modelo PCA.
-    """
-
-    # Crear una instancia de PCA
-    pca = PCA(n_components=n_componentes)
-
-    # Ajustar y transformar los datos
-    datos_transformados = pca.fit_transform(datos)
-
-    # Opcional: Visualizar los resultados
-    plt.figure(figsize=(8, 6))
-    if n_componentes == 2:
-        plt.scatter(datos_transformados[:, 0], datos_transformados[:, 1])
-        plt.xlabel('Componente Principal 1')
-        plt.ylabel('Componente Principal 2')
-    elif n_componentes > 2:
-        from mpl_toolkits.mplot3d import Axes3D
-        ax = plt.figure().gca(projection='3d')
-        ax.scatter(datos_transformados[:, 0], datos_transformados[:, 1], datos_transformados[:, 2])
-        ax.set_xlabel('Componente Principal 1')
-        ax.set_ylabel('Componente Principal 2')
-        ax.set_zlabel('Componente Principal 3')
-    plt.title('PCA de los Espectros de Potencia')
-    plt.show()
-
-    return datos_transformados, pca
-
-
-# Supongamos que tienes tus datos en un array de numpy, donde cada fila es una observación (p. ej., posición de un átomo 'O' en un instante)
-# y cada columna es una característica (p. ej., coordenadas x, y, z).
-datos = np.random.rand(100,10)  # Reemplaza esto con tus datos reales
-aplicar_pca_y_clasificar(datos)
-
-# Definir el número de clusters
-n_clusters = 3  # Ajusta esto según tus necesidades
-
-# Aplicar k-means
-kmeans = KMeans(n_clusters=n_clusters)
-kmeans.fit(datos)
-
-# Etiquetas de los clusters
-etiquetas = kmeans.labels_
-
-# Centroides de los clusters (pueden ser útiles para entender qué caracteriza a cada cluster)
-centroides = kmeans.cluster_centers_
-
-# Visualizar los resultados (opcional, pero útil)
-plt.scatter(datos[:, 0], datos[:, 1], c=etiquetas, cmap='viridis')
-plt.scatter(centroides[:, 0], centroides[:, 1], c='red', marker='X')
-plt.title('Clustering de datos de dinámica molecular')
-plt.xlabel('Coordenada X')
-plt.ylabel('Coordenada Y')
-plt.show()
-'''
+                container_list = MDA_data['molecule_formation_tracking'] = self.get_molecular_graph_tracking( sigma=values[plot].get('sigma', None), pattern=self.str_to_connectivity(values[plot].get('topology', None)) )
+                self.containers = [ c for c_i, c in enumerate(self.containers) if c_i in container_list]
+
```

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 try:
     from sage_lib.partition.PartitionManager import PartitionManager
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing PartitionManager: {str(e)}\n")
     del sys
 
+try:
+    import numpy as np
+except ImportError as e:
+    import sys
+    sys.stderr.write(f"An error occurred while importing numpy: {str(e)}\n")
+    del sys
+
 class PositionEditor_builder(PartitionManager):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         super().__init__(name=name, file_location=file_location)
         
-    def handleRattle(self, container, values, container_index, file_location=None):
-        sub_directories, containers = [], []
+    def handleRattle(self, values, file_location=None):
+        containers = []
 
-        for v in values: 
-            for n in range(v['N']):
-                for std in v['std']:
-                    container_copy = self.copy_and_update_container(container, f'/rattle/{std}/{n}', file_location)
-                    container_copy.AtomPositionManager.rattle(stdev=std, seed=n)
-                    
-                    sub_directories.append(f'{std}/{n}')
-                    containers.append(container_copy)
+        for container_index, container in enumerate(self.containers):
+            for n in range(values['N']):
+                container_copy = self.copy_and_update_container(container, f'/rattle/{container_index}_{n}', file_location)
+                container_copy.AtomPositionManager.rattle(stdev=values['std'], seed=n)
+
+                containers.append(container_copy)
         
-        self.generate_execution_script_for_each_container(sub_directories, container.file_location + '/rattle')
-        return containers
+        self.containers = containers 
 
+        return containers
 
     def handleCompress(self, container, values, container_index, file_location=None):
         sub_directories, containers = [], []
 
         compress_vector = self.interpolate_vectors(values['compress_min'], values['compress_max'], values['N'])
 
         for v_i, v in enumerate(compress_vector): 
             container_copy = self.copy_and_update_container(container, f'/compress/{v_i}', file_location)
             container_copy.AtomPositionManager.compress(compress_factor=v, verbose=False)
                 
             sub_directories.append(f'/{v_i}')
             containers.append(container_copy)
     
-        self.generate_execution_script_for_each_container(sub_directories, container.file_location + '/compress')
         return containers
 
     def handleWidening(self, values, file_location=None):
         sub_directories, containers = [], []
 
         for v_i, v in enumerate(values): 
             container_init = self.containers[ v['init_index'] ]
@@ -53,9 +57,35 @@
             for n in range(v['N']):
                 container_copy.AtomPositionManager.stack(AtomPositionManager=container_mid.AtomPositionManager, direction=v['direction'] )
             container_copy.AtomPositionManager.stack(AtomPositionManager=container_end.AtomPositionManager, direction=v['direction'] )
 
             sub_directories.append(f'/{v_i}')
             containers.append(container_copy)
     
-        #self.generate_execution_script_for_each_container(sub_directories, container.file_location + '/widening')
+        return containers
+
+    def handleInterpolation(self, values, file_location=None):
+        '''
+        '''
+        interpolation_data = np.zeros((self.containers[0].AtomPositionManager.atomCount, 3, len(self.containers) ), dtype=np.float64)
+
+        for container_index, container in enumerate(self.containers):
+            if values.get('first_neighbor', False): container.AtomPositionManager.wrap()
+            interpolation_data[:,:,container_index] = container.AtomPositionManager.atomPositions_fractional
+
+        if values.get('first_neighbor', False):
+            diff = np.diff(interpolation_data, axis=2)
+            interpolation_data[:,:,1:][diff > 0.5] -= 1
+            interpolation_data[:,:,1:][diff < -0.5] += 1
+
+        new_interpolated_data = self.interpolate_with_splines(interpolation_data, M=values['images'], degree=values['degree'])
+
+        containers = [ self.copy_and_update_container(self.containers[0], f'/interpolation/init', file_location) ]
+        for container_index, container in enumerate(self.containers[1:]):
+            for n in range(values['images']+1):
+                container_copy = self.copy_and_update_container(container, f'/interpolation/{container_index}_{n}', file_location)
+                container_copy.AtomPositionManager.set_atomPositions_fractional( new_interpolated_data[:,:,container_index*(values['images']+1) + n + 1] ) 
+                if values.get('first_neighbor', False): container_copy.AtomPositionManager.wrap()
+                containers.append( container_copy )
+        self.containers = containers
+
         return containers
```

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

