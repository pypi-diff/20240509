# Comparing `tmp/spit-0.1.9.tar.gz` & `tmp/spit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/berilerdogdu/Desktop/SPIT/dist/.tmp-es5ve703/spit-0.1.9.tar", last modified: Sun Dec 17 20:10:03 2023, max compression
+gzip compressed data, was "dist/spit-0.2.0.tar", last modified: Thu May  9 04:39:30 2024, max compression
```

## Comparing `spit-0.1.9.tar` & `spit-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-17 20:03:44.000000 spit-0.1.9/LICENSE
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-17 20:03:44.000000 spit-0.1.9/MANIFEST.in
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-17 20:10:03.000000 spit-0.1.9/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-17 20:03:44.000000 spit-0.1.9/README.md
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2023-12-17 20:10:03.000000 spit-0.1.9/setup.cfg
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2023-12-17 20:09:12.000000 spit-0.1.9/setup.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:03:44.000000 spit-0.1.9/spit/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-17 20:03:44.000000 spit-0.1.9/spit/cluster_samples.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-17 20:03:44.000000 spit-0.1.9/spit/confounding_analysis.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    12799 2023-12-17 20:03:44.000000 spit-0.1.9/spit/dtu_detection.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-17 20:03:44.000000 spit-0.1.9/spit/filter_and_transform_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-17 20:03:44.000000 spit-0.1.9/spit/get_p_cutoff.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1545 2023-12-17 20:03:44.000000 spit-0.1.9/spit/import_infreps.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/parameter_fitting/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4482 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/LOOCV.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/filter_and_simulate_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6779 2023-12-17 20:03:44.000000 spit-0.1.9/spit/parameter_fitting/simulate_dtu_exp.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4786 2023-12-17 20:03:44.000000 spit-0.1.9/spit/plot_spit_charts.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit/r_scripts/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3251 2023-12-17 20:03:44.000000 spit-0.1.9/spit/r_scripts/hclust.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-17 20:03:44.000000 spit-0.1.9/spit/r_scripts/tximport_quant_files.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    11991 2023-12-17 20:03:44.000000 spit-0.1.9/spit/run_spit.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2023-12-17 20:03:44.000000 spit-0.1.9/spit/spit_test.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-17 20:03:44.000000 spit-0.1.9/spit/transform_tx_counts_to_ifs.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       93 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/SOURCES.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/dependency_links.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       44 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/entry_points.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/requires.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2023-12-17 20:10:03.000000 spit-0.1.9/spit.egg-info/top_level.txt
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:39:30.000000 spit-0.2.0/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-22 00:49:28.000000 spit-0.2.0/LICENSE
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-22 00:49:28.000000 spit-0.2.0/MANIFEST.in
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:39:30.000000 spit-0.2.0/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-22 00:49:28.000000 spit-0.2.0/README.md
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2024-05-09 04:39:30.000000 spit-0.2.0/setup.cfg
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2024-05-09 04:38:48.000000 spit-0.2.0/setup.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:39:30.000000 spit-0.2.0/spit/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.0/spit/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-22 00:49:28.000000 spit-0.2.0/spit/cluster_samples.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-22 00:49:28.000000 spit-0.2.0/spit/confounding_analysis.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    12927 2024-04-25 05:59:48.000000 spit-0.2.0/spit/dtu_detection.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-22 00:49:28.000000 spit-0.2.0/spit/filter_and_transform_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-22 00:49:28.000000 spit-0.2.0/spit/get_p_cutoff.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1723 2023-12-22 00:49:28.000000 spit-0.2.0/spit/import_infreps.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:39:30.000000 spit-0.2.0/spit/parameter_fitting/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4563 2024-04-25 01:46:05.000000 spit-0.2.0/spit/parameter_fitting/LOOCV.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.0/spit/parameter_fitting/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-22 00:49:28.000000 spit-0.2.0/spit/parameter_fitting/filter_and_simulate_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     7033 2024-04-14 19:07:27.000000 spit-0.2.0/spit/parameter_fitting/simulate_dtu_exp.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4713 2024-04-25 01:36:00.000000 spit-0.2.0/spit/plot_spit_charts.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:39:30.000000 spit-0.2.0/spit/r_scripts/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3254 2024-03-12 02:48:44.000000 spit-0.2.0/spit/r_scripts/hclust.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-22 00:49:28.000000 spit-0.2.0/spit/r_scripts/tximport_quant_files.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    13293 2024-05-09 04:38:00.000000 spit-0.2.0/spit/run_spit.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2024-02-25 23:55:54.000000 spit-0.2.0/spit/spit_test.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-22 00:49:28.000000 spit-0.2.0/spit/transform_tx_counts_to_ifs.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/SOURCES.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/dependency_links.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       45 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/entry_points.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/requires.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2024-05-09 04:39:30.000000 spit-0.2.0/spit.egg-info/top_level.txt
```

### Comparing `spit-0.1.9/LICENSE` & `spit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/README.md` & `spit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/setup.py` & `spit-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='spit',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'matplotlib>=3.4.3',
         'matplotlib_venn>=0.11.6',
         'numpy>=1.20.3',
         'pandas>=1.3.4',
