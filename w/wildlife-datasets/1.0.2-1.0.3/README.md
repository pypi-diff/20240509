# Comparing `tmp/wildlife-datasets-1.0.2.tar.gz` & `tmp/wildlife_datasets-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildlife-datasets-1.0.2.tar", last modified: Wed Feb 28 09:15:17 2024, max compression
+gzip compressed data, was "wildlife_datasets-1.0.3.tar", last modified: Thu May  9 07:58:17 2024, max compression
```

## Comparing `wildlife-datasets-1.0.2.tar` & `wildlife_datasets-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.795935 wildlife-datasets-1.0.2/
--rw-rw-rw-   0        0        0     1110 2024-01-12 06:51:35.000000 wildlife-datasets-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    10523 2024-02-28 09:15:17.794928 wildlife-datasets-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8075 2024-02-28 09:13:03.000000 wildlife-datasets-1.0.2/README.md
--rw-rw-rw-   0        0        0     1670 2024-02-28 09:13:45.000000 wildlife-datasets-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 09:15:17.795935 wildlife-datasets-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.746818 wildlife-datasets-1.0.2/wildlife_datasets/
--rw-rw-rw-   0        0        0      113 2024-01-12 06:51:35.000000 wildlife-datasets-1.0.2/wildlife_datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.766489 wildlife-datasets-1.0.2/wildlife_datasets/analysis/
--rw-rw-rw-   0        0        0      109 2023-02-16 18:10:22.000000 wildlife-datasets-1.0.2/wildlife_datasets/analysis/__init__.py
--rw-rw-rw-   0        0        0     3186 2024-02-28 09:12:57.000000 wildlife-datasets-1.0.2/wildlife_datasets/analysis/plots.py
--rw-rw-rw-   0        0        0     2688 2024-01-12 06:51:35.000000 wildlife-datasets-1.0.2/wildlife_datasets/analysis/statistics.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.766489 wildlife-datasets-1.0.2/wildlife_datasets/datasets/
--rw-rw-rw-   0        0        0     3112 2024-02-28 09:13:03.000000 wildlife-datasets-1.0.2/wildlife_datasets/datasets/__init__.py
--rw-rw-rw-   0        0        0    88324 2024-02-28 09:13:03.000000 wildlife-datasets-1.0.2/wildlife_datasets/datasets/datasets.py
--rw-rw-rw-   0        0        0     8880 2024-02-28 09:13:03.000000 wildlife-datasets-1.0.2/wildlife_datasets/datasets/metadata.csv
--rw-rw-rw-   0        0        0      852 2023-02-16 18:10:22.000000 wildlife-datasets-1.0.2/wildlife_datasets/datasets/metadata.py
--rw-rw-rw-   0        0        0     5178 2024-02-28 09:12:57.000000 wildlife-datasets-1.0.2/wildlife_datasets/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.778133 wildlife-datasets-1.0.2/wildlife_datasets/loader/
--rw-rw-rw-   0        0        0       23 2023-02-16 18:10:22.000000 wildlife-datasets-1.0.2/wildlife_datasets/loader/__init__.py
--rw-rw-rw-   0        0        0     3054 2024-02-28 09:13:03.000000 wildlife-datasets-1.0.2/wildlife_datasets/loader/loader.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.780138 wildlife-datasets-1.0.2/wildlife_datasets/metrics/
--rw-rw-rw-   0        0        0       24 2023-03-11 18:14:35.000000 wildlife-datasets-1.0.2/wildlife_datasets/metrics/__init__.py
--rw-rw-rw-   0        0        0    10403 2024-01-24 14:31:26.000000 wildlife-datasets-1.0.2/wildlife_datasets/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.783780 wildlife-datasets-1.0.2/wildlife_datasets/splits/
--rw-rw-rw-   0        0        0      213 2024-01-12 06:51:35.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/__init__.py
--rw-rw-rw-   0        0        0     3688 2024-02-26 10:06:41.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/analysis.py
--rw-rw-rw-   0        0        0     1953 2024-01-15 08:49:13.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/balanced_split.py
--rw-rw-rw-   0        0        0    12804 2024-01-03 12:22:54.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/identity_split.py
--rw-rw-rw-   0        0        0     1816 2023-03-11 18:14:35.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/lcg.py
--rw-rw-rw-   0        0        0    10435 2024-01-03 12:22:54.000000 wildlife-datasets-1.0.2/wildlife_datasets/splits/time_aware_split.py
-drwxrwxrwx   0        0        0        0 2024-02-28 09:15:17.783780 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/
--rw-rw-rw-   0        0        0    10523 2024-02-28 09:15:17.000000 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2024-02-28 09:15:17.000000 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 09:15:17.000000 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-02-28 09:15:17.000000 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-28 09:15:17.000000 wildlife-datasets-1.0.2/wildlife_datasets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.698774 wildlife_datasets-1.0.3/
+-rw-rw-rw-   0        0        0     1110 2024-01-12 06:51:35.000000 wildlife_datasets-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10601 2024-05-09 07:58:17.697768 wildlife_datasets-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8153 2024-05-09 07:53:59.000000 wildlife_datasets-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1670 2024-05-09 07:53:59.000000 wildlife_datasets-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:58:17.698774 wildlife_datasets-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.656853 wildlife_datasets-1.0.3/wildlife_datasets/
+-rw-rw-rw-   0        0        0      113 2024-01-12 06:51:35.000000 wildlife_datasets-1.0.3/wildlife_datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.682614 wildlife_datasets-1.0.3/wildlife_datasets/analysis/
+-rw-rw-rw-   0        0        0      109 2023-02-16 18:10:22.000000 wildlife_datasets-1.0.3/wildlife_datasets/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3186 2024-02-28 09:12:57.000000 wildlife_datasets-1.0.3/wildlife_datasets/analysis/plots.py
+-rw-rw-rw-   0        0        0     2688 2024-01-12 06:51:35.000000 wildlife_datasets-1.0.3/wildlife_datasets/analysis/statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.683576 wildlife_datasets-1.0.3/wildlife_datasets/datasets/
+-rw-rw-rw-   0        0        0     3508 2024-05-09 07:53:59.000000 wildlife_datasets-1.0.3/wildlife_datasets/datasets/__init__.py
+-rw-rw-rw-   0        0        0    94022 2024-05-09 07:53:59.000000 wildlife_datasets-1.0.3/wildlife_datasets/datasets/datasets.py
+-rw-rw-rw-   0        0        0     9964 2024-05-09 07:53:59.000000 wildlife_datasets-1.0.3/wildlife_datasets/datasets/metadata.csv
+-rw-rw-rw-   0        0        0      852 2023-02-16 18:10:22.000000 wildlife_datasets-1.0.3/wildlife_datasets/datasets/metadata.py
+-rw-rw-rw-   0        0        0     5178 2024-02-28 09:12:57.000000 wildlife_datasets-1.0.3/wildlife_datasets/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.688037 wildlife_datasets-1.0.3/wildlife_datasets/loader/
+-rw-rw-rw-   0        0        0       23 2023-02-16 18:10:22.000000 wildlife_datasets-1.0.3/wildlife_datasets/loader/__init__.py
+-rw-rw-rw-   0        0        0     3054 2024-03-28 09:36:12.000000 wildlife_datasets-1.0.3/wildlife_datasets/loader/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.689037 wildlife_datasets-1.0.3/wildlife_datasets/metrics/
+-rw-rw-rw-   0        0        0       24 2023-03-11 18:14:35.000000 wildlife_datasets-1.0.3/wildlife_datasets/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10403 2024-01-24 14:31:26.000000 wildlife_datasets-1.0.3/wildlife_datasets/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.690117 wildlife_datasets-1.0.3/wildlife_datasets/splits/
+-rw-rw-rw-   0        0        0      213 2024-01-12 06:51:35.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/__init__.py
+-rw-rw-rw-   0        0        0     3688 2024-02-26 10:06:41.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/analysis.py
+-rw-rw-rw-   0        0        0     1953 2024-01-15 08:49:13.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/balanced_split.py
+-rw-rw-rw-   0        0        0    12804 2024-01-03 12:22:54.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/identity_split.py
+-rw-rw-rw-   0        0        0     1816 2023-03-11 18:14:35.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/lcg.py
+-rw-rw-rw-   0        0        0    10435 2024-01-03 12:22:54.000000 wildlife_datasets-1.0.3/wildlife_datasets/splits/time_aware_split.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:58:17.690117 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/
+-rw-rw-rw-   0        0        0    10601 2024-05-09 07:58:17.000000 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2024-05-09 07:58:17.000000 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:58:17.000000 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-09 07:58:17.000000 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-09 07:58:17.000000 wildlife_datasets-1.0.3/wildlife_datasets.egg-info/top_level.txt
```

### Comparing `wildlife-datasets-1.0.2/LICENSE` & `wildlife_datasets-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/PKG-INFO` & `wildlife_datasets-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2024 Lukáš Adam and Vojtěch Čermák
         
