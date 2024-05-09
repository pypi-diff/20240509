# Comparing `tmp/gaussian_step-2024.1.19.tar.gz` & `tmp/gaussian_step-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussian_step-2024.1.19.tar", last modified: Fri Jan 19 18:18:13 2024, max compression
+gzip compressed data, was "gaussian_step-2024.5.8.tar", last modified: Thu May  9 10:32:05 2024, max compression
```

## Comparing `gaussian_step-2024.1.19.tar` & `gaussian_step-2024.5.8.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.038490 gaussian_step-2024.1.19/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-01-19 18:18:13.038490 gaussian_step-2024.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.030490 gaussian_step-2024.1.19/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.038490 gaussian_step-2024.1.19/gaussian_step/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-19 18:18:13.038490 gaussian_step-2024.1.19/gaussian_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.034490 gaussian_step-2024.1.19/gaussian_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)    21091 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/gaussian_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    36018 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    36445 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/substep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/tk_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/gaussian_step/tk_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.034490 gaussian_step-2024.1.19/gaussian_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-19 18:18:13.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 18:18:00.000000 gaussian_step-2024.1.19/gaussian_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-19 18:18:13.038490 gaussian_step-2024.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 18:18:13.034490 gaussian_step-2024.1.19/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/tests/test_gaussian_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68751 2024-01-19 18:17:57.000000 gaussian_step-2024.1.19/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.529320 gaussian_step-2024.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9564 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.533320 gaussian_step-2024.5.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/gaussian_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/gaussian.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36943 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/substep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11977 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/gaussian_step/tk_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/gaussian_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 10:32:05.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:31:52.000000 gaussian_step-2024.5.8/gaussian_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 10:32:05.541319 gaussian_step-2024.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:32:05.537320 gaussian_step-2024.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/tests/test_gaussian_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-09 10:31:49.000000 gaussian_step-2024.5.8/versioneer.py
```

### Comparing `gaussian_step-2024.1.19/CONTRIBUTING.rst` & `gaussian_step-2024.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/HISTORY.rst` & `gaussian_step-2024.5.8/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2024.5.8 General enhancements
+    * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
+      to the installed version of Gaussian on the machine.
+    * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
     * Added an option to just write the input file, without running
       Gaussian. This is useful for debugging, and for running Gaussian
       on a remote server.
```

### Comparing `gaussian_step-2024.1.19/LICENSE` & `gaussian_step-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/PKG-INFO` & `gaussian_step-2024.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.1.19
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,14 +86,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.8 General enhancements
+    * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
+      to the installed version of Gaussian on the machine.
+    * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
     * Added an option to just write the input file, without running
       Gaussian. This is useful for debugging, and for running Gaussian
       on a remote server.
```

### Comparing `gaussian_step-2024.1.19/README.rst` & `gaussian_step-2024.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/Makefile` & `gaussian_step-2024.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/SEAMM inverted.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/SEAMM logo.png` & `gaussian_step-2024.5.8/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/molssi_main_logo.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/molssi_main_logo_inverted_white.png` & `gaussian_step-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/molssi_square.png` & `gaussian_step-2024.5.8/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/_static/nsf.png` & `gaussian_step-2024.5.8/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/conf.py` & `gaussian_step-2024.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/developer_guide/installation.rst` & `gaussian_step-2024.5.8/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/getting_started/index.rst` & `gaussian_step-2024.5.8/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/index.rst` & `gaussian_step-2024.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/docs/make.bat` & `gaussian_step-2024.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/__init__.py` & `gaussian_step-2024.5.8/gaussian_step/__init__.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/data/references.bib` & `gaussian_step-2024.5.8/gaussian_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/energy.py` & `gaussian_step-2024.5.8/gaussian_step/energy.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,15 +178,20 @@
 
         # Set the attribute for writing just the input
         self.input_only = P["input only"]
 
         # Print what we are doing
         printer.important(__(self.description_text(PP), indent=self.indent))
 
-        # keywords = []
+        # If doing a single point, add the correct keyword for the job type
+        if self.__class__.__name__ == "Energy":
+            if P["calculate gradient"]:
+                keywords.add("FORCE")
+            else:
+                keywords.add("SP")
 
         # Figure out what we are doing!
         if P["level"] == "recommended":
             method_string = P["method"]
         else:
             method_string = P["advanced_method"]
 
@@ -272,14 +277,21 @@
             else:
                 raise ValueError(
                     "Gaussian composite methods are only for single-point calculations."
                 )
         else:
             keywords.add(f"{method}/{basis}")
 
