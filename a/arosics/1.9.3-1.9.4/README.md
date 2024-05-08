# Comparing `tmp/arosics-1.9.3.tar.gz` & `tmp/arosics-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arosics-1.9.3.tar", last modified: Mon Oct 16 14:50:44 2023, max compression
+gzip compressed data, was "arosics-1.9.4.tar", last modified: Thu Nov 23 00:14:02 2023, max compression
```

## Comparing `arosics-1.9.3.tar` & `arosics-1.9.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.788709 arosics-1.9.3/
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-10-16 14:50:10.000000 arosics-1.9.3/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-10-16 14:50:10.000000 arosics-1.9.3/.editorconfig
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.760710 arosics-1.9.3/.github/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-10-16 14:50:10.000000 arosics-1.9.3/.github/ISSUE_TEMPLATE.md
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-10-16 14:50:10.000000 arosics-1.9.3/.github/create_release_from_gitlab_ci.sh
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-10-16 14:50:10.000000 arosics-1.9.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3312 2023-10-16 14:50:10.000000 arosics-1.9.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-10-16 14:50:10.000000 arosics-1.9.3/.zenodo.json
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-10-16 14:50:10.000000 arosics-1.9.3/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-10-16 14:50:10.000000 arosics-1.9.3/CITATION
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-10-16 14:50:10.000000 arosics-1.9.3/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    25401 2023-10-16 14:50:10.000000 arosics-1.9.3/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)    10140 2023-10-16 14:50:10.000000 arosics-1.9.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-10-16 14:50:10.000000 arosics-1.9.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4072 2023-10-16 14:50:10.000000 arosics-1.9.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     9783 2023-10-16 14:50:44.788709 arosics-1.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6418 2023-10-16 14:50:10.000000 arosics-1.9.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.760710 arosics-1.9.3/arosics/
--rwxrwxrwx   0 root         (0) root         (0)    86408 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/CoReg.py
--rw-rw-rw-   0 root         (0) root         (0)    42345 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/CoReg_local.py
--rw-rw-rw-   0 root         (0) root         (0)    23187 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/DeShifter.py
--rwxrwxrwx   0 root         (0) root         (0)    70315 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/Tie_Point_Grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20799 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/arosics_cli.py
--rwxrwxrwx   0 root         (0) root         (0)     6933 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-10-16 14:50:10.000000 arosics-1.9.3/arosics/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.764710 arosics-1.9.3/arosics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9783 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1807 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      628 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-16 14:50:44.000000 arosics-1.9.3/arosics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.764710 arosics-1.9.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.756711 arosics-1.9.3/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.756711 arosics-1.9.3/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.772710 arosics-1.9.3/docs/_build/html/_images/
--rw-r--r--   0 root         (0) root         (0)    43518 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/CoregPoints_table.png
--rw-r--r--   0 root         (0) root         (0)   772233 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-r--r--   0 root         (0) root         (0)     6615 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)   994099 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/output_40_1.png
--rw-r--r--   0 root         (0) root         (0)  1009524 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/output_44_1.png
--rw-r--r--   0 root         (0) root         (0)   297816 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.772710 arosics-1.9.3/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)     6615 2023-10-16 14:43:58.000000 arosics-1.9.3/docs/_build/html/_static/arosics_logo.png
--rw-r--r--   0 root         (0) root         (0)      286 2022-10-16 10:21:34.000000 arosics-1.9.3/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.3/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.772710 arosics-1.9.3/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/about.rst
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/api_cli_reference.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/cli_reference.rst
--rwxrwxrwx   0 root         (0) root         (0)     9929 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.780709 arosics-1.9.3/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    43518 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/CoregPoints_table.png
--rw-rw-rw-   0 root         (0) root         (0)   954684 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
--rw-rw-rw-   0 root         (0) root         (0)   772233 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
--rw-rw-rw-   0 root         (0) root         (0)     6615 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/arosics_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   994099 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/output_40_1.png
--rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/output_44_1.png
--rw-rw-rw-   0 root         (0) root         (0)   297816 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/images/shift_vectors_testcase1__900x824.gif
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     6461 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 14:50:44.780709 arosics-1.9.3/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)    10547 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/usage/global_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/usage/input_data_requirements.rst
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/usage/local_coreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-10-16 14:50:10.000000 arosics-1.9.3/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-10-16 14:50:10.000000 arosics-1.9.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-10-16 14:50:44.788709 arosics-1.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4194 2023-10-16 14:50:10.000000 arosics-1.9.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-10-16 14:50:10.000000 arosics-1.9.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.771213 arosics-1.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-11-23 00:13:35.000000 arosics-1.9.4/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-11-23 00:13:35.000000 arosics-1.9.4/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.751214 arosics-1.9.4/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-11-23 00:13:35.000000 arosics-1.9.4/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-11-23 00:13:35.000000 arosics-1.9.4/.github/create_release_from_gitlab_ci.sh
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-11-23 00:13:35.000000 arosics-1.9.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2023-11-23 00:13:35.000000 arosics-1.9.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-11-23 00:13:35.000000 arosics-1.9.4/.zenodo.json
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-11-23 00:13:35.000000 arosics-1.9.4/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2023-11-23 00:13:35.000000 arosics-1.9.4/CITATION
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-11-23 00:13:35.000000 arosics-1.9.4/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    25585 2023-11-23 00:13:35.000000 arosics-1.9.4/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10140 2023-11-23 00:13:35.000000 arosics-1.9.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-11-23 00:13:35.000000 arosics-1.9.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2023-11-23 00:13:35.000000 arosics-1.9.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9921 2023-11-23 00:14:02.771213 arosics-1.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6418 2023-11-23 00:13:35.000000 arosics-1.9.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.755214 arosics-1.9.4/arosics/
+-rwxrwxrwx   0 root         (0) root         (0)    86461 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/CoReg.py
+-rw-rw-rw-   0 root         (0) root         (0)    42345 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/CoReg_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    23187 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/DeShifter.py
+-rwxrwxrwx   0 root         (0) root         (0)    70335 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/Tie_Point_Grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20799 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/arosics_cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     6933 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-11-23 00:13:35.000000 arosics-1.9.4/arosics/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.767213 arosics-1.9.4/arosics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9921 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      655 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-11-23 00:14:02.000000 arosics-1.9.4/arosics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.755214 arosics-1.9.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6769 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.747214 arosics-1.9.4/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.747214 arosics-1.9.4/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.759214 arosics-1.9.4/docs/_build/html/_images/
+-rw-r--r--   0 root         (0) root         (0)    43518 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/CoregPoints_table.png
+-rw-r--r--   0 root         (0) root         (0)   772233 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)   994099 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/output_40_1.png
+-rw-r--r--   0 root         (0) root         (0)  1009524 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/output_44_1.png
+-rw-r--r--   0 root         (0) root         (0)   297816 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.763213 arosics-1.9.4/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-11-23 00:08:58.000000 arosics-1.9.4/docs/_build/html/_static/arosics_logo.png
+-rw-r--r--   0 root         (0) root         (0)      286 2022-10-16 10:21:34.000000 arosics-1.9.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2022-10-16 10:21:34.000000 arosics-1.9.4/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.763213 arosics-1.9.4/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/about.rst
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/api_cli_reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/cli_reference.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9929 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.767213 arosics-1.9.4/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43518 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/CoregPoints_table.png
+-rw-rw-rw-   0 root         (0) root         (0)   954684 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif
+-rw-rw-rw-   0 root         (0) root         (0)   772233 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif
+-rw-rw-rw-   0 root         (0) root         (0)     6615 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/arosics_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   994099 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/output_40_1.png
+-rw-rw-rw-   0 root         (0) root         (0)  1009524 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/output_44_1.png
+-rw-rw-rw-   0 root         (0) root         (0)   297816 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/images/shift_vectors_testcase1__900x824.gif
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 00:14:02.767213 arosics-1.9.4/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)    10547 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/usage/global_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/usage/input_data_requirements.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/usage/local_coreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-11-23 00:13:35.000000 arosics-1.9.4/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-11-23 00:13:35.000000 arosics-1.9.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-11-23 00:14:02.775213 arosics-1.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2023-11-23 00:13:35.000000 arosics-1.9.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-11-23 00:13:35.000000 arosics-1.9.4/tox.ini
```

### Comparing `arosics-1.9.3/.coveragerc` & `arosics-1.9.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/.github/create_release_from_gitlab_ci.sh` & `arosics-1.9.4/.github/create_release_from_gitlab_ci.sh`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/.gitignore` & `arosics-1.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/.gitlab-ci.yml` & `arosics-1.9.4/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
   stage: test
   coverage: '/TOTAL\s+\d+\s+\d+\s+(\d+%)/'
   script:
     - source activate ci_env
 
     # update py_tools_ds and geoarray
     - mamba update py-tools-ds geoarray
-    - mamba install "scikit-image>=0.21.0"  # TODO: remove as soon as CI runner is rebuilt
 
     # run tests
     - make pytest
 
     # create the docs
     - make docs
   artifacts:
```