@@ -62,29 +62,31 @@
 <div align="center">
   <p align="center">Pipeline for wildlife re-identification including dataset zoo, training tools and trained models. Usage includes classifying new images in labelled databases and clustering individuals in unlabelled databases.</p>
   <a href="https://wildlifedatasets.github.io/wildlife-datasets/">Documentation</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D">Report Bug</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D">Request Feature</a>
+  ·
+  <a href="mailto:wilddatasets@gmail.com">:mailbox_with_mail:Email</a>
 </div>
 
 </br>
 
 | <a href="https://github.com/WildlifeDatasets/wildlife-datasets"><img src="docs/resources/datasets-logo.png" alt="Wildlife datasets" width="200"></a>  | <a href="https://huggingface.co/BVRA/MegaDescriptor-L-384"><img src="docs/resources/megadescriptor-logo.png" alt="MegaDescriptor" width="200"></a> | <a href="https://github.com/WildlifeDatasets/wildlife-tools"><img src="docs/resources/tools-logo.png" alt="Wildlife tools" width="200"></a> |
 |:--------------:|:-----------:|:------------:|
 | Datasets for identification of individual animals | Trained model for individual re&#x2011;identification  | Tools for training re&#x2011;identification models |
 
 </br>
 
 ## Wildlife Re-Identification (Re-ID) Datasets
 
 The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
 
-- overview of 33 publicly available wildlife re-identification datasets.
+- overview of 36 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format and fix some wrong labels.
 - default splits for several machine learning tasks including the ability create additional splits.
 
 An introductory example is provided in a [Jupyter notebook](notebooks/introduction.ipynb). The package provides a natural synergy with [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384) model and tools for training neural networks. 
 
 ## Summary of datasets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wildlife-datasets Version: 1.0.2 Summary: Library
+Metadata-Version: 2.1 Name: wildlife-datasets Version: 1.0.3 Summary: Library
 for easier access and research of wildlife re-identification datasets Author-
 email: LukÃ¡Å¡ Adam
 gmail.com>, VojtÄch ÄermÃ¡k
 seznam.cz> Maintainer-email: LukÃ¡Å¡ Adam
 gmail.com>, VojtÄch ÄermÃ¡k
 seznam.cz> License: MIT License Copyright (c) 2024 LukÃ¡Å¡ Adam and VojtÄch
 ÄermÃ¡k Permission is hereby granted, free of charge, to any person obtaining
@@ -32,22 +32,22 @@
 Dist: kaggle
 _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]_[_G_i_t_H_u_b_ _p_u_l_l_ _r_e_q_u_e_s_t_s_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b
                        _s_t_a_r_s_]_[_G_i_t_H_u_b_ _w_a_t_c_h_e_r_s_]_[_L_i_c_e_n_s_e_]
                               [Wildlife datasets]
  Pipeline for wildlife re-identification including dataset zoo, training tools
 and trained models. Usage includes classifying new images in labelled databases
               and clustering individuals in unlabelled databases.
-                _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+  _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â· _:_m_a_i_l_b_o_x___w_i_t_h___m_a_i_l_:_E_m_a_i_l
 | _[_W_i_l_d_l_i_f_e_ _d_a_t_a_s_e_t_s_]| _[_M_e_g_a_D_e_s_c_r_i_p_t_o_r_]| _[_W_i_l_d_l_i_f_e_ _t_o_o_l_s_]| |:--------------:|:-
 ----------:|:------------:| | Datasets for identification of individual animals
 | Trained model for individual re‑identification | Tools for training
 re‑identification models | ## Wildlife Re-Identification (Re-ID) Datasets The
 aim of the project is to provide comprehensive overview of datasets for
 wildlife individual re-identification and an easy-to-use package for developers
-of machine learning methods. The core functionality includes: - overview of 33
+of machine learning methods. The core functionality includes: - overview of 36
 publicly available wildlife re-identification datasets. - utilities to mass
 download and convert them into a unified format and fix some wrong labels. -
 default splits for several machine learning tasks including the ability create
 additional splits. An introductory example is provided in a [Jupyter notebook]
 (notebooks/introduction.ipynb). The package provides a natural synergy with
 [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which
 provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384)
```

### Comparing `wildlife-datasets-1.0.2/README.md` & `wildlife_datasets-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,31 @@
 <div align="center">
   <p align="center">Pipeline for wildlife re-identification including dataset zoo, training tools and trained models. Usage includes classifying new images in labelled databases and clustering individuals in unlabelled databases.</p>
   <a href="https://wildlifedatasets.github.io/wildlife-datasets/">Documentation</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D">Report Bug</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D">Request Feature</a>
+  ·
+  <a href="mailto:wilddatasets@gmail.com">:mailbox_with_mail:Email</a>
 </div>
 
 </br>
 
 | <a href="https://github.com/WildlifeDatasets/wildlife-datasets"><img src="docs/resources/datasets-logo.png" alt="Wildlife datasets" width="200"></a>  | <a href="https://huggingface.co/BVRA/MegaDescriptor-L-384"><img src="docs/resources/megadescriptor-logo.png" alt="MegaDescriptor" width="200"></a> | <a href="https://github.com/WildlifeDatasets/wildlife-tools"><img src="docs/resources/tools-logo.png" alt="Wildlife tools" width="200"></a> |
 |:--------------:|:-----------:|:------------:|
 | Datasets for identification of individual animals | Trained model for individual re&#x2011;identification  | Tools for training re&#x2011;identification models |
 
 </br>
 
 ## Wildlife Re-Identification (Re-ID) Datasets
 
 The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
 
