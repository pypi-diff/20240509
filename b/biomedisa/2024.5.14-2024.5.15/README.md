# Comparing `tmp/biomedisa-2024.5.14.tar.gz` & `tmp/biomedisa-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedisa-2024.5.14.tar", last modified: Wed May  8 05:36:46 2024, max compression
+gzip compressed data, was "biomedisa-2024.5.15.tar", last modified: Wed May  8 08:42:17 2024, max compression
```

## Comparing `biomedisa-2024.5.14.tar` & `biomedisa-2024.5.15.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.119691 biomedisa-2024.5.14/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/LICENSE
--rw-r--r--   0 philipp   (1000) philipp   (1000)    11678 2024-05-08 05:36:46.119691 biomedisa-2024.5.14/PKG-INFO
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11069 2024-05-08 04:32:37.000000 biomedisa-2024.5.14/README.md
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      665 2024-05-08 05:36:13.000000 biomedisa-2024.5.14/pyproject.toml
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-08 05:36:46.119691 biomedisa-2024.5.14/setup.cfg
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.115691 biomedisa-2024.5.14/src/
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.115691 biomedisa-2024.5.14/src/biomedisa/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1690 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 05:31:06.000000 biomedisa-2024.5.14/src/biomedisa/__main__.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.115691 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/DataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-02-14 23:44:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/DataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/PredictDataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18192 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/active_contour.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.115691 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/assd.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30741 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/biomedisa_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13329 2024-05-06 01:26:56.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/create_slices.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    23894 2024-05-06 01:26:56.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/crop_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/curvop_numba.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8989 2024-04-30 04:30:59.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/django_env.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50390 2024-05-08 04:29:15.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/keras_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/nc_reader.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2528 2024-01-22 02:42:52.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/pid.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    11159 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/process_image.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3274 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/pycuda_test.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.119691 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7190 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2023-12-07 02:51:22.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19852 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/rw_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14951 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/rw_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16852 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/remove_outlier.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12394 2024-05-01 07:44:46.000000 biomedisa-2024.5.14/src/biomedisa/biomedisa_features/split_volume.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27102 2024-05-08 04:29:15.000000 biomedisa-2024.5.14/src/biomedisa/deeplearning.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17335 2024-05-07 02:20:39.000000 biomedisa-2024.5.14/src/biomedisa/interpolation.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15920 2024-05-07 07:21:28.000000 biomedisa-2024.5.14/src/biomedisa/mesh.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 05:36:46.119691 biomedisa-2024.5.14/src/biomedisa.egg-info/
--rw-r--r--   0 philipp   (1000) philipp   (1000)    11678 2024-05-08 05:36:46.000000 biomedisa-2024.5.14/src/biomedisa.egg-info/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2172 2024-05-08 05:36:46.000000 biomedisa-2024.5.14/src/biomedisa.egg-info/SOURCES.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-08 05:36:46.000000 biomedisa-2024.5.14/src/biomedisa.egg-info/dependency_links.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-08 05:36:46.000000 biomedisa-2024.5.14/src/biomedisa.egg-info/top_level.txt
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/LICENSE
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    11678 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/PKG-INFO
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11069 2024-05-08 04:32:37.000000 biomedisa-2024.5.15/README.md
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      665 2024-05-08 08:41:54.000000 biomedisa-2024.5.15/pyproject.toml
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/setup.cfg
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/biomedisa/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1690 2024-05-07 07:21:28.000000 biomedisa-2024.5.15/src/biomedisa/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/__main__.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/DataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-02-14 23:44:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/DataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/PredictDataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18131 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/active_contour.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/assd.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32401 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/biomedisa_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13329 2024-05-06 01:26:56.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/create_slices.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    23894 2024-05-06 01:26:56.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/crop_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/curvop_numba.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8989 2024-04-30 04:30:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/django_env.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50343 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/keras_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/nc_reader.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2528 2024-01-22 02:42:52.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/pid.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    11159 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/process_image.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3274 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/pycuda_test.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7190 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2023-12-07 02:51:22.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/rw_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/rw_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16801 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/remove_outlier.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12394 2024-05-01 07:44:46.000000 biomedisa-2024.5.15/src/biomedisa/biomedisa_features/split_volume.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27063 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/deeplearning.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17335 2024-05-07 02:20:39.000000 biomedisa-2024.5.15/src/biomedisa/interpolation.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15920 2024-05-08 08:24:59.000000 biomedisa-2024.5.15/src/biomedisa/mesh.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-08 08:42:17.328185 biomedisa-2024.5.15/src/biomedisa.egg-info/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    11678 2024-05-08 08:42:17.000000 biomedisa-2024.5.15/src/biomedisa.egg-info/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2172 2024-05-08 08:42:17.000000 biomedisa-2024.5.15/src/biomedisa.egg-info/SOURCES.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-08 08:42:17.000000 biomedisa-2024.5.15/src/biomedisa.egg-info/dependency_links.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-08 08:42:17.000000 biomedisa-2024.5.15/src/biomedisa.egg-info/top_level.txt
```

### Comparing `biomedisa-2024.5.14/LICENSE` & `biomedisa-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/PKG-INFO` & `biomedisa-2024.5.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedisa
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: Segmentation of 3D volumetric image data
 Author: Philipp Lösel
 Author-email: philipp.loesel@anu.edu.au
 Project-URL: Homepage, https://biomedisa.info
 Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
 Project-URL: GitHub, https://github.com/biomedisa/biomedisa
 Classifier: Programming Language :: Python :: 3