+        if P["use symmetry"] == "loose":
+            keywords.add("Symmetry=Loose")
+        elif P["use symmetry"] == "identify only":
+            keywords.add("NoSymmetry")
+        elif P["use symmetry"] == "no":
+            keywords.add("Symmetry=None")
+
         if "freeze core" in method_data:
             if method_data["freeze core?"] and P["freeze-cores"] == "no":
                 keywords.add("FULL")
 
         if P["maximum iterations"] != "default":
             keywords.add(f"MaxCycle={P['maximum iterations']}")
         if P["convergence"] != "default":
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/energy_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/energy_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,32 @@
             "format_string": "s",
             "description": "Ignore lack of convergence:",
             "help_text": (
                 "Whether to ignore lack of convergence in the SCF. Otherwise, "
                 "an error is thrown."
             ),
         },
+        "use symmetry": {
+            "default": "yes",
+            "kind": "enumeration",
+            "default_units": "",
+            "enumeration": ("yes", "loose", "identify only", "no"),
+            "format_string": "s",
+            "description": "Use symmetry:",
+            "help_text": "Whether to use symmetry, and if so how much.",
+        },
+        "calculate gradient": {
+            "default": "yes",
+            "kind": "boolean",
+            "default_units": "",
+            "enumeration": ("yes", "no"),
+            "format_string": "s",
+            "description": "Calculate gradient:",
+            "help_text": "Whether to calculate the gradient:",
+        },
         "freeze-cores": {
             "default": "yes",
             "kind": "enumeration",
             "default_units": "",
             "enumeration": ("yes", "no"),
             "format_string": "s",
             "description": "Freeze core orbitals:",
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/energy_step.py` & `gaussian_step-2024.5.8/gaussian_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,23 +145,23 @@
         Returns
         -------
         None
         """
         logger.debug(f"Creating Gaussian {self}")
         self.subflowchart = seamm.Flowchart(
             parent=self, name="Gaussian", namespace=namespace
-        )  # yapf: disable
+        )
 
         super().__init__(
             flowchart=flowchart,
             title="Gaussian",
             extension=extension,
             module=__name__,
             logger=logger,
-        )  # yapf: disable
+        )
 
         self.parameters = gaussian_step.GaussianParameters()
         self._data = {}
 
     @property
     def version(self):
         """The semantic version of this module."""
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/gaussian_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/gaussian_step.py` & `gaussian_step-2024.5.8/gaussian_step/gaussian_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/metadata.py` & `gaussian_step-2024.5.8/gaussian_step/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,35 @@
 type : str
     The type of the data: string, integer, or float.
 
 units : str
     Optional units for the result. If present, the value should be in these units.
 """
 metadata["results"] = {
+    "energy": {
+        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "description": "energy",
+        "dimensionality": "scalar",
+        "type": "float",
+        "units": "E_h",
+        "format": ".6f",
+    },
+    "gradients": {
+        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "description": "gradients",
+        "dimensionality": [3, "natoms"],
+        "type": "float",
+        "units": "E_h/a0",
+        "format": ".6f",
+    },
+    "model": {
+        "description": "The model string",
+        "dimensionality": "scalar",
+        "type": "string",
+    },
     "Virial Ratio": {
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "the virial ratio",
         "dimensionality": "scalar",
         "methods": ["DFT", "HF", "MP2", "MP3", "MP4"],
         "type": "float",
         "format": ".4f",
@@ -233,14 +254,22 @@
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "total energy including all terms",
         "dimensionality": "scalar",
         "type": "float",
         "units": "E_h",
         "format": ".6f",
     },
+    "Cartesian Gradient": {
+        "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
+        "description": "the cartesian gradients",
+        "dimensionality": ["natoms", 3],
+        "type": "float",
+        "units": "E_h/a0",
+        "format": ".6f",
+    },
     "RMS Density": {
         "calculation": ["energy", "optimization", "thermodynamics", "vibrations"],
         "description": "the RMS density difference in the SCF",
         "dimensionality": "scalar",
         "methods": ["DFT", "HF", "MP2", "MP3", "MP4"],
         "type": "float",
         "format": ".2e",
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/optimization.py` & `gaussian_step-2024.5.8/gaussian_step/optimization.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/optimization_parameters.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/optimization_step.py` & `gaussian_step-2024.5.8/gaussian_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/substep.py` & `gaussian_step-2024.5.8/gaussian_step/substep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
 
 """Setup and run Gaussian"""
 
 import configparser
 import gzip
+import importlib
 import logging
 from pathlib import Path
 import pprint
 import re
 import shutil
 import string
+import sys
 
 import cclib
 import numpy as np
 
 import gaussian_step
 import seamm
 import seamm_exec
@@ -653,14 +655,15 @@
                 data["Composite/summary"] = tmp + "\n".join(text)
                 data["Total Energy"] = data["Composite/Free Energy"]
 
         return data
 
     def process_data(self, data):
         """Massage the cclib data to a more easily used form."""
+        logger.debug(pprint.pformat(data))
         # Convert numpy arrays to Python lists
         new = {}
         for key, value in data.items():
             if isinstance(value, np.ndarray):
                 new[key] = value.tolist()
             elif isinstance(value, list):
                 if len(value) > 0 and isinstance(value[0], np.ndarray):
@@ -852,62 +855,112 @@
                 x, y, z = xyz
                 lines.append(f"{symbol:2}   {x:10.6f} {y:10.6f} {z:10.6f}")
             lines.append(" ")
 
             files = {"input.dat": "\n".join(lines)}
             logger.info("input.dat:\n" + files["input.dat"])
 
+            printer.important(
+                self.indent + f"    Gaussian will use {n_threads} OpenMP threads and "
+                f"up to {memory} of memory.\n"
+            )
             if self.input_only:
                 # Just write the input files and stop
                 for filename in files:
                     path = directory / filename
                     path.write_text(files[filename])
                 data = {}
             else:
-                # Run Gaussian
                 executor = self.parent.flowchart.executor
 
-                # Read configuration file for Gaussian
-                ini_dir = Path(seamm_options["root"]).expanduser()
-                full_config = configparser.ConfigParser()
-                full_config.read(ini_dir / "gaussian.ini")
+                # Read configuration file for Gaussian if it exists
                 executor_type = executor.name
+                full_config = configparser.ConfigParser()
+                ini_dir = Path(seamm_options["root"]).expanduser()
+                path = ini_dir / "gaussian.ini"
+
+                if path.exists():
+                    full_config.read(ini_dir / "gaussian.ini")
+
+                # If the section we need doesn't exist, get the default
+                if not path.exists() or executor_type not in full_config:
+                    resources = importlib.resources.files("gaussian_step") / "data"
+                    ini_text = (resources / "gaussian.ini").read_text()
+                    full_config.read_string(ini_text)
+
+                # Getting desperate! Look for an executable in the path
                 if executor_type not in full_config:
-                    raise RuntimeError(
-                        f"No section for '{executor_type}' in the Gaussian ini file "
-                        f"({ini_dir / 'mopac.ini'})"
-                    )
+                    # See if we can find the Gaussian environment variables
+                    if "g16root" in sys.environ:
+                        g_ver = "g16"
+                        root_directory = sys.environ["g16root"]
+                    elif "g09root" in sys.environ:
+                        g_ver = "g09"
+                        root_directory = sys.environ["g09root"]
+                    else:
+                        root_directory = None
+                        exe_path = shutil.which("g16")
+                        if exe_path is None:
+                            exe_path = shutil.which("g09")
+                        if exe_path is None:
+                            raise RuntimeError(
+                                f"No section for '{executor_type}' in Gaussian ini file"
+                                f" ({ini_dir / 'gaussian.ini'}), nor in the defaults, "
+                                "nor in the path!"
+                            )
+                        g_ver = exe_path.name
+                        root_directory = str(exe_path.parent.parent)
+                        setup_directory = str(
+                            exe_path.parent / g_ver / f"{g_ver}.profile"
+                        )
+
+                        full_config[executor_type] = {
+                            "installation": "local",
+                            "code": g_ver,
+                            "root-directory": root_directory,
+                            "setup-directory": setup_directory,
+                        }
+
+                # If the ini file does not exist, write it out!
+                if not path.exists():
+                    with path.open("w") as fd:
+                        full_config.write(fd)
+                    printer.normal(f"Wrote the Gaussian configuration file to {path}")
+                    printer.normal("")
+
                 config = dict(full_config.items(executor_type))
+                # Use the matching version of the seamm-gaussian image by default.
+                config["version"] = self.version
+
+                g_ver = config["code"]
 
-                # Set up the environment
+                # Setup the calculation environment definition
                 if config["root-directory"] != "":
-                    env = {"g09root": config["root-directory"]}
+                    env = {f"{g_ver}root": config["root-directory"]}
                 else:
                     env = {}
 
                 if config["setup-environment"] != "":
-                    cmd = [". {setup-environment} ; {code}"]
+                    cmd = f". {config['setup-environment']} ; {g_ver}"
                 else:
-                    cmd = ["{code}"]
+                    cmd = g_ver
 
-                cmd.append(" < input.dat > output.txt ; formchk gaussian.chk")
-
-                printer.important(
-                    self.indent + f"    Gaussian will use {n_threads} OpenMP threads "
-                    f"and up to {memory} of memory.\n"
-                )
+                cmd += " < input.dat > output.txt ; formchk gaussian.chk"
 
                 return_files = [
                     "output.txt",
                     "gaussian.chk",
                     "gaussian.fchk",
                 ]
+
+                self.logger.info(f"{cmd=}")
+                self.logger.info(f"{env=}")
+
                 result = executor.run(
-                    cmd=cmd,
-                    ce=ce,
+                    cmd=[cmd],
                     config=config,
                     directory=self.directory,
                     files=files,
                     return_files=return_files,
                     in_situ=True,
                     shell=True,
                     env=env,
@@ -940,25 +993,45 @@
                 keys = "\n".join(data.keys())
                 logger.info(f"Data keys:\n{keys}")
             if self.logger.isEnabledFor(logging.DEBUG):
                 keys = "\n".join(data.keys())
                 logger.info(f"Data keys:\n{keys}")
                 logger.debug(f"Data:\n{pprint.pformat(data)}")
 
+            # Explicitly pull out the energy and gradients to standard name
+            if "Total Energy" in data:
+                data["energy"] = data["Total Energy"]
+                del data["Total Energy"]
+            if "Cartesian Gradient" in data:
+                tmp = np.array(data["Cartesian Gradient"])
+                data["gradients"] = tmp.reshape(-1, 3).tolist()
+                del data["Cartesian Gradient"]
+
+            # Debug output
+            if self.logger.isEnabledFor(logging.INFO):
+                keys = "\n".join(data.keys())
+                logger.info(f"Data keys:\n{keys}")
+            if self.logger.isEnabledFor(logging.DEBUG):
+                keys = "\n".join(data.keys())
+                logger.info(f"Data keys:\n{keys}")
+                logger.debug(f"Data:\n{pprint.pformat(data)}")
+
             # The model chemistry
             # self.model = f"{data['metadata/functional']}/{data['metadata/basis_set']}"
             if "Composite/model" in data:
                 self.model = data["Composite/model"]
             else:
                 self.model = (
                     f"{data['metadata/methods'][-1]}/{data['method']}/"
                     f"{data['metadata/basis_set']}"
                 )
             logger.info(f"model = {self.model}")
 
+            data["model"] = "Gaussian/" + self.model
+
             # If ran successfully, put out the success file
             if data["success"]:
                 success.write_text("success")
 
         # Add other citations here or in the appropriate place in the code.
         # Add the bibtex to data/references.bib, and add a self.reference.cite
         # similar to the above to actually add the citation to the references.
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/tk_energy.py` & `gaussian_step-2024.5.8/gaussian_step/tk_energy.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             "basis",
             "advanced_method",
             "functional",
             "advanced_functional",
             "dispersion",
             "spin-restricted",
             "freeze-cores",
+            "use symmetry",
+            "calculate gradient",
         ):
             self[key] = P[key].widget(self["calculation"])
 
         # bindings...
         for key in ("level", "method", "advanced_method"):
             self[key].bind("<<ComboboxSelected>>", self.reset_calculation)
             self[key].bind("<Return>", self.reset_calculation)
@@ -266,16 +268,26 @@
                     widgets2.append(self["dispersion"])
                     row += 1
                     sw.align_labels(widgets2, sticky=tk.E)
                 frame.columnconfigure(0, minsize=30)
         self["spin-restricted"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
         widgets.append(self["spin-restricted"])
         row += 1
+        self["use symmetry"].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
+        widgets.append(self["use symmetry"])
+        row += 1
         sw.align_labels(widgets, sticky=tk.E)
 
+        if self.__class__.__name__ == "TkEnergy":
+            self["calculate gradient"].grid(
+                row=row, column=0, columnspan=2, sticky=tk.EW
+            )
+            widgets.append(self["calculate gradient"])
+            row += 1
+
         return row
 
     def reset_convergence(self, widget=None):
         """Layout the convergence widgets as needed for the current state"""
 
         frame = self["convergence frame"]
         for slave in frame.grid_slaves():
```

### Comparing `gaussian_step-2024.1.19/gaussian_step/tk_gaussian.py` & `gaussian_step-2024.5.8/gaussian_step/tk_gaussian.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step/tk_optimization.py` & `gaussian_step-2024.5.8/gaussian_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/gaussian_step.egg-info/PKG-INFO` & `gaussian_step-2024.5.8/gaussian_step.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_step
-Version: 2024.1.19
+Version: 2024.5.8
 Summary: A SEAMM plugin for A SEAMM plug-in for Gaussian
 Home-page: https://github.com/molssi-seamm/gaussian_step
 Author: Paul Saxe
 Author-email: psaxe@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -86,14 +86,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.8 General enhancements
+    * Updated to new calculation handling, with ~/SEAMM/gaussian.ini controlling access
+      to the installed version of Gaussian on the machine.
+    * Added energy and gradients to results to support general use in e.g. energy scans.
 
 2024.1.19: Switched to new way to run Gaussian, added option to just write input file
     * Switched to using the new way to run executables, which supports containers.
     * Added an option to just write the input file, without running
       Gaussian. This is useful for debugging, and for running Gaussian
       on a remote server.
```

### Comparing `gaussian_step-2024.1.19/gaussian_step.egg-info/SOURCES.txt` & `gaussian_step-2024.5.8/gaussian_step.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,11 +48,12 @@
 gaussian_step.egg-info/PKG-INFO
 gaussian_step.egg-info/SOURCES.txt
 gaussian_step.egg-info/dependency_links.txt
 gaussian_step.egg-info/entry_points.txt
 gaussian_step.egg-info/requires.txt
 gaussian_step.egg-info/top_level.txt
 gaussian_step.egg-info/zip-safe
+gaussian_step/data/gaussian.ini
 gaussian_step/data/properties.csv
 gaussian_step/data/references.bib
 tests/__init__.py
 tests/test_gaussian_step.py
```

### Comparing `gaussian_step-2024.1.19/setup.py` & `gaussian_step-2024.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `gaussian_step-2024.1.19/versioneer.py` & `gaussian_step-2024.5.8/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -272,15 +273,14 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
-
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,59 +304,54 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
+        err = ("Versioneer was unable to run the project root directory. "
+               "Versioneer requires setup.py to be executed from "
+               "its immediate directory (like 'python setup.py COMMAND'), "
+               "or in a way that lets it use sys.argv[0] to find the root "
+               "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
-            )
+            print("Warning: build in %s is using versioneer.py from %s"
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
-
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -373,40 +368,36 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
-
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
-
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-            )
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -423,17 +414,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = '''
+LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -1000,86 +989,71 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
+            r = ref[len(tag_prefix):]
             if verbose:
                 print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
-        GITS,
-        [
-            "describe",
-            "--tags",
-            "--dirty",
-            "--always",
-            "--long",
-            "--match",
-            "%s*" % tag_prefix,
-        ],
-        cwd=root,
-    )
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1094,55 +1068,54 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = ("unable to parse git-describe output: '%s'"
+                               % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
+            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+                               % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
-        0
-    ].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1190,30 +1163,24 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print(
-            "Tried directories %s but none started with prefix %s"
-            % (str(rootdirs), parentdir_prefix)
-        )
+        print("Tried directories %s but none started with prefix %s" %
+              (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1234,30 +1201,29 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-    )
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+                   contents, re.M | re.S)
     if not mo:
-        mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-        )
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+                       contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True,
+                          indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1281,15 +1247,16 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1395,21 +1362,19 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1421,21 +1386,17 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1450,17 +1411,16 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert (
-        cfg.versionfile_source is not None
-    ), "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, \
+        "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1506,21 +1466,17 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None, "error": "unable to compute version",
+            "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1561,15 +1517,14 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1594,23 +1549,22 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib,
+                                                  cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
-
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1623,29 +1577,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if "py2exe" in sys.modules:  # py2exe enabled?
+    if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1656,25 +1606,21 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1693,18 +1639,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(
-                target_versionfile, self._versioneer_generated_versions
-            )
-
+            write_to_version_file(target_versionfile,
+                                  self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1751,41 +1695,36 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
+    except (EnvironmentError, configparser.NoSectionError,
+            configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg",
+                  file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
+        f.write(LONG % {"DOLLAR": "$",
+                        "STYLE": cfg.style,
+                        "TAG_PREFIX": cfg.tag_prefix,
+                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        })
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
+                       "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1819,18 +1758,16 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