-- overview of 33 publicly available wildlife re-identification datasets.
+- overview of 36 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format and fix some wrong labels.
 - default splits for several machine learning tasks including the ability create additional splits.
 
 An introductory example is provided in a [Jupyter notebook](notebooks/introduction.ipynb). The package provides a natural synergy with [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384) model and tools for training neural networks. 
 
 ## Summary of datasets
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]_[_G_i_t_H_u_b_ _p_u_l_l_ _r_e_q_u_e_s_t_s_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b
                        _s_t_a_r_s_]_[_G_i_t_H_u_b_ _w_a_t_c_h_e_r_s_]_[_L_i_c_e_n_s_e_]
                               [Wildlife datasets]
  Pipeline for wildlife re-identification including dataset zoo, training tools
 and trained models. Usage includes classifying new images in labelled databases
               and clustering individuals in unlabelled databases.
-                _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+  _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â· _:_m_a_i_l_b_o_x___w_i_t_h___m_a_i_l_:_E_m_a_i_l
 | _[_W_i_l_d_l_i_f_e_ _d_a_t_a_s_e_t_s_]| _[_M_e_g_a_D_e_s_c_r_i_p_t_o_r_]| _[_W_i_l_d_l_i_f_e_ _t_o_o_l_s_]| |:--------------:|:-
 ----------:|:------------:| | Datasets for identification of individual animals
 | Trained model for individual re‑identification | Tools for training
 re‑identification models | ## Wildlife Re-Identification (Re-ID) Datasets The
 aim of the project is to provide comprehensive overview of datasets for
 wildlife individual re-identification and an easy-to-use package for developers
-of machine learning methods. The core functionality includes: - overview of 33
+of machine learning methods. The core functionality includes: - overview of 36
 publicly available wildlife re-identification datasets. - utilities to mass
 download and convert them into a unified format and fix some wrong labels. -
 default splits for several machine learning tasks including the ability create
 additional splits. An introductory example is provided in a [Jupyter notebook]
 (notebooks/introduction.ipynb). The package provides a natural synergy with
 [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which
 provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384)
```

### Comparing `wildlife-datasets-1.0.2/pyproject.toml` & `wildlife_datasets-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wildlife-datasets"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
 ]
 maintainers = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
```

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/analysis/plots.py` & `wildlife_datasets-1.0.3/wildlife_datasets/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/analysis/statistics.py` & `wildlife_datasets-1.0.3/wildlife_datasets/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/datasets/__init__.py` & `wildlife_datasets-1.0.3/wildlife_datasets/datasets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from .datasets import DatasetFactory
 from .datasets import AAUZebraFish
 from .datasets import AerialCattle2017
 from .datasets import ATRW
 from .datasets import BelugaID
 from .datasets import BirdIndividualID
 from .datasets import BirdIndividualIDSegmented
+from .datasets import CatIndividualImages
 from .datasets import CTai
 from .datasets import CZoo
+from .datasets import CowDataset
 from .datasets import Cows2021, Cows2021v2
+from .datasets import DogFaceNet
 from .datasets import Drosophila
 from .datasets import FriesianCattle2015, FriesianCattle2015v2
 from .datasets import FriesianCattle2017
 from .datasets import GiraffeZebraID
 from .datasets import Giraffes
+from .datasets import GreenSeaTurtles
 from .datasets import HappyWhale
 from .datasets import HumpbackWhaleID
 from .datasets import HyenaID2022
 from .datasets import IPanda50
 from .datasets import LeopardID2022
 from .datasets import LionData
 from .datasets import MacaqueFaces
 from .datasets import MPDD
-from .datasets import NDD20
+from .datasets import NDD20, NDD20v2
 from .datasets import NOAARightWhale
 from .datasets import NyalaData
 from .datasets import OpenCows2020
 from .datasets import PolarBearVidID
 from .datasets import SealID
 from .datasets import SealIDSegmented
 from .datasets import SeaStarReID2023
@@ -41,31 +45,35 @@
 names_all = [
     AAUZebraFish,
     AerialCattle2017,
     ATRW,
     BelugaID,
     BirdIndividualID,
     BirdIndividualIDSegmented,
+    CatIndividualImages,
     CTai,
     CZoo,
+    CowDataset,
     Cows2021v2,
+    DogFaceNet,
     Drosophila,
     FriesianCattle2015v2,
     FriesianCattle2017,
     GiraffeZebraID,
     Giraffes,
+    GreenSeaTurtles,
     HappyWhale,
     HumpbackWhaleID,
     HyenaID2022,
     IPanda50,
     LeopardID2022,
     LionData,
     MacaqueFaces,
     MPDD,
-    NDD20,
+    NDD20v2,
     NOAARightWhale,
     NyalaData,
     OpenCows2020,
     PolarBearVidID,
     SealID,
     SealIDSegmented,
     SeaStarReID2023,
@@ -76,70 +84,80 @@
     WhaleSharkID,
     ZindiTurtleRecall,
 ]
 
 names_wild = [
     BelugaID,
     GiraffeZebraID,
+    GreenSeaTurtles,
     HappyWhale,
     HumpbackWhaleID,
     HyenaID2022,
     LeopardID2022,
-    NDD20,
+    NDD20v2,
     NOAARightWhale,
     NyalaData,
     SealID,
     SeaTurtleID2022,
     StripeSpotter,
     WhaleSharkID,
 ]
 
 names_small = [
     AerialCattle2017,
     BelugaID,
     CTai,
     CZoo,
+    DogFaceNet,
     FriesianCattle2015v2,
     FriesianCattle2017,
     IPanda50,
+    GreenSeaTurtles,
     MacaqueFaces,
     MPDD,
     NyalaData,
     PolarBearVidID,
     SeaTurtleIDHeads,
     StripeSpotter,
 ]
 
 names_cows = [
     AerialCattle2017,
+    CowDataset,
     Cows2021v2,
     FriesianCattle2015v2,
     FriesianCattle2017,
     OpenCows2020,
 ]
 
+names_dogs = [
+    DogFaceNet,
+    MPDD,
+]
+
 names_giraffes = [
     GiraffeZebraID,
     Giraffes,
     SMALST,
     StripeSpotter,
 ]
 
 names_primates = [
     CTai,
     CZoo,
     MacaqueFaces,
 ]
 
 names_turtles = [
+    GreenSeaTurtles,
     SeaTurtleIDHeads,
     ZindiTurtleRecall,
 ]
 
 names_whales = [
     BelugaID,
     HappyWhale,
     HumpbackWhaleID,
-    NDD20,
+    NDD20v2,
     NOAARightWhale,
     WhaleSharkID,
 ]
```

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/datasets/datasets.py` & `wildlife_datasets-1.0.3/wildlife_datasets/datasets/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     outdated_dataset = False
     download_warning = '''You are trying to download an already downloaded dataset.
         This message may have happened to due interrupted download or extract.
         To force the download use the `force=True` keyword such as
         get_data(..., force=True) or download(..., force=True).
         '''
     download_mark_name = 'already_downloaded'
+    license_file_name = 'LICENSE_link'
 
     def __init__(
             self, 
             root: str,
             df: Optional[pd.DataFrame] = None,
             update_wrong_labels: bool = True,
             **kwargs) -> None:
