# Comparing `tmp/spit-0.2.1.tar.gz` & `tmp/spit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spit-0.2.1.tar", last modified: Thu May  9 04:41:44 2024, max compression
+gzip compressed data, was "dist/spit-0.2.2.tar", last modified: Thu May  9 04:43:32 2024, max compression
```

## Comparing `spit-0.2.1.tar` & `spit-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:41:44.000000 spit-0.2.1/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-22 00:49:28.000000 spit-0.2.1/LICENSE
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-22 00:49:28.000000 spit-0.2.1/MANIFEST.in
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:41:44.000000 spit-0.2.1/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-22 00:49:28.000000 spit-0.2.1/README.md
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2024-05-09 04:41:44.000000 spit-0.2.1/setup.cfg
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2024-05-09 04:41:37.000000 spit-0.2.1/setup.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:41:44.000000 spit-0.2.1/spit/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.1/spit/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-22 00:49:28.000000 spit-0.2.1/spit/cluster_samples.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-22 00:49:28.000000 spit-0.2.1/spit/confounding_analysis.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    12927 2024-04-25 05:59:48.000000 spit-0.2.1/spit/dtu_detection.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-22 00:49:28.000000 spit-0.2.1/spit/filter_and_transform_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-22 00:49:28.000000 spit-0.2.1/spit/get_p_cutoff.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1723 2023-12-22 00:49:28.000000 spit-0.2.1/spit/import_infreps.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:41:44.000000 spit-0.2.1/spit/parameter_fitting/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4563 2024-04-25 01:46:05.000000 spit-0.2.1/spit/parameter_fitting/LOOCV.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.1/spit/parameter_fitting/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-22 00:49:28.000000 spit-0.2.1/spit/parameter_fitting/filter_and_simulate_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     7033 2024-04-14 19:07:27.000000 spit-0.2.1/spit/parameter_fitting/simulate_dtu_exp.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4713 2024-04-25 01:36:00.000000 spit-0.2.1/spit/plot_spit_charts.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:41:44.000000 spit-0.2.1/spit/r_scripts/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3254 2024-03-12 02:48:44.000000 spit-0.2.1/spit/r_scripts/hclust.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-22 00:49:28.000000 spit-0.2.1/spit/r_scripts/tximport_quant_files.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    13286 2024-05-09 04:41:20.000000 spit-0.2.1/spit/run_spit.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2024-02-25 23:55:54.000000 spit-0.2.1/spit/spit_test.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-22 00:49:28.000000 spit-0.2.1/spit/transform_tx_counts_to_ifs.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/SOURCES.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/dependency_links.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       45 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/entry_points.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/requires.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2024-05-09 04:41:44.000000 spit-0.2.1/spit.egg-info/top_level.txt
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:43:32.000000 spit-0.2.2/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-22 00:49:28.000000 spit-0.2.2/LICENSE
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-22 00:49:28.000000 spit-0.2.2/MANIFEST.in
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:43:32.000000 spit-0.2.2/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-22 00:49:28.000000 spit-0.2.2/README.md
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2024-05-09 04:43:32.000000 spit-0.2.2/setup.cfg
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2024-05-09 04:43:21.000000 spit-0.2.2/setup.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:43:32.000000 spit-0.2.2/spit/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.2/spit/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-22 00:49:28.000000 spit-0.2.2/spit/cluster_samples.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-22 00:49:28.000000 spit-0.2.2/spit/confounding_analysis.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    12927 2024-04-25 05:59:48.000000 spit-0.2.2/spit/dtu_detection.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-22 00:49:28.000000 spit-0.2.2/spit/filter_and_transform_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-22 00:49:28.000000 spit-0.2.2/spit/get_p_cutoff.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1723 2023-12-22 00:49:28.000000 spit-0.2.2/spit/import_infreps.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:43:32.000000 spit-0.2.2/spit/parameter_fitting/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4563 2024-04-25 01:46:05.000000 spit-0.2.2/spit/parameter_fitting/LOOCV.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.2/spit/parameter_fitting/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-22 00:49:28.000000 spit-0.2.2/spit/parameter_fitting/filter_and_simulate_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     7033 2024-04-14 19:07:27.000000 spit-0.2.2/spit/parameter_fitting/simulate_dtu_exp.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4713 2024-04-25 01:36:00.000000 spit-0.2.2/spit/plot_spit_charts.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:43:32.000000 spit-0.2.2/spit/r_scripts/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3254 2024-03-12 02:48:44.000000 spit-0.2.2/spit/r_scripts/hclust.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-22 00:49:28.000000 spit-0.2.2/spit/r_scripts/tximport_quant_files.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    13290 2024-05-09 04:43:00.000000 spit-0.2.2/spit/run_spit.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2024-02-25 23:55:54.000000 spit-0.2.2/spit/spit_test.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-22 00:49:28.000000 spit-0.2.2/spit/transform_tx_counts_to_ifs.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/SOURCES.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/dependency_links.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       45 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/entry_points.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/requires.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2024-05-09 04:43:32.000000 spit-0.2.2/spit.egg-info/top_level.txt
```

### Comparing `spit-0.2.1/LICENSE` & `spit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/README.md` & `spit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/setup.py` & `spit-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='spit',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'matplotlib>=3.4.3',
         'matplotlib_venn>=0.11.6',
         'numpy>=1.20.3',
         'pandas>=1.3.4',
