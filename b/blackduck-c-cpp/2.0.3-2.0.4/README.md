# Comparing `tmp/blackduck-c-cpp-2.0.3.tar.gz` & `tmp/blackduck-c-cpp-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackduck-c-cpp-2.0.3.tar", last modified: Wed Mar 27 13:20:36 2024, max compression
+gzip compressed data, was "blackduck-c-cpp-2.0.4.tar", last modified: Wed May  8 13:13:27 2024, max compression
```

## Comparing `blackduck-c-cpp-2.0.3.tar` & `blackduck-c-cpp-2.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.056293 blackduck-c-cpp-2.0.3/
--rw-r--r--   0 kakarlas   (503) staff       (20)      140 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/LICENSE
--rw-r--r--   0 kakarlas   (503) staff       (20)       84 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/MANIFEST.in
--rw-r--r--   0 kakarlas   (503) staff       (20)    34247 2024-03-27 13:20:36.056039 blackduck-c-cpp-2.0.3/PKG-INFO
--rw-r--r--   0 kakarlas   (503) staff       (20)    33387 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/README.md
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.046458 blackduck-c-cpp-2.0.3/blackduck_c_cpp/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/__init__.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.048235 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdba/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdba/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     4763 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdba/upload_bdba.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.048640 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdio/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdio/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     5336 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdio/bdio2_python_transformer.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.049083 blackduck-c-cpp-2.0.3/blackduck_c_cpp/coverity_json/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/coverity_json/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     8650 2024-03-27 13:07:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/coverity_json/cov_json_parse.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.049805 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/__init__.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.050682 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    26467 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/bdio_entries.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     6407 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/bdio_paths.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     4912 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/custom_types.py
--rw-r--r--   0 kakarlas   (503) staff       (20)      681 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/version_king.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.052093 blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     4049 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/ld_debug_parse.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    53451 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     3584 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    43732 2024-03-27 13:07:45.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/run_build_capture.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.052796 blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     5883 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/emit_wrapper.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    37367 2024-03-27 13:07:45.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/run_sig_scanner.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.055604 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/
--rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/__init__.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    11784 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/build_log_parser.py
--rw-r--r--   0 kakarlas   (503) staff       (20)    16440 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/c_arg_parser.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     7245 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/cov_install.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     2635 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/global_settings.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     6381 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/hub_api.py
--rw-r--r--   0 kakarlas   (503) staff       (20)     6363 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/util.py
--rw-r--r--   0 kakarlas   (503) staff       (20)      948 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/zip_file.py
-drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-03-27 13:20:36.047932 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/
--rw-r--r--   0 kakarlas   (503) staff       (20)    34247 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/PKG-INFO
--rw-r--r--   0 kakarlas   (503) staff       (20)     1422 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 kakarlas   (503) staff       (20)        1 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 kakarlas   (503) staff       (20)       74 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/entry_points.txt
--rw-r--r--   0 kakarlas   (503) staff       (20)      306 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/requires.txt
--rw-r--r--   0 kakarlas   (503) staff       (20)       16 2024-03-27 13:20:36.000000 blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/top_level.txt
--rw-r--r--   0 kakarlas   (503) staff       (20)       38 2024-03-27 13:20:36.056337 blackduck-c-cpp-2.0.3/setup.cfg
--rw-r--r--   0 kakarlas   (503) staff       (20)     1542 2024-03-27 13:19:33.000000 blackduck-c-cpp-2.0.3/setup.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.683212 blackduck-c-cpp-2.0.4/
+-rw-r--r--   0 kakarlas   (503) staff       (20)      140 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/LICENSE
+-rw-r--r--   0 kakarlas   (503) staff       (20)       84 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/MANIFEST.in
+-rw-r--r--   0 kakarlas   (503) staff       (20)    34400 2024-05-08 13:13:27.682584 blackduck-c-cpp-2.0.4/PKG-INFO
+-rw-r--r--   0 kakarlas   (503) staff       (20)    33540 2024-05-08 13:10:10.000000 blackduck-c-cpp-2.0.4/README.md
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.664132 blackduck-c-cpp-2.0.4/blackduck_c_cpp/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/__init__.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.668258 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdba/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdba/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     4763 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdba/upload_bdba.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.669251 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdio/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdio/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     5351 2024-05-08 13:10:10.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdio/bdio2_python_transformer.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.669963 blackduck-c-cpp-2.0.4/blackduck_c_cpp/coverity_json/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/coverity_json/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     8650 2024-03-27 13:07:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/coverity_json/cov_json_parse.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.671198 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/__init__.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.673004 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    26467 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/bdio_entries.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     6407 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/bdio_paths.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     4912 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/custom_types.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)      681 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/version_king.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.676146 blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     4049 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/ld_debug_parse.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    53451 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     3584 2024-03-29 16:57:59.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    43732 2024-05-08 13:09:59.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/run_build_capture.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.677457 blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     5883 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/emit_wrapper.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    37367 2024-03-27 13:07:45.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/run_sig_scanner.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.681953 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/
+-rw-r--r--   0 kakarlas   (503) staff       (20)        0 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/__init__.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    11784 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/build_log_parser.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)    16440 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/c_arg_parser.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     7245 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/cov_install.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     2635 2024-01-16 17:48:47.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/global_settings.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     6381 2024-03-20 14:51:21.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/hub_api.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)     6388 2024-05-08 13:10:10.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/util.py
+-rw-r--r--   0 kakarlas   (503) staff       (20)      948 2023-12-21 13:13:38.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/zip_file.py
+drwxr-xr-x   0 kakarlas   (503) staff       (20)        0 2024-05-08 13:13:27.667608 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/
+-rw-r--r--   0 kakarlas   (503) staff       (20)    34400 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 kakarlas   (503) staff       (20)     1422 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 kakarlas   (503) staff       (20)        1 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 kakarlas   (503) staff       (20)       74 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/entry_points.txt
+-rw-r--r--   0 kakarlas   (503) staff       (20)      306 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/requires.txt
+-rw-r--r--   0 kakarlas   (503) staff       (20)       16 2024-05-08 13:13:27.000000 blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/top_level.txt
+-rw-r--r--   0 kakarlas   (503) staff       (20)       38 2024-05-08 13:13:27.683263 blackduck-c-cpp-2.0.4/setup.cfg
+-rw-r--r--   0 kakarlas   (503) staff       (20)     1542 2024-05-08 13:10:10.000000 blackduck-c-cpp-2.0.4/setup.py
```

### Comparing `blackduck-c-cpp-2.0.3/PKG-INFO` & `blackduck-c-cpp-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackduck-c-cpp
-Version: 2.0.3
+Version: 2.0.4
 Summary: Scanning for c/c++ projects using blackduck and coverity tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
