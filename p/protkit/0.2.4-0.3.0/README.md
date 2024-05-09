# Comparing `tmp/protkit-0.2.4.tar.gz` & `tmp/protkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protkit-0.2.4.tar", last modified: Tue Apr 23 13:51:15 2024, max compression
+gzip compressed data, was "protkit-0.3.0.tar", last modified: Thu May  9 13:47:13 2024, max compression
```

## Comparing `protkit-0.2.4.tar` & `protkit-0.3.0.tar`

### file list

```diff
@@ -1,101 +1,107 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.163340 protkit-0.2.4/
--rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.2.4/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)    18964 2024-04-23 13:51:15.163340 protkit-0.2.4/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.2.4/README.md
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/
--rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.2.4/protkit/__init__.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/core/
--rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.2.4/protkit/core/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.2.4/protkit/core/extend_attributes.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/download/
--rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.2.4/protkit/download/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12986 2024-03-11 08:37:40.000000 protkit-0.2.4/protkit/download/download.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/file_io/
--rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/file_io/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3870 2024-03-11 10:09:24.000000 protkit-0.2.4/protkit/file_io/fasta_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/file_io/mmcif_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/file_io/mmtf_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    49366 2024-04-23 09:40:38.000000 protkit-0.2.4/protkit/file_io/pdb_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/file_io/pqr_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/file_io/prot_io.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/geometry/
--rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.2.4/protkit/geometry/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.2.4/protkit/geometry/math.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.2.4/protkit/geometry/space_query.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/protkit/metrics/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.2.4/protkit/metrics/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.2.4/protkit/metrics/classification_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.2.4/protkit/metrics/regression_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.2.4/protkit/metrics/scoring_matrix.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.2.4/protkit/metrics/sequence_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.2.4/protkit/metrics/structure_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.2.4/protkit/metrics/utility_eval.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/protkit/properties/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-04-11 09:05:09.000000 protkit-0.2.4/protkit/properties/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.2.4/protkit/properties/bond_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.2.4/protkit/properties/bond_lengths.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.2.4/protkit/properties/bounds.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.2.4/protkit/properties/charge.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.2.4/protkit/properties/chemical_class.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.2.4/protkit/properties/circular_variance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.2.4/protkit/properties/dihedral_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.2.4/protkit/properties/donors_acceptors.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.2.4/protkit/properties/hydrophobicity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.2.4/protkit/properties/interface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.2.4/protkit/properties/mass.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.2.4/protkit/properties/polarity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4290 2024-04-11 11:55:05.000000 protkit-0.2.4/protkit/properties/surface_area.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.2.4/protkit/properties/vdw_radius.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.2.4/protkit/properties/volume.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/protkit/seq/
--rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.2.4/protkit/seq/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/seq/antibody_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/seq/nucleotide_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/seq/protein_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5710 2024-03-11 10:00:59.000000 protkit-0.2.4/protkit/seq/sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.2.4/protkit/seq/sequence_alignment.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/protkit/structure/
--rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.2.4/protkit/structure/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    13382 2024-04-12 10:30:44.000000 protkit-0.2.4/protkit/structure/atom.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20258 2024-04-23 07:17:33.000000 protkit-0.2.4/protkit/structure/chain.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.2.4/protkit/structure/protein.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20645 2024-03-06 15:24:06.000000 protkit-0.2.4/protkit/structure/residue.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/protkit/tasks/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-04-03 08:07:09.000000 protkit-0.2.4/protkit/tasks/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1369 2024-03-08 13:46:26.000000 protkit-0.2.4/protkit/tasks/protonator.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.2.4/protkit/tasks/surface_area_calculator.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/protkit/tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      344 2024-04-17 09:52:59.000000 protkit-0.2.4/protkit/tools/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.2.4/protkit/tools/freesasa_adaptor.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5488 2024-04-11 08:41:57.000000 protkit-0.2.4/protkit/tools/pdb2pqr_adaptor.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4462 2024-04-23 09:55:42.000000 protkit-0.2.4/protkit/tools/propka_adaptor.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8569 2024-04-03 07:58:04.000000 protkit-0.2.4/protkit/tools/reduce_adaptor.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.163340 protkit-0.2.4/protkit.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)    18964 2024-04-23 13:51:15.000000 protkit-0.2.4/protkit.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     2363 2024-04-23 13:51:15.000000 protkit-0.2.4/protkit.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-04-23 13:51:15.000000 protkit-0.2.4/protkit.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      189 2024-04-23 13:51:15.000000 protkit-0.2.4/protkit.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       45 2024-04-23 13:51:15.000000 protkit-0.2.4/protkit.egg-info/top_level.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)     1377 2024-04-23 13:20:47.000000 protkit-0.2.4/pyproject.toml
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-04-23 13:51:15.163340 protkit-0.2.4/setup.cfg
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.159340 protkit-0.2.4/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)    23316 2024-04-11 12:12:53.000000 protkit-0.2.4/tests/quick_start_guide.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      192 2024-04-12 10:25:26.000000 protkit-0.2.4/tests/test_occupancy_claudio.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      638 2024-04-10 12:06:45.000000 protkit-0.2.4/tests/test_pdb2pqr.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      586 2024-04-23 09:44:20.000000 protkit-0.2.4/tests/test_propka.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      565 2024-04-10 08:46:58.000000 protkit-0.2.4/tests/test_reduce.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.155340 protkit-0.2.4/venv/
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-23 13:51:15.163340 protkit-0.2.4/venv/bin/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.2.4/venv/bin/activate_this.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      612 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2html.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      732 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2html4.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)     1100 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2html5.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      809 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2latex.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      617 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2man.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      782 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2odt.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)     1744 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      619 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      655 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2s5.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      889 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2xetex.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      620 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rst2xml.py
--rwxrwxr-x   0 fred      (1000) fred      (1000)      688 2024-04-03 10:09:30.000000 protkit-0.2.4/venv/bin/rstpep2html.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:13.001497 protkit-0.3.0/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.3.0/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)    18993 2024-05-09 13:47:13.001497 protkit-0.3.0/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.3.0/README.md
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.981497 protkit-0.3.0/protkit/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.3.0/protkit/__init__.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.981497 protkit-0.3.0/protkit/core/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.3.0/protkit/core/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.3.0/protkit/core/extend_attributes.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.981497 protkit-0.3.0/protkit/download/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.3.0/protkit/download/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12986 2024-03-11 08:37:40.000000 protkit-0.3.0/protkit/download/download.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.985498 protkit-0.3.0/protkit/file_io/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/file_io/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3870 2024-03-11 10:09:24.000000 protkit-0.3.0/protkit/file_io/fasta_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/file_io/mmcif_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/file_io/mmtf_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    49366 2024-04-23 09:40:38.000000 protkit-0.3.0/protkit/file_io/pdb_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/file_io/pqr_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/file_io/prot_io.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.985498 protkit-0.3.0/protkit/geometry/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.3.0/protkit/geometry/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.3.0/protkit/geometry/math.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.3.0/protkit/geometry/space_query.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.985498 protkit-0.3.0/protkit/metrics/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.3.0/protkit/metrics/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.3.0/protkit/metrics/classification_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.3.0/protkit/metrics/regression_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.3.0/protkit/metrics/scoring_matrix.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.3.0/protkit/metrics/sequence_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.3.0/protkit/metrics/structure_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.3.0/protkit/metrics/utility_eval.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.985498 protkit-0.3.0/protkit/ml/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      299 2024-05-07 13:00:55.000000 protkit-0.3.0/protkit/ml/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11753 2024-05-09 13:41:43.000000 protkit-0.3.0/protkit/ml/dataframe.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.989498 protkit-0.3.0/protkit/properties/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-04-11 09:05:09.000000 protkit-0.3.0/protkit/properties/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.3.0/protkit/properties/bond_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.3.0/protkit/properties/bond_lengths.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.3.0/protkit/properties/bounds.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.3.0/protkit/properties/charge.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.3.0/protkit/properties/chemical_class.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.3.0/protkit/properties/circular_variance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.3.0/protkit/properties/dihedral_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.3.0/protkit/properties/donors_acceptors.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.3.0/protkit/properties/hydrophobicity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.3.0/protkit/properties/interface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.3.0/protkit/properties/mass.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.3.0/protkit/properties/polarity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4290 2024-04-11 11:55:05.000000 protkit-0.3.0/protkit/properties/surface_area.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.3.0/protkit/properties/vdw_radius.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.3.0/protkit/properties/volume.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.993497 protkit-0.3.0/protkit/seq/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.3.0/protkit/seq/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/seq/antibody_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/seq/nucleotide_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/seq/protein_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5710 2024-03-11 10:00:59.000000 protkit-0.3.0/protkit/seq/sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.3.0/protkit/seq/sequence_alignment.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.993497 protkit-0.3.0/protkit/structure/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.3.0/protkit/structure/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    14756 2024-05-08 09:12:29.000000 protkit-0.3.0/protkit/structure/atom.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20521 2024-05-08 09:17:33.000000 protkit-0.3.0/protkit/structure/chain.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.3.0/protkit/structure/protein.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    21470 2024-05-08 09:16:31.000000 protkit-0.3.0/protkit/structure/residue.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.993497 protkit-0.3.0/protkit/tasks/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-04-03 08:07:09.000000 protkit-0.3.0/protkit/tasks/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1369 2024-03-08 13:46:26.000000 protkit-0.3.0/protkit/tasks/protonator.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.3.0/protkit/tasks/surface_area_calculator.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.993497 protkit-0.3.0/protkit/tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      344 2024-04-17 09:52:59.000000 protkit-0.3.0/protkit/tools/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      354 2024-04-24 08:16:28.000000 protkit-0.3.0/protkit/tools/abnumber_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.3.0/protkit/tools/freesasa_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5488 2024-04-11 08:41:57.000000 protkit-0.3.0/protkit/tools/pdb2pqr_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4462 2024-04-23 09:55:42.000000 protkit-0.3.0/protkit/tools/propka_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8569 2024-04-03 07:58:04.000000 protkit-0.3.0/protkit/tools/reduce_adaptor.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:13.001497 protkit-0.3.0/protkit.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)    18993 2024-05-09 13:47:12.000000 protkit-0.3.0/protkit.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     2493 2024-05-09 13:47:12.000000 protkit-0.3.0/protkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-05-09 13:47:12.000000 protkit-0.3.0/protkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      203 2024-05-09 13:47:12.000000 protkit-0.3.0/protkit.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       45 2024-05-09 13:47:12.000000 protkit-0.3.0/protkit.egg-info/top_level.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1398 2024-05-09 13:43:50.000000 protkit-0.3.0/pyproject.toml
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-05-09 13:47:13.001497 protkit-0.3.0/setup.cfg
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.997497 protkit-0.3.0/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    25200 2024-05-09 13:33:10.000000 protkit-0.3.0/tests/quick_start_guide.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      229 2024-04-30 08:07:51.000000 protkit-0.3.0/tests/test_biopandas.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1981 2024-05-09 13:25:23.000000 protkit-0.3.0/tests/test_featurizer.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      192 2024-04-12 10:25:26.000000 protkit-0.3.0/tests/test_occupancy_claudio.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      638 2024-04-10 12:06:45.000000 protkit-0.3.0/tests/test_pdb2pqr.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      586 2024-04-23 09:44:20.000000 protkit-0.3.0/tests/test_propka.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      565 2024-04-10 08:46:58.000000 protkit-0.3.0/tests/test_reduce.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.981497 protkit-0.3.0/venv/
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-05-09 13:47:12.997497 protkit-0.3.0/venv/bin/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.3.0/venv/bin/activate_this.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      612 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2html.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      732 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2html4.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)     1100 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2html5.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      809 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2latex.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      617 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2man.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      782 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2odt.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)     1744 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      619 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      655 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2s5.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      889 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      620 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rst2xml.py
+-rwxrwxr-x   0 fred      (1000) fred      (1000)      688 2024-04-03 10:09:30.000000 protkit-0.3.0/venv/bin/rstpep2html.py
```

### Comparing `protkit-0.2.4/LICENSE` & `protkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/PKG-INFO` & `protkit-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.4
+Version: 0.3.0
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
@@ -19,14 +19,15 @@
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: biopython>=1.83
 Requires-Dist: mmtf-python>=1.1.3
 Requires-Dist: freesasa>=2.2.1
 Requires-Dist: pdb2pqr>=3.6.2
 Requires-Dist: propka>=3.5.1