```

### Comparing `spit-0.1.9/spit/cluster_samples.py` & `spit-0.2.0/spit/cluster_samples.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/confounding_analysis.py` & `spit-0.2.0/spit/confounding_analysis.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/dtu_detection.py` & `spit-0.2.0/spit/dtu_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,14 @@
     pheno = pd.read_csv(args.l, sep='\t')
     ctrl_samples = pheno[pheno.condition == 0].id.to_list()
     case_samples = pheno[pheno.condition == 1].id.to_list()
     likelihood_arr, wrst_p_arr, genotype_cluster_df = compute_double_stats(IFs, gene_counts, tx2gene_dict, ctrl_samples, case_samples, args.n_small, args.p_cutoff, args.bandwidth, args.f_cpm)
     mad_scores = MADsfromMedian(likelihood_arr)
     likelihood_cutoff = filter_likelihood_on_mad(likelihood_arr, mad_scores)
     wrst_pos_genes, flagged_genes = find_and_flag_dtu_genes(IFs, likelihood_arr, likelihood_cutoff, wrst_p_arr, args.p_cutoff)
-    pd.DataFrame(wrst_p_arr, index = IFs.index, columns = ['p_value']).to_csv(os.path.join(args.O, "SPIT_analysis", "all_p_values.txt"), sep = '\t')
     if(args.infReps):
         all_samples = pheno.id.to_list()
         infReps = []
         for i in all_samples:
             infReps_dir = os.path.join(args.O, "SPIT_analysis", "infReps", "tximport_infReps_sample_" + i + ".txt")
             infReps_sample = pd.read_csv(infReps_dir, sep = '\t', index_col = 0)
             infReps_sample = infReps_sample.loc[IFs.index.to_list()].to_numpy()
@@ -246,13 +245,14 @@
         dtu_genes_stable, flagged_genes_stable = get_stable_dtu(num_of_infReps, infReps_dtu_genes, infReps_flagged_genes, wrst_pos_genes, flagged_genes)
         wrst_pos_genes = dtu_genes_stable
         flagged_genes = flagged_genes_stable
     if(args.exp):
         write_dir = args.exp
         write_final_results(wrst_pos_genes, flagged_genes, os.path.join(write_dir, "spit_out_k" + str(round(args.k, 1)) + ".b" + str(format(args.bandwidth, '.2f')) + ".txt"))
         genotype_cluster_df.to_csv(os.path.join(write_dir, "spit_cluster_matrix_k"+ str(round(args.k, 1)) + ".b" + str(format(args.bandwidth, '.2f')) + ".txt"), sep = '\t')
+        pd.DataFrame(wrst_p_arr, index = IFs.index, columns = ['p_value']).to_csv(os.path.join(write_dir, "all_p_values.txt"), sep = '\t')
     else:
         write_dir = os.path.join(args.O, "SPIT_analysis")
         write_final_results(wrst_pos_genes, flagged_genes, os.path.join(write_dir, "spit_out.txt"))
         genotype_cluster_df.to_csv(os.path.join(write_dir, "spit_cluster_matrix.txt"), sep = '\t')
