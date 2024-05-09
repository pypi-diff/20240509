# Comparing `tmp/nctoolkit-1.1.7.tar.gz` & `tmp/nctoolkit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nctoolkit-1.1.7.tar", last modified: Tue Mar 19 14:50:46 2024, max compression
+gzip compressed data, was "nctoolkit-1.1.9.tar", last modified: Mon Apr 22 08:16:34 2024, max compression
```

## Comparing `nctoolkit-1.1.7.tar` & `nctoolkit-1.1.9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.853594 nctoolkit-1.1.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)  2588969 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/benchmarks/benchmark_nctoolkit_versus_xarray.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.857594 nctoolkit-1.1.7/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (127)   123355 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/cheatsheet/nctoolkit_cheatsheet.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   383473 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/cheatsheet/nctoolkit_cheatsheet.pptx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.857594 nctoolkit-1.1.7/checklists/
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/checklists/api_checker.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.861594 nctoolkit-1.1.7/data/
--rw-r--r--   0 runner    (1001) docker     (127)   802316 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/data/geotiff.tif
--rw-r--r--   0 runner    (1001) docker     (127)   163943 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/data/pubplot_test.png
--rw-r--r--   0 runner    (1001) docker     (127)   488867 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/data/test1.html
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/data/test2.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/nctoolkit/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1097 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22633 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/add_etc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/anomaly.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    59943 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2372 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/append.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/cdo_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2163 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/cellareas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/centres.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/clear.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7893 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7515 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/compare_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/corr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/create_ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5253 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/distgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3667 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/esoteric.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/fill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/fldstat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/format.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2560 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/generate_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/inttime.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      817 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/invert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/masking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/matchpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/mergers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/meridonials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/mp_adders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/mp_matchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/mp_matchups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/nco_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/phenology.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/reduce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1003 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/reduce_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6908 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/regrid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/rename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/rollstat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1290 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/runthis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/session.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    24976 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/static_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/strip_vars.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16124 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1837 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/sumall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    24211 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/temporal_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/temporals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/thresholds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/to_lonlat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4924 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/to_nc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3757 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/toxarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/tozlev.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/unify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/validator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22714 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/validator_funs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21545 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/verticals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      468 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/nctoolkit/zonals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/nctoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-19 14:50:46.000000 nctoolkit-1.1.7/nctoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3305 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:50:46.873594 nctoolkit-1.1.7/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/testing/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 14:50:34.000000 nctoolkit-1.1.7/testing/test_scripting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.565391 nctoolkit-1.1.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)  2588969 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/benchmarks/benchmark_nctoolkit_versus_xarray.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.569392 nctoolkit-1.1.9/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)   141560 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/cheatsheet/nctoolkit_cheatsheet.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   383473 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/cheatsheet/nctoolkit_cheatsheet.pptx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.573392 nctoolkit-1.1.9/checklists/
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/checklists/api_checker.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.573392 nctoolkit-1.1.9/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   802316 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/data/geotiff.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   163943 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/data/pubplot_test.png
+-rw-r--r--   0 runner    (1001) docker     (127)   488867 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/data/test1.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-04-22 08:16:25.000000 nctoolkit-1.1.9/data/test2.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/nctoolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1097 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22633 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/add_etc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/anomaly.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59943 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2372 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/append.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/cdo_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2163 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/cellareas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/centres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/clear.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7893 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7515 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/compare_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/corr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1431 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/create_ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5253 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/distgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3667 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/esoteric.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/fill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/fldstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/format.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2560 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/generate_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/inttime.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      817 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/invert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/matchpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/meridonials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/mp_adders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/mp_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/mp_matchups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/nco_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/phenology.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3769 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/reduce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1003 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/reduce_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6908 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/regrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/rename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/rollstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1290 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/runthis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24881 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/static_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/strip_vars.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16124 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1837 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/sumall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24211 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/temporal_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/temporals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/thresholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/to_lonlat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4924 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/to_nc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3757 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/toxarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/tozlev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/unify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22714 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/validator_funs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21545 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/verticals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      468 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/nctoolkit/zonals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/nctoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-22 08:16:34.000000 nctoolkit-1.1.9/nctoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3400 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:34.593392 nctoolkit-1.1.9/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/testing/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 08:16:26.000000 nctoolkit-1.1.9/testing/test_scripting.py
```

### Comparing `nctoolkit-1.1.7/CITATION.cff` & `nctoolkit-1.1.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/CODE_OF_CONDUCT.md` & `nctoolkit-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/LICENSE` & `nctoolkit-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/MANIFEST.in` & `nctoolkit-1.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/PKG-INFO` & `nctoolkit-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nctoolkit
-Version: 1.1.7
+Version: 1.1.9
 Summary: A Python package for netCDF analysis and post-processing
 Home-page: https://github.com/pmlmodelling/nctoolkit
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/nctoolkit/issues
 Project-URL: Documentation, https://nctoolkit.readthedocs.io/en/stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6.1
+Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: xarray
 Requires-Dist: netCDF4
 Requires-Dist: hvplot
 Requires-Dist: panel
 Requires-Dist: pandas
 Requires-Dist: ncplot>=0.2.8
```

### Comparing `nctoolkit-1.1.7/README.md` & `nctoolkit-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/benchmarks/benchmark_nctoolkit_versus_xarray.ipynb` & `nctoolkit-1.1.9/benchmarks/benchmark_nctoolkit_versus_xarray.ipynb`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/cheatsheet/nctoolkit_cheatsheet.pdf` & `nctoolkit-1.1.9/cheatsheet/nctoolkit_cheatsheet.pdf`

 * *Files 15% similar despite different names*

#### Comparing `nctoolkit-1.1.7/cheatsheet/nctoolkit_cheatsheet.pdf` & `nctoolkit-1.1.9/cheatsheet/nctoolkit_cheatsheet.pdf`

 * *Document info*

```diff
@@ -1,2 +1,2 @@
-CreationDate: "D:20240206031054-08'00'"
-ModDate: "D:20240206031054-08'00'"
+CreationDate: "D:20240402013215-07'00'"
+ModDate: "D:20240402013215-07'00'"
```

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 Exporting datasets
 
-nctoolkit v1.1.6
+nctoolkit v1.1.8
 Cheat Sheet
 
 Creating datasets
 ds = nc.open_data(foo.nc)
 Open a local file as a dataset.
 ds = nc.open_url(‘https://foo.foo.nc’)
 Open/download a file as a dataset.
```

### Comparing `nctoolkit-1.1.7/cheatsheet/nctoolkit_cheatsheet.pptx` & `nctoolkit-1.1.9/cheatsheet/nctoolkit_cheatsheet.pptx`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/checklists/api_checker.ipynb` & `nctoolkit-1.1.9/checklists/api_checker.ipynb`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/data/geotiff.tif` & `nctoolkit-1.1.9/data/geotiff.tif`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/data/pubplot_test.png` & `nctoolkit-1.1.9/data/pubplot_test.png`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/data/test1.html` & `nctoolkit-1.1.9/data/test1.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/data/test2.html` & `nctoolkit-1.1.9/data/test2.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/__init__.py` & `nctoolkit-1.1.9/nctoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/add_etc.py` & `nctoolkit-1.1.9/nctoolkit/add_etc.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/anomaly.py` & `nctoolkit-1.1.9/nctoolkit/anomaly.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/api.py` & `nctoolkit-1.1.9/nctoolkit/api.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/append.py` & `nctoolkit-1.1.9/nctoolkit/append.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/assign.py` & `nctoolkit-1.1.9/nctoolkit/assign.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/cdo_command.py` & `nctoolkit-1.1.9/nctoolkit/cdo_command.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/cellareas.py` & `nctoolkit-1.1.9/nctoolkit/cellareas.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/centres.py` & `nctoolkit-1.1.9/nctoolkit/centres.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/checks.py` & `nctoolkit-1.1.9/nctoolkit/checks.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/cleanup.py` & `nctoolkit-1.1.9/nctoolkit/cleanup.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/clear.py` & `nctoolkit-1.1.9/nctoolkit/clear.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/compare.py` & `nctoolkit-1.1.9/nctoolkit/compare.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/compare_data.py` & `nctoolkit-1.1.9/nctoolkit/compare_data.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/corr.py` & `nctoolkit-1.1.9/nctoolkit/corr.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/create_ensemble.py` & `nctoolkit-1.1.9/nctoolkit/create_ensemble.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/crop.py` & `nctoolkit-1.1.9/nctoolkit/crop.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/deprecated.py` & `nctoolkit-1.1.9/nctoolkit/deprecated.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/distgrid.py` & `nctoolkit-1.1.9/nctoolkit/distgrid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/drop.py` & `nctoolkit-1.1.9/nctoolkit/drop.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/ensembles.py` & `nctoolkit-1.1.9/nctoolkit/ensembles.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/esoteric.py` & `nctoolkit-1.1.9/nctoolkit/esoteric.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/fill.py` & `nctoolkit-1.1.9/nctoolkit/fill.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/fldstat.py` & `nctoolkit-1.1.9/nctoolkit/fldstat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/format.py` & `nctoolkit-1.1.9/nctoolkit/format.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/generate_grid.py` & `nctoolkit-1.1.9/nctoolkit/generate_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/inttime.py` & `nctoolkit-1.1.9/nctoolkit/inttime.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/invert.py` & `nctoolkit-1.1.9/nctoolkit/invert.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/masking.py` & `nctoolkit-1.1.9/nctoolkit/masking.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/matchpoint.py` & `nctoolkit-1.1.9/nctoolkit/matchpoint.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/mergers.py` & `nctoolkit-1.1.9/nctoolkit/mergers.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/meridonials.py` & `nctoolkit-1.1.9/nctoolkit/meridonials.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/mp_adders.py` & `nctoolkit-1.1.9/nctoolkit/mp_adders.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/mp_matchers.py` & `nctoolkit-1.1.9/nctoolkit/mp_matchers.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/mp_matchups.py` & `nctoolkit-1.1.9/nctoolkit/mp_matchups.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/nco_command.py` & `nctoolkit-1.1.9/nctoolkit/nco_command.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/phenology.py` & `nctoolkit-1.1.9/nctoolkit/phenology.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/plot.py` & `nctoolkit-1.1.9/nctoolkit/plot.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/reduce.py` & `nctoolkit-1.1.9/nctoolkit/reduce.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/reduce_grid.py` & `nctoolkit-1.1.9/nctoolkit/reduce_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/regrid.py` & `nctoolkit-1.1.9/nctoolkit/regrid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/remove.py` & `nctoolkit-1.1.9/nctoolkit/remove.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/rename.py` & `nctoolkit-1.1.9/nctoolkit/rename.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/resample.py` & `nctoolkit-1.1.9/nctoolkit/resample.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/rollstat.py` & `nctoolkit-1.1.9/nctoolkit/rollstat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/run.py` & `nctoolkit-1.1.9/nctoolkit/run.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/runners.py` & `nctoolkit-1.1.9/nctoolkit/runners.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/runthis.py` & `nctoolkit-1.1.9/nctoolkit/runthis.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/session.py` & `nctoolkit-1.1.9/nctoolkit/session.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/set.py` & `nctoolkit-1.1.9/nctoolkit/set.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/setters.py` & `nctoolkit-1.1.9/nctoolkit/setters.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/shape.py` & `nctoolkit-1.1.9/nctoolkit/shape.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/shift.py` & `nctoolkit-1.1.9/nctoolkit/shift.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/show.py` & `nctoolkit-1.1.9/nctoolkit/show.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/split.py` & `nctoolkit-1.1.9/nctoolkit/split.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/static_plot.py` & `nctoolkit-1.1.9/nctoolkit/static_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
                 fixed = True
 
         if kk.lower().startswith("trans"):
             if norm is None:
                 norm = kwargs[kk]
                 fixed = True
 
-        #if kk.lower().startswith("mid") and kk.lower().endswith("nt"):
+        # if kk.lower().startswith("mid") and kk.lower().endswith("nt"):
         #    if mid_point is None:
         #        mid_point = kwargs[kk]
         #        fixed = True
 
         if kk.lower().startswith("proj"):
             if projection == "auto":
                 projection = kwargs[kk]
@@ -458,15 +458,14 @@
                 min_value = np.nanpercentile(np.ma.filled(values, np.nan), 2)
                 max_value = np.nanpercentile(np.ma.filled(values, np.nan), 98)
             if r_min is not None:
                 min_value = np.nanpercentile(np.ma.filled(values, np.nan), r_min)
             if r_max is not None:
                 max_value = np.nanpercentile(np.ma.filled(values, np.nan), r_max)
 
-
     # generate the figure and the axes where to plot the map. When the axes are generated (either with add_subplot or add_axes, or any other way), the projection to be used need to be specified
     # the axes generated show the entire globe up to the cutoff latitude
     if fig is None:
         if size is not None:
             fig = plt.figure(figsize=size)
         else:
             fig = plt.figure(figsize=(10, 10))
@@ -504,15 +503,15 @@
             vmin = np.nanpercentile(np.ma.filled(values, np.nan), 2)
             vmax = np.nanpercentile(np.ma.filled(values, np.nan), 98)
         if limits is None:
             if r_min is not None:
                 vmin = np.nanpercentile(np.ma.filled(values, np.nan), r_min)
             if r_max is not None:
                 vmax = np.nanpercentile(np.ma.filled(values, np.nan), r_max)
-            
+
         if mid_point is None:
             if vmin < 0 and vmax > 0:
                 mid_point = 0
                 limits[0] = vmin
                 limits[1] = vmax
                 try:
                     if limits[0] < 0 and limits[1] > 0:
@@ -534,16 +533,14 @@
                     colours = "RdBu_r"
                     if land_auto and land is not None:
                         if land != "auto":
                             land = "grey"
             except:
                 pass
 
-
-
         if mid_point is not None:
             val_min = values.min()
             val_max = values.max()
 
             if mid_point == 0.0:
                 if limits is not None:
                     val_min = limits[0]
@@ -554,18 +551,14 @@
             if mid_point < val_min:
                 raise ValueError("mid_point is outside value range")
             if mid_point > val_max:
                 raise ValueError("mid_point is outside value range")
             adjustment = max(val_max - mid_point, mid_point - val_min)
             vmin = mid_point - adjustment
             vmax = mid_point + adjustment
-            # else:
-            #     print(limits)
-            #     vmin = limits[0]
-            #     vmax = limits[1]
 
         norm_plot = False
         if norm in ["log", "log10"]:
             norm = mpl.colors.LogNorm(vmin=vmin, vmax=vmax)
             norm_plot = True
         if norm is not None:
             vmin = None
@@ -587,32 +580,32 @@
                     colours = "viridis"
             except:
                 pass
 
         if colours == "auto":
             colours = "viridis"
 
-        if vmin < 0 and vmax >0:
-            # ensure vmin and vmax are symmetric
-            vmax = max(abs(vmin), abs(vmax))
-            vmin = -vmax
+        if norm is None:
+            if vmin < 0 and vmax > 0:
+                # ensure vmin and vmax are symmetric
+                vmax = max(abs(vmin), abs(vmax))
+                vmin = -vmax
 
         im = ax.pcolormesh(
             lon,
             lat,
             values,
             cmap=colours,
             transform=data_crs,
             shading="nearest",
             norm=norm,
             vmin=vmin,
             vmax=vmax,
         )
 
-
     # add coastline and land colour. More options, including about resolution of coastline, colour and so on can be found here
     # https://scitools.org.uk/cartopy/docs/v0.14/matplotlib/feature_interface.html
     #
     # add grid lineshttp://localhost:8890/notebooks/Untitled4.ipynb?kernel_name=python3#
     # first define the gridliner object
     # crs define the units of the values (here spehric coorindates)
     # the other options are for grpahics, more details can be found here
```

### Comparing `nctoolkit-1.1.7/nctoolkit/strip_vars.py` & `nctoolkit-1.1.9/nctoolkit/strip_vars.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/subset.py` & `nctoolkit-1.1.9/nctoolkit/subset.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/sumall.py` & `nctoolkit-1.1.9/nctoolkit/sumall.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/temp_file.py` & `nctoolkit-1.1.9/nctoolkit/temp_file.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/temporal_stat.py` & `nctoolkit-1.1.9/nctoolkit/temporal_stat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/temporals.py` & `nctoolkit-1.1.9/nctoolkit/temporals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/thresholds.py` & `nctoolkit-1.1.9/nctoolkit/thresholds.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/to_lonlat.py` & `nctoolkit-1.1.9/nctoolkit/to_lonlat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/to_nc.py` & `nctoolkit-1.1.9/nctoolkit/to_nc.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/toxarray.py` & `nctoolkit-1.1.9/nctoolkit/toxarray.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/tozlev.py` & `nctoolkit-1.1.9/nctoolkit/tozlev.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/unify.py` & `nctoolkit-1.1.9/nctoolkit/unify.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/utils.py` & `nctoolkit-1.1.9/nctoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/validator.py` & `nctoolkit-1.1.9/nctoolkit/validator.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/validator_funs.py` & `nctoolkit-1.1.9/nctoolkit/validator_funs.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/verticals.py` & `nctoolkit-1.1.9/nctoolkit/verticals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit/zonals.py` & `nctoolkit-1.1.9/nctoolkit/zonals.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/nctoolkit.egg-info/SOURCES.txt` & `nctoolkit-1.1.9/nctoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nctoolkit-1.1.7/setup.py` & `nctoolkit-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,17 +43,19 @@
 
 
 extras_require["complete"] = ["geoviews", "rioxarray", "cfchecker", "geocube", "geopandas"]
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(name='nctoolkit',
-      version='1.1.7',
+      version='1.1.9',
       description=DESCRIPTION,
+      description_content_type='text/plain',
       long_description=LONG_DESCRIPTION,
+      long_description_content_type='text/plain',
       python_requires='>=3.6.1',
       classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `nctoolkit-1.1.7/testing/test_parallel.py` & `nctoolkit-1.1.9/testing/test_parallel.py`

 * *Files identical despite different names*