```

### Comparing `biomedisa-2024.5.14/README.md` & `biomedisa-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/pyproject.toml` & `biomedisa-2024.5.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biomedisa"
-version = "2024.5.14"
+version = "2024.5.15"
 authors = [
   { name="Philipp Lösel"}, {email="philipp.loesel@anu.edu.au" },
 ]
 description = "Segmentation of 3D volumetric image data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/__init__.py` & `biomedisa-2024.5.15/src/biomedisa/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/__main__.py` & `biomedisa-2024.5.15/src/biomedisa/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/DataGenerator.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/DataGeneratorCrop.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/DataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/PredictDataGenerator.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/PredictDataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/PredictDataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/active_contour.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/active_contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import sys, os
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if not BASE_DIR in sys.path:
     sys.path.append(BASE_DIR)
 import biomedisa
 from biomedisa_features.curvop_numba import curvop, evolution
-from biomedisa_features.biomedisa_helper import (load_data, save_data,
+from biomedisa_features.biomedisa_helper import (unique_file_path, load_data, save_data,
     pre_processing, img_to_uint8, silent_remove)
 import numpy as np
 import numba
 import argparse
 import traceback
 import subprocess
 
@@ -194,15 +194,14 @@
         # return to original data size
         final = np.zeros((zsh, ysh, xsh), dtype=np.uint8)
         final[argmin_z:argmax_z, argmin_y:argmax_y, argmin_x:argmax_x] = bm.labelData
         final = np.copy(final[1:-1, 1:-1, 1:-1], order='C')
 
         # save result
         if bm.django_env and not bm.remote:
-            from biomedisa_app.views import unique_file_path
             path_to_acwe = unique_file_path(path_to_acwe)
         if bm.path_to_data:
             save_data(path_to_acwe, final, bm.header, bm.final_image_type, bm.compression)
 
         # post processing
         if bm.django_env:
             post_processing(path_to_acwe, bm.img_id, bm.friend_id, bm.simple, bm.remote)
@@ -284,15 +283,15 @@
         Fails silently
     '''
 
     import django
     django.setup()
     from biomedisa_app.models import Upload
     from biomedisa_app.config import config
-    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop, unique_file_path
+    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop
 
     # get objects
     try:
         image = Upload.objects.get(pk=image_id)
         label = Upload.objects.get(pk=label_id)
         friend = Upload.objects.get(pk=friend_id)
         success = True
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_data_stream.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_grammar.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_header.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/amira_to_np/amira_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/assd.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/assd.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/biomedisa_helper.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/biomedisa_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,22 +39,73 @@
 import random
 import cv2
 import time
 import zipfile
 import numba
 import shutil
 import subprocess
+import re
 import math
 
 def silent_remove(filename):
     try:
         os.remove(filename)
     except OSError:
         pass
 
+# create a unique filename
+def unique_file_path(path, dir_path=BASE_DIR+'/private_storage/'):
+
+    # get extension
+    username = os.path.basename(os.path.dirname(path))
+    filename = os.path.basename(path)
+    filename, extension = os.path.splitext(filename)
+    if extension == '.gz':
+        filename, extension = os.path.splitext(filename)
+        if extension == '.nii':
+            extension = '.nii.gz'
+        elif extension == '.tar':
+            extension = '.tar.gz'
+
+    # get suffix
+    suffix = re.search("-[0-999]"+extension, path)
+    if suffix:
+        suffix = suffix.group()
+        filename = os.path.basename(path)
+        filename = filename[:-len(suffix)]
+        i = int(suffix[1:-len(extension)]) + 1
+    else:
+        suffix = extension
+        i = 1
+
+    # get finaltype
+    addon = ''
+    for feature in ['.filled','.smooth','.acwe','.cleaned','.8bit','.refined', '.cropped',
+                    '.uncertainty','.smooth.cleaned','.cleaned.filled','.denoised']:
+        if filename[-len(feature):] == feature:
+            addon = feature
+
+    if addon:
+        filename = filename[:-len(addon)]
+
+    # maximum lenght of path
+    pic_path = f'images/{username}/{filename}'
+    limit = 100 - len(addon) - len(suffix)
+    path = dir_path + pic_path[:limit] + addon + suffix
+
+    # check if file already exists
+    file_already_exists = os.path.exists(path)
+    while file_already_exists:
+        limit = 100 - len(addon) - len('-') - len(str(i)) - len(extension)
+        path = dir_path + pic_path[:limit] + addon + '-' + str(i) + extension
+        file_already_exists = os.path.exists(path)
+        i += 1
+
+    return path
+
 def Dice_score(ground_truth, result, average_dice=False):
     if average_dice:
         dice = 0
         allLabels = np.unique(ground_truth)
         for l in allLabels[1:]:
             dice += 2 * np.logical_and(ground_truth==l, result==l).sum() / float((ground_truth==l).sum() + (result==l).sum())
         dice /= float(len(allLabels)-1)
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/create_slices.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/create_slices.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/crop_helper.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/crop_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/curvop_numba.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/curvop_numba.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/django_env.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/django_env.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/keras_helper.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/keras_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Dense, Dropout, MaxPool3D, Flatten, Multiply)
 from tensorflow.keras import backend as K
 from tensorflow.keras.utils import to_categorical
 from tensorflow.keras.callbacks import Callback, ModelCheckpoint, EarlyStopping
 from biomedisa_features.DataGenerator import DataGenerator
 from biomedisa_features.PredictDataGenerator import PredictDataGenerator
 from biomedisa_features.biomedisa_helper import (
-    img_resize, load_data, save_data, set_labels_to_zero, id_generator)
+    img_resize, load_data, save_data, set_labels_to_zero, id_generator, unique_file_path)
 from biomedisa_features.remove_outlier import clean, fill
 from biomedisa_features.active_contour import activeContour
 import matplotlib.pyplot as plt
 import SimpleITK as sitk
 import tensorflow as tf
 import numpy as np
 import cv2
@@ -1144,15 +1144,14 @@
         # update file extension
         if header is not None and bm.path_to_image:
             extension = os.path.splitext(bm.header_file)[1]
             if extension == '.gz':
                 extension = '.nii.gz'
             bm.path_to_final = os.path.splitext(bm.path_to_final)[0] + extension
             if bm.django_env and not bm.remote and not bm.tmp_dir:
-                from biomedisa_app.views import unique_file_path
                 bm.path_to_final = unique_file_path(bm.path_to_final)
 
     # handle amira header
     if header is not None:
         if extension == '.am':
             header = get_image_dimensions(header[0], label)
             if img_header is not None:
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/nc_reader.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/nc_reader.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/pid.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/pid.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/process_image.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/process_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 ##########################################################################
 
 import os, sys
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if not BASE_DIR in sys.path:
     sys.path.append(BASE_DIR)
 import numpy as np
-from biomedisa_features.biomedisa_helper import (load_data, save_data,
+from biomedisa_features.biomedisa_helper import (load_data, save_data, unique_file_path,
     img_to_uint8, smooth_img_3x3)
 from biomedisa_features.create_slices import create_slices
 from shutil import copytree
 import argparse
 import traceback
 import subprocess
 
 def init_process_image(id, process=None):
 
     import django
     django.setup()
     from biomedisa_app.models import Upload
     from biomedisa_app.config import config
-    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop, unique_file_path
+    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop
     from redis import Redis
     from rq import Queue
 
     # get object
     try:
         img = Upload.objects.get(pk=id)
     except Upload.DoesNotExist:
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/pycuda_test.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/pycuda_test.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/gpu_kernels.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_large_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pycuda_small_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pyopencl_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/pyopencl_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/rw_large.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/rw_large.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ##  See the Licence for the specific language governing                 ##
 ##  permissions and limitations under the Licence.                      ##
 ##                                                                      ##
 ##########################################################################
 
 from biomedisa_features.remove_outlier import clean, fill
 from biomedisa_features.active_contour import activeContour
-from biomedisa_features.biomedisa_helper import (_get_device, save_data, _error_,
+from biomedisa_features.biomedisa_helper import (_get_device, save_data, _error_, unique_file_path,
     splitlargedata, read_labeled_slices_allx_large, read_labeled_slices_large, sendToChildLarge,
     Dice_score)
 from mpi4py import MPI
 import numpy as np
 import time
 import socket
 import os
@@ -180,15 +180,14 @@
 
             # regular result
             final_result = np.zeros((bm.zsh, bm.ysh, bm.xsh), dtype=np.uint8)
             final_result[bm.argmin_z:bm.argmax_z, bm.argmin_y:bm.argmax_y, bm.argmin_x:bm.argmax_x] = final
             final_result = final_result[1:-1, 1:-1, 1:-1]
             results['regular'] = final_result
             if bm.django_env and not bm.remote:
-                from biomedisa_app.views import unique_file_path
                 bm.path_to_final = unique_file_path(bm.path_to_final)
             if bm.path_to_data:
                 save_data(bm.path_to_final, final_result, bm.header, bm.final_image_type, bm.compression)
 
             # uncertainty
             if final_uncertainty is not None:
                 final_uncertainty *= 255
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/random_walk/rw_small.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/random_walk/rw_small.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ##  See the Licence for the specific language governing                 ##
 ##  permissions and limitations under the Licence.                      ##
 ##                                                                      ##
 ##########################################################################
 
 from biomedisa_features.remove_outlier import clean, fill
 from biomedisa_features.active_contour import activeContour
-from biomedisa_features.biomedisa_helper import (_get_device, save_data,
+from biomedisa_features.biomedisa_helper import (_get_device, save_data, unique_file_path,
     sendToChild, _split_indices, get_labels, Dice_score)
 from mpi4py import MPI
 import numpy as np
 import time
 import socket
 import os
 
@@ -101,17 +101,14 @@
         block = (32, 32, 1)
         x_grid = (xsh_tmp // 32) + 1
         y_grid = (ysh_tmp // 32) + 1
         grid = (int(x_grid), int(y_grid), int(zsh_tmp))
         xsh_gpu = np.int32(xsh_tmp)
         ysh_gpu = np.int32(ysh_tmp)
 
-        if bm.django_env:
-            from biomedisa_app.views import unique_file_path
-
         # smooth
         if bm.smooth:
             try:
                 update_gpu = _build_update_gpu()
                 curvature_gpu = _build_curvature_gpu()
                 a_gpu = gpuarray.empty((zsh_tmp, ysh_tmp, xsh_tmp), dtype=np.float32)
                 b_gpu = gpuarray.zeros((zsh_tmp, ysh_tmp, xsh_tmp), dtype=np.float32)
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/remove_outlier.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/remove_outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 ##########################################################################
 
 import sys, os
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if not BASE_DIR in sys.path:
     sys.path.append(BASE_DIR)
 import biomedisa
-from biomedisa_features.biomedisa_helper import load_data, save_data, silent_remove
+from biomedisa_features.biomedisa_helper import (load_data, save_data,
+    unique_file_path, silent_remove)
 import numpy as np
 from scipy import ndimage
 import argparse
 import traceback
 import subprocess
 
 def reduce_blocksize(data):
@@ -175,15 +176,14 @@
     final_cleaned = clean(final, clean_threshold)
     if fill_holes:
         final_filled = fill(final, fill_threshold)
         final_cleaned_filled = final_cleaned + (final_filled - final)
 
     # unique_file_paths
     if django_env and not remote:
-        from biomedisa_app.views import unique_file_path
         path_to_cleaned = unique_file_path(path_to_cleaned)
         path_to_filled = unique_file_path(path_to_filled)
         path_to_cleaned_filled = unique_file_path(path_to_cleaned_filled)
 
     # save results
     save_data(path_to_cleaned, final_cleaned, header, extension, compression)
     if fill_holes:
@@ -262,15 +262,15 @@
         Fails silently
     '''
 
     import django
     django.setup()
     from biomedisa_app.models import Upload
     from biomedisa_app.config import config
-    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop, unique_file_path
+    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop
 
     # get objects
     try:
         image = Upload.objects.get(pk=image_id)
         final = Upload.objects.get(pk=final_id)
         label = Upload.objects.get(pk=label_id)
         success = True
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/biomedisa_features/split_volume.py` & `biomedisa-2024.5.15/src/biomedisa/biomedisa_features/split_volume.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/deeplearning.py` & `biomedisa-2024.5.15/src/biomedisa/deeplearning.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import sys, os
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.append(BASE_DIR)
 import biomedisa
 import biomedisa_features.crop_helper as ch
 from biomedisa_features.keras_helper import *
-from biomedisa_features.biomedisa_helper import _error_
+from biomedisa_features.biomedisa_helper import _error_, unique_file_path
 from tensorflow.python.framework.errors_impl import ResourceExhaustedError
 import tensorflow as tf
 import numpy as np
 import traceback
 import argparse
 import h5py
 import time
@@ -96,16 +96,14 @@
     if bm.no_normalization:
         bm.normalize = 0
     else:
         bm.normalize = 1
 
     # django environment
     if bm.django_env:
-        from biomedisa_app.views import unique_file_path
-        from biomedisa_features.django_env import create_pid_object
 
         # path to image data
         if bm.train:
 
             # training files
             bm.path_to_images = bm.path_to_images.split(',')[:-1]
             bm.path_to_labels = bm.path_to_labels.split(',')[:-1]
@@ -126,14 +124,15 @@
             if not bm.remote:
                 bm.path_to_model = unique_file_path(bm.path_to_model)
 
         if bm.predict:
             project = os.path.splitext(os.path.basename(bm.path_to_model))[0]
 
         # create pid object
+        from biomedisa_features.django_env import create_pid_object
         create_pid_object(os.getpid(), bm.remote, bm.queue, bm.img_id, (bm.path_to_model if bm.train else ''))
 
         # write in log file
         with open(bm.path_to_logfile, 'a') as logfile:
             print('%s %s %s %s' %(time.ctime(), bm.username, bm.shortfilename, 'Process was started.'), file=logfile)
             print(f'PROJECT:{project} PREDICT:{bm.predict} IMG:{bm.shortfilename}', file=logfile)
             if bm.train:
```

### Comparing `biomedisa-2024.5.14/src/biomedisa/interpolation.py` & `biomedisa-2024.5.15/src/biomedisa/interpolation.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.14/src/biomedisa/mesh.py` & `biomedisa-2024.5.15/src/biomedisa/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ##########################################################################
 
 import os, sys
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 if not BASE_DIR in sys.path:
     sys.path.append(BASE_DIR)
 import numpy as np
-from biomedisa_features.biomedisa_helper import load_data
+from biomedisa_features.biomedisa_helper import load_data, unique_file_path
 from biomedisa_features.django_env import create_pid_object
 from vtk.util.numpy_support import vtk_to_numpy, numpy_to_vtk
 from stl import mesh
 import vtk
 import re
 import argparse
 import traceback
@@ -211,15 +211,15 @@
 
 def init_create_mesh(id):
 
     import django
     django.setup()
     from biomedisa_app.models import Upload
     from biomedisa_app.config import config
-    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop, unique_file_path
+    from biomedisa_app.views import send_data_to_host, qsub_start, qsub_stop
 
     # get object
     try:
         img = Upload.objects.get(pk=id)
     except Upload.DoesNotExist:
         img.status = 0
         img.save()
```

### Comparing `biomedisa-2024.5.14/src/biomedisa.egg-info/PKG-INFO` & `biomedisa-2024.5.15/src/biomedisa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedisa
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: Segmentation of 3D volumetric image data
 Author: Philipp Lösel
 Author-email: philipp.loesel@anu.edu.au
 Project-URL: Homepage, https://biomedisa.info
 Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
 Project-URL: GitHub, https://github.com/biomedisa/biomedisa
 Classifier: Programming Language :: Python :: 3
```

### Comparing `biomedisa-2024.5.14/src/biomedisa.egg-info/SOURCES.txt` & `biomedisa-2024.5.15/src/biomedisa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