-
+        pd.DataFrame(wrst_p_arr, index = IFs.index, columns = ['p_value']).to_csv(os.path.join(write_dir, "all_p_values.txt"), sep = '\t')
```

### Comparing `spit-0.1.9/spit/filter_and_transform_tx_counts.py` & `spit-0.2.0/spit/filter_and_transform_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/get_p_cutoff.py` & `spit-0.2.0/spit/get_p_cutoff.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/import_infreps.py` & `spit-0.2.0/spit/import_infreps.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,9 +32,13 @@
     infReps_directory_path = os.path.join(directory_path, "infReps")
     if os.path.exists(infReps_directory_path) == False:
         os.mkdir(infReps_directory_path)
     robjects.r.assign("directory_path", directory_path)
     current_script_dir = os.path.dirname(os.path.abspath(__file__))
     tximport_path = os.path.join(current_script_dir, 'r_scripts/tximport_quant_files.R')
     robjects.r.source(tximport_path)
+    args.l = os.path.join("..", args.l)
+    args.m = os.path.join("..", args.m)
+    args.i = os.path.join("..", args.i)
+    args.quant_path = os.path.join("..", args.quant_path)
     import_infreps = robjects.r['import_infreps']
     import_infreps(args.l, args.m, args.quant_type, args.quant_path, args.i)
```

### Comparing `spit-0.1.9/spit/parameter_fitting/LOOCV.py` & `spit-0.2.0/spit/parameter_fitting/LOOCV.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,19 @@
     pdf_file_path = os.path.join(fit_param_directory_path, "LOOCV_venn_diags.pdf")
     f_prime = 0
     plot_counter = 0
     pdf_pages = PdfPages(pdf_file_path)
     for e_out in exps:
         l_o = e_out
         f_bar_max = 0
-        k_best = 0
-        b_best = 0
+        k_best = 0.1
+        b_best = 0.02
         test_f = 0
-        for b in np.round(np.arange(0.02, 0.21, 0.02), 2):
+        b_search = np.array([1]) if (args.n_splicotypes == 1) else np.round(np.arange(0.02, 0.21, 0.02), 2)
+        for b in b_search:
             b = format(b, '.2f')
             for k in np.round(np.arange(0.1, 1, 0.1), 1):
                 f_bar = 0
                 for e_in in exps:
                     if e_in is not l_o:
                         dtu_genes = exp_dtu_genes_dict[e_in]
                         spit_cluster_arr = pd.read_csv(os.path.join(fit_param_directory_path, e_in, "spit_cluster_matrix_k" + str(k) + ".b" + str(b) + ".txt"), sep='\t', index_col=0)
```

### Comparing `spit-0.1.9/spit/parameter_fitting/filter_and_simulate_tx_counts.py` & `spit-0.2.0/spit/parameter_fitting/filter_and_simulate_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/parameter_fitting/simulate_dtu_exp.py` & `spit-0.2.0/spit/parameter_fitting/simulate_dtu_exp.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,37 @@
 import pandas as pd
 import warnings
 import random
 import math
 from collections import defaultdict
 
 
-def select_dtu_genes(IFs, ctrl_samples, gene_names):
-    pot_dtu_genes = random.sample(gene_names, 1000)
+def select_dtu_genes(IFs, ctrl_samples, gene_names, n_splicotypes, n_dtu_genes, p_dom):
+    pot_dtu_genes = gene_names
     dtu_IFs = IFs[IFs.gene_id.isin(pot_dtu_genes)]
     dtu_IFs.insert(0, "ctrl_IF_mean", dtu_IFs[ctrl_samples].mean(axis = 1))
     ctrl_IF_max = dtu_IFs.sort_values('ctrl_IF_mean', ascending=False).drop_duplicates(['gene_id'])
     ctrl_IF_no_max = dtu_IFs.drop(ctrl_IF_max.index)
     ctrl_IF_second_max = ctrl_IF_no_max.sort_values('ctrl_IF_mean', ascending=False).drop_duplicates(['gene_id'])
     ctrl_IF_min = dtu_IFs.sort_values('ctrl_IF_mean', ascending=True).drop_duplicates(['gene_id'])
     dtu_gene_counter = 0
     final_dtu_genes = set()