@@ -90,14 +91,17 @@
             print(cls.download_warning)
         else:
             if os.path.exists(mark_file_name):
                 os.remove(mark_file_name)
             with utils.data_directory(root):
                 cls._download(**kwargs)
             open(mark_file_name, 'a').close()
+            if hasattr(cls, 'metadata') and 'licenses_url' in cls.metadata:
+                with open(os.path.join(root, cls.license_file_name), 'w') as file:
+                    file.write(cls.metadata['licenses_url'])
         
     @classmethod    
     def extract(cls, root, **kwargs):
         with utils.data_directory(root):
             cls._extract(**kwargs)
         mark_file_name = os.path.join(root, cls.download_mark_name)
         open(mark_file_name, 'a').close()
@@ -845,14 +849,49 @@
     def _download(cls):
         print(cls.warning)
 
     @classmethod
     def _extract(cls):
         print(cls.warning)
 
+
+class CatIndividualImages(DatasetFactory):
+    metadata = metadata['CatIndividualImages']
+    archive = 'cat-individuals.zip'
+    
+    @classmethod
+    def _download(cls):
+        command = f"datasets download -d timost1234/cat-individuals --force"
+        exception_text = '''Kaggle must be setup.
+            Check https://wildlifedatasets.github.io/wildlife-datasets/downloads#catindividualimages'''
+        utils.kaggle_download(command, exception_text=exception_text, required_file=cls.archive)
+
+    @classmethod
+    def _extract(cls):
+        utils.extract_archive(cls.archive, delete=True)
+
+    def create_catalogue(self) -> pd.DataFrame:
+        # Find all images in root
+        data = utils.find_images(self.root)
+        folders = data['path'].str.split(os.path.sep, expand=True)
+        
+        # Remove 85 duplicate images
+        idx = folders[2].isnull()
+        data = data[idx]
+        folders = folders[idx]
+
+        # Finalize the dataframe
+        df = pd.DataFrame({
+            'image_id': data['file'].apply(lambda x: os.path.splitext(x)[0]),
+            'path': data['path'] + os.path.sep + data['file'],
+            'identity': folders[1].astype(int),
+        })
+        return self.finalize_catalogue(df)
+
+
 class CTai(DatasetFactory):
     metadata = metadata['CTai']
     url = 'https://github.com/cvjena/chimpanzee_faces/archive/refs/heads/master.zip'
     archive = 'master.zip'
 
     @classmethod
     def _download(cls):
@@ -932,14 +971,46 @@
             'age': data[5],
             'age_group': data[7],
             'gender': data[9],
         })
         return self.finalize_catalogue(df)
 
 
+class CowDataset(DatasetFactory):
+    metadata = metadata['CowDataset']
+    url = 'https://figshare.com/ndownloader/files/31210192'
+    archive = 'cow-dataset.zip'
+
+    @classmethod
+    def _download(cls):
+        utils.download_url(cls.url, cls.archive)
+
+    @classmethod
+    def _extract(cls):
+        utils.extract_archive(cls.archive, delete=True)
+        # Rename the folder with non-ASCII characters
+        dirs = [x for x in os.listdir() if os.path.isdir(x)]
+        if len(dirs) != 1:
+            raise Exception('There should be only one directory after extracting the file.')
+        os.rename(dirs[0], 'images')
+    
+    def create_catalogue(self) -> pd.DataFrame:
+        # Find all images in root
+        data = utils.find_images(self.root)
+        folders = data['path'].str.split(os.path.sep, expand=True)
+
+        # Finalize the dataframe
+        df = pd.DataFrame({
+            'image_id': utils.create_id(data['file']),
+            'path': data['path'] + os.path.sep + data['file'],
+            'identity': folders[1].str.strip('cow_').astype(int),
+        })
+        return self.finalize_catalogue(df)
+
+
 class Cows2021(DatasetFactory):
     outdated_dataset = True
     metadata = metadata['Cows2021']
     url = 'https://data.bris.ac.uk/datasets/tar/4vnrca7qw1642qlwxjadp87h7.zip'
     archive = '4vnrca7qw1642qlwxjadp87h7.zip'
 
     @classmethod
@@ -993,14 +1064,41 @@
         replace_identity2 = [
             ('image_0001226_2020-02-11_12-43-7_roi_001.jpg', 137, 107)
         ]
         df = self.fix_labels_replace_identity(df, replace_identity1)
         return self.fix_labels_replace_images(df, replace_identity2)
         
 
+class DogFaceNet(DatasetFactory):
+    metadata = metadata['DogFaceNet']
+    url = 'https://github.com/GuillaumeMougeot/DogFaceNet/releases/download/dataset/DogFaceNet_Dataset_224_1.zip'
+    archive = 'DogFaceNet_Dataset_224_1.zip'
+
+    @classmethod
+    def _download(cls):
+        utils.download_url(cls.url, cls.archive)
+
+    @classmethod
+    def _extract(cls):
+        utils.extract_archive(cls.archive, delete=True)
+    
+    def create_catalogue(self) -> pd.DataFrame:
+        # Find all images in root
+        data = utils.find_images(self.root)
+        folders = data['path'].str.split(os.path.sep, expand=True)
+
+        # Finalize the dataframe
+        df = pd.DataFrame({
+            'image_id': utils.create_id(data['file']),
+            'path': data['path'] + os.path.sep + data['file'],
+            'identity': folders[1].astype(int),
+        })
+        return self.finalize_catalogue(df)
+
+
 class Drosophila(DatasetFactory):
     metadata = metadata['Drosophila']
     downloads = [
         ('https://dataverse.scholarsportal.info/api/access/datafile/71066', 'week1_Day1_train_01to05.zip'),
         ('https://dataverse.scholarsportal.info/api/access/datafile/71067', 'week1_Day1_train_06to10.zip'),
         ('https://dataverse.scholarsportal.info/api/access/datafile/71068', 'week1_Day1_train_11to15.zip'),
         ('https://dataverse.scholarsportal.info/api/access/datafile/71069', 'week1_Day1_train_16to20.zip'),
@@ -1522,14 +1620,15 @@
             'identity': identity,
             'original_split': folders[2]
         })
         return self.finalize_catalogue(df)
 
 
 class NDD20(DatasetFactory):
+    outdated_dataset = True
     metadata = metadata['NDD20']
     url = 'https://data.ncl.ac.uk/ndownloader/files/22774175'
     archive = 'NDD20.zip'
 
     @classmethod
     def _download(cls):
         utils.download_url(cls.url, cls.archive)
@@ -1598,14 +1697,28 @@
         # Finalize the dataframe
         df['image_id'] = range(len(df))
         df['path'] = df['orientation'].str.upper() + os.path.sep + df['file_name']
         df = df.drop(['reg_type', 'file_name'], axis=1)
         return self.finalize_catalogue(df)
 
 
+class NDD20v2(NDD20):
+    outdated_dataset = False
+
+    def fix_labels(self, df: pd.DataFrame) -> pd.DataFrame:
+        for i, df_row in df.iterrows():
+            # Rewrite wrong segmentations. There is no dolphin -> should be deleted.
+            # But that would break compability and the identity is unknown anyway.
+            if len(df_row['segmentation']) == 4:
+                img = utils.get_image(os.path.join(self.root, df_row['path']))
+                w, h = img.size
+                df.at[i, 'segmentation'] = np.array(utils.bbox_segmentation([0, 0, w, h]))
+        return df
+
+
 class NOAARightWhale(DatasetFactory):
     metadata = metadata['NOAARightWhale']
     archive = 'noaa-right-whale-recognition.zip'
 
     @classmethod
     def _download(cls):
         command = f"competitions download -c noaa-right-whale-recognition --force"