@@ -54,14 +54,20 @@
 The signature scan and binary scan will be completed on all supported platforms as permitted by your Black Duck license.
 Any scan cli parameters can be used and passed to blackduck-c-cpp tool through the additional_sig_scan_args parameter.
 
 On Unix-like operating systems, a package manager scan will also be run. Since Windows doesn't have a supported package
 manager, blackduck-c-cpp scans run on Windows won't include the package manager scan and won't produce a BDIO file.
 Here, package manager scan refers to usage of O/S package managers such as yum, apt etc.
 
+## Supported Compilers and Linkers
+
+Run ./cov-configure --list-compiler-types to get complete set of supported compilers
+
+Linkers supported: gcc, msvc.
+
 ## Installation
 
 Minimum version of Black Duck required is 2020.10.0
 
 To install from pypi:
 
 ```
```

### Comparing `blackduck-c-cpp-2.0.3/README.md` & `blackduck-c-cpp-2.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 The signature scan and binary scan will be completed on all supported platforms as permitted by your Black Duck license.
 Any scan cli parameters can be used and passed to blackduck-c-cpp tool through the additional_sig_scan_args parameter.
 
 On Unix-like operating systems, a package manager scan will also be run. Since Windows doesn't have a supported package
 manager, blackduck-c-cpp scans run on Windows won't include the package manager scan and won't produce a BDIO file.
 Here, package manager scan refers to usage of O/S package managers such as yum, apt etc.
 
+## Supported Compilers and Linkers
+
+Run ./cov-configure --list-compiler-types to get complete set of supported compilers
+
+Linkers supported: gcc, msvc.
+
 ## Installation
 
 Minimum version of Black Duck required is 2020.10.0
 
 To install from pypi:
 
 ```
```

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdba/upload_bdba.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdba/upload_bdba.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/bdio/bdio2_python_transformer.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/bdio/bdio2_python_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,27 +74,27 @@
 
         fileentry_project_base = bdio_builder.fileentry_project_base(scanned_path, scan_size)
         bdio_builder.project(project_name, project_version, fileentry_project_base)
         dir_comp_dict = dict()  # key: direct dependency compoenent ,value:(comp value, set of fullpath)
 
         for entry in cov_results[0]["extended-objects"]:
             # all entrys are direct deps