### Comparing `arosics-1.9.3/.zenodo.json` & `arosics-1.9.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/CITATION` & `arosics-1.9.4/CITATION`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/CONTRIBUTING.rst` & `arosics-1.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/HISTORY.rst` & `arosics-1.9.4/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+1.9.4 (2023-11-23)
+------------------
+
+* !42: Fixed https://github.com/GFZ/arosics/issues/33
+  ('TypeError: ufunc 'invert' not supported for the input types' when using input mask).
+
+
 1.9.3 (2023-10-16)
 ------------------
 
 * !41: Fixed #86 (ValueError when calling CoReg.show_matchWin(interactive=True))
   and improved interactive output of CoReg.show_matchWin.
```

### Comparing `arosics-1.9.3/LICENSE` & `arosics-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/Makefile` & `arosics-1.9.4/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/PKG-INFO` & `arosics-1.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.9.3
+Version: 1.9.4
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
@@ -46,38 +46,41 @@
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shapely
 Provides-Extra: interactive-plotting
 Requires-Dist: holoviews; extra == "interactive-plotting"
 Requires-Dist: ipython; extra == "interactive-plotting"
+Requires-Dist: nbformat; extra == "interactive-plotting"
 Provides-Extra: doc
 Requires-Dist: sphinx-argparse; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-reporter-html1; extra == "test"
 Requires-Dist: urlchecker; extra == "test"
 Requires-Dist: holoviews; extra == "test"
 Requires-Dist: ipython; extra == "test"