+    if(n_splicotypes > 1):
+        target_dtu_gene_n = (n_splicotypes-1)*n_dtu_genes
+    else:
+        target_dtu_gene_n = n_dtu_genes
     for g in pot_dtu_genes:
-        if(dtu_gene_counter == 100):
+        if(dtu_gene_counter == target_dtu_gene_n):
             return list(final_dtu_genes)
         min_if = ctrl_IF_min[ctrl_IF_min.gene_id == g].ctrl_IF_mean
         min_iso = ctrl_IF_min[ctrl_IF_min.gene_id == g].index
         max_if = ctrl_IF_max[ctrl_IF_max.gene_id == g].ctrl_IF_mean
         max_iso = ctrl_IF_max[ctrl_IF_max.gene_id == g].index
         second_max_iso = ctrl_IF_second_max[ctrl_IF_second_max.gene_id == g].index
-        if(np.sum(dtu_IFs.loc[max_iso, ctrl_samples].to_numpy() > dtu_IFs.loc[second_max_iso, ctrl_samples].to_numpy()) < (len(ctrl_samples) * 0.75
+        if(np.sum(dtu_IFs.loc[max_iso, ctrl_samples].to_numpy() > dtu_IFs.loc[second_max_iso, ctrl_samples].to_numpy()) < (len(ctrl_samples) * p_dom
         )):
             pass
         else:
             final_dtu_genes.add(g)
             dtu_gene_counter += 1
             
     return list(final_dtu_genes)
@@ -52,23 +56,23 @@
             genotype_sample_dict[genotype].append(i)
         for i in range(1, n_of_genotypes+1):
             genotype_samples = genotype_sample_dict[i]
             if(len(genotype_samples) < n_small):
                 val_sample_size = False
         c+=1
 
-def simulate_dtu(IFs, dtu_genes, ctrl_samples, case_samples, n_of_genotypes, n_small):
+def simulate_dtu(IFs, dtu_genes, ctrl_samples, case_samples, n_of_genotypes, n_dtu_genes, n_small):
     genotype_gene_dict = defaultdict(list)
     genotype_cluster_df = pd.DataFrame(0, index=IFs.index, columns=IFs.columns)
     dtu_IFs = IFs[IFs.gene_id.isin(dtu_genes)]
     dtu_IFs.insert(0, "ctrl_IF_mean", dtu_IFs[ctrl_samples].mean(axis = 1))
     ctrl_IF_max = dtu_IFs.sort_values('ctrl_IF_mean', ascending=False).drop_duplicates(['gene_id'])
     ctrl_IF_min = dtu_IFs.sort_values('ctrl_IF_mean', ascending=True).drop_duplicates(['gene_id'])
     for i in range(n_of_genotypes+1):
-        genotype_gene_dict[i] = random.sample(dtu_genes, 30)
+        genotype_gene_dict[i] = random.sample(dtu_genes, n_dtu_genes)
     genotype_sample_dict = partition_samples_to_subgroups(case_samples, n_of_genotypes, n_small)
     for i in range(1, n_of_genotypes+1):
         genotype_samples = genotype_sample_dict[i]
         for g in genotype_gene_dict[i]:
             min_if = ctrl_IF_min[ctrl_IF_min.gene_id == g].ctrl_IF_mean
             min_iso = ctrl_IF_min[ctrl_IF_min.gene_id == g].index
             max_if = ctrl_IF_max[ctrl_IF_max.gene_id == g].ctrl_IF_mean
@@ -120,15 +124,15 @@
     with open(case_file) as case_file:
         case_samples = [line.strip() for line in case_file]
     all_ids = ctrl_samples + case_samples
     sim_pheno_condition = [0 for i in range(len(ctrl_samples))] + [1 for i in range(len(case_samples))]
     sim_pheno = (pd.DataFrame([all_ids, sim_pheno_condition])).transpose()
     sim_pheno.columns = ['id', 'condition']
     sim_pheno.to_csv(os.path.join(args.exp, 'simulation_pheno.txt'), sep = '\t', index = False)
-    dtu_genes = select_dtu_genes(IFs, ctrl_samples, gene_names)
-    simulated_dtu_ifs, genotype_cluster_df = simulate_dtu(IFs, dtu_genes, ctrl_samples, case_samples, args.n_splicotypes, args.n_small)
+    dtu_genes = select_dtu_genes(IFs, ctrl_samples, gene_names, args.n_splicotypes, args.n_dtu_genes, args.p_dom)
+    simulated_dtu_ifs, genotype_cluster_df = simulate_dtu(IFs, dtu_genes, ctrl_samples, case_samples, args.n_splicotypes, args.n_dtu_genes, args.n_small)
     simulated_dtu_counts = recreate_tx_counts_matrix(simulated_dtu_ifs, gene_level_counts, all_ids)
     corrected_IFs, corrected_gene_level_counts = convert_counts_to_IF_and_gene_level(simulated_dtu_counts)
     corrected_IFs.to_csv(os.path.join(args.exp, 'simulated_ifs.txt'), sep = '\t')
     simulated_dtu_counts.to_csv(os.path.join(args.exp, 'simulated_tx_counts.txt'), sep = '\t')
     corrected_gene_level_counts.to_csv(os.path.join(args.exp, 'simulated_gene_counts.txt'), sep = '\t')
     genotype_cluster_df.drop(columns=['gene_id']).to_csv(os.path.join(args.exp, 'true_cluster_matrix.txt'), sep = '\t')
```

### Comparing `spit-0.1.9/spit/plot_spit_charts.py` & `spit-0.2.0/spit/plot_spit_charts.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,26 +60,25 @@
     ctrl_ids = pheno_df[pheno_df.condition == 0].id.to_list()
     ifs = pd.read_csv(args.i, sep = '\t', index_col = 0)
     confounding_controlled, orig_matrix = check_confounding_control(args.O)
     if(confounding_controlled):
         clm_dtu = pd.read_csv(confounding_controlled, sep = '\t', index_col = 0)
     else:
         clm_dtu = pd.read_csv(orig_matrix, sep = '\t', index_col = 0)
-    sig_tx_ids = clm_dtu.index.to_list()
+    sig_tx_ids = clm_dtu[clm_dtu.any(axis = 1)].index.to_list()
     for i in tqdm(sig_tx_ids):
         spit_v = clm_dtu.loc[i]
         dtu_plus = spit_v.index[(spit_v == 1)]
         df_index = ctrl_ids + dtu_plus.to_list()
         df_class = ["Ctrl" for i in range(len(ctrl_ids))] + ["DTU+" for i in range(len(dtu_plus))]
         df_if = ifs.loc[i][ctrl_ids].to_list() + ifs.loc[i][dtu_plus].to_list()
         tx_df = pd.DataFrame({'sample': df_index, 'group': df_class, 'IF':df_if})
         custom_palette = ["darkgreen", "pink"]
         sns.set_palette(custom_palette)
-        sns.violinplot(data=tx_df, x="IF", y="group", hue="group", fontdict = { 'fontsize': 30})
-        plt.legend(loc="center right", bbox_to_anchor=(1.3, 0.5))
+        sns.violinplot(data=tx_df, x="IF", y="group", hue="group")
         plt.title(i + " - Isoform Fraction Violin Plots", size = 10, pad = 10)
         plt.savefig(os.path.join(args.O, "SPIT_analysis", "violin_plots", i+".png"))
         plt.close()
     return
         
 def main(args):
     matplotlib.use('Agg')
```

### Comparing `spit-0.1.9/spit/r_scripts/hclust.R` & `spit-0.2.0/spit/r_scripts/hclust.R`

 * *Files 4% similar despite different names*

```diff
@@ -60,13 +60,13 @@
     density.info = 'none',
     key.xtickfun = function() {
         breaks <- parent.frame()$breaks
         return(list(
         at = parent.frame()$scale01(c(breaks[1], breaks[length(breaks)])),
         labels = c(as.character(breaks[1]), as.character(breaks[length(breaks)]))
         ))
-    },
-    key.par=list(mgp=c(0.5, 0.5, 0),
-    mar=c(pdf_h-3, pdf_w/5, pdf_h-3, pdf_w/5)),
-    main = "Dendrogram of Case Samples Based on DTU Events Detected by SPIT")
+    })
+    #key.par=list(mgp=c(0.5, 0.5, 0),
+    #mar=c(pdf_h-3, pdf_w/5, pdf_h-3, pdf_w/5)),
+    #main = "Dendrogram of Case Samples Based on DTU Events Detected by SPIT")
     dev.off()
 }