+Requires-Dist: pandas>=2.2.2
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: setuptools>=61.0; extra == "dev"
 
 <p align="center">
     <!--img src="media/logo/protkit800px.png" width="400"-->
     <img src="https://raw.githubusercontent.com/silicogenesis/protkit/main/media/logo/protkit800px.png" width="400px">
```

### Comparing `protkit-0.2.4/README.md` & `protkit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/__init__.py` & `protkit-0.3.0/protkit/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/core/extend_attributes.py` & `protkit-0.3.0/protkit/core/extend_attributes.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/download/download.py` & `protkit-0.3.0/protkit/download/download.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/__init__.py` & `protkit-0.3.0/protkit/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/fasta_io.py` & `protkit-0.3.0/protkit/file_io/fasta_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/mmcif_io.py` & `protkit-0.3.0/protkit/file_io/mmcif_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/mmtf_io.py` & `protkit-0.3.0/protkit/file_io/mmtf_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/pdb_io.py` & `protkit-0.3.0/protkit/file_io/pdb_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/pqr_io.py` & `protkit-0.3.0/protkit/file_io/pqr_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/file_io/prot_io.py` & `protkit-0.3.0/protkit/file_io/prot_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/geometry/math.py` & `protkit-0.3.0/protkit/geometry/math.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/geometry/space_query.py` & `protkit-0.3.0/protkit/geometry/space_query.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/metrics/__init__.py` & `protkit-0.3.0/protkit/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/metrics/scoring_matrix.py` & `protkit-0.3.0/protkit/metrics/scoring_matrix.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/metrics/sequence_eval.py` & `protkit-0.3.0/protkit/metrics/sequence_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/metrics/structure_eval.py` & `protkit-0.3.0/protkit/metrics/structure_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/__init__.py` & `protkit-0.3.0/protkit/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/bond_angles.py` & `protkit-0.3.0/protkit/properties/bond_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/bond_lengths.py` & `protkit-0.3.0/protkit/properties/bond_lengths.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/bounds.py` & `protkit-0.3.0/protkit/properties/bounds.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/charge.py` & `protkit-0.3.0/protkit/properties/charge.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/chemical_class.py` & `protkit-0.3.0/protkit/properties/chemical_class.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/circular_variance.py` & `protkit-0.3.0/protkit/properties/circular_variance.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/dihedral_angles.py` & `protkit-0.3.0/protkit/properties/dihedral_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/donors_acceptors.py` & `protkit-0.3.0/protkit/properties/donors_acceptors.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/hydrophobicity.py` & `protkit-0.3.0/protkit/properties/hydrophobicity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/interface.py` & `protkit-0.3.0/protkit/properties/interface.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/mass.py` & `protkit-0.3.0/protkit/properties/mass.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/polarity.py` & `protkit-0.3.0/protkit/properties/polarity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/surface_area.py` & `protkit-0.3.0/protkit/properties/surface_area.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/vdw_radius.py` & `protkit-0.3.0/protkit/properties/vdw_radius.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/properties/volume.py` & `protkit-0.3.0/protkit/properties/volume.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/__init__.py` & `protkit-0.3.0/protkit/seq/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/antibody_sequence.py` & `protkit-0.3.0/protkit/seq/antibody_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/nucleotide_sequence.py` & `protkit-0.3.0/protkit/seq/nucleotide_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/protein_sequence.py` & `protkit-0.3.0/protkit/seq/protein_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/sequence.py` & `protkit-0.3.0/protkit/seq/sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/seq/sequence_alignment.py` & `protkit-0.3.0/protkit/seq/sequence_alignment.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/structure/__init__.py` & `protkit-0.3.0/protkit/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/structure/atom.py` & `protkit-0.3.0/protkit/structure/atom.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Any
 from copy import deepcopy
 
 if TYPE_CHECKING:
     from protkit.structure.residue import Residue