+Requires-Dist: nbformat; extra == "test"
 Provides-Extra: lint
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: pycodestyle; extra == "lint"
 Requires-Dist: pydocstyle; extra == "lint"
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: setuptools-git; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-reporter-html1; extra == "dev"
 Requires-Dist: urlchecker; extra == "dev"
 Requires-Dist: holoviews; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: nbformat; extra == "dev"
 Requires-Dist: sphinx-argparse; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 Requires-Dist: pydocstyle; extra == "dev"
```

### Comparing `arosics-1.9.3/README.rst` & `arosics-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/CoReg.py` & `arosics-1.9.4/arosics/CoReg.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             self.footprint_poly = self.footprint_poly.buffer(0)
 
         if not self.q:
             print('Bounding box of calculated footprint for %s:\n\t%s' % (self.imName, self.footprint_poly.bounds))
 
         # add bad data mask
         given_mask = CoReg_params['mask_baddata_%s' % ('ref' if imID == 'ref' else 'tgt')]
-        if given_mask:
+        if given_mask is not None:
             self.mask_baddata = given_mask  # runs GeoArray.mask_baddata.setter -> sets it to BadDataMask()
 
     poly = alias_property('footprint_poly')  # ensures that self.poly is updated if self.footprint_poly is updated
 
 
 class COREG(object):
     """The COREG class detects and corrects global X/Y shifts between a target and reference image.
@@ -1242,19 +1242,21 @@
         y_shift = peakpos[0] - arr_shape[0] // 2
         x_shift = peakpos[1] - arr_shape[1] // 2
         return x_shift, y_shift
 
     @staticmethod
     def _clip_image(im, center_YX, winSzYX):  # TODO this is also implemented in GeoArray
 
-        def get_bounds(YX, wsY, wsX):
-            return int(YX[1] - (wsX / 2)),\
-                   int(YX[1] + (wsX / 2)),\
-                   int(YX[0] - (wsY / 2)),\
-                   int(YX[0] + (wsY / 2))
+        def get_bounds(YX: tuple, wsY: float, wsX: float):
+            return (
+                int(YX[1] - (wsX / 2)),
+                int(YX[1] + (wsX / 2)),
+                int(YX[0] - (wsY / 2)),
+                int(YX[0] + (wsY / 2))
+            )
 
         wsY, wsX = winSzYX
         xmin, xmax, ymin, ymax = get_bounds(center_YX, wsY, wsX)
 
         return im[ymin:ymax, xmin:xmax]
 
     def _get_grossly_deshifted_images(self, im0, im1, x_intshift, y_intshift):
```

### Comparing `arosics-1.9.3/arosics/CoReg_local.py` & `arosics-1.9.4/arosics/CoReg_local.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/DeShifter.py` & `arosics-1.9.4/arosics/DeShifter.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/Tie_Point_Grid.py` & `arosics-1.9.4/arosics/Tie_Point_Grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         XY_mapPoints[:, 1] = mapYarr.flat
 
         assert XY_points.shape == XY_mapPoints.shape
 
         return XY_points, XY_mapPoints
 
     def _exclude_bad_XYpos(self, GDF):
-        """Exclude all points outside of the image overlap area and where the bad data mask is True (if given).
+        """Exclude all points outside the image overlap area and where the bad data mask is True (if given).
 
         :param GDF:     <geopandas.GeoDataFrame> must include the columns 'X_MAP' and 'Y_MAP'
         :return:
         """
         from skimage.measure import points_in_poly  # import here to avoid static TLS ImportError
 
         # exclude all points outside of overlap area