@@ -1749,14 +1862,47 @@
         })
         df = pd.merge(df, metadata, on='id', how='left')
         df.rename({'name': 'identity', 'sex': 'gender'}, axis=1, inplace=True)
         df = df.drop(['id', 'zoo', 'tracklets'], axis=1)
         return self.finalize_catalogue(df)
 
 
+class GreenSeaTurtles(DatasetFactory):
+    # TODO: add metadata
+    # TODO: change the names everywhere
+    # TODO: fix documentation everywhere
+    archive = 'sarahzelvy.zip'
+
+    @classmethod
+    def _download(cls):
+        command = f"datasets download -d wildlifedatasets/sarahzelvy --force"
+        exception_text = '''Kaggle must be setup.
+            Check https://wildlifedatasets.github.io/wildlife-datasets/downloads#greenseaturtles'''
+        utils.kaggle_download(command, exception_text=exception_text, required_file=cls.archive)
+
+    @classmethod
+    def _extract(cls):
+        utils.extract_archive(cls.archive, delete=True)
+
+    def create_catalogue(self) -> pd.DataFrame:
+        file_name = os.path.join(self.root, 'annotations.csv')
+        data = pd.read_csv(file_name)
+
+        df = pd.DataFrame({
+            'image_id': range(len(data)),
+            'path': 'data' + os.path.sep + data['image_name'],
+            'identity': data['identity'],
+            'orientation': data['orientation'],
+            'daytime': data['daytime']
+        })
+        if 'bbox_x' in data.columns:
+            df['bbox'] = data[['bbox_x', 'bbox_y', 'bbox_width', 'bbox_height']].values.tolist()
+        return self.finalize_catalogue(df)
+
+
 class SealID(DatasetFactory):
     metadata = metadata['SealID']
     prefix = 'source_'
     archive = '22b5191e-f24b-4457-93d3-95797c900fc0_ui65zipk.zip'
     
     @classmethod
     def _download(cls, url=None):
@@ -1870,15 +2016,21 @@
         with open(os.path.join(self.root, path_json)) as file:
             data = json.load(file)
         path_csv = os.path.join('turtles-data', 'data', 'metadata_splits.csv')
         with open(os.path.join(self.root, path_csv)) as file:
             df_images = pd.read_csv(file)
 
         # Extract data from the JSON file
-        create_dict = lambda i: {'id': i['id'], 'bbox': i['bbox'], 'image_id': i['image_id'], 'segmentation': i['segmentation']}
+        create_dict = lambda i: {
+            'id': i['id'],
+            'bbox': i['bbox'],
+            'image_id': i['image_id'],
+            'segmentation': i['segmentation'],
+            'orientation': i['attributes']['orientation'] if 'orientation' in i['attributes'] else np.nan
+        }
         df_annotation = pd.DataFrame([create_dict(i) for i in data['annotations'] if i['category_id'] == 3])
         idx_bbox = ~df_annotation['bbox'].isnull()
         df_annotation.loc[idx_bbox,'bbox'] = df_annotation.loc[idx_bbox,'bbox'].apply(lambda x: eval(x) if isinstance(x, str) else x)
         df_images.rename({'id': 'image_id'}, axis=1, inplace=True)
 
         # Merge the information from the JSON file
         df = pd.merge(df_images, df_annotation, on='image_id', how='outer')
