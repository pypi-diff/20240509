# Comparing `tmp/markarth-0.0.4.tar.gz` & `tmp/markarth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markarth-0.0.4.tar", last modified: Sun Mar 24 15:20:39 2024, max compression
+gzip compressed data, was "markarth-0.0.5.tar", last modified: Thu May  9 19:45:55 2024, max compression
```

## Comparing `markarth-0.0.4.tar` & `markarth-0.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.600647 markarth-0.0.4/
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1063 2023-06-21 20:36:40.000000 markarth-0.0.4/LICENSE
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2686 2024-03-24 15:20:39.599647 markarth-0.0.4/PKG-INFO
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2360 2024-03-23 08:34:48.000000 markarth-0.0.4/README.md
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.592647 markarth-0.0.4/markarth/
--rw-r--r--   0 nuc       (1000) nuc       (1000)      140 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/__init__.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.593647 markarth-0.0.4/markarth/ast_utils/
--rw-r--r--   0 nuc       (1000) nuc       (1000)       77 2024-03-11 21:53:59.000000 markarth-0.0.4/markarth/ast_utils/__init__.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1258 2024-03-11 21:53:59.000000 markarth-0.0.4/markarth/ast_utils/ast_utils.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.593647 markarth-0.0.4/markarth/convert/
--rw-r--r--   0 nuc       (1000) nuc       (1000)       39 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/__init__.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.594647 markarth-0.0.4/markarth/convert/collect/
--rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/collect/__init__.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.595647 markarth-0.0.4/markarth/convert/collect/ast_to_typ/
--rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/collect/ast_to_typ/__init__.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4237 2024-03-24 15:15:58.000000 markarth-0.0.4/markarth/convert/collect/ast_to_typ/ast_assign.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4357 2024-03-24 11:21:41.000000 markarth-0.0.4/markarth/convert/collect/ast_to_typ/ast_to_typ.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     7947 2024-03-14 09:27:40.000000 markarth-0.0.4/markarth/convert/collect/func_collect.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     5964 2024-03-11 21:53:59.000000 markarth-0.0.4/markarth/convert/collect/mod_collect.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4682 2024-03-11 21:53:59.000000 markarth-0.0.4/markarth/convert/collect/vartyp_tracker.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)      730 2024-01-03 22:23:49.000000 markarth-0.0.4/markarth/convert/convert_pure.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.595647 markarth-0.0.4/markarth/convert/cythonize/
--rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/cythonize/__init__.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     3151 2024-01-03 22:23:49.000000 markarth-0.0.4/markarth/convert/cythonize/cy_options.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)      926 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/cythonize/cy_typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     8637 2024-03-24 11:21:41.000000 markarth-0.0.4/markarth/convert/cythonize/pure.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.595647 markarth-0.0.4/markarth/convert/preprocess/
--rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/preprocess/__init__.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2058 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/preprocess/code_process.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.596647 markarth-0.0.4/markarth/convert/typs/
--rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/typs/__init__.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1209 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/typs/merge_typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1911 2024-03-11 21:53:59.000000 markarth-0.0.4/markarth/convert/typs/typ_store.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4468 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/typs/typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)      429 2023-11-27 21:53:14.000000 markarth-0.0.4/markarth/convert/typs/typs_parse.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.599647 markarth-0.0.4/markarth.egg-info/
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2686 2024-03-24 15:20:39.000000 markarth-0.0.4/markarth.egg-info/PKG-INFO
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1429 2024-03-24 15:20:39.000000 markarth-0.0.4/markarth.egg-info/SOURCES.txt
--rw-r--r--   0 nuc       (1000) nuc       (1000)        1 2024-03-24 15:20:39.000000 markarth-0.0.4/markarth.egg-info/dependency_links.txt
--rw-r--r--   0 nuc       (1000) nuc       (1000)       32 2024-03-24 15:20:39.000000 markarth-0.0.4/markarth.egg-info/requires.txt
--rw-r--r--   0 nuc       (1000) nuc       (1000)        9 2024-03-24 15:20:39.000000 markarth-0.0.4/markarth.egg-info/top_level.txt
--rw-r--r--   0 nuc       (1000) nuc       (1000)       38 2024-03-24 15:20:39.600647 markarth-0.0.4/setup.cfg
--rw-r--r--   0 nuc       (1000) nuc       (1000)      539 2024-03-24 15:15:58.000000 markarth-0.0.4/setup.py
-drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-03-24 15:20:39.598647 markarth-0.0.4/tests/
--rw-r--r--   0 nuc       (1000) nuc       (1000)     5386 2024-03-24 15:15:58.000000 markarth-0.0.4/tests/test_ast_assign.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     5484 2024-03-11 22:04:11.000000 markarth-0.0.4/tests/test_ast_to_typ.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1844 2024-03-11 21:53:59.000000 markarth-0.0.4/tests/test_ast_utils.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1790 2024-03-11 21:53:59.000000 markarth-0.0.4/tests/test_code_process.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2672 2024-03-14 09:27:40.000000 markarth-0.0.4/tests/test_convert_pure.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     1337 2023-11-27 21:53:14.000000 markarth-0.0.4/tests/test_cy_opts.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)      460 2023-12-03 22:42:01.000000 markarth-0.0.4/tests/test_cy_typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4925 2024-03-24 11:21:41.000000 markarth-0.0.4/tests/test_cythonize_pure.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     2336 2024-03-11 22:00:42.000000 markarth-0.0.4/tests/test_dict_typ_store.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     5716 2024-03-11 21:53:59.000000 markarth-0.0.4/tests/test_func_collect.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4144 2023-11-27 21:53:14.000000 markarth-0.0.4/tests/test_merge_typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     3198 2024-03-11 21:53:59.000000 markarth-0.0.4/tests/test_mod_collect.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     4214 2024-03-11 22:08:57.000000 markarth-0.0.4/tests/test_typs.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)      818 2023-11-27 21:53:14.000000 markarth-0.0.4/tests/test_typs_parse.py
--rw-r--r--   0 nuc       (1000) nuc       (1000)     7634 2024-03-11 21:53:59.000000 markarth-0.0.4/tests/test_vartyp_tracker.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.726185 markarth-0.0.5/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1063 2023-06-21 20:36:40.000000 markarth-0.0.5/LICENSE
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     3629 2024-05-09 19:45:55.725185 markarth-0.0.5/PKG-INFO
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     2706 2024-05-09 19:37:24.000000 markarth-0.0.5/README.md
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.722185 markarth-0.0.5/markarth/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      140 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/__init__.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.722185 markarth-0.0.5/markarth/ast_utils/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)       77 2024-03-11 21:53:59.000000 markarth-0.0.5/markarth/ast_utils/__init__.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1258 2024-03-11 21:53:59.000000 markarth-0.0.5/markarth/ast_utils/ast_utils.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.723185 markarth-0.0.5/markarth/convert/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)       39 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/__init__.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.723185 markarth-0.0.5/markarth/convert/collect/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/collect/__init__.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.724185 markarth-0.0.5/markarth/convert/collect/ast_to_typ/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/collect/ast_to_typ/__init__.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4237 2024-04-16 21:11:37.000000 markarth-0.0.5/markarth/convert/collect/ast_to_typ/ast_assign.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4357 2024-04-16 21:11:37.000000 markarth-0.0.5/markarth/convert/collect/ast_to_typ/ast_to_typ.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     7947 2024-03-14 09:27:40.000000 markarth-0.0.5/markarth/convert/collect/func_collect.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     5964 2024-03-11 21:53:59.000000 markarth-0.0.5/markarth/convert/collect/mod_collect.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4682 2024-03-11 21:53:59.000000 markarth-0.0.5/markarth/convert/collect/vartyp_tracker.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      730 2024-01-03 22:23:49.000000 markarth-0.0.5/markarth/convert/convert_pure.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.724185 markarth-0.0.5/markarth/convert/cythonize/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/cythonize/__init__.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     3151 2024-01-03 22:23:49.000000 markarth-0.0.5/markarth/convert/cythonize/cy_options.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      926 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/cythonize/cy_typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     8639 2024-05-09 19:17:21.000000 markarth-0.0.5/markarth/convert/cythonize/pure.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.724185 markarth-0.0.5/markarth/convert/preprocess/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/preprocess/__init__.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1825 2024-05-09 19:07:11.000000 markarth-0.0.5/markarth/convert/preprocess/code_process.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.724185 markarth-0.0.5/markarth/convert/typs/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        0 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/typs/__init__.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1209 2023-11-27 21:53:14.000000 markarth-0.0.5/markarth/convert/typs/merge_typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1911 2024-03-11 21:53:59.000000 markarth-0.0.5/markarth/convert/typs/typ_store.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4468 2024-04-16 21:11:37.000000 markarth-0.0.5/markarth/convert/typs/typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      429 2024-04-16 21:11:37.000000 markarth-0.0.5/markarth/convert/typs/typs_parse.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.725185 markarth-0.0.5/markarth.egg-info/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     3629 2024-05-09 19:45:55.000000 markarth-0.0.5/markarth.egg-info/PKG-INFO
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1429 2024-05-09 19:45:55.000000 markarth-0.0.5/markarth.egg-info/SOURCES.txt
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        1 2024-05-09 19:45:55.000000 markarth-0.0.5/markarth.egg-info/dependency_links.txt
+-rw-r--r--   0 nuc       (1000) nuc       (1000)       32 2024-05-09 19:45:55.000000 markarth-0.0.5/markarth.egg-info/requires.txt
+-rw-r--r--   0 nuc       (1000) nuc       (1000)        9 2024-05-09 19:45:55.000000 markarth-0.0.5/markarth.egg-info/top_level.txt
+-rw-r--r--   0 nuc       (1000) nuc       (1000)       38 2024-05-09 19:45:55.726185 markarth-0.0.5/setup.cfg
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1149 2024-05-09 19:45:50.000000 markarth-0.0.5/setup.py
+drwxr-xr-x   0 nuc       (1000) nuc       (1000)        0 2024-05-09 19:45:55.725185 markarth-0.0.5/tests/
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     5386 2024-04-16 21:11:37.000000 markarth-0.0.5/tests/test_ast_assign.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     5949 2024-05-09 19:24:19.000000 markarth-0.0.5/tests/test_ast_to_typ.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1844 2024-03-11 21:53:59.000000 markarth-0.0.5/tests/test_ast_utils.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1790 2024-03-11 21:53:59.000000 markarth-0.0.5/tests/test_code_process.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     2672 2024-03-14 09:27:40.000000 markarth-0.0.5/tests/test_convert_pure.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     1337 2023-11-27 21:53:14.000000 markarth-0.0.5/tests/test_cy_opts.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      460 2023-12-03 22:42:01.000000 markarth-0.0.5/tests/test_cy_typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     5363 2024-05-09 19:13:20.000000 markarth-0.0.5/tests/test_cythonize_pure.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     2336 2024-03-11 22:00:42.000000 markarth-0.0.5/tests/test_dict_typ_store.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     5716 2024-04-16 21:11:37.000000 markarth-0.0.5/tests/test_func_collect.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4144 2023-11-27 21:53:14.000000 markarth-0.0.5/tests/test_merge_typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     3198 2024-03-11 21:53:59.000000 markarth-0.0.5/tests/test_mod_collect.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     4419 2024-05-09 19:04:52.000000 markarth-0.0.5/tests/test_typs.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)      818 2024-04-16 21:11:37.000000 markarth-0.0.5/tests/test_typs_parse.py
+-rw-r--r--   0 nuc       (1000) nuc       (1000)     7634 2024-03-11 21:53:59.000000 markarth-0.0.5/tests/test_vartyp_tracker.py
```

### Comparing `markarth-0.0.4/LICENSE` & `markarth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/PKG-INFO` & `markarth-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: markarth
-Version: 0.0.4
-Summary: Automatic code conversion from python to cython
-Home-page: https://github.com/nucccc/markarth
-Author: Domenico Nucera
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic>=2.4.2
-Requires-Dist: coverage>=7.3.2
-
 # markarth
 
 ![Coverage badge](https://raw.githubusercontent.com/nucccc/markarth/python-coverage-comment-action-data/badge.svg)
 
 markarth is a library to automatically cythonize python code.
 
 It can receive in input python code, evaluate the primitive types that variables are going to possess, and then add codelines for [pure python cython mode](https://cython.readthedocs.io/en/latest/src/tutorial/pure.html).
@@ -65,27 +53,31 @@
         sum = 5 * 18
     return float(sum)
 
 ```
 
 ## Installation
 
-At the moment there is no PyPI package, so if someone really (really?) wants to run such thing, the repo should be cloned, to then run the `setup.py` script in the cloning folder 
+Markarth is available on the [PyPI index](https://pypi.org/project/markarth). You can install it using pip:
 
 ```
-git clone https://github.com/nucccc/markarth
-cd markarth
-pip install .
+pip install markarth
 ```
 
 ## Internal functioning
 
 It makes heavy usage of the `ast` module in order to parse python code, while leveraging type annotations to infer variable types, thus adding some declarations that with python would speed the code up.
 
+The module's functionality is divided in two main steps:
+ - one in which the code parsed with `ast` is analyzed to detect types of variables. Results of elementary operations are used, together with invocations of functions like `len()`.
+ - another in which the types collected are converted to cython codelines.
+
+There are additional functionalities to provide conversion options, in order to use `cython.double` instead of `cython.float` as type during conversion.
+
 ## Possible improvements
 
 Several possible improvements can be done (apart from testing and discovering bugs, obviously). Among them:
 
 - Store and extrapolate types of containers (lists, dicts, sets, ecc.)
 - Identify numpy array and type them as memory views
 - Detect `:=` walrus operators
-- Possibility of selecting between pure python mode conversion and old style pure cython with `cdef VARNAME int` codelines
+- Possibility of selecting between pure python mode conversion and old style pure cython with `cdef VARNAME int` codelines
```

### Comparing `markarth-0.0.4/markarth/ast_utils/ast_utils.py` & `markarth-0.0.5/markarth/ast_utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/collect/ast_to_typ/ast_assign.py` & `markarth-0.0.5/markarth/convert/collect/ast_to_typ/ast_assign.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/collect/ast_to_typ/ast_to_typ.py` & `markarth-0.0.5/markarth/convert/collect/ast_to_typ/ast_to_typ.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/collect/func_collect.py` & `markarth-0.0.5/markarth/convert/collect/func_collect.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/collect/mod_collect.py` & `markarth-0.0.5/markarth/convert/collect/mod_collect.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/collect/vartyp_tracker.py` & `markarth-0.0.5/markarth/convert/collect/vartyp_tracker.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/convert_pure.py` & `markarth-0.0.5/markarth/convert/convert_pure.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/cythonize/cy_options.py` & `markarth-0.0.5/markarth/convert/cythonize/cy_options.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/cythonize/cy_typs.py` & `markarth-0.0.5/markarth/convert/cythonize/cy_typs.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/cythonize/pure.py` & `markarth-0.0.5/markarth/convert/cythonize/pure.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,16 @@
 def could_be_docstring(stat : ast.AST) -> bool:
     '''
     could_be_docstring returns True if an ast statement could be seen as a
     docstring
     '''
     if not type(stat) is ast.Expr:
         return False
-    if not hasattr(stat, 'value'):
-        return False
+    #if not hasattr(stat, 'value'):
+    #    return False
     if not hasattr(stat.value, 'n'):
         return False
     return type(stat.value.n) is str
 
 
 def cdeclares_ins_point(func_ast : ast.FunctionDef) -> int:
     '''
```

### Comparing `markarth-0.0.4/markarth/convert/preprocess/code_process.py` & `markarth-0.0.5/markarth/convert/preprocess/code_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,22 +36,14 @@
 def process_func_code(code : str) -> tuple[ast.FunctionDef, list[str]]:
     '''
     process_func_code
     '''
     ast_code, codelines = process_code(code)
     func_ast = ast_code.body[0]
     return (func_ast, codelines)
-
-
-def process_file(filepath : str) -> tuple[ast.Module, list[str]]:
-    '''
-    process_file opens a python code file, returns its code being processed
-    '''
-    with open(filepath, 'r') as f:
-        return process_code(f.read())
     
 
 def indentation_pattern(
     ast_with_body : ast.AST,
     codelines : list[str],
     indent_level : int = 1
 ) -> str:
```

### Comparing `markarth-0.0.4/markarth/convert/typs/merge_typs.py` & `markarth-0.0.5/markarth/convert/typs/merge_typs.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/typs/typ_store.py` & `markarth-0.0.5/markarth/convert/typs/typ_store.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth/convert/typs/typs.py` & `markarth-0.0.5/markarth/convert/typs/typs.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/markarth.egg-info/PKG-INFO` & `markarth-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 Metadata-Version: 2.1
 Name: markarth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatic code conversion from python to cython
 Home-page: https://github.com/nucccc/markarth
 Author: Domenico Nucera
 License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.4.2
 Requires-Dist: coverage>=7.3.2
 
 # markarth
 
@@ -65,26 +77,30 @@
         sum = 5 * 18
     return float(sum)
 
 ```
 
 ## Installation
 
-At the moment there is no PyPI package, so if someone really (really?) wants to run such thing, the repo should be cloned, to then run the `setup.py` script in the cloning folder 
+Markarth is available on the [PyPI index](https://pypi.org/project/markarth). You can install it using pip:
 
 ```
-git clone https://github.com/nucccc/markarth
-cd markarth
-pip install .
+pip install markarth
 ```
 
 ## Internal functioning
 
 It makes heavy usage of the `ast` module in order to parse python code, while leveraging type annotations to infer variable types, thus adding some declarations that with python would speed the code up.
 
+The module's functionality is divided in two main steps:
+ - one in which the code parsed with `ast` is analyzed to detect types of variables. Results of elementary operations are used, together with invocations of functions like `len()`.
+ - another in which the types collected are converted to cython codelines.
+
+There are additional functionalities to provide conversion options, in order to use `cython.double` instead of `cython.float` as type during conversion.
+
 ## Possible improvements
 
 Several possible improvements can be done (apart from testing and discovering bugs, obviously). Among them:
 
 - Store and extrapolate types of containers (lists, dicts, sets, ecc.)
 - Identify numpy array and type them as memory views
 - Detect `:=` walrus operators
```

### Comparing `markarth-0.0.4/markarth.egg-info/SOURCES.txt` & `markarth-0.0.5/markarth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_ast_assign.py` & `markarth-0.0.5/tests/test_ast_assign.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_ast_to_typ.py` & `markarth-0.0.5/tests/test_ast_to_typ.py`

 * *Files 13% similar despite different names*

```diff
@@ -206,13 +206,34 @@
     code = 'a = bool(7)'
     mod = ast.parse(code)
     call = mod.body[0].value
 
     call_typ = typ_from_call(call = call)
     assert call_typ.is_bool()
 
+    code = 'a = str(7)'
+    mod = ast.parse(code)
+    call = mod.body[0].value
+
+    call_typ = typ_from_call(call = call)
+    assert call_typ.is_str()
+
+    code = 'a = len([1,2,3])'
+    mod = ast.parse(code)
+    call = mod.body[0].value
+
+    call_typ = typ_from_call(call = call)
+    assert call_typ.is_int()
+
+    code = 'a = np.mean()'
+    mod = ast.parse(code)
+    call = mod.body[0].value
+
+    call_typ = typ_from_call(call = call)
+    assert call_typ.is_any()
+
     code = 'a = asfasf(7)'
     mod = ast.parse(code)
     call = mod.body[0].value
 
     call_typ = typ_from_call(call = call)
     assert call_typ.is_any()
```

### Comparing `markarth-0.0.4/tests/test_ast_utils.py` & `markarth-0.0.5/tests/test_ast_utils.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_code_process.py` & `markarth-0.0.5/tests/test_code_process.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_convert_pure.py` & `markarth-0.0.5/tests/test_convert_pure.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_cy_opts.py` & `markarth-0.0.5/tests/test_cy_opts.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_cythonize_pure.py` & `markarth-0.0.5/tests/test_cythonize_pure.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,14 +146,20 @@
 def test_could_be_docstring():
     m = ast.parse('a = 3')
     assert not could_be_docstring(m.body[0])
 
     m = ast.parse('3')
     assert not could_be_docstring(m.body[0])
 
+    m = ast.parse('[i for i in range(4)]')
+    assert not could_be_docstring(m.body[0])
+
+    m = ast.parse('len([i for i in range(4)])')
+    assert not could_be_docstring(m.body[0])
+
     m = ast.parse('"""beh"""')
     assert could_be_docstring(m.body[0])
 
     m = ast.parse('"string"')
     assert could_be_docstring(m.body[0])
 
 
@@ -171,14 +177,22 @@
 
     func_asts = collect_func_defs(mod_ast)
 
     assert cdeclares_ins_point(func_asts['f1']) == 8
     assert cdeclares_ins_point(func_asts['f2']) == 15
     assert cdeclares_ins_point(func_asts['f3']) == 19
 
+    # testing the case of a docstring as the only element of a code section
+    cod = """def func():\n\t'''a docstring'''"""
+    mod_ast = ast.parse(cod)
+    func_asts = collect_func_defs(mod_ast)
+
+    assert cdeclares_ins_point(func_asts['func']) == 2
+
+
 
 def test_sort_funcs_by_line(mod3):
     mod_ast, _ = mod3
 
     func_asts = collect_func_defs(mod_ast)
     
     funcs_names_ordered = sort_funcs_by_line(func_asts)
```

### Comparing `markarth-0.0.4/tests/test_dict_typ_store.py` & `markarth-0.0.5/tests/test_dict_typ_store.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_func_collect.py` & `markarth-0.0.5/tests/test_func_collect.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_merge_typs.py` & `markarth-0.0.5/tests/test_merge_typs.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_mod_collect.py` & `markarth-0.0.5/tests/test_mod_collect.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_typs.py` & `markarth-0.0.5/tests/test_typs.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 def test_str_to_prim_cod():
     assert typs.str_to_prim_cod('bool') == typs.PrimitiveCod.BOOL
     assert typs.str_to_prim_cod('float') == typs.PrimitiveCod.FLOAT
     assert typs.str_to_prim_cod('int') == typs.PrimitiveCod.INT
     assert typs.str_to_prim_cod('str') == typs.PrimitiveCod.STR
 
+    with pytest.raises(typs.InvalidPrimitiveStr):
+        typs.str_to_prim_cod('hakahakahaka')
+
     assert typs.str_to_prim_cod_or_none('bool') == typs.PrimitiveCod.BOOL
     assert typs.str_to_prim_cod_or_none('float') == typs.PrimitiveCod.FLOAT
     assert typs.str_to_prim_cod_or_none('int') == typs.PrimitiveCod.INT
     assert typs.str_to_prim_cod_or_none('str') == typs.PrimitiveCod.STR
 
     assert typs.str_to_prim_cod_or_none('hakahakahaka') is None
 
@@ -21,14 +24,21 @@
 def test_prim_cod_to_str():
     assert typs.prim_cod_to_str(typs.PrimitiveCod.BOOL) == 'bool'
     assert typs.prim_cod_to_str(typs.PrimitiveCod.FLOAT) == 'float'
     assert typs.prim_cod_to_str(typs.PrimitiveCod.INT) == 'int'
     assert typs.prim_cod_to_str(typs.PrimitiveCod.STR) == 'str'
 
 
+def test_typ():
+    typ = typs.Typ()
+
+    with pytest.raises(NotImplementedError):
+        typ.as_string()
+
+
 def test_typ_primitive():
     # bool test
     typ = typs.TypPrimitive('bool')
 
     assert typ.is_primitive()
     assert not typ.is_container()
     assert not typ.is_none()
```

### Comparing `markarth-0.0.4/tests/test_typs_parse.py` & `markarth-0.0.5/tests/test_typs_parse.py`

 * *Files identical despite different names*

### Comparing `markarth-0.0.4/tests/test_vartyp_tracker.py` & `markarth-0.0.5/tests/test_vartyp_tracker.py`

 * *Files identical despite different names*