```

### Comparing `spit-0.1.9/spit/r_scripts/tximport_quant_files.R` & `spit-0.2.0/spit/r_scripts/tximport_quant_files.R`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/run_spit.py` & `spit-0.2.0/spit/run_spit.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,19 +18,32 @@
 
 
 def handle_shared_args(parser):
     parser._optionals.title = 'Command-line arguments:'
     parser.add_argument('-i', metavar='tx_counts.txt', type=str, required=True, help='Transcript level counts file (tsv)')
     parser.add_argument('-m', metavar='tx2gene.txt', type=str, required=True, help='Transcript to gene mapping file (tsv)')
     parser.add_argument('-l', metavar='labels.txt', type=str, required=True, help='Labels/metadata file (tsv)')
+    parser_filter.add_argument('--no_clusters', action='store_true', help='Assume case samples do not form clusters/subgroups.  "n_small" will be overwritten to the higher value of either 0.75 times the case group size or 12 for filtering purposes.')
     parser.add_argument('--n_small', metavar='12', type=int, default=12, help='Smallest sample size for the subgroups')
     parser.add_argument('-O', metavar='/path/', type=str, default=os.getcwd(), help="Output directory path where the SPIT output folder will be written")
     return
+
+def set_no_cluster_nsmall(args):
+    pheno = pd.read_csv(label_file, sep = '\t')
+    case_sample_size = (pheno.condition == 1).sum()
+    n_small_ = int(case_sample_size*0.75)
+    if(case_sample_size < 12):
+        n_small_ = case_sample_size
+    elif (n_small_ < 12):
+        n_small_ = 12
+    return n_small_
     
 def handle_filter(args):
+    if(args.no_clusters):
+        args.n_small = set_no_cluster_nsmall(args)
     if(args.keep_all_nonzeros):
         transform_counts(args)
     else:
         filter_counts(args)
     
 def handle_dtu(args):
     dominance_filtered_file = os.path.join(args.O, "SPIT_analysis", "dominance_selected_ifs.txt")
@@ -43,14 +56,17 @@
     if(args.infReps):
         if((args.quant_path==None) or (args.quant_type==None)):
             print("Parameters --quant_path and --quant_type are required in order to use infReps.")
             exit(1)
         print("Importing inferential replicates using tximport:")
         import_infreps(args)
     args.exp = False
+    if(args.no_clusters):
+        args.n_small = set_no_cluster_nsmall(args)
+        args.bandwidth = 1
     spit_test(args)
     args.p = os.path.join(args.O, "SPIT_analysis", "spit_test_min_p_values.txt")
     p_cutoff = round(get_p(args), 16)
     args.p_cutoff = p_cutoff
     print("Determined p-value threshold: ", p_cutoff)
     if(p_cutoff > 0.05):
         print("WARNING: Determined p-value threshold is larger than 0.05. In this case we recommend using a simple Mann-Whitney U test instead of using SPIT.")
@@ -74,31 +90,38 @@
     
 def handle_param_fit(args):
     fit_param_directory_path = os.path.join(args.O, "SPIT_analysis", "parameter_fitting")
     if os.path.exists(fit_param_directory_path) == False:
         os.mkdir(fit_param_directory_path)
     initial_ifs = args.i
     initial_pheno = args.l
+    if(args.no_clusters):
+        args.n_splicotypes = 1
     for i in range(1, args.n_exps+1):
         print("--Simulating Experiment No " + str(i))
         args.exp = os.path.join(fit_param_directory_path, 'exp'+str(i))
         os.mkdir(args.exp)
         args.i = initial_ifs
         args.l = initial_pheno
+        if(args.no_clusters):
+            args.n_small = set_no_cluster_nsmall(args)
         fit_param_filter_and_partition(args)
         args.i = os.path.join(args.exp, "filtered_ifs.txt")
         args.g = os.path.join(args.exp, "filtered_gene_counts.txt")
         simulate_exp(args)
         print("Running SPIT-Test on Experiment No " + str(i))
         args.i = os.path.join(args.exp, "simulated_ifs.txt")
         args.g = os.path.join(args.exp, "simulated_gene_counts.txt")
         args.l = os.path.join(args.exp, "simulation_pheno.txt")
         args.infReps = False
+        if(args.no_clusters):
+            args.n_small = set_no_cluster_nsmall(args)
         spit_test(args)
-        for b in np.arange(0.02, 0.21, 0.02):
+        b_search = np.array([1]) if (args.n_splicotypes == 1) else np.arange(0.02, 0.21, 0.02)
+        for b in b_search:
             b = round(b, 2)
             for k in np.arange(0.1, 1, 0.1):
                 k = round(k, 1)
                 print("Detecting DTU on Experiment No " + str(i) + " with bandwidth = " + str(b) + " and k= " + str(k))
                 args.p = os.path.join(args.exp, "spit_test_min_p_values.txt")
                 args.bandwidth = b
                 args.k = k
@@ -116,15 +139,15 @@
 
 
 def main(argv=None):
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
     subparsers = parser.add_subparsers(help='Available SPIT functions')
     # Filter subcommand
-    parser_filter = subparsers.add_parser('filter', help='Apply pre-filtering on transcript counts. For specific parameters, run "spit filter -h".')
+    parser_filter = subparsers.add_parser('preprocess', help='Apply pre-filtering on transcript counts and generate isoform fractions. For specific parameters, run "spit filter -h".')
     handle_shared_args(parser_filter)
     parser_filter.add_argument('-w', '--write', action='store_true', help='Write the number of transcripts & genes left after each filtering step to stdout.')
     parser_filter.add_argument('--keep_all_nonzeros', action='store_true', help='If used, this options skips all SPIT prefiltering steps and only removes transcripts that do not have any non-zero counts in any sample. Any other filtering argument becomes irrelevant.')
     parser_filter.add_argument('-p', '--pr_fraction', metavar='0.2', type=float, default=0.2, help='Each transcript must have a positive read count in at least a fraction p_r of the samples in both the case and control groups.')
     parser_filter.add_argument('-f', '--if_fraction', metavar='0.1', type=float, default=0.1, help='Each transcript must have an IF value larger than f in at least n_small samples.')
     parser_filter.add_argument('-c', '--genefilter_count', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
     parser_filter.add_argument('-s', '--genefilter_sample', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
@@ -135,16 +158,16 @@
     parser_dtu = subparsers.add_parser('dtu', help='Run DTU analysis on transcript abundances. For specific parameters, run "spit dtu -h".')
     handle_shared_args(parser_dtu)
     parser_dtu.add_argument('--n_iter', metavar='100', type=int, default=100, help='Number of iterations')
     parser_dtu.add_argument('-k', metavar='0.6', type=float, default=0.6, help='-K hyperparameter for p-value thresholding')
     parser_dtu.add_argument('--infReps', action='store_true', default=None, help='Use inferential replicates in DTU analysis. Parameters "--quant_path" and "--quant_type" must be specified.')
     parser_dtu.add_argument('--quant_path', metavar='/path/', type=str, default=None, help='Path to the parent output directory of Salmon, kallisto, or other quantification tool compatible with tximport (the directory will contain a folder for each sample).')
     parser_dtu.add_argument('--quant_type', metavar='salmon', type=str, default=None, help='The quantification tool used to generate counts. Options compatible with tximport are "salmon", "sailfish", "alevin", "kallisto", "rsem", and "stringtie".')
-    parser_dtu.add_argument('-b', '--bandwidth', metavar='0.09', type=float, default=0.09, help='choice of bandwidth for kernel density estimation')
-    parser_dtu.add_argument('--f_cpm', action='store_true', help='Apply filter-CPM thresholding')
+    parser_dtu.add_argument('-b', '--bandwidth', metavar='0.09', type=float, default=0.09, help='Choice of bandwidth for kernel density estimation. It will be overwritten and set to 1 if "--no_clusters" option is used.')
+    parser_dtu.add_argument('--f_cpm', action='store_true', help='Apply filtered-CPM thresholding')
     parser_dtu.add_argument('--plot', action='store_true', help='Plot permutation importances')
     parser_dtu.set_defaults(func=handle_dtu)
     
     # Clustering subcommand
     parser_cluster = subparsers.add_parser('cluster', help='Cluster case samples based on detected DTU events. For specific parameters, run "spit cluster -h".')
     parser_cluster.add_argument('-l', metavar='labels.txt', type=str, required=True, help='Labels/metadata file (tsv)')
     parser_cluster.add_argument('-O', metavar='/path/', type=str, default=os.getcwd(), help="Output directory path where the SPIT output folder will be written")
@@ -154,30 +177,30 @@
     parser_cluster.set_defaults(func=handle_clustering)
     
     # Parameter-fitting subcommand
     parser_fit = subparsers.add_parser('fit_parameters', help='Apply parameter-fitting on your dataset (Optional) For specific parameters, run "spit fit_parameters -h".')
     handle_shared_args(parser_fit)
     parser_fit.add_argument('--n_exps', metavar='10', type=int, default=10, help='Number of experiments to simulate.')
     parser_fit.add_argument('--n_splicotypes', metavar='5', type=int, default=5, help='Number of splicotypes (subgroups) to simulate.')
+    parser_fit.add_argument('--n_dtu_genes', metavar='30', type=int, default=30, help='Number of DTU genes to simulate per splicotypes (subgroups).')
     parser_fit.add_argument('-w', '--write', action='store_true', help='Write the number of transcripts & genes left after each filtering step to stdout.')
     parser_fit.add_argument('--keep_all_nonzeros', action='store_true', help='If used, this options skips all SPIT prefiltering steps and only removes transcripts that do not have any non-zero counts in any sample. Any other filtering argument becomes irrelevant.')
     parser_fit.add_argument('-p', '--pr_fraction', metavar='0.2', type=float, default=0.2, help='Each transcript must have a positive read count in at least a fraction p_r of the samples in both the case and control groups.')
     parser_fit.add_argument('-f', '--if_fraction', metavar='0.1', type=float, default=0.1, help='Each transcript must have an IF value larger than f in at least n_small samples.')
     parser_fit.add_argument('-c', '--genefilter_count', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
     parser_fit.add_argument('-s', '--genefilter_sample', metavar='10', type=int, default=10, help='Each gene must have a read count of at least c in at least s samples.')
     parser_fit.add_argument('-d', '--p_dom', metavar='0.75', type=float, default=0.75, help='Dominance selection threshold')
     parser_fit.add_argument('--n_iter', metavar='100', type=int, default=100, help='Number of iterations')
-    parser_fit.add_argument('--f_cpm', action='store_true', help='Apply filter-CPM thresholding')
+    parser_fit.add_argument('--f_cpm', action='store_true', help='Apply filtered-CPM thresholding')
     parser_fit.set_defaults(func=handle_param_fit)
     
-    
 
     args = parser.parse_args()
-    make_output_dir(args.O, args.l)
-    args.func(args)
     if not any(vars(args).values()):
         parser.print_help()
         exit(1)
+    make_output_dir(args.O, args.l)
+    args.func(args)
 
 
 if __name__ == "__main__":
    main(sys.argv[1:])
```

### Comparing `spit-0.1.9/spit/spit_test.py` & `spit-0.2.0/spit/spit_test.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit/transform_tx_counts_to_ifs.py` & `spit-0.2.0/spit/transform_tx_counts_to_ifs.py`

 * *Files identical despite different names*

### Comparing `spit-0.1.9/spit.egg-info/SOURCES.txt` & `spit-0.2.0/spit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

