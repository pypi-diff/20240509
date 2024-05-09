# Comparing `tmp/tshirt-0.3.1.tar.gz` & `tmp/tshirt-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tshirt-0.3.1.tar", last modified: Fri Nov 17 19:12:50 2023, max compression
+gzip compressed data, was "tshirt-0.4.tar", last modified: Thu May  9 16:42:22 2024, max compression
```

## Comparing `tshirt-0.3.1.tar` & `tshirt-0.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.777271 tshirt-0.3.1/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       40 2017-01-16 05:08:31.000000 tshirt-0.3.1/.gitattributes
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1803 2021-07-03 05:50:30.000000 tshirt-0.3.1/.gitignore
--rw-r--r--   0 everettschlawin   (501) staff       (20)        0 2020-02-18 20:41:06.000000 tshirt-0.3.1/.gitmodules
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1073 2020-07-06 05:04:56.000000 tshirt-0.3.1/LICENSE
--rw-r--r--   0 everettschlawin   (501) staff       (20)       30 2020-09-13 03:03:55.000000 tshirt-0.3.1/MANIFEST.in
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1134 2023-11-17 19:12:50.777069 tshirt-0.3.1/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)      758 2020-07-06 05:04:31.000000 tshirt-0.3.1/README.md
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.759933 tshirt-0.3.1/docs/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      634 2020-06-22 23:17:25.000000 tshirt-0.3.1/docs/Makefile
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2264 2023-11-17 18:39:49.000000 tshirt-0.3.1/docs/conf.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.760176 tshirt-0.3.1/docs/images/
--rw-r--r--   0 everettschlawin   (501) staff       (20)   176987 2020-06-23 17:58:22.000000 tshirt-0.3.1/docs/images/t_shirt_logo.jpg
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1013 2022-01-18 07:12:31.000000 tshirt-0.3.1/docs/index.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3631 2022-01-18 07:20:02.000000 tshirt-0.3.1/docs/installation.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      795 2020-06-22 23:17:25.000000 tshirt-0.3.1/docs/make.bat
--rw-r--r--   0 everettschlawin   (501) staff       (20)      896 2020-11-08 04:57:30.000000 tshirt-0.3.1/docs/modules.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.761523 tshirt-0.3.1/docs/phot_pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)    37697 2020-07-12 04:40:36.000000 tshirt-0.3.1/docs/phot_pipeline/box_time_series_cookbook.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)      439 2020-07-12 04:40:36.000000 tshirt-0.3.1/docs/phot_pipeline/example_phot_param_file.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      397 2020-07-12 04:40:36.000000 tshirt-0.3.1/docs/phot_pipeline/phot_pipeline.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     5995 2023-09-14 18:51:30.000000 tshirt-0.3.1/docs/phot_pipeline/phot_pipeline_parameters.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1049 2021-03-29 20:26:21.000000 tshirt-0.3.1/docs/phot_pipeline/running_phot_pipeline.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.761787 tshirt-0.3.1/docs/reduction/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      915 2021-02-18 21:10:57.000000 tshirt-0.3.1/docs/reduction/reduction.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      178 2020-06-23 18:40:40.000000 tshirt-0.3.1/docs/reduction/reduction_param.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       78 2020-12-07 06:50:34.000000 tshirt-0.3.1/docs/requirements.txt
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.764019 tshirt-0.3.1/docs/spec_pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)   921939 2020-07-06 05:04:31.000000 tshirt-0.3.1/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2669 2020-07-12 04:40:36.000000 tshirt-0.3.1/docs/spec_pipeline/batch_processing.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     4557 2022-08-05 00:10:07.000000 tshirt-0.3.1/docs/spec_pipeline/parameter_file.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      481 2020-07-12 04:40:36.000000 tshirt-0.3.1/docs/spec_pipeline/spec_pipeline.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)    34730 2020-07-13 07:19:44.000000 tshirt-0.3.1/docs/spec_pipeline/test_spec_pipeline.ipynb
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.765077 tshirt-0.3.1/docs/specific_modules/
--rw-r--r--   0 everettschlawin   (501) staff       (20)    36491 2022-01-18 07:07:34.000000 tshirt-0.3.1/docs/specific_modules/ROEBA.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)      182 2022-01-18 07:09:23.000000 tshirt-0.3.1/docs/specific_modules/specific_modules.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       38 2023-11-17 19:12:50.777310 tshirt-0.3.1/setup.cfg
--rw-r--r--   0 everettschlawin   (501) staff       (20)      869 2023-11-17 18:40:12.000000 tshirt-0.3.1/setup.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.767238 tshirt-0.3.1/tshirt/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      120 2023-11-17 18:39:27.000000 tshirt-0.3.1/tshirt/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      212 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/allk1255_centroid.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.768016 tshirt-0.3.1/tshirt/chisquare/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/chisquare/directory_placeholder.dat
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.768291 tshirt-0.3.1/tshirt/cleaned_tser/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/cleaned_tser/directory_placeholder.dat
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.768722 tshirt-0.3.1/tshirt/directory_info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2326 2023-08-04 16:38:50.000000 tshirt-0.3.1/tshirt/directory_info/directory_list.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1081 2021-12-03 07:54:32.000000 tshirt-0.3.1/tshirt/directory_info/example_data_list.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)      767 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/example_fits.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.756291 tshirt-0.3.1/tshirt/existing_dat/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.769033 tshirt-0.3.1/tshirt/existing_dat/spectra/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      738 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/existing_dat/spectra/fratio_yang2016.csv
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2122 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/fit_models.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    52675 2020-06-14 23:10:48.000000 tshirt-0.3.1/tshirt/fit_tser_emcee.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     6638 2020-10-16 22:10:25.000000 tshirt-0.3.1/tshirt/mie_model.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.769297 tshirt-0.3.1/tshirt/parameters/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      308 2020-07-12 22:57:27.000000 tshirt-0.3.1/tshirt/parameters/fit_params.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.769446 tshirt-0.3.1/tshirt/parameters/mie_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      434 2020-07-12 22:57:38.000000 tshirt-0.3.1/tshirt/parameters/mie_params/simplePoly.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.770116 tshirt-0.3.1/tshirt/parameters/phot_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2385 2020-07-12 22:54:25.000000 tshirt-0.3.1/tshirt/parameters/phot_params/example_batch_phot.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3425 2021-08-17 21:22:42.000000 tshirt-0.3.1/tshirt/parameters/phot_params/example_phot_parameters.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)      423 2020-07-12 22:53:44.000000 tshirt-0.3.1/tshirt/parameters/phot_params/keywords_for_phot_pipeline.csv
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.770968 tshirt-0.3.1/tshirt/parameters/phot_params/test_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2558 2021-04-13 04:23:56.000000 tshirt-0.3.1/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2924 2021-04-13 04:23:56.000000 tshirt-0.3.1/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2479 2021-07-03 05:50:30.000000 tshirt-0.3.1/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2483 2021-12-03 07:54:32.000000 tshirt-0.3.1/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.771185 tshirt-0.3.1/tshirt/parameters/reduction_parameters/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      456 2020-07-12 22:55:39.000000 tshirt-0.3.1/tshirt/parameters/reduction_parameters/example_reduction_parameters.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.771722 tshirt-0.3.1/tshirt/parameters/spec_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     5216 2023-09-14 18:56:16.000000 tshirt-0.3.1/tshirt/parameters/spec_params/default_params.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1847 2020-07-12 22:55:24.000000 tshirt-0.3.1/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1888 2020-07-13 07:19:44.000000 tshirt-0.3.1/tshirt/parameters/spec_params/example_spec_parameters.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.771880 tshirt-0.3.1/tshirt/parameters/spec_params/test_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2196 2021-03-29 20:26:21.000000 tshirt-0.3.1/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)       50 2020-07-12 22:57:46.000000 tshirt-0.3.1/tshirt/parameters/telluric_bands.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.774558 tshirt-0.3.1/tshirt/pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       56 2020-10-29 18:02:05.000000 tshirt-0.3.1/tshirt/pipeline/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    10465 2020-12-19 05:05:58.000000 tshirt-0.3.1/tshirt/pipeline/analysis.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3825 2021-09-30 04:43:40.000000 tshirt-0.3.1/tshirt/pipeline/fit_2dgauss.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.775695 tshirt-0.3.1/tshirt/pipeline/instrument_specific/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       84 2021-12-17 05:29:57.000000 tshirt-0.3.1/tshirt/pipeline/instrument_specific/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2020-02-22 00:15:21.000000 tshirt-0.3.1/tshirt/pipeline/instrument_specific/check_wavecal.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2542 2020-08-04 02:08:51.000000 tshirt-0.3.1/tshirt/pipeline/instrument_specific/hst_inst_funcs.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3982 2023-08-04 16:38:50.000000 tshirt-0.3.1/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    13895 2023-11-17 16:56:16.000000 tshirt-0.3.1/tshirt/pipeline/instrument_specific/rowamp_sub.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)   107050 2023-10-17 23:09:21.000000 tshirt-0.3.1/tshirt/pipeline/phot_pipeline.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    15131 2022-01-18 07:02:08.000000 tshirt-0.3.1/tshirt/pipeline/prep_images.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2878 2022-07-09 15:42:59.000000 tshirt-0.3.1/tshirt/pipeline/sim_data.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)   134581 2023-08-17 05:28:29.000000 tshirt-0.3.1/tshirt/pipeline/spec_pipeline.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    13318 2021-12-03 07:54:32.000000 tshirt-0.3.1/tshirt/pipeline/utils.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1446 2019-02-19 20:21:03.000000 tshirt-0.3.1/tshirt/quick_timeit.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      449 2020-06-14 23:28:01.000000 tshirt-0.3.1/tshirt/specific_fits.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.776778 tshirt-0.3.1/tshirt/tests/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     5527 2022-01-18 06:52:08.000000 tshirt-0.3.1/tshirt/tests/test_phot_algorithms.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2889 2021-10-14 22:43:01.000000 tshirt-0.3.1/tshirt/tests/test_pipe_basics.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      244 2021-12-03 07:54:32.000000 tshirt-0.3.1/tshirt/tests/test_rowamp_sub.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      957 2021-10-14 23:26:52.000000 tshirt-0.3.1/tshirt/tests/test_window_placement.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3232 2020-11-30 06:14:07.000000 tshirt-0.3.1/tshirt/tser_tests.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-11-17 19:12:50.767913 tshirt-0.3.1/tshirt.egg-info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1134 2023-11-17 19:12:50.000000 tshirt-0.3.1/tshirt.egg-info/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2894 2023-11-17 19:12:50.000000 tshirt-0.3.1/tshirt.egg-info/SOURCES.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2023-11-17 19:12:50.000000 tshirt-0.3.1/tshirt.egg-info/dependency_links.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)       98 2023-11-17 19:12:50.000000 tshirt-0.3.1/tshirt.egg-info/requires.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        7 2023-11-17 19:12:50.000000 tshirt-0.3.1/tshirt.egg-info/top_level.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:22.004647 tshirt-0.4/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       40 2017-01-16 05:08:31.000000 tshirt-0.4/.gitattributes
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1803 2021-07-03 05:50:30.000000 tshirt-0.4/.gitignore
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        0 2020-02-18 20:41:06.000000 tshirt-0.4/.gitmodules
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1073 2020-07-06 05:04:56.000000 tshirt-0.4/LICENSE
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       30 2020-09-13 03:03:55.000000 tshirt-0.4/MANIFEST.in
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1225 2024-05-09 16:42:22.004433 tshirt-0.4/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      989 2023-11-20 05:39:19.000000 tshirt-0.4/README.md
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.982703 tshirt-0.4/docs/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      634 2020-06-22 23:17:25.000000 tshirt-0.4/docs/Makefile
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2262 2024-05-09 16:40:53.000000 tshirt-0.4/docs/conf.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.982991 tshirt-0.4/docs/images/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   176987 2020-06-23 17:58:22.000000 tshirt-0.4/docs/images/t_shirt_logo.jpg
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1013 2022-01-18 07:12:31.000000 tshirt-0.4/docs/index.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3631 2022-01-18 07:20:02.000000 tshirt-0.4/docs/installation.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      795 2020-06-22 23:17:25.000000 tshirt-0.4/docs/make.bat
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      973 2023-11-19 20:53:15.000000 tshirt-0.4/docs/modules.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.987748 tshirt-0.4/docs/phot_pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    37697 2020-07-12 04:40:36.000000 tshirt-0.4/docs/phot_pipeline/box_time_series_cookbook.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      439 2020-07-12 04:40:36.000000 tshirt-0.4/docs/phot_pipeline/example_phot_param_file.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      397 2020-07-12 04:40:36.000000 tshirt-0.4/docs/phot_pipeline/phot_pipeline.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5995 2023-09-14 18:51:30.000000 tshirt-0.4/docs/phot_pipeline/phot_pipeline_parameters.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1049 2021-03-29 20:26:21.000000 tshirt-0.4/docs/phot_pipeline/running_phot_pipeline.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.988073 tshirt-0.4/docs/reduction/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      915 2021-02-18 21:10:57.000000 tshirt-0.4/docs/reduction/reduction.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      178 2020-06-23 18:40:40.000000 tshirt-0.4/docs/reduction/reduction_param.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       88 2023-11-19 20:54:31.000000 tshirt-0.4/docs/requirements.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.991510 tshirt-0.4/docs/spec_pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   921939 2020-07-06 05:04:31.000000 tshirt-0.4/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2669 2020-07-12 04:40:36.000000 tshirt-0.4/docs/spec_pipeline/batch_processing.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5224 2024-05-09 16:40:53.000000 tshirt-0.4/docs/spec_pipeline/parameter_file.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      481 2020-07-12 04:40:36.000000 tshirt-0.4/docs/spec_pipeline/spec_pipeline.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    34730 2020-07-13 07:19:44.000000 tshirt-0.4/docs/spec_pipeline/test_spec_pipeline.ipynb
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.992726 tshirt-0.4/docs/specific_modules/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    36491 2022-01-18 07:07:34.000000 tshirt-0.4/docs/specific_modules/ROEBA.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      182 2022-01-18 07:09:23.000000 tshirt-0.4/docs/specific_modules/specific_modules.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       38 2024-05-09 16:42:22.004689 tshirt-0.4/setup.cfg
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      867 2024-05-09 16:40:53.000000 tshirt-0.4/setup.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.995678 tshirt-0.4/tshirt/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      118 2024-05-09 16:40:53.000000 tshirt-0.4/tshirt/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      212 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/allk1255_centroid.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.996322 tshirt-0.4/tshirt/chisquare/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/chisquare/directory_placeholder.dat
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.996531 tshirt-0.4/tshirt/cleaned_tser/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/cleaned_tser/directory_placeholder.dat
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.996942 tshirt-0.4/tshirt/directory_info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2326 2023-08-04 16:38:50.000000 tshirt-0.4/tshirt/directory_info/directory_list.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1081 2021-12-03 07:54:32.000000 tshirt-0.4/tshirt/directory_info/example_data_list.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      767 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/example_fits.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.979075 tshirt-0.4/tshirt/existing_dat/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.997183 tshirt-0.4/tshirt/existing_dat/spectra/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      738 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/existing_dat/spectra/fratio_yang2016.csv
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2122 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/fit_models.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    52675 2020-06-14 23:10:48.000000 tshirt-0.4/tshirt/fit_tser_emcee.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     6638 2020-10-16 22:10:25.000000 tshirt-0.4/tshirt/mie_model.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.997514 tshirt-0.4/tshirt/parameters/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      308 2020-07-12 22:57:27.000000 tshirt-0.4/tshirt/parameters/fit_params.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.997676 tshirt-0.4/tshirt/parameters/mie_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      434 2020-07-12 22:57:38.000000 tshirt-0.4/tshirt/parameters/mie_params/simplePoly.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.998083 tshirt-0.4/tshirt/parameters/phot_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2385 2020-07-12 22:54:25.000000 tshirt-0.4/tshirt/parameters/phot_params/example_batch_phot.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3425 2021-08-17 21:22:42.000000 tshirt-0.4/tshirt/parameters/phot_params/example_phot_parameters.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      423 2020-07-12 22:53:44.000000 tshirt-0.4/tshirt/parameters/phot_params/keywords_for_phot_pipeline.csv
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.998630 tshirt-0.4/tshirt/parameters/phot_params/test_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2558 2021-04-13 04:23:56.000000 tshirt-0.4/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2924 2021-04-13 04:23:56.000000 tshirt-0.4/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2479 2021-07-03 05:50:30.000000 tshirt-0.4/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2483 2021-12-03 07:54:32.000000 tshirt-0.4/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.998813 tshirt-0.4/tshirt/parameters/reduction_parameters/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      456 2020-07-12 22:55:39.000000 tshirt-0.4/tshirt/parameters/reduction_parameters/example_reduction_parameters.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.999357 tshirt-0.4/tshirt/parameters/spec_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5360 2024-05-09 16:40:53.000000 tshirt-0.4/tshirt/parameters/spec_params/default_params.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1847 2020-07-12 22:55:24.000000 tshirt-0.4/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1888 2020-07-13 07:19:44.000000 tshirt-0.4/tshirt/parameters/spec_params/example_spec_parameters.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:21.999516 tshirt-0.4/tshirt/parameters/spec_params/test_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2196 2021-03-29 20:26:21.000000 tshirt-0.4/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       50 2020-07-12 22:57:46.000000 tshirt-0.4/tshirt/parameters/telluric_bands.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:22.002068 tshirt-0.4/tshirt/pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       56 2020-10-29 18:02:05.000000 tshirt-0.4/tshirt/pipeline/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    10465 2020-12-19 05:05:58.000000 tshirt-0.4/tshirt/pipeline/analysis.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3825 2021-09-30 04:43:40.000000 tshirt-0.4/tshirt/pipeline/fit_2dgauss.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:22.003062 tshirt-0.4/tshirt/pipeline/instrument_specific/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       84 2021-12-17 05:29:57.000000 tshirt-0.4/tshirt/pipeline/instrument_specific/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2020-02-22 00:15:21.000000 tshirt-0.4/tshirt/pipeline/instrument_specific/check_wavecal.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2542 2020-08-04 02:08:51.000000 tshirt-0.4/tshirt/pipeline/instrument_specific/hst_inst_funcs.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     4858 2024-05-09 16:40:53.000000 tshirt-0.4/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    13895 2023-11-17 16:56:16.000000 tshirt-0.4/tshirt/pipeline/instrument_specific/rowamp_sub.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   107050 2024-03-18 21:29:30.000000 tshirt-0.4/tshirt/pipeline/phot_pipeline.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    15131 2022-01-18 07:02:08.000000 tshirt-0.4/tshirt/pipeline/prep_images.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2878 2022-07-09 15:42:59.000000 tshirt-0.4/tshirt/pipeline/sim_data.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   136438 2024-05-09 16:40:53.000000 tshirt-0.4/tshirt/pipeline/spec_pipeline.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    13318 2021-12-03 07:54:32.000000 tshirt-0.4/tshirt/pipeline/utils.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1446 2019-02-19 20:21:03.000000 tshirt-0.4/tshirt/quick_timeit.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      449 2020-06-14 23:28:01.000000 tshirt-0.4/tshirt/specific_fits.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:22.003983 tshirt-0.4/tshirt/tests/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5527 2022-01-18 06:52:08.000000 tshirt-0.4/tshirt/tests/test_phot_algorithms.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2889 2021-10-14 22:43:01.000000 tshirt-0.4/tshirt/tests/test_pipe_basics.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      244 2021-12-03 07:54:32.000000 tshirt-0.4/tshirt/tests/test_rowamp_sub.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      957 2021-10-14 23:26:52.000000 tshirt-0.4/tshirt/tests/test_window_placement.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3232 2020-11-30 06:14:07.000000 tshirt-0.4/tshirt/tser_tests.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2024-05-09 16:42:22.004177 tshirt-0.4/tshirt.egg-info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1225 2024-05-09 16:42:21.000000 tshirt-0.4/tshirt.egg-info/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2894 2024-05-09 16:42:21.000000 tshirt-0.4/tshirt.egg-info/SOURCES.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2024-05-09 16:42:21.000000 tshirt-0.4/tshirt.egg-info/dependency_links.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       98 2024-05-09 16:42:21.000000 tshirt-0.4/tshirt.egg-info/requires.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        7 2024-05-09 16:42:21.000000 tshirt-0.4/tshirt.egg-info/top_level.txt
```

### Comparing `tshirt-0.3.1/.gitignore` & `tshirt-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/LICENSE` & `tshirt-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/PKG-INFO` & `tshirt-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: tshirt
-Version: 0.3.1
+Version: 0.4
 Summary: A package to analyze time series data, especially for exoplanets
 Home-page: https://github.com/eas342/tshirt
 Author: Everett Schlawin, Kayli Glidic
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.15
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: astropy>=2.0
 Requires-Dist: tqdm>=4.46.0
 Requires-Dist: photutils>=0.4.1
 Requires-Dist: bokeh>=1.4.0
 Requires-Dist: pytest
 Requires-Dist: celerite2
 