@@ -266,15 +266,15 @@
         assert not GDF.empty, 'No coregistration point could be placed within the overlap area. Check your input data!'
 
         # exclude all points where bad data mask is True (e.g. points on clouds etc.)
         orig_len_GDF = len(GDF)  # length of GDF after dropping all points outside the overlap polygon
         mapXY = np.array(GDF.loc[:, ['X_MAP', 'Y_MAP']])
         GDF['REF_BADDATA'] = self.COREG_obj.ref.mask_baddata.read_pointData(mapXY) \
             if self.COREG_obj.ref.mask_baddata is not None else False
-        GDF['TGT_BADDATA'] = self.COREG_obj.shift.mask_baddata.read_pointData(mapXY) \
+        GDF['TGT_BADDATA'] = self.COREG_obj.shift.mask_baddata.read_pointData(mapXY).flatten().astype(bool) \
             if self.COREG_obj.shift.mask_baddata is not None else False
         GDF = GDF[(~GDF['REF_BADDATA']) & (~GDF['TGT_BADDATA'])]
         if self.COREG_obj.ref.mask_baddata is not None or self.COREG_obj.shift.mask_baddata is not None:
             if not self.q:
                 if not GDF.empty:
                     print('With respect to the provided bad data mask(s) %s points of initially %s have been excluded.'
                           % (orig_len_GDF - len(GDF), orig_len_GDF))
```

### Comparing `arosics-1.9.3/arosics/__init__.py` & `arosics-1.9.4/arosics/__init__.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/arosics_cli.py` & `arosics-1.9.4/arosics/arosics_cli.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/geometry.py` & `arosics-1.9.4/arosics/geometry.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/plotting.py` & `arosics-1.9.4/arosics/plotting.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/arosics/version.py` & `arosics-1.9.4/arosics/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.9.3'
-__versionalias__ = '2023-10-16_01'
+__version__ = '1.9.4'
+__versionalias__ = '2023-11-23_01'
```

### Comparing `arosics-1.9.3/arosics.egg-info/PKG-INFO` & `arosics-1.9.4/arosics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arosics
-Version: 1.9.3
+Version: 1.9.4
 Summary: An Automated and Robust Open-Source Image Co-Registration Software for Multi-Sensor Satellite Data
 Home-page: https://git.gfz-potsdam.de/danschef/arosics
 Author: Daniel Scheffler
 Author-email: daniel.scheffler@gfz-potsdam.de
 License: Apache-2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/danschef/arosics
 Project-URL: Issue Tracker, https://git.gfz-potsdam.de/danschef/arosics/-/issues