```

### Comparing `spit-0.2.1/spit/cluster_samples.py` & `spit-0.2.2/spit/cluster_samples.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/confounding_analysis.py` & `spit-0.2.2/spit/confounding_analysis.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/dtu_detection.py` & `spit-0.2.2/spit/dtu_detection.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/filter_and_transform_tx_counts.py` & `spit-0.2.2/spit/filter_and_transform_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/get_p_cutoff.py` & `spit-0.2.2/spit/get_p_cutoff.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/import_infreps.py` & `spit-0.2.2/spit/import_infreps.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/parameter_fitting/LOOCV.py` & `spit-0.2.2/spit/parameter_fitting/LOOCV.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/parameter_fitting/filter_and_simulate_tx_counts.py` & `spit-0.2.2/spit/parameter_fitting/filter_and_simulate_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/parameter_fitting/simulate_dtu_exp.py` & `spit-0.2.2/spit/parameter_fitting/simulate_dtu_exp.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/plot_spit_charts.py` & `spit-0.2.2/spit/plot_spit_charts.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/r_scripts/hclust.R` & `spit-0.2.2/spit/r_scripts/hclust.R`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/r_scripts/tximport_quant_files.R` & `spit-0.2.2/spit/r_scripts/tximport_quant_files.R`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/run_spit.py` & `spit-0.2.2/spit/run_spit.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
 
 def main(argv=None):
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
     subparsers = parser.add_subparsers(help='Available SPIT functions')
     # Filter subcommand
-    parser_filter = subparsers.add_parser('preprocess', help='Apply pre-filtering on transcript counts and generate isoform fractions. For specific parameters, run "spit filter -h".')
+    parser_filter = subparsers.add_parser('preprocess', help='Apply pre-filtering on transcript counts and generate isoform fractions. For specific parameters, run "spit preprocess -h".')
     handle_shared_args(parser_filter)
     parser_filter.add_argument('-w', '--write', action='store_true', help='Write the number of transcripts & genes left after each filtering step to stdout.')
     parser_filter.add_argument('--keep_all_nonzeros', action='store_true', help='If used, this options skips all SPIT prefiltering steps and only removes transcripts that do not have any non-zero counts in any sample. Any other filtering argument becomes irrelevant.')
     parser_filter.add_argument('-p', '--pr_fraction', metavar='0.2', type=float, default=0.2, help='Each transcript must have a positive read count in at least a fraction p_r of the samples in both the case and control groups.')
     parser_filter.add_argument('-f', '--if_fraction', metavar='0.1', type=float, default=0.1, help='Each transcript must have an IF value larger than f in at least n_small samples.')
     parser_filter.add_argument('-c', '--genefilter_count', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
     parser_filter.add_argument('-s', '--genefilter_sample', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
```

### Comparing `spit-0.2.1/spit/spit_test.py` & `spit-0.2.2/spit/spit_test.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit/transform_tx_counts_to_ifs.py` & `spit-0.2.2/spit/transform_tx_counts_to_ifs.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.1/spit.egg-info/SOURCES.txt` & `spit-0.2.2/spit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