-            comp = entry["distro"] + entry["package-name"] + entry["package-version"] + entry["package-architecture"]
+            comp = entry["distro"] + entry["package-name"] + str(entry["package-version"]) + entry["package-architecture"]
 
             if comp in dir_comp_dict and entry['fullpath'][1] in dir_comp_dict[comp][1]:
                 continue
 
             if comp in dir_comp_dict:  # use existing direct dependency component
                 direct_dep_component = dir_comp_dict[comp][0]
                 dir_comp_dict[comp][1].add(entry['fullpath'][1])  # append path
             else:  # else create new one if it was never seen before
                 direct_dep_component = bdio_builder.component(
                     entry["distro"],
                     entry["package-name"],
-                    entry["package-version"],
+                    str(entry["package-version"]),
                     entry["package-architecture"],
                     fallback_forge=True,
                     allow_duplicates=True,
                 )
                 dir_comp_dict[comp] = (direct_dep_component, {entry['fullpath'][1]})
 
             direct_dep_file = bdio_builder.fileentry_from_fullpath(
@@ -110,15 +110,15 @@
 
             # add all transitive components
             transitive_entry: Dict = {}  # needed for type checker to stop complaining
             for transitive_entry in entry.get("trans-dep", []):
                 transitive_dep_component = bdio_builder.component(
                     transitive_entry["distro"],
                     transitive_entry["package-name"],
-                    transitive_entry["package-version"],
+                    str(transitive_entry["package-version"]),
                     transitive_entry["package-architecture"],
                     fallback_forge=True,
                     allow_duplicates=True,
                 )
                 transitive_dep_file = bdio_builder.fileentry_from_fullpath(
                     transitive_entry["fullpath"],
                     transitive_entry["timestamp"],
```

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/coverity_json/cov_json_parse.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/coverity_json/cov_json_parse.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/bdio_entries.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/bdio_entries.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/bdio/bdio_paths.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/bdio/bdio_paths.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/custom_types.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/custom_types.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/katiska/version_king.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/katiska/version_king.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/ld_debug_parse.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/ld_debug_parse.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/pkg_manager_bom.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/pkg_manager/pkg_manager_detector.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/run_build_capture.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/run_build_capture.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/emit_wrapper.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/emit_wrapper.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/sig_scanner/run_sig_scanner.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/sig_scanner/run_sig_scanner.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/build_log_parser.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/build_log_parser.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/c_arg_parser.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/c_arg_parser.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/cov_install.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/cov_install.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/global_settings.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/global_settings.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/hub_api.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/hub_api.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/util.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 
 def zip_files(files_to_zip, zip_output_path):
     if os.path.exists(zip_output_path):
         os.remove(zip_output_path)
     logging.debug("using zipfile module")
 
-    with zipfile.ZipFile(zip_output_path, 'w', compression=zipfile.ZIP_DEFLATED) as zip_object:
+    with zipfile.ZipFile(zip_output_path, 'w', compression=zipfile.ZIP_DEFLATED, strict_timestamps=False) as zip_object:
         with tqdm.tqdm(total=len(files_to_zip)) as bar:
             for file_path in files_to_zip:
                 try:
                     path = os.path.realpath(file_path)
                     zip_object.write(path, arcname=path)
                     bar.update(1)
                 except FileNotFoundError:
```

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp/util/zip_file.py` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp/util/zip_file.py`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/PKG-INFO` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackduck-c-cpp
-Version: 2.0.3
+Version: 2.0.4
 Summary: Scanning for c/c++ projects using blackduck and coverity tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
@@ -54,14 +54,20 @@
 The signature scan and binary scan will be completed on all supported platforms as permitted by your Black Duck license.
 Any scan cli parameters can be used and passed to blackduck-c-cpp tool through the additional_sig_scan_args parameter.
 
 On Unix-like operating systems, a package manager scan will also be run. Since Windows doesn't have a supported package
 manager, blackduck-c-cpp scans run on Windows won't include the package manager scan and won't produce a BDIO file.
 Here, package manager scan refers to usage of O/S package managers such as yum, apt etc.
 
+## Supported Compilers and Linkers
+
+Run ./cov-configure --list-compiler-types to get complete set of supported compilers
+
+Linkers supported: gcc, msvc.
+
 ## Installation
 
 Minimum version of Black Duck required is 2020.10.0
 
 To install from pypi:
 
 ```
```

### Comparing `blackduck-c-cpp-2.0.3/blackduck_c_cpp.egg-info/SOURCES.txt` & `blackduck-c-cpp-2.0.4/blackduck_c_cpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackduck-c-cpp-2.0.3/setup.py` & `blackduck-c-cpp-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="blackduck-c-cpp",
-    version="2.0.3",
+    version="2.0.4",
     description="Scanning for c/c++ projects using blackduck and coverity tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=["requests>=2.28.2",
                       "numpy>=1.24.2, <=1.26.4",
                       "python-dateutil>=2.8.1",
```