+    from protkit.structure.chain import Chain
+    from protkit.structure.protein import Protein
 
 
 class Atom:
     # ------------------------------------------------------------
     # Constructor
     # ------------------------------------------------------------
     def __init__(self,
@@ -299,17 +301,21 @@
         Returns:
             bool: The disordered flag.
 
         """
         return self._is_disordered
 
     # ------------------------------------------------------------
-    # Methods for managing the atom's residue
+    # Methods for managing the atom's residue, chain or protein
     # - residue (property)
     # - residue (setter)
+    # - chain (property)
+    # - chain_id (property)
+    # - protein (property)
+    # - pdb_id (property)
     # ------------------------------------------------------------
 
     @property
     def residue(self) -> Optional[Residue]:
         """
         Returns the residue the atom forms part of.
 
@@ -327,14 +333,58 @@
             residue (Residue): The residue the atom forms part of.
 
         Returns:
             None
         """
         self._residue = residue
 
+    @property
+    def chain(self) -> Optional[Chain]:
+        """
+        Returns the chain the atom forms part of.
+
+        Returns:
+            Optional[Chain]: The chain the atom forms part of.
+        """
+        if self._residue is not None:
+            return self._residue.chain
+
+    @property
+    def chain_id(self) -> Optional[str]:
+        """
+        Returns the chain ID the atom forms part of.
+
+        Returns:
+            Optional[str]: The chain ID the atom forms part of.
+        """
+        if self.chain is not None:
+            return self.chain.chain_id
+
+    @property
+    def protein(self) -> Optional[Protein]:
+        """
+        Returns the protein the atom forms part of.
+
+        Returns:
+            Optional[Protein]: The protein the atom forms part of.
+        """
+        if self.chain is not None:
+            return self.chain.protein
+
+    @property
+    def pdb_id(self) -> Optional[str]:
+        """
+        Returns the PDB ID the atom forms part of.
+
+        Returns:
+            Optional[str]: The PDB ID the atom forms part of.
+        """
+        if self.protein is not None:
+            return self.protein.pdb_id
+
     # ------------------------------------------------------------
     # Disordered state
     # - merge_disordered_atom
     # - fix_disordered_atom
     # ------------------------------------------------------------
 
     def merge_disordered_atom(self, atom: Atom) -> None:
```

### Comparing `protkit-0.2.4/protkit/structure/chain.py` & `protkit-0.3.0/protkit/structure/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         sequence = "".join(sequence)
         return sequence
 
     # ------------------------------------------------------------
     # Methods for managing the chain's protein.
     # - protein (property)
     # - protein (setter)
+    # - pdb_id (property)
     # ------------------------------------------------------------
 
     @property
     def protein(self) -> Protein:
         """
         Returns the chain's protein.
 
@@ -144,14 +145,25 @@
             protein (Protein): The chain's protein.
 
         Returns:
             None
         """
         self._protein = protein
 
+    @property
+    def pdb_id(self) -> str:
+        """
+        Returns the chain's PDB ID.
+
+        Returns:
+            str: The chain's PDB ID.
+        """
+        if self._protein is not None:
+            return self._protein.pdb_id
+
     # ------------------------------------------------------------
     # Methods for managing the chain's residues.
     # Create
     # - add_residue
     # Read
     # - residues (property, iterator)
     # - num_residues (property)
```

### Comparing `protkit-0.2.4/protkit/structure/protein.py` & `protkit-0.3.0/protkit/structure/protein.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/structure/residue.py` & `protkit-0.3.0/protkit/structure/residue.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Dict, List, Set, TYPE_CHECKING, Optional, Any, Iterator
 from copy import deepcopy
 
 from protkit.structure.atom import Atom
 
 if TYPE_CHECKING:
     from protkit.structure.chain import Chain
+    from protkit.structure.protein import Protein
 
 
 class Residue:
     HEAVY_ATOMS = {
         "ALA": {"N", "CA", "C", "O", "CB"},
         "ARG": {"N", "CA", "C", "O", "CB", "CG", "CD", "NE", "CZ", "NH1", "NH2"},
         "ASN": {"N", "CA", "C", "O", "CB", "CG", "OD1", "ND2"},
@@ -293,17 +294,20 @@
         """
         if self._residue_type not in Residue.SHORT_CODE:
             raise Exception("Residue type {self._residue_type} not found in Residue.SHORT_CODE.")
 
         return Residue.SHORT_CODE[self._residue_type]
 
     # ------------------------------------------------------------
-    # Methods for managing the residue's chain.
+    # Methods for managing the residue's chain and protein
     # - chain (property)
     # - chain (setter)
+    # - chain_id (property)
+    # - protein (property)
+    # - pdb_id (property)
     # ------------------------------------------------------------
 
     @property
     def chain(self) -> Chain:
         """
         Returns the residue's chain.
 
@@ -321,14 +325,47 @@
             chain (Chain): The residue's chain.
 
         Returns:
             None
         """
         self._chain = chain
 
+    @property
+    def chain_id(self) -> str:
+        """
+        Returns the chain ID.
+
+        Returns:
+            str: The chain ID.
+        """
+        if self._chain is not None:
+            return self._chain.chain_id
+
+    @property
+    def protein(self) -> Protein:
+        """
+        Returns the protein.
+
+        Returns:
+            Protein: The protein.
+        """
+        if self._chain is not None:
+            return self._chain.protein
+
+    @property
+    def pdb_id(self) -> Optional[str]:
+        """
+        Returns the PDB ID.
+
+        Returns:
+            str: The PDB ID.
+        """
+        if self.protein is not None:
+            return self.protein.pdb_id
+
     # ------------------------------------------------------------
     # Methods for managing the residue's atoms.
     # Create
     # - add_atom
     # Read
     # - atoms (property, iterator)
     # - num_atoms (property)
```

### Comparing `protkit-0.2.4/protkit/tasks/protonator.py` & `protkit-0.3.0/protkit/tasks/protonator.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/tasks/surface_area_calculator.py` & `protkit-0.3.0/protkit/tasks/surface_area_calculator.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/tools/freesasa_adaptor.py` & `protkit-0.3.0/protkit/tools/freesasa_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/tools/pdb2pqr_adaptor.py` & `protkit-0.3.0/protkit/tools/pdb2pqr_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/tools/propka_adaptor.py` & `protkit-0.3.0/protkit/tools/propka_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit/tools/reduce_adaptor.py` & `protkit-0.3.0/protkit/tools/reduce_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/protkit.egg-info/PKG-INFO` & `protkit-0.3.0/protkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.4
+Version: 0.3.0
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
@@ -19,14 +19,15 @@
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: biopython>=1.83
 Requires-Dist: mmtf-python>=1.1.3
 Requires-Dist: freesasa>=2.2.1
 Requires-Dist: pdb2pqr>=3.6.2
 Requires-Dist: propka>=3.5.1
+Requires-Dist: pandas>=2.2.2
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: setuptools>=61.0; extra == "dev"
 
 <p align="center">
     <!--img src="media/logo/protkit800px.png" width="400"-->
     <img src="https://raw.githubusercontent.com/silicogenesis/protkit/main/media/logo/protkit800px.png" width="400px">
```

### Comparing `protkit-0.2.4/protkit.egg-info/SOURCES.txt` & `protkit-0.3.0/protkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 protkit/metrics/__init__.py
 protkit/metrics/classification_eval.py
 protkit/metrics/regression_eval.py
 protkit/metrics/scoring_matrix.py
 protkit/metrics/sequence_eval.py
 protkit/metrics/structure_eval.py
 protkit/metrics/utility_eval.py
+protkit/ml/__init__.py
+protkit/ml/dataframe.py
 protkit/properties/__init__.py
 protkit/properties/bond_angles.py
 protkit/properties/bond_lengths.py
 protkit/properties/bounds.py
 protkit/properties/charge.py
 protkit/properties/chemical_class.py
 protkit/properties/circular_variance.py
@@ -55,19 +57,22 @@
 protkit/structure/chain.py
 protkit/structure/protein.py
 protkit/structure/residue.py
 protkit/tasks/__init__.py
 protkit/tasks/protonator.py
 protkit/tasks/surface_area_calculator.py
 protkit/tools/__init__.py
+protkit/tools/abnumber_adaptor.py
 protkit/tools/freesasa_adaptor.py
 protkit/tools/pdb2pqr_adaptor.py
 protkit/tools/propka_adaptor.py
 protkit/tools/reduce_adaptor.py
 tests/quick_start_guide.py
+tests/test_biopandas.py
+tests/test_featurizer.py
 tests/test_occupancy_claudio.py
 tests/test_pdb2pqr.py
 tests/test_propka.py
 tests/test_reduce.py
 venv/bin/activate_this.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
```

### Comparing `protkit-0.2.4/pyproject.toml` & `protkit-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package-dir = "protkit"
 
 [tool.setuptools.packages]
 find = {}
 
 [project]
 name = "protkit"
-version = "0.2.4"
+version = "0.3.0"
 requires-python = ">=3.6"
 authors = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
 maintainers = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
@@ -31,14 +31,15 @@
     "numpy>=1.20.3",
     "scikit-learn>=1.4.1.post1",
     "biopython>=1.83",
     "mmtf-python>=1.1.3",
     "freesasa>=2.2.1",
     "pdb2pqr>=3.6.2",
     "propka>=3.5.1",
+    "pandas>=2.2.2",
 ]
 keywords = ["protein", "protein engineering", "structural biology", "computational biology", "biology", "bioinformatics", "sequence", "amino acid", "residue", "dataset", "PDB", "antibody", "antibody engineering", "cdr"]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=6.2.5",
     "setuptools>=61.0",