+   <img src="docs/images/t_shirt_logo.jpg" alt="T shirt logot" width="200 px">
+   </br>
+</p>
 
 `tshirt` README
 ==========================================
 The Time Series Helper & Integration Reduction Tool `tshirt` is a general-purpose tool for time series science.
 Its main application is to process raw data on exoplanet systems.
 `tshirt` can:
```

### Comparing `tshirt-0.3.1/README.md` & `tshirt-0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![PyPI status](https://img.shields.io/pypi/v/tshirt.svg)](https://pypi.python.org/pypi/tshirt/)
+[![Documentation Status](https://readthedocs.org/projects/tshirt/badge/?version=latest)](http://tshirt.readthedocs.io/?badge=latest)
+
 <p align="center">
    <img src="docs/images/t_shirt_logo.jpg" alt="T shirt logot" width="200 px">
    </br>
 </p>
 
 `tshirt` README
 ==========================================
```

### Comparing `tshirt-0.3.1/docs/Makefile` & `tshirt-0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/conf.py` & `tshirt-0.4/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'tshirt'
 copyright = '2020, Everett Schlawin'
 author = 'Everett Schlawin'
 
 # The full version, including alpha/beta/rc tags
-release = '0.3.1'
+release = '0.4'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `tshirt-0.3.1/docs/images/t_shirt_logo.jpg` & `tshirt-0.4/docs/images/t_shirt_logo.jpg`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/index.rst` & `tshirt-0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/installation.rst` & `tshirt-0.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/make.bat` & `tshirt-0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/modules.rst` & `tshirt-0.4/docs/modules.rst`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. automodule:: tshirt.pipeline.instrument_specific.hst_inst_funcs
    :members:
 
 .. automodule:: tshirt.pipeline.instrument_specific.jwst_inst_funcs
    :members:
 
+.. automodule:: tshirt.pipeline.instrument_specific.rowamp_sub
+   :members:
+
 
 Image Preparation Module
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. automodule:: tshirt.pipeline.prep_images
    :members:
 
 Pipeline Utilities
```

### Comparing `tshirt-0.3.1/docs/phot_pipeline/box_time_series_cookbook.ipynb` & `tshirt-0.4/docs/phot_pipeline/box_time_series_cookbook.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/phot_pipeline/phot_pipeline_parameters.rst` & `tshirt-0.4/docs/phot_pipeline/phot_pipeline_parameters.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/phot_pipeline/running_phot_pipeline.rst` & `tshirt-0.4/docs/phot_pipeline/running_phot_pipeline.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/reduction/reduction.rst` & `tshirt-0.4/docs/reduction/reduction.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb` & `tshirt-0.4/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/spec_pipeline/batch_processing.rst` & `tshirt-0.4/docs/spec_pipeline/batch_processing.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/spec_pipeline/parameter_file.rst` & `tshirt-0.4/docs/spec_pipeline/parameter_file.rst`

 * *Files 13% similar despite different names*

```diff
@@ -76,11 +76,34 @@
 ~~~~~~~~~~~~~~~~~~~~~~~
 If True, save the spatial profile centroid and FWHM for de-trending from the median profile. If False, those are populated with NaN.
 
 profilePix
 ~~~~~~~~~~
 If None, all dispersion pixels (along the wavelength direction) are used in calculating spatial profile statistics. If a 2 element list like :code:`[50,100]`, pixels 50 through 100 in the dispersion/wavelength direction will be used to measure the spatial profile statistics. Note that this only has an effect if :code:`saveSpatialProfileStats` is :code:`True` and this will not affect the extraction in current versions of tshirt. It will ony affect the saved profile statistics.
 
+profileFitWidth
+~~~~~~~~~~~~~~~
+If None, the profile fit width is the `apWidth`. Otherwise, it can be customized here by profileFitWidth for the full size in the spatial direction ( in pixels).
+
 useSmoothProfileForStats
 ~~~~~~~~~~~~~~~~~~~~~~~~
 Use the smoothed profile for the profile statistics? If True, the statistics will be on the man profile along the dispersion direction. Otherwise, a median of the data is calculated. Note that if :code:`fixedProfile` is True, this will give constant statistics for all images
 
+traceCurvedSpectrum
+~~~~~~~~~~~~~~~~~~~~
+Trace a curved spectrum? If True, allows a curved aperture instead of a rectangular one
+
+traceOrder
+~~~~~~~~~~~
+Polynomial order for the trace fitting
+
+traceFitBoxSize
+~~~~~~~~~~~~~~~~
+The spatial box size used to fit the trace
+
+traceFWHMguess
+~~~~~~~~~~~~~~
+Guess size for the spatial FWHM when fitting to a Gaussian
+
+traceReference
+~~~~~~~~~~~~~~
+If you want to use the trace from a previous file, give the path name as a string
```

### Comparing `tshirt-0.3.1/docs/spec_pipeline/test_spec_pipeline.ipynb` & `tshirt-0.4/docs/spec_pipeline/test_spec_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/docs/specific_modules/ROEBA.ipynb` & `tshirt-0.4/docs/specific_modules/ROEBA.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/setup.py` & `tshirt-0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     ## skip the HTML, which doesn't work on PyPI
     long_description = "".join(fh.readlines()[4:])
 
 setup(
     name='tshirt',
-    version='0.3.1',
+    version='0.4',
     author='Everett Schlawin, Kayli Glidic',
     packages=['tshirt','tshirt.pipeline',
               'tshirt.pipeline.instrument_specific'],
     url="https://github.com/eas342/tshirt",
     description="A package to analyze time series data, especially for exoplanets",
     include_package_data=True,
     install_requires=[
```

### Comparing `tshirt-0.3.1/tshirt/directory_info/directory_list.yaml` & `tshirt-0.4/tshirt/directory_info/directory_list.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/directory_info/example_data_list.txt` & `tshirt-0.4/tshirt/directory_info/example_data_list.txt`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/example_fits.py` & `tshirt-0.4/tshirt/example_fits.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/existing_dat/spectra/fratio_yang2016.csv` & `tshirt-0.4/tshirt/existing_dat/spectra/fratio_yang2016.csv`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/fit_models.py` & `tshirt-0.4/tshirt/fit_models.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/fit_tser_emcee.py` & `tshirt-0.4/tshirt/fit_tser_emcee.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/mie_model.py` & `tshirt-0.4/tshirt/mie_model.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/example_batch_phot.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/example_batch_phot.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/example_phot_parameters.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/example_phot_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml` & `tshirt-0.4/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/spec_params/default_params.yaml` & `tshirt-0.4/tshirt/parameters/spec_params/default_params.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -55,16 +55,18 @@
 superWeights: False ## Use (S/N)^2 to weight instead of optimal extraction
 fixedProfile: False ## Use a fixed profile for all images?
 readFromTshirtExamples: False ## read the data from T-shirt examples within the package? Use only for examples.
 saveRefRow: False ## save rows of reference pixels?
 dateKeyword: DATE-OBS ## default FITS keyword to find date/time information from
 DATE-OBS: None ## manually supply a DATE-OBS if nothing is available in the header
 saveSpatialProfileStats: False ## save the spatial profile stats
-profilePix: null ## the pixels to use in calculating the spatial profile statistics (not used in extraction)
+profilePix: null ## the dispersion pixels to use in calculating the spatial profile statistics (not used in extraction)
+profileFitWidth: null ## the spatial profile width in calculating spatial profile statistics
 useSmoothProfileForStats: False ## use the spline-smoothed profile for profile statistics?
 traceCurvedSpectrum: False ## Fit the trace to the spectrum?
 traceOrder: 3 ## polynomial order for the trace fitting
 traceFitBoxSize: 18 ## the spatial box size used to fit the trace
 traceFWHMguess: 2 ## Guess size for the spatial FWHM
+traceReference: null ## Reference trace
 backgMinRadius: 5 ## minimum distance for background
 skyPositions: None ## use RA and Dec for positions (only works for photometry though)
 downselectImgWithCoord: False ## Check images for source w/ coordinates (only works for photometry though)
```

### Comparing `tshirt-0.3.1/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml` & `tshirt-0.4/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/spec_params/example_spec_parameters.yaml` & `tshirt-0.4/tshirt/parameters/spec_params/example_spec_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml` & `tshirt-0.4/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/analysis.py` & `tshirt-0.4/tshirt/pipeline/analysis.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/fit_2dgauss.py` & `tshirt-0.4/tshirt/pipeline/fit_2dgauss.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/instrument_specific/check_wavecal.py` & `tshirt-0.4/tshirt/pipeline/instrument_specific/check_wavecal.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/instrument_specific/hst_inst_funcs.py` & `tshirt-0.4/tshirt/pipeline/instrument_specific/hst_inst_funcs.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py` & `tshirt-0.4/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py`

 * *Files 20% similar despite different names*

```diff
@@ -110,8 +110,31 @@
         domain = np.array([   0., 2047.])
     else:
         raise NotImplementedError
     
     poly_fun = np.polynomial.Polynomial(coeff,domain=domain)
     return poly_fun(pixels)
 
-    
+def miri_lrs(pixels):
+    """
+    Polynomial fit to transformed Y coordinate
+
+    ## See this file
+    /Users/~/Documents/jwst/flight_data/proc/01185/wasp69b_proc/miri_lrs_rate/lrs_wavecal.ipynb
+    I ran wcs_step = assign_wcs.AssignWcsStep()
+    Then calculated wavelengths with:
+    xcor,ycor,wavearr = wcs_res.meta.wcs(37 * np.ones(NY),y_array)
+    """
+    input_arr = np.array(pixels)
+    good_pt = input_arr <= 394.
+    y_transform =  np.array((394. - input_arr[good_pt])**0.5)
+    coeff = np.array([-4.33398729e-08,  2.68709385e-06, -4.92122230e-05, -2.30504962e-04,
+                       1.67742638e-02,  3.77253454e-01,  3.80071027e+00])
+    poly_fun = np.polyval(coeff,y_transform)
+    output_arr = np.zeros(input_arr.size) * np.nan
+    
+    output_arr[good_pt] = poly_fun
+    
+    
+    if (input_arr.ndim == 0):
+        output_arr = output_arr[0]
+    return output_arr
```

### Comparing `tshirt-0.3.1/tshirt/pipeline/instrument_specific/rowamp_sub.py` & `tshirt-0.4/tshirt/pipeline/instrument_specific/rowamp_sub.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/phot_pipeline.py` & `tshirt-0.4/tshirt/pipeline/phot_pipeline.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/prep_images.py` & `tshirt-0.4/tshirt/pipeline/prep_images.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/sim_data.py` & `tshirt-0.4/tshirt/pipeline/sim_data.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/pipeline/spec_pipeline.py` & `tshirt-0.4/tshirt/pipeline/spec_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 import yaml
 import warnings
 from scipy.stats import binned_statistic
 from scipy.stats import norm
 from scipy.interpolate import interp1d
 import astropy
 from astropy.table import Table
-from astropy.stats import LombScargle
+try:
+    from astropy.stats import LombScargle
+except ImportError as errLS:
+    from astropy.timeseries import LombScargle
 import multiprocessing
 from multiprocessing import Pool
 import tqdm
 try:
     import bokeh.plotting
     from bokeh.models import ColumnDataSource, HoverTool
     from bokeh.models import Range1d
@@ -117,19 +120,25 @@
         
         wavebin_fileName_prefix = 'wavebin_spec_{}'.format(self.dataFileDescrip)
         self.wavebin_file_prefix = os.path.join(self.baseDir,'tser_data','wavebin_spec',
                                                 wavebin_fileName_prefix)
         
         self.profile_dir = os.path.join(self.baseDir,'tser_data','saved_profiles')
         self.weight_dir = os.path.join(self.baseDir,'tser_data','saved_weights')
-        
-        self.traceFile = os.path.join(self.baseDir,'traces','trace_functions',
-                                      'trace_'+self.dataFileDescrip+'.ecsv')
-        self.traceDataFile = os.path.join(self.baseDir,'traces','trace_data',
-                                          'trace_data_'+self.dataFileDescrip+'.ecsv')
+
+        self.traceReference = self.param['traceReference']
+        if self.traceReference is None:
+            self.traceFile = os.path.join(self.baseDir,'traces','trace_functions',
+                                        'trace_'+self.dataFileDescrip+'.ecsv')
+            self.traceDataFile = os.path.join(self.baseDir,'traces','trace_data',
+                                            'trace_data_'+self.dataFileDescrip+'.ecsv')
+        else:
+            self.traceDataFile = None
+            self.traceFile = self.traceReference
+
         self.check_trace_requirements()
 
         self.master_profile_prefix = 'master_{}'.format(self.dataFileDescrip)
         #self.centroidFile = 'centroids/cen_'+self.dataFileDescrip+'.fits'
         #self.refCorPhotFile = 'tser_data/refcor_phot/refcor_'+self.dataFileDescrip+'.fits'
         self.get_summation_direction()
         
@@ -264,14 +273,16 @@
         return medImg, head
 
 
     def do_extraction(self,useMultiprocessing=False):
         """
         Extract all spectroscopy
         """
+        from ..__init__ import __version__
+        
         fileCountArray = np.arange(self.nImg)
         
         if self.param['fixedProfile'] == True:
             if (self.nImg > self.param['nImgForProfile']) & (self.param['nImgForProfile'] > 1):
                 img, head = self.get_median_img(self.param['nImgForProfile'])
             else:
                 img, head = self.get_default_im()
@@ -346,14 +357,15 @@
         hdu.header['NSOURCE'] = (self.nsrc,'Number of sources with spectroscopy')
         hdu.header['NIMG'] = (self.nImg,'Number of images')
         hdu.header['AXIS1'] = ('disp','dispersion axis')
         hdu.header['AXIS2'] = ('image','image axis')
         hdu.header['AXIS3'] = ('src','source axis')
         hdu.header['SRCNAME'] = (self.param['srcName'], 'Source name')
         hdu.header['NIGHT'] = (self.param['nightName'], 'Night Name')
+        hdu.header['TSHIRTV'] = (__version__,'tshirt version number')
         hdu.name = 'Optimal Spec'
         
         hdu.header = self.add_parameters_to_header(hdu.header)
         
         hduOptErr = fits.ImageHDU(optSpec_err,hdu.header)
         hduOptErr.name = 'Opt Spec Err'
         
@@ -666,15 +678,18 @@
             if numSubtractions == 1:
                 if self.param['dispDirection'] == 'x':
                     assert (self.param['bkgSubDirections'][0] == 'Y'),'x dispersion must have Y backsub'
                     assert (len(self.param['bkgRegionsY']) == 1),'Must have 1 subtraction only'
                 else:
                     assert (self.param['bkgSubDirections'][0] == 'X'),'y dispersion must have X backsub'
                     assert (len(self.param['bkgRegionsX']) == 1),'Must have 1 subtraction only'
-
+        if self.traceReference is None:
+            pass
+        else:
+            assert os.path.exists(self.traceReference), 'Trace Reference not found'
 
     def eval_trace(self,dispArray,src=0):
         """
         Evaluate the trace function
         
         Parameters
         ------------
@@ -687,24 +702,27 @@
             spatial_position = np.polyval(poly1,np.array(dispArray))
         else:
             spatial_position = self.param['starPositions'][src] * np.ones_like(dispArray,dtype=int)
         return spatial_position
         
 
     def find_trace(self,recalculateTrace=False,
-                   recalculateTraceData=False):
+                   recalculateTraceData=False,
+                   showPlot=False):
         """
         Find the trace either from saved file or trace data
 
         Parameters
         -----------
         recalculateTrace: bool
             Recalculate the trace?
         recalculateTraceData: bool
             Recalculate the trace data?
+        showPlot: bool
+            Show plot of fitting the trace?
         """
         if (os.path.exists(self.traceFile) == True) & (recalculateTrace == False):
             pass
         else:
             if (os.path.exists(self.traceDataFile) == True) & (recalculateTraceData == False):
                 pass
             else:
@@ -720,15 +738,22 @@
                 tracePoly = phot_pipeline.robust_poly(traceData['x'],
                                                       traceData['cen {}'.format(oneSrc)],
                                                       traceOrder)
                 tpoly['poly {}'.format(oneSrc)] = tracePoly
             tpoly.write(self.traceFile,overwrite=True)
 
         self.traceInfo = ascii.read(self.traceFile)
-
+        if showPlot == True:
+            traceData = ascii.read(self.traceDataFile)
+            
+            for oneSrc in np.arange(self.nsrc):
+                plt.plot(traceData['x'],traceData['cen {}'.format(oneSrc)],'o')
+                y_eval = self.eval_trace(traceData['x'],src=oneSrc)
+                plt.plot(traceData['x'],y_eval)
+            plt.show()
 
     def fit_trace(self,img,head,showEach=False,
                    fitMethod='astropy'):
         """
         Use Gaussian to fit trace and FWHM
 
         Parameters
@@ -739,19 +764,19 @@
             FITS header to do fitting on
         showEach: bool
             Show each line fit?
         fitMethod: str
             'astropy' : will use models Gaussian2D + linear
             'sckpyQuick' : will fit w/ scipy.stats.norm
         """
-        dispDirection =  self.param['dispDirection']
-        if dispDirection.upper() == 'Y':
+        dispDirection = self.param['dispDirection'].upper()
+        if dispDirection == 'Y':
             spatialIndexArrayLength = img.shape[1]
 #            dispersionIndexArrayLength = img.shape[0]
-        elif dispDirection.upper() == 'X':
+        elif dispDirection == 'X':
             spatialIndexArrayLength = img.shape[0]
  #           dispersionIndexArrayLength = img.shape[1]
         else:
             raise Exception("Unrecognized spatial direction")
         ## eventually use self.param['dispOffsets'][srcInd]
         dispStart, dispEnd = self.param['dispPixels']
         dispersionIndexArrayLength = int(dispEnd - dispStart)
@@ -798,15 +823,15 @@
                 ind_var = spatialIndexArray ## independent variable
                 if dispDirection == 'Y':
                     dep_var = img[dispersion_Ind,:]
                 else:
                     dep_var = img[:,dispersion_Ind]
 
                 
-                good_pts = np.isfinite(dep_var)
+                good_pts = np.isfinite(dep_var) & pts
                 spatial_profile = dep_var[good_pts]
                 if np.sum(good_pts) < 5:
                     cenArr[dispersion_counter,srcInd] = np.nan
                     fwhmArr[dispersion_counter,srcInd] = np.nan
                     dep_var_model = np.ones_like(dep_var) * np.nan
                 elif fitMethod == 'astropy':
                     fitter = fitting.LevMarLSQFitter()
@@ -845,15 +870,15 @@
                 # if dispDirection == 'Y':
                 #     bkgModel[dispersion_Ind,ind_var[ptsTofit]] = dep_var_model[ptsTofit]
                 # else:
                 #     bkgModel[ind_var[ptsTofit],dispersion_Ind] = dep_var_model[ptsTofit]
                 
                 if showEach == True:
                     plt.plot(ind_var,dep_var,label='data')
-                    plt.plot(ind_var[pts],dep_var[pts],'o',color='red',label='pts fit')
+                    plt.plot(ind_var[good_pts],dep_var[good_pts],'o',color='red',label='pts fit')
                     plt.plot(ind_var,dep_var_model(ind_var),label='model')
                     plt.show()
                     pdb.set_trace()
                 disperion_counter = dispersion_counter + 1
 
         t = Table()
         t['x'] = dispersionIndexArray
@@ -1011,15 +1036,15 @@
             
             ## Renormalize            
             norm_profile = self.profile_normalize(profile_img)
             profile_img_list.append(norm_profile)
             
             ## save the smoothed image
             smooth_img_list.append(smooth_img)
-                
+
         if saveFits == True:
             primHDU = fits.PrimaryHDU(img,head)
             if masterProfile == True:
                 prefixName = self.master_profile_prefix
             elif ind == None:
                 prefixName = 'unnamed'
             else:
@@ -1262,15 +1287,15 @@
             profile_img = profile_img_list[oneSrc]
             smooth_img = smooth_img_list[oneSrc]
             
             ## Find the bad pixels and their missing weights
             finitep = (np.isfinite(img) & np.isfinite(varImg) & np.isfinite(smooth_img))
             badPx = finitep == False ## start by marking NaNs as bad pixels
             ## also mark large deviations from profile fit
-            badPx[finitep] = np.abs(smooth_img[finitep] - img[finitep]) > self.param['sigForBadPx'] * np.sqrt(varImg[finitep])
+            badPx[finitep] = np.abs(smooth_img[finitep] - imgSub[finitep]) > self.param['sigForBadPx'] * np.sqrt(varImg[finitep])
             holey_profile = deepcopy(profile_img)
             holey_profile[badPx] = 0.
             holey_weights = np.sum(holey_profile,self.spatialAx)
             correctionFactor = np.ones_like(holey_weights)
             goodPts = holey_weights > 0.
             correctionFactor[goodPts] = 1./holey_weights[goodPts]
             
@@ -1383,16 +1408,21 @@
                 profDispStart = profDispStart_0 + self.dispOffsets[oneSrc]
                 profDispEnd = profDispEnd_0 + self.dispOffsets[oneSrc]
                 
                 profilePix = ((dispIndices > profDispStart) &
                              (dispIndices <= profDispEnd))
                 
                 oneSourcePos = self.param['starPositions'][oneSrc]
-                startSpatial = int(oneSourcePos - self.param['apWidth'] / 2.)
-                endSpatial = int(oneSourcePos + self.param['apWidth'] / 2.)
+                if self.param['profileFitWidth'] is None:
+                    spatialWidthToFit = self.param['apWidth']
+                else:
+                    spatialWidthToFit = self.param['profileFitWidth']
+                
+                startSpatial = int(oneSourcePos - spatialWidthToFit / 2.)
+                endSpatial = int(oneSourcePos + spatialWidthToFit / 2.)
                 spatial_var = np.arange(startSpatial,endSpatial) ## independent variable
                 
                 if self.param['useSmoothProfileForStats'] == True:
                     if self.param['dispDirection'] == 'x':
                         spatial_profile = np.nanmean(profile_img[startSpatial:endSpatial,profilePix],axis=1)
                     else:
                         spatial_profile = np.nanmean(profile_img[profilePix,startSpatial:endSpatial],axis=0)
@@ -2000,15 +2030,15 @@
         
         if showPlot == True:
             fig.show()
         else:
             outName = 'noise_spec_{}.pdf'.format(self.dataFileDescrip)
             outPath = os.path.join(self.baseDir,'plots','spectra','noise_spectrum',outName)
             print("Writing noise spectrum to {}".format(outPath))
-            fig.savefig(outPath,overwrite=True)
+            fig.savefig(outPath)
         if waveBin == False:
             HDUList.close()
         
         if returnNoiseSpec == True:
             t = Table()
             t['x'] = x_plot
             t['y'] = y
@@ -2941,14 +2971,16 @@
             else:
                 if 'FILTER' in head:
                     obsFilter = head['FILTER']
                 else:
                     warning.warn('No filter specified. Assuming F322W2')
                     obsFilter = 'F322W2'
             wavelengths = instrument_specific.jwst_inst_funcs.flight_poly_grismr_nc(dispIndices,obsFilter=obsFilter)
+        elif waveCalMethod == 'miri_lrs':
+            wavelengths = instrument_specific.jwst_inst_funcs.miri_lrs(dispIndices)
         else:
             raise Exception("Unrecognized wavelength calibration method {}".format(waveCalMethod))
             
         wavelengths = wavelengths - self.param['waveCalOffset']
         return wavelengths
         
     def inverse_wavecal(self,waveArr):
@@ -2968,23 +3000,39 @@
         Given a set of wavelengths centers and widths, find the pixels
         that will approximately give you those wavelengths, but with 
         no pixels repeated or skipped.
         """
         waveEdges = np.array(waveMid) - np.array(waveWidth) * 0.5
         waveEdges = np.append(waveEdges,waveMid[-1] + waveWidth[-1] * 0.5) ## last edge
         pxEdges = np.array(np.round(self.inverse_wavecal(waveEdges)),dtype=int)
+
         t = Table()
         t['px start'] = pxEdges[0:-1]
         t['px end'] = pxEdges[1:]
         t['wave start'] = self.wavecal(t['px start'])
         t['wave end'] = self.wavecal(t['px end'])
         t['px mid'] = (t['px start'] + t['px end'])/2.
         t['px width'] = t['px end'] - t['px start']
         t['wave mid'] = (t['wave start'] + t['wave end'])/2.
         t['wave width'] = t['wave end'] - t['wave start']
+
+        ## Check whether dispersion is negative
+        
+        if np.sum(t['px width'] < 0) == len(t):
+            ## Negative dispersion
+            t['px width'] = np.abs(t['px width'])
+            prevStart = deepcopy(t['px start'])
+            t['px start'] = t['px end']
+            t['px end'] = prevStart
+        elif np.sum(t['px width'] > 0) == len(t):
+            ## Positive dispersion
+            pass
+        else:
+            raise Exception("Detected zero or flipped dispersion")
+
         return t
     
     def make_constant_Rgrid(self,wStart=None,wEnd=None,Rfixed=100,plotBins=True):
         """
         Make an approximately constant R grid rounded to whole pixels
 
         Parameters
```

### Comparing `tshirt-0.3.1/tshirt/pipeline/utils.py` & `tshirt-0.4/tshirt/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/quick_timeit.py` & `tshirt-0.4/tshirt/quick_timeit.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/tests/test_phot_algorithms.py` & `tshirt-0.4/tshirt/tests/test_phot_algorithms.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/tests/test_pipe_basics.py` & `tshirt-0.4/tshirt/tests/test_pipe_basics.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/tests/test_window_placement.py` & `tshirt-0.4/tshirt/tests/test_window_placement.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt/tser_tests.py` & `tshirt-0.4/tshirt/tser_tests.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.3.1/tshirt.egg-info/PKG-INFO` & `tshirt-0.4/tshirt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: tshirt
-Version: 0.3.1
+Version: 0.4
 Summary: A package to analyze time series data, especially for exoplanets
 Home-page: https://github.com/eas342/tshirt
 Author: Everett Schlawin, Kayli Glidic
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.15
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: astropy>=2.0
 Requires-Dist: tqdm>=4.46.0
 Requires-Dist: photutils>=0.4.1
 Requires-Dist: bokeh>=1.4.0
 Requires-Dist: pytest
 Requires-Dist: celerite2
 
+   <img src="docs/images/t_shirt_logo.jpg" alt="T shirt logot" width="200 px">
+   </br>
+</p>
 
 `tshirt` README
 ==========================================
 The Time Series Helper & Integration Reduction Tool `tshirt` is a general-purpose tool for time series science.
 Its main application is to process raw data on exoplanet systems.
 `tshirt` can:
```

### Comparing `tshirt-0.3.1/tshirt.egg-info/SOURCES.txt` & `tshirt-0.4/tshirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