@@ -46,38 +46,41 @@
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shapely
 Provides-Extra: interactive-plotting
 Requires-Dist: holoviews; extra == "interactive-plotting"
 Requires-Dist: ipython; extra == "interactive-plotting"
+Requires-Dist: nbformat; extra == "interactive-plotting"
 Provides-Extra: doc
 Requires-Dist: sphinx-argparse; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-reporter-html1; extra == "test"
 Requires-Dist: urlchecker; extra == "test"
 Requires-Dist: holoviews; extra == "test"
 Requires-Dist: ipython; extra == "test"
+Requires-Dist: nbformat; extra == "test"
 Provides-Extra: lint
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: pycodestyle; extra == "lint"
 Requires-Dist: pydocstyle; extra == "lint"
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: setuptools-git; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-reporter-html1; extra == "dev"
 Requires-Dist: urlchecker; extra == "dev"
 Requires-Dist: holoviews; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: nbformat; extra == "dev"
 Requires-Dist: sphinx-argparse; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pycodestyle; extra == "dev"
 Requires-Dist: pydocstyle; extra == "dev"
```

### Comparing `arosics-1.9.3/arosics.egg-info/SOURCES.txt` & `arosics-1.9.4/arosics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/Makefile` & `arosics-1.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/CoregPoints_table.png` & `arosics-1.9.4/docs/_build/html/_images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.4/docs/_build/html/_images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/arosics_logo.png` & `arosics-1.9.4/docs/_build/html/_images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/output_40_1.png` & `arosics-1.9.4/docs/_build/html/_images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/output_44_1.png` & `arosics-1.9.4/docs/_build/html/_images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.4/docs/_build/html/_images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/_build/html/_static/arosics_logo.png` & `arosics-1.9.4/docs/_build/html/_static/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/about.rst` & `arosics-1.9.4/docs/about.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/cli_reference.rst` & `arosics-1.9.4/docs/cli_reference.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/conf.py` & `arosics-1.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/CoregPoints_table.png` & `arosics-1.9.4/docs/images/CoregPoints_table.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif` & `arosics-1.9.4/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_1066x540.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif` & `arosics-1.9.4/docs/images/animation_testcase1_zoom_L8_S2_global_coreg_before_after_900x456.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/arosics_logo.png` & `arosics-1.9.4/docs/images/arosics_logo.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/output_40_1.png` & `arosics-1.9.4/docs/images/output_40_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/output_44_1.png` & `arosics-1.9.4/docs/images/output_44_1.png`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/images/shift_vectors_testcase1__900x824.gif` & `arosics-1.9.4/docs/images/shift_vectors_testcase1__900x824.gif`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/installation.rst` & `arosics-1.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/make.bat` & `arosics-1.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/usage/global_coreg.rst` & `arosics-1.9.4/docs/usage/global_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/usage/input_data_requirements.rst` & `arosics-1.9.4/docs/usage/input_data_requirements.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/usage/local_coreg.rst` & `arosics-1.9.4/docs/usage/local_coreg.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/docs/usage.rst` & `arosics-1.9.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `arosics-1.9.3/setup.py` & `arosics-1.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ]
 
 req_setup = [
     'setuptools',
     'setuptools-git'
 ]
 
-req_intplot = ['holoviews', 'ipython']
+req_intplot = ['holoviews', 'ipython', 'nbformat']
 
 req_test = ['pytest', 'pytest-cov', 'pytest-reporter-html1', 'urlchecker'] + req_intplot
 
 req_doc = ['sphinx-argparse', 'sphinx_rtd_theme', 'sphinx-autodoc-typehints']
 
 req_lint = ['flake8', 'pycodestyle', 'pydocstyle']
```