```

### Comparing `protkit-0.2.4/tests/quick_start_guide.py` & `protkit-0.3.0/tests/quick_start_guide.py`

 * *Files 4% similar despite different names*

```diff
@@ -681,37 +681,91 @@
     protein = ProtIO.load("1ahw.prot")[0]
 
     atoms = list(protein.atoms)
     atom_areas = freesasa.calculate_surface_area(atoms)
     protein_area = sum(atom_areas)
     print(protein_area)
 
+def ml_dataframe():
+    from protkit.file_io import ProtIO
+    from protkit.ml import ProteinToDataframe
 
-# prep_data()
+    featurizer = ProteinToDataframe()
+    protein = ProtIO.load("1ahw.prot")[0]
+    protein.pdb_id = "1ahw"
+
+    df_chains = featurizer.chains_dataframe(protein)
+    df_residues = featurizer.residues_dataframe(protein)
+    df_atoms = featurizer.atoms_dataframe(protein)
+
+    print(df_atoms.head())
+
+def ml_dataframe2():
+    from protkit.file_io import ProtIO
+    from protkit.ml import ProteinToDataframe
 
-quick_start_example()
+    featurizer = ProteinToDataframe()
+    protein1 = ProtIO.load("1ahw.prot")[0]
+    protein1.pdb_id = "1ahw"
+    protein2 = ProtIO.load("3i40.prot")[0]
+    protein2.pdb_id = "3i40"
 