```

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/datasets/metadata.csv` & `wildlife_datasets-1.0.3/wildlife_datasets/datasets/metadata.csv`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-name,licenses,licenses_url,url,cite,animals,real_animals,year,reported_n_total,reported_n_identified,reported_n_photos,reported_n_individuals,wild,clear_photos,pose,unique_pattern,from_video,cropped,span,size
-AAUZebraFish,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://www.kaggle.com/datasets/aalborguniversity/aau-zebrafish-reid,bruslund2020re,"{'zebrafish'}",True,2020,6672,6672,2224,6,False,True,double,False,True,False,1 day,12093
-AerialCattle2017,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/3owflku95bxsx24643cybxu3qh,andrew2017visual,"{'Friesian cattle'}",True,2017,46340,46340,46340,23,False,True,single,True,True,True,1 day,724
-ATRW,Attribution-NonCommercial-ShareAlike 4.0 International,https://creativecommons.org/licenses/by-nc-sa/4.0/,https://lila.science/datasets/atrw,li2019atrw,"{'amur tiger'}",True,2019,9496,3649,8076,92,False,False,double,True,True,False,short,1760
-BelugaID,Attribution-NonCommercial-NoDerivs License,http://creativecommons.org/licenses/by-nc-nd/2.0/,https://lila.science/datasets/beluga-id-2022/,belugaid,"{'beluga whale'}",True,2022,5902,5902,5902,788,True,True,single,False,False,True,2.1 years,590
-BirdIndividualID,,,https://github.com/AndreCFerreira/Bird_individualID,ferreira2020deep,"{'sociable weaver', 'great tit', 'zebra finch'}",True,2019,50643,50643,50643,50,False,True,single,False,False,False,15 days,70656
-CTai,,,https://github.com/cvjena/chimpanzee_faces,freytag2016chimpanzee,"{'chimpanzee'}",True,2016,5078,5078,5078,78,True,True,single,False,False,True,unknown,634
-CZoo,,,https://github.com/cvjena/chimpanzee_faces,freytag2016chimpanzee,"{'chimpanzee'}",True,2016,2109,2109,2109,24,False,True,single,False,False,True,unknown,634
-Cows2021,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/4vnrca7qw1642qlwxjadp87h7,gao2021towards,"{'cow'}",True,2021,13784,13784,13784,181,False,True,single,True,True,True,1 month,18881
-Drosophila,,,https://github.com/j-schneider/fly_eye,schneider2018can,"{'drosophila'}",True,2018,2592000,2592000,2592000,60,False,True,single,True,True,True,3 days,74856
-FriesianCattle2015,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/wurzq71kfm561ljahbwjhx9n3,andrew2016automatic,"{'Friesian cattle'}",True,2016,377,377,377,40,False,True,single,True,True,True,1 day,76
-FriesianCattle2017,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/2yizcfbkuv4352pzc32n54371r,andrew2017visual,"{'Friesian cattle'}",True,2017,940,940,940,89,False,True,single,True,True,True,1 day,343
-GiraffeZebraID,Attribution-NonCommercial-NoDerivs License,http://creativecommons.org/licenses/by-nc-nd/2.0/,https://lila.science/datasets/great-zebra-giraffe-id,parham2017animal,"{'giraffe masai', 'zebra plains'}",True,2017,6925,6925,4948,2056,True,True,double,True,False,False,12 days,10433
-Giraffes,,,ftp://pbil.univ-lyon1.fr/pub/datasets/miele2021,miele2021revisiting,"{'giraffe'}",True,2021,,,,,True,True,double,True,True,True,unknown,1719
-HappyWhale,,,https://www.kaggle.com/competitions/happy-whale-and-dolphin,cheeseman2017happywhale,"{'whale','dolphin'}",True,2022,,,,,True,True,multiple,True,False,False,very long,61912
-HumpbackWhaleID,,,https://www.kaggle.com/competitions/humpback-whale-identification,humpbackwhale,"{'whale'}",True,2019,,,,,True,True,single,True,False,True,very long,5911
-HyenaID2022,Attribution-NonCommercial-NoDerivs License,http://creativecommons.org/licenses/by-nc-nd/2.0/,https://lila.science/datasets/hyena-id-2022/,botswana2022,"{'spotted hyena'}",True,2022,3129,3129,3104,256,True,False,multiple,True,False,False,unknown,3441
-IPanda50,,,https://github.com/iPandaDateset/iPanda-50,wang2021giant,"{'great panda'}",True,2021,6874,6874,6874,50,False,True,multiple,True,False,True,unknown,929
-LeopardID2022,Attribution-NonCommercial-NoDerivs License,http://creativecommons.org/licenses/by-nc-nd/2.0/,https://lila.science/datasets/leopard-id-2022/,botswana2022,"{'leopard'}",True,2022,,6805,6795,430,True,False,multiple,True,False,False,unknown,8565
-LionData,,,https://github.com/tvanzyl/wildlife_reidentification,dlamini2020automated,"{'lion'}",True,2020,750,750,750,98,True,True,multiple,True,False,True,unknown,495
-MacaqueFaces,The 3-Clause BSD License,https://github.com/clwitham/MacaqueFaces/blob/master/license.md,https://github.com/clwitham/MacaqueFaces,witham2018automated,"{'rhesus macaque'}",True,2018,6460,6460,6460,34,False,True,single,False,True,True,1.4 years,12
-MPDD,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://data.mendeley.com/datasets/v5j6m8dzhv/1,he2023animal,"{'dog'}",True,2023,1657,1657,1657,192,False,True,multiple,False,False,True,short,29.6
-NDD20,Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0),https://creativecommons.org/licenses/by-nc-sa/4.0/,https://doi.org/10.25405/data.ncl.c.4982342,trotter2020ndd20,"{'Northumberland dolphin'}",True,2020,,,4402,82,True,True,multiple,True,False,False,7 years,2441
-NOAARightWhale,,,https://www.kaggle.com/c/noaa-right-whale-recognition,rightwhale,"{'right whale'}",True,2015,,,,,True,False,single,False,False,False,10 years,9790
-NyalaData,,,https://github.com/tvanzyl/wildlife_reidentification,dlamini2020automated,"{'nyala'}",True,2020,1934,1934,1934,274,True,True,double,True,False,False,unknown,495
-OpenCows2020,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/10m32xl88x2b61zlkkgz3fml17,andrew2021visual,"{'cow'}",True,2020,4736,4736,4736,46,False,True,double,True,True,True,short,2272
-PolarBearVidID,Creative Commons Attribution 4.0 International,https://creativecommons.org/licenses/by/4.0/legalcode,https://zenodo.org/records/7564529,zuerl2023polarbearvidid,"{'polar bear'}",True,2023,138363,138363,138363,13,False,True,multiple,False,True,True,short,1501
-SealID,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://doi.org/10.23729/0f4a3296-3b10-40c8-9ad3-0cf00a5a4a53,nepovinnykh2022sealid,"{'ringed seal'}",True,2022,2080,2080,2080,57,True,False,multiple,True,False,False,10 years,1816
-SeaStarReID2023,"Community Data License Agreement – Permissive, Version 1.0",https://cdla.dev/permissive-1-0/,https://lila.science/sea-star-re-id-2023/,wahltinez2024open,"{'sea star'}",True,2023,2187,2187,2187,95,False,True,single,True,False,True,short,1689
-SeaTurtleID2022,Other,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleid2022,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleid2022,papafitsoros2022seaturtleid,"{'loggerhead turtle'}",True,2022,8729,8729,8729,438,True,False,multiple,True,False,False,12 years,2000
-SeaTurtleIDHeads,Other,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleidheads,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleidheads,papafitsoros2022seaturtleid,"{'loggerhead turtle'}",True,2022,7582,7582,7582,400,True,False,multiple,True,False,True,9 years,425
-SMALST,MIT License,https://github.com/silviazuffi/smalst/blob/master/LICENSE.txt,https://github.com/silviazuffi/smalst,zuffi2019three,"{'zebra'}",False,2019,12850,12850,12850,10,False,True,multiple,True,False,False,artificial,11978
-StripeSpotter,"GNU General Public License, version 2",http://www.gnu.org/licenses/old-licenses/gpl-2.0.html,https://code.google.com/archive/p/stripespotter/downloads,lahiri2011biometric,"{'zebra'}",True,2011,,,,,True,True,double,True,False,False,7 days,229
-WhaleSharkID,Attribution-NonCommercial-NoDerivs 2.0 Generic (CC BY-NC-ND 2.0),http://creativecommons.org/licenses/by-nc-nd/2.0/,https://lila.science/datasets/whale-shark-id,holmberg2009estimating,"{'whale shark'}",True,2020,7693,7693,7693,543,True,False,multiple,True,False,False,5.2 years,6466
-WNIGiraffes,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/wni-giraffes,clavadetscher2021development,"{'giraffe'}",True,2021,29806,29806,29806,,True,True,double,True,False,False,7 years,196000
-ZindiTurtleRecall,Attribution-ShareAlike 4.0 International (CC BY-SA 4.0),https://creativecommons.org/licenses/by-sa/4.0/,https://zindi.africa/competitions/turtle-recall-conservation-challenge,zinditurtles,"{'sea turtle'}",True,2022,,,,,False,True,double,True,False,True,unknown,6482
+name,licenses,licenses_url,url,cite,animals,animals_simple,real_animals,year,reported_n_total,reported_n_identified,reported_n_photos,reported_n_individuals,wild,clear_photos,pose,unique_pattern,from_video,cropped,span,size
+AAUZebraFish,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://www.kaggle.com/datasets/aalborguniversity/aau-zebrafish-reid,bruslund2020re,"{'zebrafish'}",fish,True,2020,6672,6672,2224,6,False,True,double,False,True,False,1 day,12093
+AerialCattle2017,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/3owflku95bxsx24643cybxu3qh,andrew2017visual,"{'Friesian cattle'}",cows,True,2017,46340,46340,46340,23,False,True,single,True,True,True,1 day,724
+ATRW,Attribution-NonCommercial-ShareAlike 4.0 International,https://creativecommons.org/licenses/by-nc-sa/4.0/,https://lila.science/datasets/atrw,li2019atrw,"{'amur tiger'}",tigers,True,2019,9496,3649,8076,92,False,False,double,True,True,False,short,1760
+BelugaID,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/beluga-id-2022/,belugaid,"{'beluga whale'}",whales,True,2022,5902,5902,5902,788,True,True,single,False,False,True,2.1 years,590
+BirdIndividualID,,,https://github.com/AndreCFerreira/Bird_individualID,ferreira2020deep,"{'sociable weaver', 'great tit', 'zebra finch'}",birds,True,2019,50643,50643,50643,50,False,True,single,False,False,False,15 days,70656
+CatIndividualImages,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://www.kaggle.com/datasets/timost1234/cat-individuals,catindividuals,"{'cat'}",cats,True,2020,13536,13536,13536,518,False,True,multiple,True,False,True,short,11000
+CTai,Other,https://github.com/cvjena/chimpanzee_faces/blob/master/README.md,https://github.com/cvjena/chimpanzee_faces,freytag2016chimpanzee,"{'chimpanzee'}",chimpanzees,True,2016,5078,5078,5078,78,True,True,single,False,False,True,unknown,634
+CZoo,Other,https://github.com/cvjena/chimpanzee_faces/blob/master/README.md,https://github.com/cvjena/chimpanzee_faces,freytag2016chimpanzee,"{'chimpanzee'}",chimpanzees,True,2016,2109,2109,2109,24,False,True,single,False,False,True,unknown,634
+CowDataset,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://figshare.com/articles/dataset/data_set_zip/16879780,cowdataset,"{'cow'}",cows,True,2021,1485,1485,1485,13,False,True,double,True,False,False,short,4150
+Cows2021,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/4vnrca7qw1642qlwxjadp87h7,gao2021towards,"{'cow'}",cows,True,2021,13784,13784,13784,181,False,True,single,True,True,True,1 month,18881
+DogFaceNet,MIT License,https://github.com/GuillaumeMougeot/DogFaceNet/blob/master/LICENSE,https://github.com/GuillaumeMougeot/DogFaceNet,mougeot2019deep,"{'dog'}",dogs,True,2019,8363,8363,8363,1393,False,True,single,False,False,True,short,76
+Drosophila,,,https://github.com/j-schneider/fly_eye,schneider2018can,"{'drosophila'}",flies,True,2018,2592000,2592000,2592000,60,False,True,single,True,True,True,3 days,74856
+FriesianCattle2015,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/wurzq71kfm561ljahbwjhx9n3,andrew2016automatic,"{'Friesian cattle'}",cows,True,2016,377,377,377,40,False,True,single,True,True,True,1 day,76
+FriesianCattle2017,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/2yizcfbkuv4352pzc32n54371r,andrew2017visual,"{'Friesian cattle'}",cows,True,2017,940,940,940,89,False,True,single,True,True,True,1 day,343
+GiraffeZebraID,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/great-zebra-giraffe-id,parham2017animal,"{'giraffe masai', 'zebra plains'}",giraffes+zebras,True,2017,6925,6925,4948,2056,True,True,double,True,False,False,12 days,10433
+Giraffes,,,ftp://pbil.univ-lyon1.fr/pub/datasets/miele2021,miele2021revisiting,"{'giraffe'}",giraffes,True,2021,,,,,True,True,double,True,True,True,unknown,1719
+HappyWhale,Other,https://www.kaggle.com/competitions/happy-whale-and-dolphin/rules/#7.-competition-data.,https://www.kaggle.com/competitions/happy-whale-and-dolphin,cheeseman2017happywhale,"{'whale','dolphin'}",dolphins+whales,True,2022,,,,,True,True,multiple,True,False,False,very long,61912
+HumpbackWhaleID,Other,https://www.kaggle.com/competitions/humpback-whale-identification/rules#7.-competition-data.,https://www.kaggle.com/competitions/humpback-whale-identification,humpbackwhale,"{'whale'}",whales,True,2019,,,,,True,True,single,True,False,True,very long,5911
+HyenaID2022,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/hyena-id-2022/,botswana2022,"{'spotted hyena'}",hyenas,True,2022,3129,3129,3104,256,True,False,multiple,True,False,False,unknown,3441
+IPanda50,,,https://github.com/iPandaDateset/iPanda-50,wang2021giant,"{'great panda'}",pandas,True,2021,6874,6874,6874,50,False,True,multiple,True,False,True,unknown,929
+LeopardID2022,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/leopard-id-2022/,botswana2022,"{'leopard'}",leopards,True,2022,,6805,6795,430,True,False,multiple,True,False,False,unknown,8565
+LionData,,,https://github.com/tvanzyl/wildlife_reidentification,dlamini2020automated,"{'lion'}",lions,True,2020,750,750,750,98,True,True,multiple,True,False,True,unknown,495
+MacaqueFaces,Other,https://github.com/clwitham/MacaqueFaces/blob/master/license.md,https://github.com/clwitham/MacaqueFaces,witham2018automated,"{'rhesus macaque'}",macaques,True,2018,6460,6460,6460,34,False,True,single,False,True,True,1.4 years,12
+MPDD,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://data.mendeley.com/datasets/v5j6m8dzhv/1,he2023animal,"{'dog'}",dogs,True,2023,1657,1657,1657,192,False,True,multiple,False,False,True,short,29.6
+NDD20,Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0),https://creativecommons.org/licenses/by-nc-sa/4.0/,https://doi.org/10.25405/data.ncl.c.4982342,trotter2020ndd20,"{'Northumberland dolphin'}",doplhins,True,2020,,,4402,82,True,True,multiple,True,False,False,7 years,2441
+NOAARightWhale,Other,https://www.kaggle.com/c/noaa-right-whale-recognition/rules#data,https://www.kaggle.com/c/noaa-right-whale-recognition,rightwhale,"{'right whale'}",whales,True,2015,,,,,True,False,single,False,False,False,10 years,9790
+NyalaData,,,https://github.com/tvanzyl/wildlife_reidentification,dlamini2020automated,"{'nyala'}",nyalas,True,2020,1934,1934,1934,274,True,True,double,True,False,False,unknown,495
+OpenCows2020,Non-Commercial Government Licence for public sector information,https://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/,https://data.bris.ac.uk/data/dataset/10m32xl88x2b61zlkkgz3fml17,andrew2021visual,"{'cow'}",cows,True,2020,4736,4736,4736,46,False,True,double,True,True,True,short,2272
+PolarBearVidID,Creative Commons Attribution 4.0 International,https://creativecommons.org/licenses/by/4.0/legalcode,https://zenodo.org/records/7564529,zuerl2023polarbearvidid,"{'polar bear'}",polar bears,True,2023,138363,138363,138363,13,False,True,multiple,False,True,True,short,1501
+SealID,Attribution 4.0 International (CC BY 4.0),https://creativecommons.org/licenses/by/4.0/,https://doi.org/10.23729/0f4a3296-3b10-40c8-9ad3-0cf00a5a4a53,nepovinnykh2022sealid,"{'ringed seal'}",seals,True,2022,2080,2080,2080,57,True,False,multiple,True,False,False,10 years,1816
+SeaStarReID2023,"Community Data License Agreement – Permissive, Version 1.0",https://cdla.dev/permissive-1-0/,https://lila.science/sea-star-re-id-2023/,wahltinez2024open,"{'sea star'}",sea stars,True,2023,2187,2187,2187,95,False,True,single,True,False,True,short,1689
+SeaTurtleID2022,Other,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleid2022,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleid2022,adam2024seaturtleid,"{'loggerhead turtle'}",sea turtles,True,2022,8729,8729,8729,438,True,False,multiple,True,False,False,12 years,2000
+SeaTurtleIDHeads,Other,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleidheads,https://www.kaggle.com/datasets/wildlifedatasets/seaturtleidheads,adam2024seaturtleid,"{'loggerhead turtle'}",sea turtles,True,2022,7582,7582,7582,400,True,False,multiple,True,False,True,9 years,425
+SMALST,MIT License,https://github.com/silviazuffi/smalst/blob/master/LICENSE.txt,https://github.com/silviazuffi/smalst,zuffi2019three,"{'zebra'}",zebras,False,2019,12850,12850,12850,10,False,True,multiple,True,False,False,artificial,11978
+StripeSpotter,Attribution-ShareAlike 3.0 Unported,https://creativecommons.org/licenses/by-sa/3.0/,https://code.google.com/archive/p/stripespotter/downloads,lahiri2011biometric,"{'zebra'}",zebras,True,2011,,,,,True,True,double,True,False,False,7 days,229
+WhaleSharkID,Community Data License Agreement – Permissive,https://cdla.dev/permissive-1-0/,https://lila.science/datasets/whale-shark-id,holmberg2009estimating,"{'whale shark'}",sharks,True,2020,7693,7693,7693,543,True,False,multiple,True,False,False,5.2 years,6466
+ZindiTurtleRecall,Attribution-ShareAlike 4.0 International (CC BY-SA 4.0),https://creativecommons.org/licenses/by-sa/4.0/,https://zindi.africa/competitions/turtle-recall-conservation-challenge,zinditurtles,"{'sea turtle'}",sea turtles,True,2022,,,,,False,True,double,True,False,True,unknown,6482
```

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/datasets/metadata.py` & `wildlife_datasets-1.0.3/wildlife_datasets/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/datasets/utils.py` & `wildlife_datasets-1.0.3/wildlife_datasets/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/loader/loader.py` & `wildlife_datasets-1.0.3/wildlife_datasets/loader/loader.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/metrics/metrics.py` & `wildlife_datasets-1.0.3/wildlife_datasets/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/splits/analysis.py` & `wildlife_datasets-1.0.3/wildlife_datasets/splits/analysis.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/splits/balanced_split.py` & `wildlife_datasets-1.0.3/wildlife_datasets/splits/balanced_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/splits/identity_split.py` & `wildlife_datasets-1.0.3/wildlife_datasets/splits/identity_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/splits/lcg.py` & `wildlife_datasets-1.0.3/wildlife_datasets/splits/lcg.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets/splits/time_aware_split.py` & `wildlife_datasets-1.0.3/wildlife_datasets/splits/time_aware_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets.egg-info/PKG-INFO` & `wildlife_datasets-1.0.3/wildlife_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2024 Lukáš Adam and Vojtěch Čermák
         
@@ -62,29 +62,31 @@
 <div align="center">
   <p align="center">Pipeline for wildlife re-identification including dataset zoo, training tools and trained models. Usage includes classifying new images in labelled databases and clustering individuals in unlabelled databases.</p>
   <a href="https://wildlifedatasets.github.io/wildlife-datasets/">Documentation</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=bug&projects=&template=bug_report.md&title=%5BBUG%5D">Report Bug</a>
   ·
   <a href="https://github.com/WildlifeDatasets/wildlife-datasets/issues/new?assignees=aerodynamic-sauce-pan&labels=enhancement&projects=&template=enhancement.md&title=%5BEnhancement%5D">Request Feature</a>
+  ·
+  <a href="mailto:wilddatasets@gmail.com">:mailbox_with_mail:Email</a>
 </div>
 
 </br>
 
 | <a href="https://github.com/WildlifeDatasets/wildlife-datasets"><img src="docs/resources/datasets-logo.png" alt="Wildlife datasets" width="200"></a>  | <a href="https://huggingface.co/BVRA/MegaDescriptor-L-384"><img src="docs/resources/megadescriptor-logo.png" alt="MegaDescriptor" width="200"></a> | <a href="https://github.com/WildlifeDatasets/wildlife-tools"><img src="docs/resources/tools-logo.png" alt="Wildlife tools" width="200"></a> |
 |:--------------:|:-----------:|:------------:|
 | Datasets for identification of individual animals | Trained model for individual re&#x2011;identification  | Tools for training re&#x2011;identification models |
 
 </br>
 
 ## Wildlife Re-Identification (Re-ID) Datasets
 
 The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
 
-- overview of 33 publicly available wildlife re-identification datasets.
+- overview of 36 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format and fix some wrong labels.
 - default splits for several machine learning tasks including the ability create additional splits.
 
 An introductory example is provided in a [Jupyter notebook](notebooks/introduction.ipynb). The package provides a natural synergy with [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384) model and tools for training neural networks. 
 
 ## Summary of datasets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wildlife-datasets Version: 1.0.2 Summary: Library
+Metadata-Version: 2.1 Name: wildlife-datasets Version: 1.0.3 Summary: Library
 for easier access and research of wildlife re-identification datasets Author-
 email: LukÃ¡Å¡ Adam
 gmail.com>, VojtÄch ÄermÃ¡k
 seznam.cz> Maintainer-email: LukÃ¡Å¡ Adam
 gmail.com>, VojtÄch ÄermÃ¡k
 seznam.cz> License: MIT License Copyright (c) 2024 LukÃ¡Å¡ Adam and VojtÄch
 ÄermÃ¡k Permission is hereby granted, free of charge, to any person obtaining
@@ -32,22 +32,22 @@
 Dist: kaggle
 _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]_[_G_i_t_H_u_b_ _p_u_l_l_ _r_e_q_u_e_s_t_s_]_[_G_i_t_H_u_b_ _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b
                        _s_t_a_r_s_]_[_G_i_t_H_u_b_ _w_a_t_c_h_e_r_s_]_[_L_i_c_e_n_s_e_]
                               [Wildlife datasets]
  Pipeline for wildlife re-identification including dataset zoo, training tools
 and trained models. Usage includes classifying new images in labelled databases
               and clustering individuals in unlabelled databases.
-                _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+  _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e Â· _:_m_a_i_l_b_o_x___w_i_t_h___m_a_i_l_:_E_m_a_i_l
 | _[_W_i_l_d_l_i_f_e_ _d_a_t_a_s_e_t_s_]| _[_M_e_g_a_D_e_s_c_r_i_p_t_o_r_]| _[_W_i_l_d_l_i_f_e_ _t_o_o_l_s_]| |:--------------:|:-
 ----------:|:------------:| | Datasets for identification of individual animals
 | Trained model for individual re‑identification | Tools for training
 re‑identification models | ## Wildlife Re-Identification (Re-ID) Datasets The
 aim of the project is to provide comprehensive overview of datasets for
 wildlife individual re-identification and an easy-to-use package for developers
-of machine learning methods. The core functionality includes: - overview of 33
+of machine learning methods. The core functionality includes: - overview of 36
 publicly available wildlife re-identification datasets. - utilities to mass
 download and convert them into a unified format and fix some wrong labels. -
 default splits for several machine learning tasks including the ability create
 additional splits. An introductory example is provided in a [Jupyter notebook]
 (notebooks/introduction.ipynb). The package provides a natural synergy with
 [Wildlife tools](https://github.com/WildlifeDatasets/wildlife-tools), which
 provides our [MegaDescriptor](https://huggingface.co/BVRA/MegaDescriptor-L-384)
```

### Comparing `wildlife-datasets-1.0.2/wildlife_datasets.egg-info/SOURCES.txt` & `wildlife_datasets-1.0.3/wildlife_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