-download_pdb_example()
-download_fasta_example()
-download_cif_example()
-
-properties_hydrophobicity()
-properties_hydrophobicity_class()
-properties_mass()
-properties_chemical_class()
-properties_charge()
-properties_polarity()
-properties_donors_acceptors()
-properties_surface_area()
-properties_volume()
-properties_volume_class()
-properties_bounds_and_center()
-properties_bond_lengths()
-properties_peptide_lengths()
-properties_bond_angles()
-properties_dihedral_angles()
-properties_circular_variance()  # -> double check first residue
-# properties_interface_atoms()
-# properties_interface_residues()
+    df_proteins = featurizer.proteins_dataframe([protein1, protein2])
+
+    print(df_proteins.head())
+
+def ml_dataframe3():
+    from protkit.file_io import ProtIO
+    from protkit.ml import ProteinToDataframe
+    from protkit.properties import SurfaceArea, Hydrophobicity, Mass
+
+    featurizer = ProteinToDataframe()
+    protein = ProtIO.load("1ahw.prot")[0]
+    protein.pdb_id = "1ahw"
 
-tools_reduce()
-tools_freesasa()
+    # Assign additional properties to the protein
+    SurfaceArea.surface_area_of_protein(protein, assign_attribute=True)
+    Hydrophobicity.hydrophobicity_of_protein(protein, assign_attribute=True)
+    Mass.residue_mass_of_protein(protein, assign_attribute=True)
+
+    # Create a DataFrame for the residues of the protein
+    df_residues_all = featurizer.residues_dataframe(protein)
+    df_residues_none = featurizer.residues_dataframe(protein, additional_fields=[])
+    df_residues_specific = featurizer.residues_dataframe(protein, additional_fields=["surface_area", "hydrophobicity"])
+
+    print(df_residues_all.head())
+    print(df_residues_none.head())
+    print(df_residues_specific.head())
+
+# # prep_data()
+#
+# quick_start_example()
+#
+# download_pdb_example()
+# download_fasta_example()
+# download_cif_example()
+#
+# properties_hydrophobicity()
+# properties_hydrophobicity_class()
+# properties_mass()
+# properties_chemical_class()
+# properties_charge()
+# properties_polarity()
+# properties_donors_acceptors()
+# properties_surface_area()
+# properties_volume()
+# properties_volume_class()
+# properties_bounds_and_center()
+# properties_bond_lengths()
+# properties_peptide_lengths()
+# properties_bond_angles()
+# properties_dihedral_angles()
+# properties_circular_variance()  # -> double check first residue
+# # properties_interface_atoms()
+# # properties_interface_residues()
+#
+# tools_reduce()
+# tools_freesasa()
+
+# ml_dataframe()
+# ml_dataframe2()
+ml_dataframe3()
```

### Comparing `protkit-0.2.4/tests/test_pdb2pqr.py` & `protkit-0.3.0/tests/test_pdb2pqr.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/tests/test_propka.py` & `protkit-0.3.0/tests/test_propka.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/tests/test_reduce.py` & `protkit-0.3.0/tests/test_reduce.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/activate_this.py` & `protkit-0.3.0/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2html.py` & `protkit-0.3.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2html4.py` & `protkit-0.3.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2html5.py` & `protkit-0.3.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2latex.py` & `protkit-0.3.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2man.py` & `protkit-0.3.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2odt.py` & `protkit-0.3.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2odt_prepstyles.py` & `protkit-0.3.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2pseudoxml.py` & `protkit-0.3.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2s5.py` & `protkit-0.3.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2xetex.py` & `protkit-0.3.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rst2xml.py` & `protkit-0.3.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.4/venv/bin/rstpep2html.py` & `protkit-0.3.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

