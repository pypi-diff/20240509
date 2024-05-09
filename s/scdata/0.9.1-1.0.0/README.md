# Comparing `tmp/scdata-0.9.1.tar.gz` & `tmp/scdata-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdata-0.9.1.tar", last modified: Wed Oct  4 17:09:22 2023, max compression
+gzip compressed data, was "scdata-1.0.0.tar", last modified: Thu May  9 14:11:43 2024, max compression
```

## Comparing `scdata-0.9.1.tar` & `scdata-1.0.0.tar`

### file list

```diff
@@ -1,112 +1,105 @@
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/
--rw-r--r--   0 oscar     (1000) oscar     (1000)    35120 2023-03-12 18:24:45.000000 scdata-0.9.1/LICENSE
--rw-r--r--   0 oscar     (1000) oscar     (1000)      232 2023-03-12 18:24:45.000000 scdata-0.9.1/MANIFEST.in
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4159 2023-10-04 17:09:22.896660 scdata-0.9.1/PKG-INFO
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3341 2023-03-12 18:24:45.000000 scdata-0.9.1/README.md
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/
--rw-r--r--   0 oscar     (1000) oscar     (1000)       73 2023-10-04 17:05:59.000000 scdata-0.9.1/scdata/__init__.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/_config/
--rw-r--r--   0 oscar     (1000) oscar     (1000)       46 2023-03-12 18:24:51.000000 scdata-0.9.1/scdata/_config/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    22125 2023-10-04 08:53:17.000000 scdata-0.9.1/scdata/_config/config.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/device/
--rw-r--r--   0 oscar     (1000) oscar     (1000)    41810 2023-10-04 15:05:57.000000 scdata-0.9.1/scdata/device/__init__.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/device/process/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      602 2023-06-12 16:29:41.000000 scdata-0.9.1/scdata/device/process/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    19997 2023-10-03 14:52:24.000000 scdata-0.9.1/scdata/device/process/alphasense.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    10958 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/device/process/baseline.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2378 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/device/process/formulae.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1001 2023-03-12 18:24:51.000000 scdata-0.9.1/scdata/device/process/geoseries.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3459 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/device/process/params.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1477 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/device/process/regression.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     9765 2023-06-12 16:31:56.000000 scdata-0.9.1/scdata/device/process/timeseries.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/io/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      147 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/io/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     9492 2023-10-04 15:07:31.000000 scdata-0.9.1/scdata/io/csv.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    72880 2023-10-04 15:10:26.000000 scdata-0.9.1/scdata/io/device_api.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3213 2023-07-18 15:57:39.000000 scdata-0.9.1/scdata/io/firmware.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2064 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/io/model.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2494 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/io/user_api.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/test/
--rw-r--r--   0 oscar     (1000) oscar     (1000)    16041 2023-10-04 15:07:40.000000 scdata-0.9.1/scdata/test/__init__.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/test/export/
--rw-r--r--   0 oscar     (1000) oscar     (1000)       36 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/export/__init__.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/test/export/templates/
--rw-r--r--   0 oscar     (1000) oscar     (1000)    10453 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/export/templates/sc_template.html
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)     3082 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/export/to_file.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata/test/load/
--rw-r--r--   0 oscar     (1000) oscar     (1000)       22 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/load/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     9704 2023-10-04 13:51:32.000000 scdata-0.9.1/scdata/test/load/load.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/test/plot/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      744 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3938 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/box_plot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2404 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/heatmap_iplot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3095 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/heatmap_plot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    19867 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/maps.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    12810 2023-06-14 13:45:17.000000 scdata-0.9.1/scdata/test/plot/plot_tools.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     5429 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/scatter_dispersion_grid.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2057 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/scatter_iplot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     8107 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/scatter_plot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3110 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/target_diagram.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     3726 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_dendrogram.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     5012 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_dispersion_grid.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     7349 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_dispersion_plot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     9989 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_dispersion_uplot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4310 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_iplot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     7438 2023-06-12 16:39:27.000000 scdata-0.9.1/scdata/test/plot/ts_plot.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4827 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/plot/ts_scatter.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     6357 2023-06-12 16:39:30.000000 scdata-0.9.1/scdata/test/plot/ts_uplot.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/test/utils/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      190 2023-06-12 16:33:13.000000 scdata-0.9.1/scdata/test/utils/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     5389 2023-06-14 13:49:59.000000 scdata-0.9.1/scdata/test/utils/checks.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2142 2023-03-12 18:24:48.000000 scdata-0.9.1/scdata/test/utils/combine.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4248 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/utils/dispersion.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2164 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/test/utils/prepare.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/utils/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      596 2023-05-22 16:38:43.000000 scdata-0.9.1/scdata/utils/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)      691 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/cleaning.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1511 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/date.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)      881 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/dictmerge.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)      856 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/headers.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/utils/interim/
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)   116684 2023-10-04 15:19:46.000000 scdata-0.9.1/scdata/utils/interim/example.csv
--rw-r--r--   0 oscar     (1000) oscar     (1000)   606435 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/interim/geodata.csv
--rw-r--r--   0 oscar     (1000) oscar     (1000)      700 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/lazy.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1222 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/location.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1080 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/logs.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     6739 2023-05-23 12:03:40.000000 scdata-0.9.1/scdata/utils/meta.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1007 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/out.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1078 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/report.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2289 2023-03-12 18:24:50.000000 scdata-0.9.1/scdata/utils/stats.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2270 2023-09-13 20:56:52.000000 scdata-0.9.1/scdata/utils/units.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/utils/uploads/
--rw-r--r--   0 oscar     (1000) oscar     (1000)      522 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/uploads/example_upload_1.json
--rw-r--r--   0 oscar     (1000) oscar     (1000)      664 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/uploads/example_zenodo_upload.yaml
--rw-r--r--   0 oscar     (1000) oscar     (1000)   132597 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/uploads/report.pdf
--rw-r--r--   0 oscar     (1000) oscar     (1000)      454 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/url_check.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    10000 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/zenodo.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/scdata/utils/zenodo_templates/
--rw-r--r--   0 oscar     (1000) oscar     (1000)        0 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/zenodo_templates/README.md
--rw-r--r--   0 oscar     (1000) oscar     (1000)      315 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/zenodo_templates/template_zenodo_dataset.json
--rw-r--r--   0 oscar     (1000) oscar     (1000)      308 2023-03-12 18:24:49.000000 scdata-0.9.1/scdata/utils/zenodo_templates/template_zenodo_publication.json
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.893327 scdata-0.9.1/scdata.egg-info/
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4159 2023-10-04 17:09:22.000000 scdata-0.9.1/scdata.egg-info/PKG-INFO
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2583 2023-10-04 17:09:22.000000 scdata-0.9.1/scdata.egg-info/SOURCES.txt
--rw-r--r--   0 oscar     (1000) oscar     (1000)        1 2023-10-04 17:09:22.000000 scdata-0.9.1/scdata.egg-info/dependency_links.txt
--rw-r--r--   0 oscar     (1000) oscar     (1000)        1 2023-03-12 18:29:20.000000 scdata-0.9.1/scdata.egg-info/not-zip-safe
--rw-r--r--   0 oscar     (1000) oscar     (1000)      319 2023-10-04 17:09:22.000000 scdata-0.9.1/scdata.egg-info/requires.txt
--rw-r--r--   0 oscar     (1000) oscar     (1000)       13 2023-10-04 17:09:22.000000 scdata-0.9.1/scdata.egg-info/top_level.txt
--rw-r--r--   0 oscar     (1000) oscar     (1000)       79 2023-10-04 17:09:22.896660 scdata-0.9.1/setup.cfg
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)     2225 2023-10-04 17:05:19.000000 scdata-0.9.1/setup.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/tools/
--rw-r--r--   0 oscar     (1000) oscar     (1000)        0 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     4895 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/asb-test.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     2685 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/backup.py
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)   128307 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/esptool.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)      106 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/options.py
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)     4983 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/register.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)    22188 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/sck.py
-drwxr-xr-x   0 oscar     (1000) oscar     (1000)        0 2023-10-04 17:09:22.896660 scdata-0.9.1/tools/serialtools/
--rw-r--r--   0 oscar     (1000) oscar     (1000)        0 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/serialtools/__init__.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     6247 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/serialtools/serialdevice.py
--rw-r--r--   0 oscar     (1000) oscar     (1000)     1878 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/serialtools/serialworker.py
--rwxr-xr-x   0 oscar     (1000) oscar     (1000)     9532 2023-03-12 18:24:44.000000 scdata-0.9.1/tools/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-05-09 14:11:38.000000 scdata-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 14:11:38.000000 scdata-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-09 14:11:43.016889 scdata-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-09 14:11:38.000000 scdata-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 14:11:38.000000 scdata-1.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.004889 scdata-1.0.0/scdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.004889 scdata-1.0.0/scdata/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/_config/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.004889 scdata-1.0.0/scdata/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27674 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/device/process/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/alphasense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/formulae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/geoseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/device/process/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75998 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/io/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/io/device_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/io/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/test/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/checks/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/test/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/dispersion/dispersion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/test/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.008889 scdata-1.0.0/scdata/test/export/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/export/templates/sc_template.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3098 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/export/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.012889 scdata-1.0.0/scdata/test/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/box_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/heatmap_iplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/heatmap_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19932 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/plot_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/scatter_dispersion_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/scatter_iplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/scatter_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/target_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_dispersion_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_dispersion_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_dispersion_uplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_iplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/plot/ts_uplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13700 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.012889 scdata-1.0.0/scdata/test/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/tools/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/tools/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/test/tools/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/scdata/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/gets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/scdata/tools/interim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   115671 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/interim/example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   606435 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/interim/geodata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/scdata/tools/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/uploads/example_upload_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/uploads/example_zenodo_upload.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   132597 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/uploads/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/url_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/scdata/tools/zenodo_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/zenodo_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/zenodo_templates/template_zenodo_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-09 14:11:38.000000 scdata-1.0.0/scdata/tools/zenodo_templates/template_zenodo_publication.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:11:43.016889 scdata-1.0.0/scdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-09 14:11:42.000000 scdata-1.0.0/scdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-09 14:11:43.000000 scdata-1.0.0/scdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:11:42.000000 scdata-1.0.0/scdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:11:42.000000 scdata-1.0.0/scdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 14:11:42.000000 scdata-1.0.0/scdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 14:11:42.000000 scdata-1.0.0/scdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 14:11:43.020889 scdata-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-05-09 14:11:38.000000 scdata-1.0.0/setup.py
```

### Comparing `scdata-0.9.1/LICENSE` & `scdata-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/PKG-INFO` & `scdata-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 Metadata-Version: 2.1
 Name: scdata
-Version: 0.9.1
+Version: 1.0.0
 Summary: Analysis of sensors and time series data
 Home-page: https://github.com/fablabbcn/smartcitizen-data
 Author: oscgonfer
 License: GNU-GPL3.0
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-data
 Keywords: air,sensors,Smart Citizen
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: branca~=0.4.0
+Requires-Dist: Flask~=2.2.2
+Requires-Dist: folium~=0.12.1
+Requires-Dist: geopy~=1.21.0
+Requires-Dist: Jinja2~=3.1.2
+Requires-Dist: matplotlib
+Requires-Dist: missingno~=0.5.2
+Requires-Dist: numpy~=1.25.2
+Requires-Dist: pandas~=2.2.2
+Requires-Dist: pydantic
+Requires-Dist: pytest
+Requires-Dist: PyYAML==5.3.1
+Requires-Dist: requests
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: seaborn
+Requires-Dist: smartcitizen-connector
+Requires-Dist: termcolor==1.1.0
+Requires-Dist: tqdm~=4.50.2
+Requires-Dist: timezonefinder~=6.1.9
+Requires-Dist: urllib3
 
 Smart Citizen Data
 =======
 
 [![DOI](https://zenodo.org/badge/97752018.svg)](https://zenodo.org/badge/latestdoi/97752018)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks)
 [![PyPI version](https://badge.fury.io/py/scdata.svg)](https://badge.fury.io/py/scdata)
+[![Python application](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml/badge.svg)](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml)
 
 Welcome to **SmartCitizen Data**. This is a data analysis framework for working with sensor data in different ways:
 
 - Interacting with several sensors APIs
 - Clean data, export and calculate metrics
 - Model sensor data and calibrate sensors
 - Generate data visualisations - matplotlib, [plotly](https://plotly.com/) or [uplot](https://leeoniya.github.io/uPlot)
 - Generate analysis reports in html or pdf and upload them to [Zenodo](http://zenodo.org)
 
-A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/). 
+A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/).
 
 ## Installation
 
 You can check it out in the [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks) before installing if you want. Works with `Python 3.*` (tested until `python 3.9.5`).
 
 You can just run:
 
@@ -105,9 +126,7 @@
 ## Contribute
 
 Issues and PR more than welcome!
 
 ## Funding
 
 This work has received funding from the European Union's Horizon 2020 research and innovation program under the grant agreement [No. 689954](https://cordis.europa.eu/project/rcn/202639_en.html)
-
-
```

### Comparing `scdata-0.9.1/README.md` & `scdata-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Smart Citizen Data
 =======
 
 [![DOI](https://zenodo.org/badge/97752018.svg)](https://zenodo.org/badge/latestdoi/97752018)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks)
 [![PyPI version](https://badge.fury.io/py/scdata.svg)](https://badge.fury.io/py/scdata)
+[![Python application](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml/badge.svg)](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml)
 
 Welcome to **SmartCitizen Data**. This is a data analysis framework for working with sensor data in different ways:
 
 - Interacting with several sensors APIs
 - Clean data, export and calculate metrics
 - Model sensor data and calibrate sensors
 - Generate data visualisations - matplotlib, [plotly](https://plotly.com/) or [uplot](https://leeoniya.github.io/uPlot)
 - Generate analysis reports in html or pdf and upload them to [Zenodo](http://zenodo.org)
 
-A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/). 
+A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/).
 
 ## Installation
 
 You can check it out in the [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks) before installing if you want. Works with `Python 3.*` (tested until `python 3.9.5`).
 
 You can just run:
```

### Comparing `scdata-0.9.1/scdata/_config/config.py` & `scdata-1.0.0/scdata/_config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,61 @@
 import yaml
 import json
-
-from scdata.utils.dictmerge import dict_fmerge
-from scdata.utils.meta import (get_paths, load_blueprints,
-                                load_calibrations, load_connectors,
-                                load_env, load_names)
-
 from os import pardir, environ
 from os.path import join, abspath, dirname, exists
 import sys
-
 from math import inf
 from numpy import array
+import logging
+from os import pardir, environ, name, makedirs
+from os.path import join, dirname, expanduser, exists, basename
+from urllib.parse import urlparse
+import os
+from shutil import copyfile
+from requests import get
+# from traceback import print_exc
+import json
+from pydantic import TypeAdapter
+from typing import List
 
-class Config(object):
-
-    # Output level
-    #   'QUIET': nothing
-    #   'NORMAL': warn, err,
-    #   'DEBUG': info, warn, err
-    _out_level = 'NORMAL'
+from scdata.models import Name, Blueprint, Metric
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.gets import get_json_from_url
 
-    # Timestamp for log output
-    _timestamp = True
+class Config(object):
+    ### ---------------------------------------
+    ### ---------------LOG-LEVEL---------------
+    ### ---------------------------------------
+    _log_level = logging.INFO
 
     # Framework option
     # For renderer plots and config files
     # Options:
     # - 'script': no plots in jupyter, updates config
     # - 'jupyterlab': for plots, updates config
     # - 'chupiflow': no plots in jupyter, does not update config
     framework = 'script'
 
     if 'IPython' in sys.modules: _ipython_avail = True
     else: _ipython_avail = False
 
-    # Default timezone
-    _timezone = 'Europe/Madrid'
-    _epsg = 4326
-
     # Returns when iterables cannot be fully processed
     _strict = False
 
     # Timeout for http requests
     _timeout = 3
+    _max_http_retries = 2
 
-    ### ---------------------------------------
-    ### ----------------CRONTAB----------------
-    ### ---------------------------------------
-    # Tabfile for cronjobs
-    _tabfile = 'tabfile'
-
-    # Scheduler
-    _scheduler_interval_days = 1
-    _device_scheduler = 'dschedule'
-    _scheduler_log = 'scheduler.log'
-    # Tasks
-    _postprocessing_interval_hours = 1
-    _device_processor = 'dprocess'
-    _max_forward_retries = 2
+    # Max concurrent requests
+    _max_concurrent_requests = 30
 
     ### ---------------------------------------
     ### -----------------DATA------------------
     ### ---------------------------------------
 
-    ## Place here options for data load and handling
-    _combined_devices_name = 'COMBINED_DEVICES'
-
     data = {
         # Whether or not to reload metadata from git repo
         'reload_metadata': True,
         # Whether or not to load or store cached data (saves time when requesting a lot of data)
         'load_cached_api': True,
         'store_cached_api': True,
         # If reloading data from the API, how much gap between the saved data and the
@@ -78,182 +63,95 @@
         'cached_data_margin': 1,
         # clean_na
         'clean_na': None,
         # Ignore additional channels from API or CSV that are not in the blueprint.json
         'strict_load': False
     }
 
-    # If using multiple training datasets, how to call the joint df
-    _name_multiple_training_data = 'CDEV'
-
     # Maximum amount of points to load when postprocessing data
     _max_load_amount = 500
 
-    # Ignore duplicate sensor ids
-    _sc_ignore_keys = ['DALLAS_TEMP', 'GB_TEMP', 'GB_HUM']
-
     # Ingore Nas when loading data (for now only in CSVs)
     # Similar to na_values in https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
     _ignore_na_values = [' nan']
 
     ### ---------------------------------------
     ### --------------ALGORITHMS---------------
     ### ---------------------------------------
 
+    ## TODO - move out from here
     # Whether or not to plot intermediate debugging visualisations in the algorithms
     _intermediate_plots = False
 
     # Plot out level (priority of the plot to show - 'DEBUG' or 'NORMAL')
     _plot_out_level = 'DEBUG'
 
-    # Alphasense sensor codes
-    _as_sensor_codes =  {
-        '132':  'ASA4_CO',
-        '133':  'ASA4_H2S',
-        '130':  'ASA4_NO',
-        '212':  'ASA4_NO2',
-        '214':  'ASA4_OX',
-        '134':  'ASA4_SO2',
-        '162':  'ASB4_CO',
-        '133':  'ASB4_H2S',#
-        '130':  'ASB4_NO', #
-        '202':  'ASB4_NO2',
-        '204':  'ASB4_OX',
-        '164':  'ASB4_SO2'
-    }
-
     ### ---------------------------------------
     ### ----------------ZENODO-----------------
     ### ---------------------------------------
 
     # Urls
     zenodo_sandbox_base_url='http://sandbox.zenodo.org'
     zenodo_real_base_url='https://zenodo.org'
 
     ### ---------------------------------------
     ### -------------SMART CITIZEN-------------
     ### ---------------------------------------
     # # Urls
-    _base_postprocessing_url = 'https://raw.githubusercontent.com/fablabbcn/smartcitizen-data/master/'
+    _base_postprocessing_url = 'https://raw.githubusercontent.com/fablabbcn/smartcitizen-data/enhacement/flexible-handlers/'
     _default_file_type = 'json'
 
     calibrations_urls = [
         f'{_base_postprocessing_url}calibrations/calibrations.{_default_file_type}'
     ]
 
     blueprints_urls = [
-        f'{_base_postprocessing_url}blueprints/base.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/csic_station.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/muv_station.{_default_file_type}',
-        # f'{_base_postprocessing_url}blueprints/parrot_soil.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sc_20_station_iscape.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sc_21_station_iscape.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sc_21_station_module.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_15.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_20.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21_sps30.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21_sen5x.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21_gps.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21_nilu.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sck_21_co2.{_default_file_type}',
-        f'{_base_postprocessing_url}blueprints/sc_21_water.{_default_file_type}'
+        # f'{_base_postprocessing_url}blueprints/base.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/csic_station.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/muv_station.{_default_file_type}',
+        # # f'{_base_postprocessing_url}blueprints/parrot_soil.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sc_20_station_iscape.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sc_21_station_iscape.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sc_21_station_module.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_15.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_20.{_default_file_type}',
+        f'{_base_postprocessing_url}blueprints/sc_air.{_default_file_type}',
+        f'{_base_postprocessing_url}blueprints/sc_water.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_21_sps30.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_21_sen5x.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_21_gps.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_21_nilu.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sck_21_co2.{_default_file_type}',
+        # f'{_base_postprocessing_url}blueprints/sc_21_water.{_default_file_type}'
     ]
 
-    connectors_urls = [
-        f'{_base_postprocessing_url}connectors/nilu.{_default_file_type}'
-    ]
+    # connectors_urls = [
+    #     f'{_base_postprocessing_url}connectors/nilu.{_default_file_type}'
+    # ]
 
     names_urls = [
-        f'{_base_postprocessing_url}names/sc_sensor_names.{_default_file_type}'
+        # Revert to base postprocessing url
+        # f'{_base_postprocessing_url}names/SCDevice.json'
+        'https://raw.githubusercontent.com/fablabbcn/smartcitizen-data/enhacement/flexible-handlers/names/SCDevice.json'
     ]
 
-    # Convertion table from API SC to Pandas
-    # https://stackoverflow.com/questions/35339139/where-is-the-documentation-on-pandas-freq-tags
-    # https://developer.smartcitizen.me/#get-historical-readings
-    _freq_conv_lut = (
-        ['y','A'],
-        ['M','M'],
-        ['w','W'],
-        ['d','D'],
-        ['h','H'],
-        ['m','Min'],
-        ['s','S'],
-        ['ms','ms']
-    )
-
 
     ### ---------------------------------------
     ### -------------METRICS DATA--------------
     ### ---------------------------------------
     # Metrics levels
     _channel_bins = {
         'NOISE': [-inf, 52, 54, 56, 58, 60, 62, 64, 66, 68, inf],
         'PM': [-inf, 10, 20, 30, 40, 50, 75, 100, 150, 200, inf],
         'GPS_HDOP': [-inf, 0, 40, 80, 120, 160, 200, 240, 260, 300, inf]
     }
 
-    _channel_bin_n = 11
 
-    # Molecular weights of certain pollutants for unit convertion
-    _molecular_weights = {
-        'CO':   28,
-        'NO':   30,
-        'NO2':  46,
-        'O3':   48,
-        'C6H6': 78,
-        'SO2':  64,
-        'H2S':  34
-    }
-
-    # This look-up table is comprised of channels you want always want to have with the same units and that might come from different sources
-    # i.e. pollutant data in various units (ppm or ug/m3) from different analysers
-    # The table should be used as follows:
-    # 'key': 'units',
-    # - 'key' is the channel that will lately be used in the analysis. It supports regex
-    # - target_unit is the unit you want this channel to be and that will be converted in case of it being found in the channels list of your source
-
-    _channel_lut = {
-        "TEMP": "degC",
-        "HUM": "%rh",
-        "PRESS": "kPa",
-        "PM_(\d|[A,B]_\d)": "ug/m3",
-        "^CO2": "ppm",
-        "^CO": "ppb", # Always start with CO
-        "NOISE_A": "dBA",
-        "NO\Z": "ppb",
-        "NO2": "ppb",
-        "NOX": "ppb",
-        "O3": "ppb",
-        "C6H6": "ppb",
-        "H2S": "ppb",
-        "SO2": "ppb",
-        "CO2": "ppm"
-    }
-
-    # This table is used to convert units
-    # ['from_unit', 'to_unit', 'multiplicative_factor', 'requires_M']
-    # - 'from_unit'/'to_unit' = 'multiplicative_factor'
-    # - 'requires_M' = whether it
-    # It accepts reverse operations - you don't need to put them twice but in reverse
-
-    _unit_convertion_lut = (
-        ['ppm', 'ppb', 1000, False],
-        ['mg/m3', 'ug/m3', 1000, False],
-        ['mgm3', 'ugm3', 1000, False],
-        ['mg/m3', 'ppm', 24.45, True],
-        ['mgm3', 'ppm', 24.45, True],
-        ['ug/m3', 'ppb', 24.45, True],
-        ['ugm3', 'ppb', 24.45, True],
-        ['mg/m3', 'ppb', 1000*24.45, True],
-        ['mgm3', 'ppb', 1000*24.45, True],
-        ['ug/m3', 'ppm', 1./1000*24.45, True],
-        ['ugm3', 'ppm', 1./1000*24.45, True]
-    )
+    _channel_bin_n = 11
 
     ### ---------------------------------------
     ### ----------------PLOTS------------------
     ### ---------------------------------------
     _plot_def_opt = {
         'min_date': None,
         'max_date': None,
@@ -279,16 +177,15 @@
         'markers': True
     }
 
     _map_colors_palette = array(['#053061','#2166ac','#4393c3','#92c5de',
                                  '#d1e5f0','#fddbc7','#f4a582','#d6604d',
                                  '#b2182b','#67001f'])
 
-
-    _plot_style = "seaborn-whitegrid"
+    _plot_style = "seaborn-v0_8-whitegrid"
 
     _ts_plot_def_fmt = {
         'mpl': {
             'width': 12,
             'height': 8,
             'sharex': True,
             'ylabel': None,
@@ -522,49 +419,34 @@
         # Do not perform dispersion analysis on these channels
         'ignore_channels': ['BATT'],
         # Normal or t-student distribution threshold
         'nt_threshold': 30
     }
 
     ### ---------------------------------------
-    ### ----------------DISCARD----------------
+    ### ----------------CSV--------------------
     ### ---------------------------------------
 
-    _discvars = [
-        'readings',
-        'api_device',
-        'options',
-        'loaded',
-        'hw_id',
-        'blueprint_url',
-        'hardware_url',
-        'processed',
-        'forwarding_params',
-        'meta',
-        'processed',
-        'postprocessing_info',
-        'hw_updated_at',
-        'description',
-        'latest_postprocessing',
-        'blueprint_loaded_from_url',
-        'hardware_loaded_from_url'
-    ]
-
     _csv_defaults = {
         'index_name': 'TIME',
         'sep': ',',
         'skiprows': None
     }
 
+    ### ---------------------------------------
+    ### ---------------------------------------
+    ### ---------------------------------------
+
     def __init__(self):
-        self._env_file = False
-        self.paths = get_paths()
+        self._env_file = None
+        self.paths = self.get_paths()
         self.load()
         self.get_meta_data()
 
+
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError:
             raise AttributeError
 
     def __getitem__(self, key):
@@ -574,83 +456,271 @@
             raise KeyError
         else:
             return val
 
     def __iter__(self):
         return (i for i in dir(self))
 
+    def load_env(self):
+        with open(self._env_file) as f:
+            for line in f:
+                # Ignore empty lines or lines that start with #
+                if line.startswith('#') or not line.strip():
+                    continue
+                # Load to local environ
+                key, value = line.strip().split('=', 1)
+                environ[key] = value
+
+    def load_calibrations(self, urls):
+        '''
+            Loads calibrations from urls.
+            The calibrations are meant for alphasense's 4 electrode sensors. The files contains:
+            {
+            "162031254": {
+                "ae_electronic_zero_mv": "",
+                "ae_sensor_zero_mv": "-16.64",
+                "ae_total_zero_mv": "",
+                "pcb_gain_mv_na": "0.8",
+                "we_cross_sensitivity_no2_mv_ppb": "0",
+                "we_cross_sensitivity_no2_na_ppb": "0",
+                "we_electronic_zero_mv": "",
+                "we_sensitivity_mv_ppb": "0.45463999999999993",
+                "we_sensitivity_na_ppb": "0.5682999999999999",
+                "we_sensor_zero_mv": "-27.200000000000003",
+                "we_total_zero_mv": ""
+            },
+            ...
+            }
+            Parameters
+            ----------
+                urls: [String]
+                    json file urls
+            Returns
+            ---------
+                Dictionary containing calibrations otherwise None
+        '''
+
+        calibrations = dict()
+        for url in urls:
+            try:
+                rjson, _ = get_json_from_url(url)
+                calibrations = dict_fmerge(rjson, calibrations)
+            except:
+                print(f'Problem loading calibrations from {url}')
+                return None
+
+        return calibrations
+
+    # def load_connectors(self, urls):
+    #     connectors = dict()
+    #     for url in urls:
+    #         try:
+    #             c = get_json_from_url(url)
+    #             _nc = basename(urlparse(str(url)).path).split('.')[0]
+    #             connectors[_nc] = c
+    #         except:
+    #             print(f'Problem loading connectors from {url}')
+    #             print_exc()
+    #             return None
+
+    #     return connectors
+
+    def load_blueprints(self, urls):
+        blueprints = dict()
+        for url in urls:
+            if url is None: continue
+            _nblueprint = basename(urlparse(str(url)).path).split('.')[0]
+            rjson, _ = get_json_from_url(url)
+
+            if rjson is None:
+                continue
+            if _nblueprint not in blueprints:
+                blueprints[_nblueprint] = TypeAdapter(Blueprint).validate_python(rjson).model_dump()
+
+        return blueprints
+
+    def load_names(self, urls):
+        isn = True
+        names = dict()
+
+        for url in urls:
+            result = list()
+            _nc = basename(urlparse(str(url)).path).split('.')[0]
+
+            while isn:
+                try:
+                    rjson, rheaders = get_json_from_url(url)
+                    result += TypeAdapter(List[Name]).validate_python(rjson)
+                except:
+                    isn = False
+                    pass
+                else:
+                    if 'next' in rheaders:
+                        if rheaders['next'] == url: isn = False
+                        elif rheaders['next'] != url: url = rheaders['next']
+                    else:
+                        isn = False
+            names[_nc] = result
+
+        return names
+
+    def get_paths(self):
+
+        # Check if windows
+        _mswin = name == "nt"
+        # Get user_home
+        _user_home = expanduser("~")
+
+        # Get .config dir
+        if _mswin:
+            _cdir = environ["APPDATA"]
+        elif 'XDG_CONFIG_HOME' in environ:
+            _cdir = environ['XDG_CONFIG_HOME']
+        else:
+            _cdir = join(expanduser("~"), '.config')
+
+        # Get .cache dir - maybe change it if found in config.json
+        if _mswin:
+            _ddir = environ["APPDATA"]
+        elif 'XDG_CACHE_HOME' in environ:
+            _ddir = environ['XDG_CACHE_HOME']
+        else:
+            _ddir = join(expanduser("~"), '.cache')
+
+        # Set config and cache (data) dirs
+        _sccdir = join(_cdir, 'scdata')
+        _scddir = join(_ddir, 'scdata')
+
+        makedirs(_sccdir, exist_ok=True)
+        makedirs(_scddir, exist_ok=True)
+
+        _paths = dict()
+
+        _paths['config'] = _sccdir
+        _paths['data'] = _scddir
+
+        # Auxiliary folders
+
+        # - Processed data
+        _paths['processed'] = join(_paths['data'], 'processed')
+        makedirs(_paths['processed'], exist_ok=True)
+
+        # - Internal data: blueprints and calibrations
+        _paths['interim'] = join(_paths['data'], 'interim')
+        makedirs(_paths['interim'], exist_ok=True)
+
+        # Check for blueprints and calibrations
+        # Find the path to the interim folder
+        _dir = dirname(__file__)
+        _idir = join(_dir, '../tools/interim')
+
+        # - Models and local tests
+        _paths['models'] = join(_paths['data'], 'models')
+        makedirs(_paths['models'], exist_ok=True)
+
+        # - Exports
+        _paths['export'] = join(_paths['data'], 'export')
+        makedirs(_paths['export'], exist_ok=True)
+
+        # - Raw
+        _paths['raw'] = join(_paths['data'], 'raw')
+        makedirs(_paths['raw'], exist_ok=True)
+        # Copy example csvs
+        _enames = ['example.csv', 'geodata.csv']
+        for _ename in _enames:
+            s = join(_idir, _ename)
+            d = join(_paths['raw'], _ename)
+            if not exists(join(_paths['raw'], _ename)): copyfile(s, d)
+
+        # - Reports
+        _paths['reports'] = join(_paths['data'], 'reports')
+        makedirs(_paths['reports'], exist_ok=True)
+
+        # - Tasks
+        _paths['tasks'] = join(_paths['data'], 'tasks')
+        makedirs(_paths['tasks'], exist_ok=True)
+
+        # - Uploads
+        _paths['uploads'] = join(_paths['data'], 'uploads')
+        makedirs(_paths['uploads'], exist_ok=True)
+
+        # Check for uploads
+        _example_uploads = ['example_upload_1.json', 'example_zenodo_upload.yaml']
+        _udir = join(_dir, '../tools/uploads')
+        for item in _example_uploads:
+            s = join(_udir, item)
+            d = join(_paths['uploads'], item)
+            if not exists(d): copyfile(s, d)
+
+        # Inventory (normally not used by user)
+        _paths['inventory'] = ''
+
+        return _paths
+
     def get_meta_data(self):
         """ Get meta data from blueprints and _calibrations """
 
-        # (re)load calibrations
+        # Load blueprints, calibrations and names
         bppath = join(self.paths['interim'], 'blueprints.json')
         if self.data['reload_metadata'] or not exists(bppath):
-            blueprints = load_blueprints(self.blueprints_urls)
+            blueprints = self.load_blueprints(self.blueprints_urls)
             bpreload = True
         else:
             with open(bppath, 'r') as file: blueprints = json.load(file)
             bpreload = False
 
         calpath = join(self.paths['interim'], 'calibrations.json')
         if self.data['reload_metadata'] or not exists(calpath):
-            calibrations = load_calibrations(self.calibrations_urls)
+            calibrations = self.load_calibrations(self.calibrations_urls)
             calreload = True
         else:
             with open(calpath, 'r') as file: calibrations = json.load(file)
             calreload = False
 
-        conpath = join(self.paths['interim'], 'connectors.json')
-        if self.data['reload_metadata'] or not exists(conpath):
-            connectors = load_connectors(self.connectors_urls)
-            conreload = True
-        else:
-            with open(conpath, 'r') as file: connectors = json.load(file)
-            conreload = False
-
         namespath = join(self.paths['interim'], 'names.json')
         if self.data['reload_metadata'] or not exists(namespath):
-            names = load_names(self.names_urls)
-            # sc_sensor_names = load_firmware_names(self.sensor_names_url_21)
-            # sc_sensor_names = load_api_names(self.sensors_api_names_url)
+            names = self.load_names(self.names_urls)
             namesreload = True
         else:
-            with open(namespath, 'r') as file: names = json.load(file)
+            names = dict()
+            with open(namespath, 'r') as file:
+                names_load = json.load(file)
+            for item in names_load:
+                names[item] = TypeAdapter(List[Name]).validate_python(names_load[item])
             namesreload = False
 
+        # Dump blueprints, calibrations and names
         if blueprints is not None:
             self.blueprints = blueprints
             if bpreload:
-                with open(bppath, 'w') as file: json.dump(blueprints, file)
+                with open(bppath, 'w') as file:
+                    json.dump(blueprints, file)
+
         if calibrations is not None:
             self.calibrations = calibrations
             if calreload:
-                with open(calpath, 'w') as file: json.dump(calibrations, file)
-        if connectors is not None:
-            self.connectors = connectors
-            if conreload:
-                with open(conpath, 'w') as file: json.dump(connectors, file)
+                with open(calpath, 'w') as file:
+                    json.dump(calibrations, file)
+
         if names is not None:
             self.names = names
             if namesreload:
-                with open(namespath, 'w') as file: json.dump(names, file)
+                for item in self.names:
+                    names_dump = {item: [name.model_dump() for name in self.names[item]]}
+                with open(namespath, 'w') as file:
+                    json.dump(names_dump, file)
 
         # Find environment file in root or in scdata/ for clones
         if exists(join(self.paths['data'],'.env')):
-            env_file = join(self.paths['data'],'.env')
+            self._env_file = join(self.paths['data'],'.env')
+            print(f'Found Environment file at: {self._env_file}')
+            self.load_env()
         else:
-            print (f'No environment file found. \
-                    If you had an environment file (.env) before, \
-                    make sure its now here:')
+            print(f'No environment file found. If you had an environment file (.env) before, make sure its now here')
             print(join(self.paths['data'],'.env'))
-            env_file = None
-
-        # Load .env for tokens and stuff if found
-        if env_file is not None and not self._env_file:
-            print(f'Found Environment file at: {env_file}')
-            if load_env(env_file): self._env_file = True
 
     def load(self):
         """ Override config if config file exists. """
         _sccpath = join(self.paths['config'], 'config.yaml')
 
         # Thankfully inspired in config.py by mps-youtube
         if exists(_sccpath):
@@ -660,42 +730,22 @@
             for k, v in saved_config.items():
 
                 try:
                     self.__setattr__(k, v)
 
                 except KeyError:  # Ignore unrecognised data in config
                     print ("Unrecognised config item: %s", k)
+
         if self.framework != 'chupiflow':
             self.save()
 
     def save(self):
         """ Save current config to file. """
         c = dict()
         for setting in self:
-            if not setting.startswith('_') and not callable(self.__getitem__(setting)):
+            if not setting.startswith('_') and not callable(self.__getitem__(setting)) and setting not in ['blueprints', 'names', 'calibrations']:
                 c[setting] = self[setting]
 
         _sccpath = join(self.paths['config'], 'config.yaml')
         with open(_sccpath, "w") as cf:
             yaml.dump(c, cf)
 
-    def set_testing(self, env_file = None):
-        '''
-        Convenience method for setting variables as development
-        in jupyterlab
-        Parameters
-        ----------
-            None
-        Returns
-        ----------
-            None
-        '''
-
-        print ('Setting test mode')
-        self._out_level = 'DEBUG'
-        self.framework = 'jupyterlab'
-        self._intermediate_plots = True
-        self._plot_out_level = 'DEBUG'
-
-        # Load Environment
-        if env_file is not None and not self._env_file:
-            if load_env(env_file): self._env_file = True
```

### Comparing `scdata-0.9.1/scdata/device/process/__init__.py` & `scdata-1.0.0/scdata/device/process/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ''' Implementation of different processes to be done in each device '''
 
-from scdata.utils import LazyCallable
+from scdata.tools.lazy import LazyCallable
 from .formulae import absolute_humidity, exp_f, fit_exp_f
 from .geoseries import is_within_circle
 from .timeseries import clean_ts, merge_ts, rolling_avg, poly_ts, geo_located, time_derivative, delta_index_ts
 from .baseline import find_min_max, baseline_calc, get_delta_baseline, get_als_baseline
 from .alphasense import alphasense_803_04, alphasense_pt1000, channel_names, basic_4electrode_alg, baseline_4electrode_alg, deconvolution, ec_sensor_temp
-from .regression import apply_regressor
+from .regression import apply_regressor
```

### Comparing `scdata-0.9.1/scdata/device/process/alphasense.py` & `scdata-1.0.0/scdata/device/process/alphasense.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,59 @@
-from scdata.utils import std_out, get_units_convf, find_dates, localise_date
+from scdata.tools.custom_logger import logger
+from scdata.tools.units import get_units_convf
+from scdata.tools.date import find_dates, localise_date
 from scdata._config import config
 from scdata.device.process.params import *
 from scdata.device.process import baseline_calc, clean_ts
-from scipy.stats.stats import linregress
+from scipy.stats import linregress
 import matplotlib.pyplot as plt
 from pandas import date_range, DataFrame, Series, isnull
 
+# Alphasense sensor codes
+alphasense_sensor_codes =  {
+    '132':  'ASA4_CO',
+    '133':  'ASA4_H2S',
+    '130':  'ASA4_NO',
+    '212':  'ASA4_NO2',
+    '214':  'ASA4_OX',
+    '134':  'ASA4_SO2',
+    '162':  'ASB4_CO',
+    '133':  'ASB4_H2S',#
+    '130':  'ASB4_NO', #
+    '202':  'ASB4_NO2',
+    '204':  'ASB4_OX',
+    '164':  'ASB4_SO2'
+}
+
+# Alphasense temperature channels (in order of priority)
+alphasense_temp_channel = [
+    "ASPT1000",
+    "SHT31_EXT_TEMP",
+    "SHT35_EXT_TEMP",
+    "PM_DALLAS_TEMP",
+]
+
 def alphasense_803_04(dataframe, **kwargs):
     """
     Calculates pollutant concentration based on 4 electrode sensor readings (mV)
     and calibration ID. It adds a configurable background concentration and correction
     based on AAN803-04
     Parameters
     ----------
-        from_date: string, datetime object
-            Date from which this calibration id is valid from
-        to_date: string, datetime object
-            Date until which this calibration id is valid to. None if current
         alphasense_id: string
             Alphasense sensor ID (must be in calibrations.json)
         we: string
             Name of working electrode found in dataframe (V)
         ae: string
             Name of auxiliary electrode found in dataframe (V)
         t: string
             Name of reference temperature
         use_alternative: boolean
             Default false
             Use alternative algorithm as shown in the AAN
-        timezone: string
-            Valid timezone for date localisation
     Returns
     -------
         calculation of pollutant in ppb
     """
 
     def comp_t(x, comp_lut):
         if isnull(x['t']): return None
@@ -57,49 +77,31 @@
     flag_error = False
     if 'we' not in kwargs: flag_error = True
     if 'ae' not in kwargs: flag_error = True
     if 'alphasense_id' not in kwargs: flag_error = True
     if 't' not in kwargs: flag_error = True
 
     if flag_error:
-        std_out('Problem with input data', 'ERROR')
+        logger.warning('Problem with input data')
         return None
 
     if kwargs['alphasense_id'] is None:
-        std_out(f"Empty ID. Ignoring", 'WARNING')
+        logger.warning(f"Empty ID. Ignoring")
         return None
 
     # Get Sensor data
     if kwargs['alphasense_id'] not in config.calibrations:
-        std_out(f"Sensor {kwargs['alphasense_id']} not in calibration data", 'ERROR')
+        logger.warning(f"Sensor {kwargs['alphasense_id']} not in calibration data")
         return None
 
-    # Process input dates
-    if 'from_date' not in kwargs: from_date = None
-    else:
-        if 'timezone' not in kwargs:
-            std_out('Cannot localise date without timezone')
-            return None
-        from_date = localise_date(kwargs['from_date'], kwargs['timezone'])
-
-    if 'to_date' not in kwargs: to_date = None
-    else:
-        if 'timezone' not in kwargs:
-            std_out('Cannot localise date without timezone')
-            return None
-        to_date = localise_date(kwargs['to_date'], kwargs['timezone'])
-
     # Make copy
     df = dataframe.copy()
-    # Trim data
-    if from_date is not None: df = df[df.index > from_date]
-    if to_date is not None: df = df[df.index < to_date]
 
     # Get sensor type
-    as_type = config._as_sensor_codes[kwargs['alphasense_id'][0:3]]
+    as_type = alphasense_sensor_codes[kwargs['alphasense_id'][0:3]]
 
     # Use alternative method or not
     if 'use_alternative' not in kwargs: kwargs['use_alternative'] = False
     if kwargs['use_alternative']: algorithm_idx = 1
     else: algorithm_idx = 0
 
     # Get algorithm name
@@ -109,21 +111,21 @@
 
     # Retrieve calibration data - verify its all float
     cal_data = config.calibrations[kwargs['alphasense_id']]
     for item in cal_data:
         try:
             cal_data[item] = float (cal_data[item])
         except:
-            std_out(f"Alphasense calibration data for {kwargs['alphasense_id']} is not correct", 'ERROR')
-            std_out(f'Error on {item}: \'{cal_data[item]}\'', 'ERROR')
+            logger.error(f"Alphasense calibration data for {kwargs['alphasense_id']} is not correct")
+            logger.error(f'Error on {item}: \'{cal_data[item]}\'')
             return
 
     # Remove spurious voltages (0V < electrode < 5V)
     for electrode in ['we', 'ae']:
-        subkwargs = {'name': kwargs[electrode], 
+        subkwargs = {'name': kwargs[electrode],
                         'limits': (0, 5), # In V
                         'window_size': None
                     }
 
         df[f'{electrode}_clean'] = clean_ts(df, **subkwargs)
 
     # Compensate electronic zero
@@ -167,19 +169,20 @@
         priority: string
             Name of channel to be used as prioritary
     Returns
     -------
         Temperature series
     """
     if 'priority' in kwargs:
-        if kwargs['priority'] in dataframe.columns: return dataframe[kwargs['priority']]
-    if 'ASPT1000' in dataframe.columns: return dataframe['ASPT1000']
-    if 'PM_DALLAS_TEMP' in dataframe.columns: return dataframe['PM_DALLAS_TEMP']
-    if 'SHT31_EXT_TEMP' in dataframe.columns: return dataframe['SHT31_EXT_TEMP']
-    std_out('Problem with input data', 'ERROR')
+        if kwargs['priority'] in dataframe.columns:
+            return dataframe[kwargs['priority']]
+    for option in alphasense_temp_channel:
+        if option in dataframe.columns:
+            return dataframe[option]
+    logger.error('Problem with input data')
     return None
 
 def alphasense_pt1000(dataframe, **kwargs):
     """
     Calculates temperature in degC of a PT1000, given positive and negative voltage
     levels (in V), considering negative PT1000 value is grounded
     Parameters
@@ -202,56 +205,38 @@
     """
     # Check inputs
     flag_error = False
     if 'pt1000plus' not in kwargs: flag_error = True
     if 'pt1000minus' not in kwargs: flag_error = True
 
     if flag_error:
-        std_out('Problem with input data', 'ERROR')
+        logger.error('Problem with input data')
         return None
 
     if kwargs['afe_id'] is None:
-        std_out(f"Empty ID. Ignoring", 'WARNING')
+        logger.warning(f"Empty ID. Ignoring")
         return None
 
     # Get Sensor data
     if kwargs['afe_id'] not in config.calibrations:
-        std_out(f"AFE {kwargs['afe_id']} not in calibration data", 'ERROR')
+        logger.error(f"AFE {kwargs['afe_id']} not in calibration data")
         return None
 
-    # Process input dates
-    if 'from_date' not in kwargs: from_date = None
-    else:
-        if 'timezone' not in kwargs:
-            std_out('Cannot localise date without timezone', 'ERROR')
-            return None
-        from_date = localise_date(kwargs['from_date'], kwargs['timezone'])
-
-    if 'to_date' not in kwargs: to_date = None
-    else:
-        if 'timezone' not in kwargs:
-            std_out('Cannot localise date without timezone', 'ERROR')
-            return None
-        to_date = localise_date(kwargs['to_date'], kwargs['timezone'])
-
     # Retrieve calibration data - verify its all float
     cal_data = config.calibrations[kwargs['afe_id']]
     for item in cal_data:
         try:
             cal_data[item] = float (cal_data[item])
         except:
-            std_out(f"Alphasense calibration data for {kwargs['afe_id']} is not correct", 'ERROR')
-            std_out(f'Error on {item}: \'{cal_data[item]}\'', 'ERROR')
+            logger.error(f"Alphasense calibration data for {kwargs['afe_id']} is not correct")
+            logger.error(f'Error on {item}: \'{cal_data[item]}\'')
             return
 
     # Make copy
     df = dataframe.copy()
-    # Trim data
-    if from_date is not None: df = df[df.index > from_date]
-    if to_date is not None: df = df[df.index < to_date]
 
     # Calculate temperature
     df['v20'] = cal_data['v20'] - (cal_data['t20'] - 20.0) / 1000.0
     df['temp'] = (df[kwargs['pt1000plus']] - df['v20']) * 1000.0 + 20.0 # in degC
 
     return df['temp']
 
@@ -272,19 +257,19 @@
     -------
         Channel named accordingly
     """
     # Check inputs
     flag_error = False
     if 'channel' not in kwargs: flag_error = True
     if kwargs['channel'] not in dataframe:
-        std_out(f"Channel {kwargs['channel']} not in dataframe. Ignoring", 'WARNING')
+        logger.warning(f"Channel {kwargs['channel']} not in dataframe. Ignoring")
         return None
 
     if flag_error:
-        std_out('Problem with input data', 'ERROR')
+        logger.error('Problem with input data')
         return None
 
     # Make copy
     df = dataframe.copy()
     return df[kwargs['channel']]
 
 def basic_4electrode_alg(dataframe, **kwargs):
@@ -293,15 +278,15 @@
     and calibration ID. It adds a configurable background concentration.
     Parameters
     ----------
         working: string
             Name of working electrode found in dataframe
         auxiliary: string
             Name of auxiliary electrode found in dataframe
-        id: int 
+        id: int
             Sensor ID
         pollutant: string
             Pollutant name. Must be included in the corresponding LUTs for unit convertion and additional parameters:
             MOLECULAR_WEIGHTS, background_conc, CHANNEL_LUT
         hardware: alphadelta or isb
     Returns
     -------
@@ -310,37 +295,37 @@
 
     flag_error = False
     if 'working' not in kwargs: flag_error = True
     if 'auxiliary' not in kwargs: flag_error = True
     if 'id' not in kwargs: flag_error = True
     if 'pollutant' not in kwargs: flag_error = True
 
-    if flag_error: 
-        std_out('Problem with input data', 'ERROR')
+    if flag_error:
+        logger.error('Problem with input data')
         return None
 
     # Get Sensor data
-    if kwargs['id'] not in config.calibrations: 
-        std_out(f"Sensor {kwargs['id']} not in calibration data", 'ERROR')
+    if kwargs['id'] not in config.calibrations:
+        logger.error(f"Sensor {kwargs['id']} not in calibration data")
         return None
 
     we_sensitivity_na_ppb = config.calibrations[kwargs['id']]['we_sensitivity_na_ppb']
     we_cross_sensitivity_no2_na_ppb = config.calibrations[kwargs['id']]['we_cross_sensitivity_no2_na_ppb']
     sensor_type = config.calibrations[kwargs['id']]['sensor_type']
     nWA = config.calibrations[kwargs['id']]['we_sensor_zero_mv']/config.calibrations[kwargs['id']]['ae_sensor_zero_mv']
 
-    if sensor_type != kwargs['pollutant']: 
-        std_out(f"Sensor {kwargs['id']} doesn't coincide with calibration data", 'ERROR')
+    if sensor_type != kwargs['pollutant']:
+        logger.error(f"Sensor {kwargs['id']} doesn't coincide with calibration data")
         return None
 
     # This is always in ppm since the calibration data is in signal/ppm
     if kwargs['hardware'] == 'alphadelta': current_factor = alphadelta_pcb
     elif kwargs['hardware'] == 'isb': current_factor = 1 #TODO make it so we talk in mV
-    else: 
-        std_out(f"Measurement hardware {kwargs['hardware']} not supported", 'ERROR')
+    else:
+        logger.error(f"Measurement hardware {kwargs['hardware']} not supported")
         return None
 
     result = current_factor*(dataframe[kwargs['working']] - nWA*dataframe[kwargs['auxiliary']])/abs(we_sensitivity_na_ppb)
 
     # Convert units
     result *= get_units_convf(kwargs['pollutant'], from_units = 'ppm')
     # Add Background concentration
@@ -348,24 +333,24 @@
 
     return result
 
 def baseline_4electrode_alg(dataframe, **kwargs):
     """
     Calculates pollutant concentration based on 4 electrode sensor readings (mV), but using
     one of the metrics (baseline) as a baseline of the others. It uses the baseline correction algorithm
-    explained here: 
+    explained here:
     https://docs.smartcitizen.me/Components/sensors/Electrochemical%20Sensors/#baseline-correction-based-on-temperature
     and the calibration ID. It adds a configurable background concentration.
     Parameters
     ----------
         target: string
             Name of working electrode found in dataframe
         baseline: string
             Name of auxiliary electrode found in dataframe
-        id: int 
+        id: int
             Sensor ID
         pollutant: string
             Pollutant name. Must be included in the corresponding LUTs for unit convertion and additional parameters:
             MOLECULAR_WEIGHTS, background_conc, CHANNEL_LUT
         regression_type: 'string'
             'best'
             Use a 'linear' or 'exponential' regression for the calculation of the baseline
@@ -374,15 +359,15 @@
             The period at which the baseline is calculated. If full, the whole index will be used.
             https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases
         store_baseline: boolean
             True
             Whether or not to store the baseline in the dataframe
         resample: str
             '1Min'
-            Resample frequency for the target dataframe         
+            Resample frequency for the target dataframe
         pcb_factor: int
             alphadelta_pcb (6.36)
             Factor converting mV to nA due to the board configuration
 
     Returns
     -------
         calculation of pollutant based on: pcb_factor*sensitivity(working - zero_working)/(auxiliary - zero_auxiliary)
@@ -392,42 +377,42 @@
     baseline = Series()
 
     flag_error = False
     if 'target' not in kwargs: flag_error = True
     if 'baseline' not in kwargs: flag_error = True
     if 'id' not in kwargs: flag_error = True
     if 'pollutant' not in kwargs: flag_error = True
-    
-    if 'regression_type' in kwargs: 
+
+    if 'regression_type' in kwargs:
         if kwargs['regression_type'] not in ['best', 'exponential', 'linear']: flag_error = True
         else: reg_type = kwargs['regression_type']
     else: reg_type = 'best'
-    
-    if 'period' in kwargs: 
+
+    if 'period' in kwargs:
         if kwargs['period'] not in ['best', 'exponential', 'linear']: flag_error = True
         else: period = kwargs['period']
     else: period = '1D'
 
     if 'store_baseline' in kwargs: store_baseline = kwargs['store_baseline']
     else: store_baseline = True
 
     if 'resample' in kwargs: resample = kwargs['resample']
-    else: resample = '1Min'    
+    else: resample = '1Min'
 
     if 'pcb_factor' in kwargs: pcb_factor = kwargs['pcb_factor']
     else: pcb_factor = alphadelta_pcb
-    
+
     if 'baseline_type' in kwargs: baseline_type = kwargs['baseline_type']
     else: baseline_type = 'deltas'
 
     if 'deltas' in kwargs: deltas = kwargs['deltas']
     else: deltas = baseline_deltas
-    
-    if flag_error: 
-        std_out('Problem with input data', 'ERROR')
+
+    if flag_error:
+        logger.error('Problem with input data')
         return None
 
     min_date, max_date, _ = find_dates(dataframe)
     pdates = date_range(start = min_date, end = max_date, freq = period)
 
     for pos in range(0, len(pdates)-1):
         chunk = dataframe.loc[pdates[pos]:pdates[pos+1], [kwargs['target'], kwargs['baseline']]]
@@ -439,46 +424,46 @@
 
         sensitivity_1 = config.calibrations.loc[kwargs['id'],'sensitivity_1']
         sensitivity_2 = config.calibrations.loc[kwargs['id'],'sensitivity_2']
         target_1 = config.calibrations.loc[kwargs['id'],'target_1']
         target_2 = config.calibrations.loc[kwargs['id'],'target_2']
         nWA = config.calibrations.loc[kwargs['id'],'w_zero_current']/config.calibrations.loc[kwargs['id'],'aux_zero_current']
 
-        if target_1 != kwargs['pollutant']: 
-            std_out(f"Sensor {kwargs['id']} doesn't coincide with calibration data", 'ERROR')
+        if target_1 != kwargs['pollutant']:
+            logger.error(f"Sensor {kwargs['id']} doesn't coincide with calibration data")
             return None
-        
+
         result = pcb_factor*(dataframe[kwargs['target']] - baseline)/abs(sensitivity_1)
 
         # Convert units
         result *= get_units_convf(kwargs['pollutant'], from_units = 'ppm')
         # Add Background concentration
         result += background_conc[kwargs['pollutant']]
-    
+
     else:
         # Calculate non convolved part
         result = dataframe[kwargs['target']] - baseline
 
     # Make use of DataFrame inmutable properties to store in it the baseline
     if store_baseline:
         dataframe[kwargs['target']+'_BASELINE'] = baseline
-    
+
     return result
 
 def deconvolution(dataframe, **kwargs):
     """
     Calculates pollutant concentration for convolved metrics, such as NO2+O3.
     Needs convolved metric, and target pollutant sensitivities
     Parameters
     ----------
         source: string
             Name of convolved metric containing both pollutants (such as NO2+O3)
         base: string
             Name of one of the already deconvolved pollutants (for instance NO2)
-        id: int 
+        id: int
             Sensor ID
         pollutant: string
             Pollutant name. Must be included in the corresponding LUTs for unit convertion and additional parameters:
             MOLECULAR_WEIGHTS, background_conc, CHANNEL_LUT
     Returns
     -------
         calculation of pollutant based on: 6.36 * sensitivity(working - zero_working)/(auxiliary - zero_auxiliary)
@@ -489,30 +474,30 @@
 
     flag_error = False
     if 'source' not in kwargs: flag_error = True
     if 'base' not in kwargs: flag_error = True
     if 'id' not in kwargs: flag_error = True
     if 'pollutant' not in kwargs: flag_error = True
 
-    if flag_error: 
-        std_out('Problem with input data', 'ERROR')
+    if flag_error:
+        logger.error('Problem with input data')
         return None
 
     sensitivity_1 = config.calibrations.loc[kwargs['id'],'sensitivity_1']
     sensitivity_2 = config.calibrations.loc[kwargs['id'],'sensitivity_2']
     target_1 = config.calibrations.loc[kwargs['id'],'target_1']
     target_2 = config.calibrations.loc[kwargs['id'],'target_2']
     nWA = config.calibrations.loc[kwargs['id'],'w_zero_current']/config.calibrations.loc[kwargs['id'],'aux_zero_current']
 
-    if target_1 != kwargs['pollutant']: 
-        std_out(f"Sensor {kwargs['id']} doesn't coincide with calibration data", 'ERROR')
+    if target_1 != kwargs['pollutant']:
+        logger.error(f"Sensor {kwargs['id']} doesn't coincide with calibration data")
         return None
 
     factor_unit_1 = get_units_convf(kwargs['pollutant'], from_units = 'ppm')
     factor_unit_2 = get_units_convf(kwargs['base'], from_units = 'ppm')
 
     result = factor_unit_1*(alphadelta_pcb*dataframe[kwargs['source']] - dataframe[kwargs['base']]/factor_unit_2*abs(sensitivity_2))/abs(sensitivity_1)
-    
+
     # Add Background concentration
     result += background_conc[kwargs['pollutant']]
-    
+
     return result
```

### Comparing `scdata-0.9.1/scdata/device/process/baseline.py` & `scdata-1.0.0/scdata/device/process/baseline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from numpy import ones, transpose, log
-from scipy.stats.stats import linregress
+from scipy.stats import linregress
 from scipy.sparse import (diags, spdiags)
 from scipy.sparse.linalg import spsolve
 from pandas import date_range
 from numpy import min as npmin
 from numpy import max as npmax
 from numpy import abs as npabs
 from numpy import argmax, argmin, arange, exp
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 from math import isnan
 from .formulae import exp_f
 import matplotlib.pyplot as plt
 from re import search
 
 def find_min_max(min_max, iterable = list()):
@@ -22,23 +22,23 @@
         min_max: 'string'
             whether to find the 'min' or the 'max'
         iterable: list
             list to obtain maximum value
     Returns
     -------
         Value and index of maximum in the list
-    """   
+    """
 
     if min_max == 'max':
         value = npmax(iterable)
         index = argmax(iterable)
     elif min_max == 'min':
         value = npmin(iterable)
         index = argmin(iterable)
-    else: 
+    else:
         value, index = None, None
 
     return value, index
 
 def get_delta_baseline(series, **kwargs):
     """
     Baseline based on deltas method
@@ -61,89 +61,89 @@
 
     # if 'resample' in kwargs: resample = kwargs['resample']
     # else: resample = '1Min'
 
     if 'btype' in kwargs: btype = kwargs['btype']
     else: btype = 'min'
 
-    if delta == 0: std_out(f'Not valid delta = {delta}', 'ERROR'); return None
-    
+    if delta == 0: logger.error(f'Not valid delta = {delta}'); return None
+
     result = series.copy()
     # result = result.resample(resample).mean()
 
     pdates = date_range(start = result.index[0], end = result.index[-1], freq = f'{delta}Min')
 
     for pos in range(0, len(pdates)-1):
         chunk = series[pdates[pos]:pdates[pos+1]]
-        
+
         if len(chunk.values) == 0: result[pdates[pos]:pdates[pos+1]] = 0
-        else: 
+        else:
             if btype == 'min': result[pdates[pos]:pdates[pos+1]] = min(chunk.values)
             elif btype == 'max': result[pdates[pos]:pdates[pos+1]] = max(chunk.values)
-    
+
     return result
 
 def get_als_baseline(series, lambd = 1e5, p = 0.01, n_iter=10):
 
     L = len(series)
     D = diags([1,-2,1],[0,-1,-2], shape=(L,L-2))
     w = ones(L)
 
     for i in range(n_iter):
         W = spdiags(w, 0, L, L)
         Z = W + lambd * D.dot(D.transpose())
         z = spsolve(Z, w*series)
         w = p * (series > z) + (1-p) * (series < z)
-    
+
     return z
 
 # TODO DOCUMENT
 def baseline_calc(dataframe, **kwargs):
 
     '''
     reg_type
     baseline_type
-      if als  
+      if als
         lambdas
         p
-      if deltas  
+      if deltas
         esample: int (optional)
             '1Min'
             Frequency at which the delta is based on, and therefore to resample to
         deltas
     '''
 
     if 'reg_type' not in kwargs: reg_type = 'best'
     else: reg_type = kwargs['reg_type']
 
     if 'baseline_type' not in kwargs: baseline_type = 'deltas'
     else: baseline_type = kwargs['baseline_type']
 
     pearsons =[]
-    target_name = dataframe.iloc[:,0].name; std_out ('Target: ', target_name)
-    baseline_name = dataframe.iloc[:,1].name; std_out ('Baseline: ', baseline_name)
+    target_name = dataframe.iloc[:,0].name; logger.info('Target: ', target_name)
+    baseline_name = dataframe.iloc[:,1].name; logger.info('Baseline: ', baseline_name)
 
     result = dataframe.copy()
     result.dropna(axis = 0, inplace=True)
 
     if result.empty: return None
 
-    if config._intermediate_plots and config._plot_out_level == 'DEBUG': 
+    if config._intermediate_plots and config._plot_out_level == 'DEBUG':
         fig, ax = plt.subplots(figsize=(12,8))
 
     if baseline_type == 'deltas':
 
         if 'deltas' not in kwargs: n_deltas = config._baseline_deltas
         else: n_deltas = kwargs['deltas']
-        
+
         if 'resample' not in kwargs: resample = '1Min'
         else: resample = kwargs['resample']
 
         result = result.resample(resample).mean()
-        
+
         l_iter = n_deltas
 
         for delta in n_deltas:
 
             name_delta = target_name +'_' +str(delta)
 
             result[name_delta] = get_delta_baseline(result.loc[:,target_name], delta = delta)
@@ -151,15 +151,15 @@
             # Try to resample to improve correlation of baseline and target
             off_base = int(search(r'\d+', resample).group())
             off_alias = ''.join(i for i in resample if not i.isdigit())
 
             target_resampled = result.loc[:,name_delta].resample(f'{delta*off_base}{off_alias}').mean().values
             baseline_resampled = result.loc[:,baseline_name].resample(f'{delta*off_base}{off_alias}').mean().values
 
-            if config._intermediate_plots and config._plot_out_level == 'DEBUG': 
+            if config._intermediate_plots and config._plot_out_level == 'DEBUG':
                 ax.plot(result.index, result[name_delta], label = name_delta)
 
             _, _, r_value, _, _ = linregress(transpose(target_resampled), transpose(baseline_resampled))
             pearsons.append(r_value)
 
     elif baseline_type == 'als':
 
@@ -172,113 +172,113 @@
         l_iter = lambdas
 
         for lambd in lambdas:
 
             name_lambda = name +'_' +str(lambd)
             result[name_lambda] = get_als_baseline(result.loc[:,target_name], lambd, p)
 
-            if config._intermediate_plots and config._plot_out_level == 'DEBUG': 
+            if config._intermediate_plots and config._plot_out_level == 'DEBUG':
                 ax.plot(result.index, result[name_lambda], label = name_lambda)
 
             _, _, r_value, _, _ = linregress(transpose(result[name_lambda]), transpose(result.loc[:,baseline_name].values))
             pearsons.append(r_value)
 
     if config._intermediate_plots and config._plot_out_level == 'DEBUG':
         plt.show()
         ax.plot(result.index, result.loc[:,target_name], label = target_name)
         ax.plot(result.index, result.loc[:,baseline_name], label = baseline_name)
-        
+
         ax.axis('tight')
         ax.legend(loc='best')
         ax.set_xlabel('Date')
         ax.set_ylabel('Baselines')
         ax.grid(True)
-    
+
         plt.show()
 
     ## Find Max in the pearsons - correlation can be negative, so use absolute of the pearson
     _, ind_max = find_min_max('max', npabs(pearsons))
-    # std_out(f'Max index in pearsons: {ind_max}')
+    # logger.info(f'Max index in pearsons: {ind_max}')
     result.dropna(axis = 0, inplace=True)
 
     if reg_type == 'linear':
-        
+
         ## Fit with y = A + Bx
         slope, intercept, r_value, p_value, std_err = linregress(transpose(result.loc[:,baseline_name].values), result[(target_name + f'_{l_iter[ind_max]}')])
         baseline = intercept + slope*result.loc[:,baseline_name].values
         # print (r_value)
-    
+
     elif reg_type == 'exponential':
-        
+
         ## Fit with y = Ae^(Bx) -> logy = logA + Bx
         logy = log(result[(target_name + f'_{l_iter[ind_max]}')])
         slope, intercept, r_value, p_value, std_err = linregress(transpose(result.loc[:,baseline_name].values), logy)
         baseline = exp_f(transpose(result.loc[:,baseline_name].values), exp(intercept), slope, 0)
         # print (r_value)
-    
+
     elif reg_type == 'best':
-        
+
         ## Find linear r_value
         slope_lin, intercept_lin, r_value_lin, p_value_lin, std_err_lin = linregress(transpose(result.loc[:, baseline_name].values), result[(target_name + f'_{l_iter[ind_max]}')])
-        
+
         ## Find Exponential r_value
         logy = log(result[(target_name + f'_{l_iter[ind_max]}')])
         slope_exp, intercept_exp, r_value_exp, p_value_exp, std_err_exp = linregress(transpose(result.loc[:, baseline_name].values), logy)
 
         ## Pick which one is best
         if ((not isnan(r_value_exp)) and (not isnan(r_value_lin))):
 
             if r_value_lin > r_value_exp:
                 baseline = intercept_lin + slope_lin*result.loc[:,baseline_name].values
             else:
                 baseline = exp_f(transpose(result.loc[:,baseline_name].values), exp(intercept_exp), slope_exp, 0)
-        
+
         elif not isnan(r_value_lin):
-            
+
             baseline = intercept_lin + slope_lin*result.loc[:,baseline_name].values
-        
+
         elif not isnan(r_value_exp):
-            
+
             baseline = exp_f(transpose(result.loc[:,baseline_name].values), exp(intercept_exp), slope_exp, 0)
         else:
-            std_out('Exponential and linear regression are nan', 'ERROR')
-    
+            logger.error('Exponential and linear regression are nan')
+
     # Avoid baselines higher than the target
     result[target_name + '_baseline_raw'] = baseline
     result[target_name + '_baseline'] = result[[(target_name + '_' + 'baseline_raw'), target_name]].min(axis=1)
-    
+
     if config._intermediate_plots and config._plot_out_level == 'DEBUG':
         with plt.style.context('seaborn-white'):
             fig1, (ax1, ax2) = plt.subplots(nrows=1, ncols=2, figsize=(12,8))
-            
+
             ax1.plot(result.loc[:, baseline_name].values, result[(target_name + f'_{l_iter[ind_max]}')], label = 'Baseline ' + str(l_iter[ind_max]), linewidth=0, marker='o')
             ax1.plot(result.loc[:, baseline_name].values, result[(target_name + '_baseline')] , label = 'Regressed value', linewidth=0, marker='o')
             legend = ax1.legend(loc='best')
             ax1.set_xlabel(baseline_name)
             ax1.set_ylabel('Regression values')
             ax1.grid(True)
-            
+
             lns1 = ax2.plot(result.index, result.loc[:, target_name], label = "Target", linestyle=':', linewidth=1, marker=None)
             #[ax2.plot(result.index, result[(name +'_' +str(delta))].values, label="Delta {}".format(delta), marker=None,  linestyle='-', linewidth=1) for delta in _numberDeltas]
             lns2 = ax2.plot(result.index, result[target_name + '_' + 'baseline'], label='Baseline', marker = None)
 
             ax2.axis('tight')
             ax2.set_title("Baseline Extraction")
             ax2.grid(True)
-            
+
             ax22 = ax2.twinx()
             lns22 = ax22.plot(result.index, result.loc[:, baseline_name].values, color = 'red', label = baseline_name, linestyle='-', linewidth=1, marker=None)
             ax22.set_ylabel(result.loc[:, baseline_name].name, color = 'red')
             ax22.set_ylim(ax2.get_ylim())
             ax22.tick_params(axis='y', labelcolor='red')
 
             lns = lns1+lns2+lns22
             labs = [l.get_label() for l in lns]
             ax2.legend(lns, labs, loc='best')
-            
+
             fig2, ax3 = plt.subplots(figsize=(12,8)) # two axes on figure
             ax3.plot(l_iter, pearsons)
 
             if baseline_type == 'deltas':
                 ax3.set_title("R2 vs. Delta")
                 ax3.set_xlabel('Delta')
```

### Comparing `scdata-0.9.1/scdata/device/process/formulae.py` & `scdata-1.0.0/scdata/device/process/formulae.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from numpy import exp, log, transpose
-from scipy.stats.stats import linregress
+from scipy.stats import linregress
 
 # TODO REVIEW
 def absolute_humidity(dataframe, **kwargs):
     """
     Calculate Absolute humidity based on vapour equilibrium
     Parameters
     ----------
```

### Comparing `scdata-0.9.1/scdata/device/process/geoseries.py` & `scdata-1.0.0/scdata/device/process/geoseries.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/device/process/params.py` & `scdata-1.0.0/scdata/device/process/params.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/device/process/regression.py` & `scdata-1.0.0/scdata/device/process/regression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from scdata._config import config
-from scdata.utils import std_out, dict_fmerge, clean
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.cleaning import clean
 from pandas import DataFrame
 from numpy import array
 
 def apply_regressor(dataframe, **kwargs):
 	'''
 	Applies a regressor model based on a pretrained model
 	Parameters
@@ -30,28 +32,28 @@
 	for device in kwargs['variables']['inputs']:
 		inputs = list(set(inputs).union(set(kwargs['variables']['inputs'][device])))
 
 	try:
 		inputdf = dataframe[inputs].copy()
 		inputdf = inputdf.reindex(sorted(inputdf.columns), axis=1)
 	except KeyError:
-		std_out('Inputs not in dataframe', 'ERROR')
+		logger.error('Inputs not in dataframe')
 		pass
 		return None
 
 	if 'model' not in kwargs:
-		std_out('Model not in inputs', 'ERROR')
+		logger.error('Model not in inputs')
 	else:
 		model = kwargs['model']
 
 	if 'options' not in kwargs:
 		options = config._model_def_opt
 	else:
 		options = dict_fmerge(config._model_def_opt, kwargs['options'])
-	
+
 	# Remove na
-	inputdf = clean(inputdf, options['clean_na'], how = 'any') 
+	inputdf = clean(inputdf, options['clean_na'], how = 'any')
 
 	features = array(inputdf)
 	result = DataFrame(model.predict(features)).set_index(inputdf.index)
 
 	return result
```

### Comparing `scdata-0.9.1/scdata/device/process/timeseries.py` & `scdata-1.0.0/scdata/device/process/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numpy import nan, full, power, ones, diff, convolve, append
 from scipy import ndimage
 from scdata.device.process import is_within_circle
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 
 def delta_index_ts(dataframe, **kwargs):
     result = dataframe.index.to_series().diff().astype('timedelta64[s]')
     return result
 
 def poly_ts(dataframe, **kwargs):
     """
@@ -21,27 +21,27 @@
         extra_term: float
             0
             Independent term
     Returns
     -------
         result = sum(coefficients[i]*channels[i]^exponents[i] + extra_term)
     """
-    
+
     if 'channels' not in kwargs: return None
     else: channels = kwargs['channels']
     n_channels = len(channels)
 
     result = 0 * dataframe[channels[0]].copy()
 
     if 'coefficients' not in kwargs: coefficients = ones(n_channels)
     else: coefficients = kwargs['coefficients']
-    
+
     if 'exponents' not in kwargs: exponents = ones(n_channels)
     else: exponents = kwargs['exponents']
-    
+
     if 'extra_term' not in kwargs: extra_term = 0
     else: extra_term = kwargs['extra_term']
 
     # Do it in pandas to ensure index and na handling
     for i in range(n_channels):
         result += power(dataframe[channels[i]], exponents[i]) * coefficients[i]
 
@@ -50,18 +50,18 @@
 def clean_ts(dataframe, **kwargs):
     """
     Cleans the time series measurements sensors, by filling the out of band values with NaN
     Parameters
     ----------
         name: string
             column to clean to apply.
-        limits: list, optional 
+        limits: list, optional
             (0, 99999)
             Sensor limits. The function will fill with NaN in the values that exceed the band
-        window_size: int, optional 
+        window_size: int, optional
             3
             If not None, will smooth the time series by applying a rolling window of that size
         window_type: str, optional
             None
             Accepts arguments in the list of windows for scipy.signal windows:
             https://docs.scipy.org/doc/scipy/reference/signal.html#window-functions
             Default to None implies normal rolling average
@@ -78,49 +78,49 @@
     if 'limits' in kwargs: lower_limit, upper_limit = kwargs['limits'][0], kwargs['limits'][1]
     else: lower_limit, upper_limit = 0, 99999
 
     result[result > upper_limit] = nan
     result[result < lower_limit] = nan
 
     # Smoothing
-    if 'window_size' in kwargs: window = kwargs['window_size'] 
+    if 'window_size' in kwargs: window = kwargs['window_size']
     else: window = 3
 
     if 'window_type' in kwargs: win_type = kwargs['window_type']
     else: win_type = None
 
     if window is not None:
         result.rolling(window = window, win_type = win_type).mean()
 
     return result
 
 def merge_ts(dataframe, **kwargs):
     """
-    Merges readings from sensors into one clean ts. The function checks the dispersion and 
+    Merges readings from sensors into one clean ts. The function checks the dispersion and
     picks the desired one (min, max, min_nonzero, avg)
     Parameters
     ----------
         names: list of strings
             List of sensors to merge into one. Currently only support two ts.
         pick: string
             'min'
             One of the following 'min', 'max', 'avg', 'min_nonzero'
-            Which one two pick in case of high deviation between the metrics. Picks the avg 
+            Which one two pick in case of high deviation between the metrics. Picks the avg
             otherwise
         factor: float (factor > 0)
             0.3
             Maximum allowed deviation of the difference with respect to the each of signals.
             It creates a window of [factor*signal_X, -factor*signal_X] for X being each signal
-            out of which there will be a flag where one of the signals will be picked. This 
+            out of which there will be a flag where one of the signals will be picked. This
             factor should be set to a value that is similar to the sensor typical deviation
         Same parameters as clean_ts apply below:
-        limits: list, optional 
+        limits: list, optional
             (0, 99999)
             Sensor limits. The function will fill with NaN in the values that exceed the band
-        window_size: int, optional 
+        window_size: int, optional
             3
             If not None, will smooth the time series by applying a rolling window of that size
         window_type: str, optional
             None
             Accepts arguments in the list of windows for scipy.signal windows:
             https://docs.scipy.org/doc/scipy/reference/signal.html#window-functions
             Default to None implies normal rolling average
@@ -135,37 +135,37 @@
     if 'names' not in kwargs: return None
     if 'pick' not in kwargs: pick = 'min'
     else: pick = kwargs['pick']
     if 'factor' not in kwargs: factor = 0.3
     else: factor = kwargs['factor']
 
     # Clean them
-    for name in kwargs['names']: 
-        subkwargs = {'name': name, 
-                    'limits': kwargs['limits'], 
-                    'window_size': kwargs['window_size'], 
+    for name in kwargs['names']:
+        subkwargs = {'name': name,
+                    'limits': kwargs['limits'],
+                    'window_size': kwargs['window_size'],
                     'window_type': kwargs['window_type']
                     }
         df[name + '_CLEAN'] = clean_ts(df, **subkwargs)
 
-    
+
     df['flag'] = full((df.shape[0], 1), False, dtype=bool)
     df['diff'] = df[kwargs['names'][0] + '_CLEAN'] - df[kwargs['names'][1] + '_CLEAN']
 
     lnames = []
     # Flag them
     for name in kwargs['names']:
         df['flag'] |= (df['diff'] > factor*df[name + '_CLEAN'])
         df['flag'] |= (df['diff'] < -factor*df[name + '_CLEAN'])
         lnames.append(name + '_CLEAN')
 
     df['result'] = df.loc[:, lnames].mean(skipna=True, axis = 1)
-    
+
     # Pick
-    if pick == 'min': 
+    if pick == 'min':
         df.loc[df['flag'] == True, 'result'] = df.loc[df['flag'] == True, lnames].min(skipna=True, axis = 1)
     elif pick == 'max':
         df.loc[df['flag'] == True, 'result'] = df.loc[df['flag'] == True, lnames].max(skipna=True, axis = 1)
     # elif pick == 'min_nonzero':
     #     df['result'] = df.loc[df['flag'] == True, kwargs['names']].min(skipna=True, axis = 1)
 
     return df['result']
@@ -173,45 +173,45 @@
 def rolling_avg(dataframe, **kwargs):
     """
     Performs pandas.rolling with input
     Parameters
     ----------
         name: string
             column to clean to apply.
-        window_size: int, optional 
+        window_size: int, optional
             3
             If not None, will smooth the time series by applying a rolling window of that size
         window_type: str, optional
             None
             Accepts arguments in the list of windows for scipy.signal windows:
             https://docs.scipy.org/doc/scipy/reference/signal.html#window-functions
             Default to None implies normal rolling average
         type: str, optional
             'mean'
             Accepts mean, max or min for rolling windows. Default is 'mean' as per the scipy
             implementation
     Returns
     -------
         pandas series containing the rolling average
-    """   
+    """
 
     if 'name' not in kwargs:
-        std_out (f'{kwargs[name]} not in kwargs', 'ERROR')
+        logger.error (f'{kwargs[name]} not in kwargs')
         return None
 
     result = dataframe[kwargs['name']].copy()
 
     # Smoothing
-    if 'window_size' in kwargs: window = kwargs['window_size'] 
+    if 'window_size' in kwargs: window = kwargs['window_size']
     else: window = 3
 
     if 'window_type' in kwargs: win_type = kwargs['window_type']
     else: win_type = None
 
-    if 'type' in kwargs: 
+    if 'type' in kwargs:
         if kwargs['type'] == 'mean': return result.rolling(window = window, win_type = win_type).mean()
         if kwargs['type'] == 'max': return result.rolling(window = window, win_type = win_type).max()
         if kwargs['type'] == 'min': return result.rolling(window = window, win_type = win_type).min()
     else:
         return result.rolling(window = window, win_type = win_type).mean()
 
 def time_derivative(dataframe, **kwargs):
```

### Comparing `scdata-0.9.1/scdata/io/csv.py` & `scdata-1.0.0/scdata/io/device_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,70 @@
 from os import makedirs, listdir
 from os.path import exists, join, splitext
-from scdata.utils import std_out, localise_date, clean
+import csv
+
+from scdata.tools.custom_logger import logger
+from scdata.tools.date import localise_date
+from scdata.tools.cleaning import clean
 from pandas import read_csv, to_datetime, DataFrame
 from scdata._config import config
-import csv
+from scdata.models import Metric
+
+class CSVHandler:
+    ''' Main implementation of the CSV data class '''
 
+    def __init__(self, params):
+        self.id = params.id
+        self.params = params
+        self.method = 'sync'
+        self.data = DataFrame()
+        self._metrics: List[Metric] = []
+        self.latest_postprocessing = None
+        if not self.__check__():
+            raise FileExistsError(f'File not found: {self.params.path}')
+
+    def __check__(self):
+        return exists(self.params.path)
+
+    @property
+    def timezone(self):
+        return self.params.timezone
+
+    # This returns an empty list to avoid renaming CSVs
+    @property
+    def sensors(self):
+        return []
+
+    def update_latest_postprocessing(self, date):
+
+        try:
+            self.latest_postprocessing = date.to_pydatetime()
+        except:
+            return False
+        else:
+            logger.info(f"Updated latest_postprocessing to: {self.latest_postprocessing}")
+            return True
+
+        logger.info('Nothing to update')
+
+        return True
+
+    def get_data(self, **kwargs):
+        self.data = read_csv_file(self.params.path,
+            timezone= self.timezone,
+            frequency= kwargs['frequency'],
+            clean_na= kwargs['clean_na'],
+            index_name= self.params.index,
+            skiprows=self.params.header_skip,
+            sep=self.params.separator,
+            tzaware=self.params.tzaware,
+            resample=kwargs['resample']
+        )
+
+        return self.data
 
 def export_csv_file(path, file_name, df, forced_overwrite=False):
     '''
     Exports pandas dataframe to a csv file
     Parameters
     ----------
         path: String
@@ -28,28 +84,26 @@
     # If path does not exist, create it
     if not exists(path):
         makedirs(path)
 
     # If file does not exist
     if not exists(path + '/' + str(file_name) + '.csv') or forced_overwrite:
         df.to_csv(path + '/' + str(file_name) + '.csv', sep=",")
-        std_out('File saved to: \n' + path + '/' + str(file_name) + '.csv', 'SUCCESS')
+        logger.info('File saved to: \n' + path + '/' + str(file_name) + '.csv')
     else:
-        std_out("File Already exists - delete it first, I was not asked to overwrite anything!", 'ERROR')
+        logger.error("File Already exists - delete it first, I was not asked to overwrite anything!")
         return False
-
     return True
 
-
-def read_csv_file(file_path, timezone, frequency=None, clean_na=None, index_name='', skiprows=None, sep=',', encoding='utf-8', tzaware=True, resample=True):
+def read_csv_file(path, timezone, frequency=None, clean_na=None, index_name='', skiprows=None, sep=',', encoding='utf-8', tzaware=True, resample=True):
     """
     Reads a csv file and adds cleaning, localisation and resampling and puts it into a pandas dataframe
     Parameters
     ----------
-        file_path: String
+        path: String
             File path for csv file
         timezone: String
             Time zone for the csv file
         frequency: String
             None
             Frequency in pandas format of the desired output
         clean_na: String or None
@@ -70,39 +124,39 @@
     Returns
     -------
         Pandas dataframe
     """
 
     # Read pandas dataframe
 
-    df = read_csv(file_path, verbose=False, skiprows=skiprows, sep=sep,
-                  encoding=encoding, encoding_errors='ignore')
+    df = read_csv(path, verbose=False, skiprows=skiprows, sep=sep,
+                encoding=encoding, encoding_errors='ignore')
 
     flag_found = False
     if type(index_name) == str:
         # Single joint index
         for column in df.columns:
             if index_name in column:
                 df = df.set_index(column)
                 flag_found = True
                 break
     elif type(index_name) == list:
         # Composite index (for instance, DATE and TIME in different columns)
         for iname in index_name:
             if iname not in df.columns:
-                std_out(f'{iname} not found in columns', 'ERROR')
+                logger.error(f'{iname} not found in columns')
                 return None
         joint_index_name = '_'.join(index_name)
         df[joint_index_name] = df[index_name].agg(' '.join, axis=1)
         df = df.set_index(joint_index_name)
         df.drop(index_name, axis=1, inplace=True)
         flag_found = True
 
     if not flag_found:
-        std_out('Index not found. Cannot reindex', 'ERROR')
+        logger.error('Index not found. Cannot reindex')
         return None
 
     # Set index
     df.index = localise_date(df.index, timezone, tzaware=tzaware)
     # Remove duplicates
     df = df[~df.index.duplicated(keep='first')]
 
@@ -114,15 +168,15 @@
 
     # Check for weird things in the data
     # df = df.apply(to_numeric, errors='coerce')
     df = df.astype(float, errors='ignore')
 
     # Resample
     if (resample):
-        std_out ('Resampling', 'INFO')
+        logger.info ('Resampling', 'INFO')
         df = df.resample(frequency).mean()
 
     # Remove na
     df = clean(df, clean_na, how = 'all')
 
     return df
 
@@ -154,24 +208,24 @@
 
     concat = DataFrame()
     header_tokenized = dict()
     marked_for_revision = False
 
     for file in listdir(path):
         if file != output and file not in ignore:
-            std_out(f'Loading file: {file}')
+            logger.info(f'Loading file: {file}')
             filename, _ = splitext(file)
             src_path = join(path, file)
 
             try:
                 with open(src_path, 'r', newline = '\n', errors = 'replace') as csv_file:
                     header = csv_file.readlines()[0:4]
             except:
                 ignore_file = True
-                std_out(f'Ignoring file: {file}', 'WARNING')
+                logger.warning(f'Ignoring file: {file}')
                 pass
             else:
                 ignore_file = False
 
             if ignore_file: continue
 
             if keep:
@@ -205,31 +259,31 @@
         rename = kwargs['rename_to_blueprint']
     else:
         rename = False
 
     if 'blueprint' in kwargs:
         rename_bp = kwargs['blueprint']
         if rename_bp not in config.blueprints:
-            std_out('Blueprint not in config. Cannot rename', 'WARNING')
+            logger.warning('Blueprint not in config. Cannot rename')
             rename = False
     else:
-        std_out('No blueprint specified', 'INFO')
+        logger.info('No blueprint specified')
         rename = False
 
     if rename:
-        std_out('Keep in mind that renaming doesnt change the units', 'WARNING')
+        logger.warning('Keep in mind that renaming doesnt change the units')
         rename_d = dict()
         for old_key in header_tokenized:
             for key, value in config.blueprints[rename_bp]['sensors'].items():
                 if value['id'] == header_tokenized[old_key]['id'] and old_key != key:
                     rename_d[old_key] = key
                     break
 
         for old_key in rename_d:
-            std_out(f'Renaming {old_key} to {rename_d[old_key]}')
+            logger.info(f'Renaming {old_key} to {rename_d[old_key]}')
             header_tokenized[rename_d[old_key]] = header_tokenized.pop(old_key)
             concat.rename(columns=rename_d, inplace=True)
 
     ## Save it as CSV
     if output.endswith('.CSV') or output.endswith('.csv'):
         concat.to_csv(join(path, output))
```

### Comparing `scdata-0.9.1/scdata/io/device_api.py` & `scdata-1.0.0/scdata/io/device_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from traceback import print_exc
 from requests import get, post, patch
 from re import search
 from io import StringIO
 
 from geopy.distance import distance
 from scdata._config import config
-from scdata.utils import std_out, localise_date, clean, get_elevation, url_checker, process_headers
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.date import localise_date
+from scdata.tools.cleaning import clean
+from scdata.tools.url_check import url_checker
+from scdata.tools.gets import process_headers
 # from tzwhere import tzwhere
 from timezonefinder import TimezoneFinder
 from datetime import date, datetime
 from os import environ, urandom
 from json import dumps, JSONEncoder
 
 import binascii
@@ -50,1815 +55,1815 @@
             return int(obj)
         if isinstance(obj, floating):
             return float(obj)
         if isinstance(obj, ndarray):
             return obj.tolist()
         return super(NpEncoder, self).default(obj)
 
-class ScApiDevice:
+# class ScApiDevice:
 
-    API_BASE_URL='https://api.smartcitizen.me/v0/devices/'
+#     API_BASE_URL='https://api.smartcitizen.me/v0/devices/'
 
-    def __init__ (self, did):
+#     def __init__ (self, did):
 
-        self.id = did # the number after https://smartcitizen.me/kits/######
-        self.kit_id = None # the number that defines the type of blueprint
-        self.mac = None
-        self.last_reading_at = None
-        self.added_at = None
-        self.timezone = None
-        self.lat = None
-        self.long = None
-        self.alt = None
-        self.data = None
-        self.sensors = None
-        self.devicejson = None
-        self.postprocessing = None
-        self._url = f'https://smartcitizen.me/kits/{self.id}'
-        self._api_url = f'{self.API_BASE_URL}{self.id}'
-
-    @property
-    def url(self):
-        return self._url
-
-    @property
-    def api_url(self):
-        return self._api_url
-
-    @staticmethod
-    # def new_device(name, kit_id = 26, location = None, exposure = 'indoor', user_tags = 'Lab, Research, Experimental', dry_run = False):
-    def new_device(name, location = {}, dry_run = False, **kwargs):
-        '''
-            Creates a new device in the Smart Citizen Platform provided a name
-            Parameters
-            ----------
-                name: string
-                    Device name
-                location: dict, optional
-                    None
-                    location = {
-                                'longitude': longitude (double) – sensor east-west position,
-                                'latitude': latitude (double) – sensor north-south position,
-                                'altitude': altitude (double) – sensor height above sea level
-                                }
-                dry_run: boolean
-                    False
-                    Post the payload to the API or just return it
-                **kwargs
-                ------
-                kit_id: int, optional
-                    26 (SCK 2.1)
-                    Kit ID - related to blueprint
-                exposure: string, optional
-                    'indoor'
-                    Type of exposure ('indoor', 'outdoor')
-                user_tags: string
-                    'Lab, Research, Experimental'
-                    User tags, comma separated
-                -----
-            Returns
-            -------
-                If dry_run, prints out a dict containing the payload and
-                returns False
-                If not, either False in case of error or a
-                dictionary containing:
-                    id (int) – sensor identifier
-                    message (string) – HTTP status text
-                    http-status-code (int) – HTTP status code
-        '''
-
-        API_BASE_URL = 'https://api.smartcitizen.me/v0/devices'
-
-        if 'SC_ADMIN_BEARER' not in environ:
-            std_out('Cannot post without Auth Bearer', 'ERROR')
-            return
-
-        headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'], 'Content-type': 'application/json'}
-
-        # Set defaults
-        if 'kit_id' not in kwargs:
-            kit_id = 26
-        else: kit_id = kwargs['kit_id']
-
-        if 'exposure' not in kwargs:
-            exposure = 'indoor'
-        else: exposure = kwargs['exposure']
-
-        if 'user_tags' not in kwargs:
-            user_tags = 'Lab, Research, Experimental'
-        else: user_tags = kwargs['user_tags']
-
-        payload = {}
-        try:
-            payload['name'] = name
-        except:
-            std_out('Your device needs a name!', 'ERROR')
-            sys.exit()
-
-        payload['device_token'] = binascii.b2a_hex(urandom(3)).decode('utf-8')
-        payload['description'] = ''
-        payload['kit_id'] = kit_id
-        payload['latitude'] = location['latitude']
-        payload['longitude'] = location['longitude']
-        payload['exposure'] = exposure
-        payload['user_tags'] = user_tags
-
-        if dry_run:
-            std_out(f'Dry run request to: {API_BASE_URL}sensors/configure')
-            print(dumps(payload, indent = 2))
-            return False
-
-        response = post(API_BASE_URL, data=dumps(payload), headers=headers)
-
-        if response.status_code == 200 or response.status_code == 201:
-            if 'id' in response.json():
-                platform_id = str(response.json()['id'])
-                platform_url = "https://smartcitizen.me/kits/" + platform_id
-                std_out(f'Device created with: \n{platform_url}', 'SUCCESS')
-                return response.json()
-            else:
-                std_out('Response does not contain id field')
-
-        std_out(f'Error while creating new device, platform returned {response.status_code}', 'ERROR')
-        return False
-
-    @staticmethod
-    def global_search(value = None, full = False):
-        """
-        Gets devices from Smart Citizen API based on basic search query values,
-        searching both Users and Devices at the same time.
-        Global search documentation: https://developer.smartcitizen.me/#global-search
-        Parameters
-        ----------
-            value: string
-                None
-                Query to fit
-                For null, not_null values, use 'null' or 'not_null'
-            full: bool
-                False
-                Returns a list with if False, or the whole dataframe if True
-        Returns
-        -------
-            A list of kit IDs that comply with the requirements, or the full df, depending on full.
-        """
-
-        API_BASE_URL = "https://api.smartcitizen.me/v0/search?q="
-
-        # Value check
-        if value is None: std_out(f'Value needs a value, {value} supplied', 'ERROR'); return None
-
-        url = API_BASE_URL  + f'{value}'
-
-        df = DataFrame()
-        isn = True
-        while isn:
-            try:
-                r = get(url)
-                # If status code OK, retrieve data
-                if r.status_code == 200 or r.status_code == 201:
-                    h = process_headers(r.headers)
-                    df = df.combine_first(DataFrame(r.json()).set_index('id'))
-                else:
-                    std_out('API reported {}'.format(r.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-            if 'next' in h:
-                if h['next'] == url: isn = False
-                elif h['next'] != url: url = h['next']
-            else:
-                isn = False
-
-        if full: return df
-        else: return list(df.index)
-
-    @staticmethod
-    def search_by_query(key = '', value = None, full = False):
-        """
-        Gets devices from Smart Citizen API based on ransack parameters
-        Basic query documentation: https://developer.smartcitizen.me/#basic-searching
-        Parameters
-        ----------
-            key: string
-                ''
-                Query key according to the basic query documentation. Some (not all) parameters are:
-                ['id', 'owner_id', 'name', 'description', 'mac_address', 'created_at',
-                'updated_at', 'kit_id', 'geohash', 'last_recorded_at', 'uuid', 'state',
-                'postprocessing_id', 'hardware_info']
-            value: string
-                None
-                Query to fit
-                For null, not_null values, use 'null' or 'not_null'
-            full: bool
-                False
-                Returns a list with if False, or the whole dataframe if True
-        Returns
-        -------
-            A list of kit IDs that comply with the requirements, or the full df, depending on full.
-        """
-
-        API_BASE_URL = "https://api.smartcitizen.me/v0/devices/"
-
-        # Value check
-        if value is None: std_out(f'Value needs a value, {value} supplied', 'ERROR'); return None
-
-        if value == 'null' or value == 'not_null':
-             url = API_BASE_URL  + f'?q[{key}_{value}]=1'
-        else:
-             url = API_BASE_URL  + f'?q[{key}]={value}'
-
-        df = DataFrame()
-        isn = True
-        while isn:
-            try:
-                r = get(url)
-                # If status code OK, retrieve data
-                if r.status_code == 200 or r.status_code == 201:
-                    h = process_headers(r.headers)
-                    df = df.combine_first(DataFrame(r.json()).set_index('id'))
-                else:
-                    std_out('API reported {}'.format(r.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-            if 'next' in h:
-                if h['next'] == url: isn = False
-                elif h['next'] != url: url = h['next']
-            else:
-                isn = False
-
-        if full: return df
-        else: return list(df.index)
-
-    @staticmethod
-    def get_world_map(min_date = None, max_date = None, city = None, within = None, tags = None, tag_method = 'any', full = False):
-        """
-        Gets devices from Smart Citizen API with certain requirements
-        Parameters
-        ----------
-            min_date: string, datetime-like object, optional
-                None
-                Minimum date to filter out the devices. Device started posted before min_date
-            max_date: string, datetime-like object, optional
-                None
-                Maximum date to filter out the devices. Device posted after max_date
-            city: string, optional
-                Empty string
-                City
-            within: tuple
-                Empty tuple
-                Gets the devices within a circle center on lat, long with a radius_meters
-                within = tuple(lat, long, radius_meters)
-            tags: list of strings
-                None
-                Tags for the device (system or user). Default system wide are: indoor, outdoor, online, and offline
-            tag_method: string
-                'any'
-                'any' or 'all'. Checks if 'all' the tags are to be included in the tags or it could be any
-            full: bool
-                False
-                Returns a list with if False, or the whole dataframe if True
-        Returns
-        -------
-            A list of kit IDs that comply with the requirements, or the full df, depending on full.
-            If no requirements are set, returns all of them
-        """
-
-        def is_within_circle(x, within):
-            if isnan(x['latitude']): return False
-            if isnan(x['longitude']): return False
-
-            return distance((within[0], within[1]), (x['latitude'], x['longitude'])).m<within[2]
-
-        world_map = get('https://api.smartcitizen.me/v0/devices/world_map')
-
-        df = DataFrame(world_map.json()).set_index('id')
-
-        # Filter out dates
-        if min_date is not None: df=df[(min_date > df['added_at'])]
-        if max_date is not None: df=df[(max_date < df['last_reading_at'])]
-
-        # Location
-        if city is not None: df=df[(df['city']==city)]
-        if within is not None:
-
-            df['within'] = df.apply(lambda x: is_within_circle(x, within), axis=1)
-            df=df[(df['within']==True)]
-
-        # Tags
-        if tags is not None:
-            if tag_method == 'any':
-                df['has_tags'] = df.apply(lambda x: any(tag in x['system_tags']+x['user_tags'] for tag in tags), axis=1)
-            elif tag_method == 'all':
-                df['has_tags'] = df.apply(lambda x: all(tag in x['system_tags']+x['user_tags'] for tag in tags), axis=1)
-            df=df[(df['has_tags']==True)]
-
-        if full: return df
-        else: return list(df.index)
-
-    def get_mac(self, update = False):
-        if self.mac is None or update:
-            std_out(f'Requesting MAC from API for device {self.id}')
-            # Get device
-            try:
-                deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
-
-                # If status code OK, retrieve data
-                if deviceR.status_code == 200 or deviceR.status_code == 201:
-                    if 'hardware_info' in deviceR.json().keys(): self.mac = deviceR.json()['hardware_info']['mac']
-                    std_out ('Device {} is has this MAC {}'.format(self.id, self.mac))
-                else:
-                    std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-        return self.mac
-
-    def get_device_json(self, update = False):
-        if self.devicejson is None or update:
-            try:
-                deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
-                if deviceR.status_code == 429:
-                    std_out('API reported {}. Retrying once'.format(deviceR.status_code),
-                            'WARNING')
-                    sleep(30)
-                    deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
-
-                if deviceR.status_code == 200 or deviceR.status_code == 201:
-                    self.devicejson = deviceR.json()
-                else:
-                    std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-        return self.devicejson
-
-    def get_device_description(self, update = False):
-        if self.get_device_json(update) is not None:
-            return self.get_device_json()['kit']['description']
-        return None
-
-    def get_kit_ID(self, update = False):
-
-        if self.kit_id is None or update:
-            if self.get_device_json(update) is not None:
-                self.kit_id = self.devicejson['kit']['id']
-
-        return self.kit_id
-
-    def post_kit_ID(self):
-        '''
-            Posts kit id to platform
-        '''
-
-        if 'SC_ADMIN_BEARER' not in environ:
-            std_out('Cannot post without Auth Admin Bearer', 'ERROR')
-            return
-
-        headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'], 'Content-type': 'application/json'}
-
-        if self.kit_id is not None:
-
-            payload = {'kit_id': self.kit_id}
-
-            payload_json = dumps(payload)
-            response = patch(f'{self.API_BASE_URL}{self.id}',
-                        data = payload_json, headers = headers)
-
-            if response.status_code == 200 or response.status_code == 201:
-                std_out(f'Kit ID for device {self.id} was updated to {self.kit_id}', 'SUCCESS')
-                return True
-
-        std_out(f'Problem while updating kit ID for device {self.id}')
-
-        return False
-
-    def get_device_last_reading(self, update = False):
-
-        if self.last_reading_at is None or update:
-            if self.get_device_json(update) is not None and self.get_device_json(update)['state'] != 'never_published':
-                self.last_reading_at = localise_date(self.devicejson['last_reading_at'], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-
-        std_out ('Device {} has last reading at {}'.format(self.id, self.last_reading_at))
-
-        return self.last_reading_at
-
-    def get_device_added_at(self, update = False):
-
-        if self.added_at is None or update:
-            if self.get_device_json(update) is not None:
-                self.added_at = localise_date(self.devicejson['added_at'], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-
-        std_out ('Device {} was added at {}'.format(self.id, self.added_at))
-
-        return self.added_at
-
-    def get_device_postprocessing(self, update = False):
-
-        if self.postprocessing is None or update:
-            if self.get_device_json(update) is not None:
-                self.postprocessing = self.devicejson['postprocessing']
-
-                if self.postprocessing is not None:
-                    # Check the url in hardware
-                    if 'hardware_url' in self.postprocessing:
-                        urls = url_checker(self.postprocessing['hardware_url'])
-                        # If URL is empty, try prepending base url from config
-                        if not urls:
-                            tentative_url = f"{config._base_postprocessing_url}hardware/{self.postprocessing['hardware_url']}.{config._default_file_type}"
-                        else:
-                            if len(urls)>1: std_out('URLs for postprocessing recipe are more than one, trying first', 'WARNING')
-                            tentative_url = urls[0]
-
-                        self.postprocessing['hardware_url'] = tentative_url
-
-                    std_out ('Device {} has postprocessing information:\n{}'.format(self.id, self.postprocessing))
-                else:
-                    std_out (f'Device {self.id} has no postprocessing information')
-
-        return self.postprocessing
-
-    def get_device_timezone(self, update = False):
-
-        if self.timezone is None or update:
-            latitude, longitude = self.get_device_lat_long(update)
-            # Localize it
-
-            if latitude is not None and longitude is not None:
-                # self.timezone = tz_where.tzNameAt(latitude, longitude, forceTZ=True)
-                self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
-        std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
-
-        return self.timezone
-
-    def get_device_lat_long(self, update = False):
-
-        if self.lat is None or self.long is None or update:
-            if self.get_device_json(update) is not None:
-                latidude = longitude = None
-                if 'location' in self.devicejson.keys():
-                    latitude, longitude = self.devicejson['location']['latitude'], self.devicejson['location']['longitude']
-                elif 'data' in self.devicejson.keys():
-                    if 'location' in self.devicejson['data'].keys():
-                        latitude, longitude = self.devicejson['data']['location']['latitude'], self.devicejson['data']['location']['longitude']
-
-                self.lat = latitude
-                self.long = longitude
-
-        std_out ('Device {} is located at {}, {}'.format(self.id, self.lat, self.long))
-
-        return (self.lat, self.long)
-
-    def get_device_alt(self, update = False):
-
-        if self.lat is None or self.long is None:
-            self.get_device_lat_long(update)
-
-        if self.alt is None or update:
-            self.alt = get_elevation(_lat = self.lat, _long = self.long)
-
-        std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
-
-        return self.alt
-
-    def get_device_sensors(self, update = False):
-
-        if self.sensors is None or update:
-            if self.get_device_json(update) is not None:
-                # Get available sensors in platform
-                sensors = self.devicejson['data']['sensors']
-
-                # Put the ids and the names in lists
-                self.sensors = dict()
-                for sensor in sensors:
-                    for key in config.names['sc_sensor_names']:
-                        if str(config.names['sc_sensor_names'][key]['id']) == str(sensor['id']):
-                            # IDs are unique
-                            if key in config._sc_ignore_keys: continue
-                            self.sensors[sensor['id']] = key
-
-        return self.sensors
-
-    def convert_rollup(self, frequency):
-        # Convert frequency from pandas to API's
-        for index, letter in enumerate(frequency):
-            try:
-                aux = int(letter)
-            except:
-                index_first = index
-                letter_first = letter
-                rollup_value = frequency[:index_first]
-                frequency_unit = frequency[index_first:]
-                break
-
-        for item in config._freq_conv_lut:
-            if item[1] == frequency_unit:
-                rollup_unit = item[0]
-                break
-
-        rollup = rollup_value + rollup_unit
-        return rollup
-
-    def get_device_data(self, min_date = None, max_date = None, frequency = '1Min', clean_na = None, resample = True):
-
-        if 'SC_ADMIN_BEARER' in environ:
-            std_out('Admin Bearer found, using it', 'SUCCESS')
-
-            headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER']}
-        else:
-            headers = None
-            std_out('Admin Bearer not found', 'WARNING')
-
-        std_out(f'Requesting data from SC API')
-        std_out(f'Device ID: {self.id}')
-
-        rollup = self.convert_rollup(frequency)
-        std_out(f'Using rollup: {rollup}')
-
-        # Make sure we have the everything we need beforehand
-        self.get_device_sensors()
-        self.get_device_timezone()
-        self.get_device_last_reading()
-        self.get_device_added_at()
-        self.get_kit_ID()
-
-        if self.timezone is None:
-            std_out('Device does not have timezone set, skipping', 'WARNING')
-            return None
-
-        # Check start date and end date
-        # Converting to UTC by passing None
-        # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.dt.tz_convert.html
-        if min_date is not None:
-            min_date = localise_date(to_datetime(min_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
-            std_out (f'Min Date: {min_date}')
-        else:
-            min_date = localise_date(to_datetime('2001-01-01'), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
-            std_out(f"No min_date specified")
-
-        if max_date is not None:
-            max_date = localise_date(to_datetime(max_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
-            std_out (f'Max Date: {max_date}')
-
-        # Trim based on actual data available
-        if min_date is not None and self.last_reading_at is not None:
-            if min_date > self.last_reading_at:
-                std_out(f'Device request would yield empty data (min_date). Returning', 'WARNING')
-                return None
-
-        if max_date is not None and self.added_at is not None:
-            if max_date < self.added_at:
-                std_out(f'Device request would yield empty data (max_date). Returning', 'WARNING')
-                return None
-
-        if max_date is not None and self.last_reading_at is not None:
-            if max_date > self.last_reading_at:
-                std_out('Trimming max_date to last reading', 'WARNING')
-                max_date = self.last_reading_at
-
-        # Print stuff
-        std_out('Kit ID: {}'.format(self.kit_id))
-        std_out(f'Device timezone: {self.timezone}')
-        if not self.sensors.keys():
-            std_out(f'Device is empty')
-            return None
-        else: std_out(f'Sensor IDs: {list(self.sensors.keys())}')
-
-        df = DataFrame()
-        std_out(f'Requesting from {min_date} to {max_date}')
-
-        # Get devices in the sensor first
-        for sensor_id in self.sensors.keys():
-
-            # Request sensor per ID
-            request = self.API_BASE_URL + '{}/readings?'.format(self.id)
-
-            if min_date is not None: request += f'from={min_date}'
-            if max_date is not None: request += f'&to={max_date}'
-
-            request += f'&rollup={rollup}'
-            request += f'&sensor_id={sensor_id}'
-            request += '&function=avg'
-
-            # Make request
-            response = get(request, headers = headers)
-
-            # Retry once in case of 429 after 30s
-            if response.status_code == 429:
-                std_out('Too many requests, waiting for 1 more retry', 'WARNING')
-                sleep (30)
-                response = get(request, headers = headers)
-
-            flag_error = False
-            try:
-                sensorjson = response.json()
-            except:
-                std_out(f'Problem with json data from API, {response.status_code}', 'ERROR')
-                flag_error = True
-                pass
-                continue
-
-            if 'readings' not in sensorjson.keys():
-                std_out(f'No readings key in request for sensor: {sensor_id} ({self.sensors[sensor_id]})', 'ERROR')
-                flag_error = True
-                continue
-
-            elif sensorjson['readings'] == []:
-                std_out(f'No data in request for sensor: {sensor_id} ({self.sensors[sensor_id]})', 'WARNING')
-                flag_error = True
-                continue
-
-            if flag_error: continue
-
-            try:
-                dfsensor = DataFrame(sensorjson['readings']).set_index(0)
-                dfsensor.columns = [self.sensors[sensor_id]]
-                dfsensor.index = localise_date(dfsensor.index, self.timezone)
-                dfsensor.sort_index(inplace=True)
-                dfsensor = dfsensor[~dfsensor.index.duplicated(keep='first')]
-
-                # Drop unnecessary columns
-                dfsensor.drop([i for i in dfsensor.columns if 'Unnamed' in i], axis=1, inplace=True)
-                # Check for weird things in the data
-                dfsensor = dfsensor.astype(float, errors='ignore')
-                # dfsensor = dfsensor.apply(to_numeric, errors='coerce')
-                # Resample
-                if (resample):
-                    dfsensor = dfsensor.resample(frequency).mean()
-                df = df.combine_first(dfsensor)
-            except:
-                print_exc()
-                std_out('Problem with sensor data from API', 'ERROR')
-                flag_error = True
-                pass
-                continue
-
-            try:
-                df = df.reindex(df.index.rename('TIME'))
-                df = clean(df, clean_na, how = 'all')
-                self.data = df
-
-            except:
-                std_out('Problem closing up the API dataframe', 'ERROR')
-                pass
-                return None
-
-        if flag_error == False: std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
-        return self.data
-
-    def post_device_data(self, clean_na = 'drop', chunk_size = 500):
-        '''
-            POST self.data in the SmartCitizen API
-            Parameters
-            ----------
-                clean_na: string, optional
-                    'drop'
-                    'drop', 'fill'
-                chunk_size: integer
-                    chunk size to split resulting pandas DataFrame for posting readings
-            Returns
-            -------
-                True if the data was posted succesfully
-        '''
-        if self.data is None:
-            std_out('No data to post, ignoring', 'ERROR')
-            return False
-
-        if 'SC_BEARER' not in environ:
-            std_out('Cannot post without Auth Bearer', 'ERROR')
-            return False
-
-        if 'SC_ADMIN_BEARER' in environ:
-            std_out('Using admin Bearer')
-            bearer = environ['SC_ADMIN_BEARER']
-        else:
-            bearer = environ['SC_BEARER']
-
-        headers = {'Authorization':'Bearer ' + bearer, 'Content-type': 'application/json'}
-        post_ok = True
-
-        for sensor_id in self.sensors:
-            df = DataFrame(self.data[self.sensors[sensor]]).copy()
-            post_ok &= self.post_data_to_device(df, clean_na = clean_na, chunk_size = chunk_size)
-
-        return post_ok
-
-    def post_data_to_device(self, df, clean_na = 'drop', chunk_size = 500, dry_run = False, max_retries = 2):
-        '''
-            POST external pandas.DataFrame to the SmartCitizen API
-            Parameters
-            ----------
-                df: pandas DataFrame
-                    Contains data in a DataFrame format.
-                    Data is posted using the column names of the dataframe
-                    Data is posted in UTC TZ so dataframe needs to have located
-                    timestamp
-                clean_na: string, optional
-                    'drop'
-                    'drop', 'fill'
-                chunk_size: integer
-                    chunk size to split resulting pandas DataFrame for posting readings
-                dry_run: boolean
-                    False
-                    Post the payload to the API or just return it
-                max_retries: int
-                    2
-                    Maximum number of retries per chunk
-            Returns
-            -------
-                True if the data was posted succesfully
-        '''
-        if 'SC_BEARER' not in environ:
-            std_out('Cannot post without Auth Bearer', 'ERROR')
-            return False
-
-        if 'SC_ADMIN_BEARER' in environ:
-            std_out('Using admin Bearer')
-            bearer = environ['SC_ADMIN_BEARER']
-        else:
-            bearer = environ['SC_BEARER']
-
-        headers = {'Authorization':'Bearer ' + bearer, 'Content-type': 'application/json'}
-
-        # Clean df of nans
-        df = clean(df, clean_na, how = 'all')
-        std_out(f'Posting columns to {self.API_BASE_URL}')
-        std_out(f'{list(df.columns)}')
-        df.index.name = 'recorded_at'
-
-        # Split the dataframe in chunks
-        std_out(f'Splitting post in chunks of size {chunk_size}')
-        chunked_dfs = [df[i:i+chunk_size] for i in range(0, df.shape[0], chunk_size)]
-
-        for i in trange(len(chunked_dfs), file=sys.stdout,
-                        desc=f"Posting data for {self.id}..."):
-
-            chunk = chunked_dfs[i].copy()
-
-            # Prepare json post
-            payload = {"data":[]}
-            for item in chunk.index:
-                payload["data"].append(
-                    {
-                        "recorded_at": localise_date(item, 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ'),
-                        "sensors": [{
-                            "id": column,
-                            "value": chunk.loc[item, column]
-                        } for column in chunk.columns if not isnan(chunk.loc[item, column])]
-                    }
-                )
-
-            if dry_run:
-                std_out(f'Dry run request to: {self.API_BASE_URL}{self.id}/readings for chunk ({i+1}/{len(chunked_dfs)})')
-                return dumps(payload, indent = 2, cls = NpEncoder)
-
-            post_ok = False
-            retries = 0
-
-            while post_ok == False and retries < max_retries:
-                response = post(f'{self.API_BASE_URL}{self.id}/readings',
-                            data = dumps(payload, cls = NpEncoder), headers = headers)
-
-                if response.status_code == 200 or response.status_code == 201:
-                    post_ok = True
-                    break
-                else:
-                    retries += 1
-                    std_out (f'Chunk ({i+1}/{len(chunked_dfs)}) post failed. \
-                           API responded {response.status_code}.\
-                            Retrying ({retries}/{max_retries}', 'WARNING')
-
-            if (not post_ok) or (retries == max_retries):
-                std_out (f'Chunk ({i+1}/{len(chunked_dfs)}) post failed. \
-                       API responded {response.status_code}.\
-                        Reached max_retries', 'ERROR')
-                return False
-
-        return True
-
-    def patch_postprocessing(self, dry_run = False):
-        '''
-            POST postprocessing info into the device in the SmartCitizen API
-            Updates all the post info. Changes need to be made info the keys of the postprocessing outside of here
-
-            # Example postprocessing:
-            # {
-            #   "blueprint_url": "https://github.com/fablabbcn/smartcitizen-data/blob/master/blueprints/sc_21_station_module.json",
-            #   "hardware_url": "https://raw.githubusercontent.com/fablabbcn/smartcitizen-data/master/hardware/SCAS210001.json",
-            #   "latest_postprocessing": "2020-10-29T08:35:23Z"
-            # }
-        '''
-
-        if 'SC_ADMIN_BEARER' not in environ:
-            std_out('Cannot post without Admin Auth Bearer', 'ERROR')
-            return
-
-        headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'],
-                   'Content-type': 'application/json'}
-
-        post = {"postprocessing_attributes": self.postprocessing}
-        post_json = dumps(post)
-
-        if dry_run:
-            std_out(f'Dry run request to: {self.API_BASE_URL}{self.id}/')
-            return dumps(post_json, indent = 2)
-
-        std_out(f'Posting postprocessing_attributes:\n {post_json}')
-        response = patch(f'{self.API_BASE_URL}{self.id}/',
-                         data = post_json, headers = headers)
-
-        if response.status_code == 200 or response.status_code == 201:
-            std_out(f"Postprocessing posted", "SUCCESS")
-            return True
-        else:
-            std_out(f"API responded with {response.status_code}")
-
-        return False
-
-class MuvApiDevice:
-
-    API_BASE_URL='https://data.waag.org/api/muv/'
-
-    def __init__ (self, did):
-        self.id = did
-        self.timezone = None
-        self.data = None
-        self.sensors = None
-
-    def get_device_timezone(self):
-        self.timezone = 'Europe/Madrid'
-        return self.timezone
-
-    def get_device_sensors(self):
-        if self.sensors is None:
-            self.sensors = dict()
-            for key in config.blueprints:
-                if 'muv' not in key: continue
-                if 'sensors' in config.blueprints[key]:
-                    for sensor_name in config.blueprints[key]['sensors'].keys():
-                        # IDs are unique
-                        self.sensors[config.blueprints[key]['sensors'][sensor_name]['id']] = sensor_name
-        return self.sensors
-
-    def get_device_data(self, min_date = None, max_date = None, frequency = '3Min', clean_na = None, resample = True):
-
-        if min_date is not None: days_ago = (to_datetime(date.today())-to_datetime(min_date)).days
-        else: days_ago = 365 # One year of data
-
-        std_out(f'Requesting data from MUV API')
-        std_out(f'Device ID: {self.id}')
-        self.get_device_timezone()
-        self.get_device_sensors()
-
-        # Get devices
-        try:
-            if days_ago == -1: url = f'{self.API_BASE_URL}getSensorData?sensor_id={self.id}'
-            else: url = f'{self.API_BASE_URL}getSensorData?sensor_id={self.id}&days={days_ago}'
-            df = DataFrame(get(url).json())
-        except:
-            print_exc()
-            std_out('Failed sensor request request. Probably no connection', 'ERROR')
-            pass
-            return None
-
-        try:
-            # Rename columns
-            df.rename(columns = self.sensors, inplace = True)
-            df = df.set_index('time')
-
-            df.index = localise_date(df.index, self.timezone)
-            df = df[~df.index.duplicated(keep='first')]
-            # Drop unnecessary columns
-            df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
-            df.drop('id', axis=1, inplace=True)
-            # Check for weird things in the data
-            df = df.apply(to_numeric, errors='coerce')
-            # # Resample
-            if (resample):
-                df = df.resample(frequency).mean()
-            df = df.reindex(df.index.rename('TIME'))
-
-            df = clean(df, clean_na, how = 'all')
-
-            self.data = df
-
-        except:
-            print_exc()
-            std_out('Problem closing up the API dataframe', 'ERROR')
-            pass
-            return None
-
-        std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
-        return self.data
-
-class DadesObertesApiDevice:
-
-    API_BASE_URL="https://analisi.transparenciacatalunya.cat/resource/tasf-thgu.json"
-
-    def __init__ (self, did = None, within = None):
-        if did is None and within is None:
-            std_out('Specify either station id (=codi_eoi) or within (=(lat, long, radius_meters))')
-            return
-
-        if did is not None: self.id = did
-        if within is not None: self.id = self.get_id_from_within(within)
-
-        self.timezone = None
-        self.data = None
-        self.sensors = None
-        self.devicejson = None
-        self.lat = None
-        self.long = None
-        self.alt = None
-        self.timezone = None
-
-    @staticmethod
-    def get_world_map(city = None, within = None, station_type = None, area_type = None, full = False):
-        """
-        Gets devices from Dades Obertes API with certain requirements
-        Parameters
-        ----------
-            city: string, optional
-                Empty string
-                City
-            within: tuple
-                Empty tuple
-                Gets the devices within a circle center on lat, long with a radius_meters
-                within = tuple(lat, long, radius_meters)
-            station_type: string
-                None
-                Type of station, to choose from: 'background', nan or 'traffic'
-            area_type: string
-                None
-                Type of area, to choose from:  nan, 'peri-urban', 'rural', 'suburban', 'urban'
-            full: bool
-                False
-                Return full dataframe or not
-        Returns
-        -------
-            A list of eoi codes that comply with the requirements. If no requirements are set, returns all of them
-        """
-        def is_within_circle(x, within):
-            if isnan(x['latitud']): return False
-            if isnan(x['longitud']): return False
-
-            return distance(location_A=(within[0], within[1]), location_B=(x['latitude'], x['longitude'])).m < within[2]
-
-        world_map = get("https://analisi.transparenciacatalunya.cat/resource/tasf-thgu.json")
-        df = read_json(StringIO(world_map.content.decode('utf-8'))).set_index('codi_eoi')
-
-        # Location
-        if city is not None: df=df[(df['municipi']==city)]
-        if within is not None:
-
-            df['within'] = df.apply(lambda x: is_within_circle(x, within), axis=1)
-            df=df[(df['within']==True)]
-
-        # Station type
-        if station_type is not None: df=df[(df['tipus_estacio']==station_type)]
-        # Area type
-        if area_type is not None: df=df[(df['area_urbana']==area_type)]
-
-        if full: return df
-        return list(set(list(df.index)))
-
-    def get_id_from_within(self, within):
-        '''
-            Gets the stations within a radius in meters.
-            within = tuple(lat, long, radius_meters)
-        '''
-        request = self.API_BASE_URL
-        request += f'$where=within_circle(geocoded_column,{within[0]},{within[1]},{within[2]})'
-
-        try:
-            s = get(request)
-        except:
-            std_out('Problem with request from API', 'ERROR')
-            return None
-
-        if s.status_code == 200 or s.status_code == 201:
-            df = read_json(StringIO(s.content.decode('utf-8')))
-        else:
-            std_out('API reported {}'.format(s.status_code), 'ERROR')
-            return None
-
-        if 'codi_eoi' in df.columns:
-            ids = list(set(df.codi_eoi.values))
-            if ids == []: std_out('No stations within range', 'ERROR')
-            elif len(ids) > 1:
-                for ptid in ids:
-                    municipi = next(iter(set(df[df.codi_eoi==ptid].municipi.values)))
-                    nom_estacio = next(iter(set(df[df.codi_eoi==ptid].nom_estacio.values)))
-                    area_urbana = next(iter(set(df[df.codi_eoi==ptid].area_urbana.values)))
-                    tipus_estacio = next(iter(set(df[df.codi_eoi==ptid].tipus_estacio.values)))
-
-                    std_out(f'{ids.index(ptid)+1} /- {ptid} --- {municipi} - {nom_estacio} - Type: {area_urbana} - {tipus_estacio}')
-
-                wptid = int(input('Multiple stations found, please select one: ')) - 1
-
-                devid = ids[wptid]
-                std_out(f'Selected station in {next(iter(set(df[df.codi_eoi==devid].municipi.values)))} with codi_eoi={devid}')
-            else:
-                devid = ids[0]
-                municipi = next(iter(set(df[df.codi_eoi==devid].municipi.values)))
-                nom_estacio = next(iter(set(df[df.codi_eoi==devid].nom_estacio.values)))
-                area_urbana = next(iter(set(df[df.codi_eoi==devid].area_urbana.values)))
-                tipus_estacio = next(iter(set(df[df.codi_eoi==devid].tipus_estacio.values)))
-                std_out(f'Found station in {next(iter(set(df[df.codi_eoi==devid].municipi.values)))} with codi_eoi={devid}')
-                std_out(f'Found station in {municipi} - {nom_estacio} - {devid} - Type: {area_urbana} - {tipus_estacio}')
-
-        else:
-            std_out('Data is empty', 'ERROR')
-            return None
-
-        return devid
-
-    def get_device_sensors(self):
-
-        if self.sensors is None:
-            if self.get_device_json() is not None:
-                # Get available sensors
-                sensors = list(set(self.devicejson.contaminant))
-
-                # Put the ids and the names in lists
-                self.sensors = dict()
-                for sensor in sensors:
-                    for key in config.blueprints:
-                        if not search("csic_station",key): continue
-                        if 'sensors' in config.blueprints[key]:
-                            for sensor_name in config.blueprints[key]['sensors'].keys():
-                                if config.blueprints[key]['sensors'][sensor_name]['id'] == str(sensor):
-                                    # IDs are unique
-                                    self.sensors[sensor] = sensor_name
-
-        return self.sensors
-
-    def get_device_json(self):
-
-        if self.devicejson is None:
-            try:
-                s = get(self.API_BASE_URL + f'/?codi_eoi={self.id}')
-                if s.status_code == 200 or s.status_code == 201:
-                    self.devicejson = read_json(StringIO(s.content.decode('utf-8')))
-                else:
-                    std_out('API reported {}'.format(s.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-        return self.devicejson
-
-    def get_device_timezone(self):
-
-        if self.timezone is None:
-            latitude, longitude = self.get_device_lat_long()
-            # Localize it
-            # self.timezone = tz_where.tzNameAt(latitude, longitude)
-            self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
-
-        std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
-
-        return self.timezone
-
-    def get_device_alt(self, update = False):
-
-        if self.lat is None or self.long is None:
-            self.get_device_lat_long(update)
-
-        if self.alt is None or update:
-            self.alt = get_elevation(_lat = self.lat, _long = self.long)
-
-        std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
-
-        return self.alt
-
-    def get_device_lat_long(self):
-
-        if self.lat is None or self.long is None:
-            if self.get_device_json() is not None:
-                latitude = longitude = None
-                if 'latitud' in self.devicejson.columns:
-                    latitude = next(iter(set(self.devicejson.latitud)))
-                    longitude = next(iter(set(self.devicejson.longitud)))
-
-                self.lat = latitude
-                self.long = longitude
-
-            std_out ('Device {} is located at {}, {}'.format(self.id, latitude, longitude))
-
-        return (self.lat, self.long)
-
-    def get_device_data(self, min_date = None, max_date = None, frequency = '1H', clean_na = None, resample = True):
-        '''
-        Based on code snippet from Marc Roig:
-        # I2CAT RESEARCH CENTER - BARCELONA - MARC ROIG (marcroig@i2cat.net)
-        '''
-
-        std_out(f'Requesting data from Dades Obertes API')
-        std_out(f'Device ID: {self.id}')
-        self.get_device_sensors()
-        self.get_device_timezone()
-
-        request = self.API_BASE_URL
-        request += f'/?codi_eoi={self.id}'
-
-        if min_date is not None and max_date is not None:
-            request += "&$where=data between " + to_datetime(min_date).strftime("'%Y-%m-%dT%H:%M:%S'") \
-                    + " and " + to_datetime(max_date).strftime("'%Y-%m-%dT%H:%M:%S'")
-        elif min_date is not None:
-            request += "&$where=data >= " + to_datetime(min_date).strftime("'%Y-%m-%dT%H:%M:%S'")
-        elif max_date is not None:
-            request += "&$where=data < " + to_datetime(max_date).strftime("'%Y-%m-%dT%H:%M:%S'")
-
-        try:
-            s = get(request)
-        except:
-            print_exc()
-            std_out('Problem with sensor data from API', 'ERROR')
-            pass
-            return None
-
-        if s.status_code == 200 or s.status_code == 201:
-            df = read_json(StringIO(s.content.decode('utf-8')))
-        else:
-            std_out('API reported {}'.format(s.status_code), 'ERROR')
-            pass
-            return None
-
-        # Filter columns
-        measures = ['h0' + str(i) for i in range(1,10)]
-        measures += ['h' + str(i) for i in range(10,25)]
-        # validations = ['v0' + str(i) for i in range(1,10)]
-        # validations  += ['v' + str(i) for i in range(10,25)]
-        new_measures_names = list(range(1,25))
-
-        columns = ['contaminant', 'data'] + measures# + validations
-        try:
-            df_subset = df[columns]
-            df_subset.columns  = ['contaminant', 'date'] + new_measures_names
-        except:
-            print_exc()
-            std_out('Problem while filtering columns', 'Error')
-            return None
-        else:
-            std_out('Successful filtering', 'SUCCESS')
-
-        # Pivot
-        try:
-            df = DataFrame([])
-            for contaminant in self.sensors.keys():
-                if contaminant not in df_subset['contaminant'].values:
-                    std_out(f'{contaminant} not in columns. Skipping', 'WARNING')
-                    continue
-                df_temp= df_subset.loc[df_subset['contaminant']==contaminant].drop('contaminant', 1).set_index('date').unstack().reset_index()
-                df_temp.columns = ['hours', 'date', contaminant]
-                df_temp['date'] = to_datetime(df_temp['date'])
-                timestamp_lambda = lambda x: x['date'] + DateOffset(hours=int(x['hours']))
-                df_temp['date'] = df_temp.apply( timestamp_lambda, axis=1)
-                df_temp = df_temp.set_index('date')
-                df[contaminant] = df_temp[contaminant]
-        except:
-            # print_exc()
-            std_out('Problem while filtering columns', 'Error')
-            pass
-            return None
-        else:
-            std_out('Successful pivoting', 'SUCCESS')
-
-        df.index = to_datetime(df.index).tz_localize('UTC').tz_convert(self.timezone)
-        df.sort_index(inplace=True)
-
-        # Rename
-        try:
-            df.rename(columns=self.sensors, inplace=True)
-        except:
-            # print_exc()
-            std_out('Problem while renaming columns', 'Error')
-            pass
-            return None
-        else:
-            std_out('Successful renaming', 'SUCCESS')
-
-        # Clean
-        df = df[~df.index.duplicated(keep='first')]
-        # Drop unnecessary columns
-        df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
-        # Check for weird things in the data
-        df = df.apply(to_numeric, errors='coerce')
-        # Resample
-        if (resample):
-            df = df.resample(frequency).mean()
-
-        try:
-            df = df.reindex(df.index.rename('TIME'))
-            df = clean(df, clean_na, how = 'all')
-            self.data = df
-        except:
-            std_out('Problem closing up the API dataframe', 'ERROR')
-            pass
-            return None
-
-        std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
-        return self.data
-
-class NiluApiDevice(object):
-    """docstring for IflinkDevice"""
-    API_BASE_URL='https://sensors.nilu.no/api/'
-    API_CONNECTOR='sensors.nilu.no'
-
-    # Docs
-    # https://sensors.nilu.no/api/doc#configure-sensor-schema
-    # https://sensors.nilu.no/api/doc#push--sensor-data-by-id
-
-    def __init__ (self, did):
-
-        self.id = did
-        self.timezone = None
-        self.lat = None
-        self.long = None
-        self.alt = None
-        self.data = None
-        self.sensors = None
-        self.devicejson = None
-        self.last_reading_at = None
-        self.added_at = None
-        self._api_url = self.API_BASE_URL + f'sensors/{self.id}'
-
-    @property
-    def api_url(self):
-        return self._api_url
-
-    @staticmethod
-    # def new_device(name, description = '', resolution = '1Min', epsg = config._epsg, enabled = True, location = None, sensors = None, dry_run = False):
-    def new_device(name, location = {}, dry_run = False, **kwargs):
-
-        '''
-            Configures the device as a new sensor schema.
-            This is a one-time configuration and shouldn't be necessary in a recursive way.
-            More information at: https://sensors.nilu.no/api/doc#configure-sensor-schema
-
-            Parameters
-            ----------
-                name: string
-                    Device name
-                location: dict
-                    None
-                    sensor location. If sensor is moving (i.e. position is not fixed),
-                    then location must explicitly be set to an empty object: {} when configured. Also see this section.
-                    location = {
-                                'longitude': longitude (double) – sensor east-west position,
-                                'latitude': latitude (double) – sensor north-south position,
-                                'altitude': altitude (double) – sensor height above sea level
-                                }
-                dry_run: boolean
-                    False
-                    Post the payload to the API or just return it
-                **kwargs
-                ------
-                description: string, optional
-                    ''
-                    sensor description
-                frequency: string, optional
-                    '1Min'
-                    pandas formatted frequency
-                epsg: int, optional
-                    4326
-                    SRS EPSG code. Defaults to 4326 (WGS84). More info https://spatialreference.org/
-                enabled: boolean, optional
-                    True
-                    flag indicating if sensor is enabled for data transfer
-
-                sensors: dict()
-                    Dictionary containing necessary information of the sensors to be stored. scdata format:
-                    {
-                        'SHORT_NAME': {
-                                        'desc': 'Channel description',
-                                        'id': 'sensor SC platform id',
-                                        'units': 'sensor_recording_units'
-                                    },
-                        ...
-                    }
-                ------
-
-            Returns
-            -------
-                If dry_run, prints out a dict containing the payload and
-                returns False
-                If not, either False in case of error or a
-                dictionary containing:
-                    sensorid (int) – sensor identifier
-                    message (string) – HTTP status text
-                    http-status-code (int) – HTTP status code
-                    atom (string) – atom URL to sensor
-        '''
-
-        API_BASE_URL='https://sensors.nilu.no/api/'
-        API_CONNECTOR='nilu'
-
-        if API_CONNECTOR not in config.connectors:
-            std_out(f'No connector for {API_CONNECTOR}', 'ERROR')
-            return False
-
-        if 'NILU_BEARER' not in environ:
-            std_out('Cannot configure without Auth Bearer', 'ERROR')
-            return False
-
-        headers = {'Authorization':'Bearer ' + environ['NILU_BEARER'], 'Content-type': 'application/json'}
-
-        if name is None:
-            std_out('Need a name to create a new sensor', 'ERROR')
-            return False
-        std_out (f'Configuring IFLINK device named {name}')
-
-        # Verify inputs
-        flag_error = False
-
-        dft_input_params = ['epsg', 'description', 'frequency', 'enabled', 'sensors']
-        if any([x not in kwargs for x in dft_input_params]):
-            std_out('Input params not ok for NiluApiDevice', 'ERROR')
-            return False
-
-        # EPSG int type
-        try:
-            epsg = int(kwargs['epsg'])
-        except:
-            std_out('Could not convert epsg to int', 'ERROR')
-            flag_error = True
-            pass
-
-        # Resolution in seconds
-        if not flag_error:
-            try:
-                resolution_seconds = to_timedelta(kwargs['frequency']).seconds
-            except:
-                std_out('Could not convert resolution to seconds', 'ERROR')
-                flag_error = True
-                pass
-
-        # Location
-        if not flag_error:
-            try:
-                location['longitude']
-                location['latitude']
-                location['altitude']
-            except KeyError:
-                std_out('Need latitude, longitude and altitude in location dict', 'ERROR')
-                flag_error = True
-                pass
-
-        if flag_error: return False
-
-        # Construct payload
-        payload = {
-            "name": name,
-            "description": kwargs['description'],
-            "resolution": resolution_seconds,
-            "srs": {
-                "epsg": epsg
-            },
-            "enabled": kwargs['enabled']
-        }
-
-        payload['location'] = location
-
-        parameters = []
-        components = []
-
-        # Construct
-        sensors = kwargs['sensors']
-        for sensor in sensors.keys():
-            # Check if it's in the configured connectors
-            _sid = str(sensors[sensor]['id'])
-
-            if _sid is None:
-                std_out(f"Sensor {sensor} id is None. Ignoring", "WARNING")
-                return False
-
-            if _sid not in config.connectors[API_CONNECTOR]['sensors']:
-                if config._strict:
-                    std_out(f"Sensor {sensor} not found in connectors list", "ERROR")
-                    return False
-                std_out(f"Sensor {sensor} not found in connectors list", "WARNING")
-                continue
-
-            units = sensors[sensor]['units']
-
-            _pjson = {
-                "name": sensor,
-                "type": "double",
-                "doc": f"{sensors[sensor]['desc']} in {units}"
-            }
-
-            _cjson = {
-                "componentid": config.connectors[API_CONNECTOR]['sensors'][_sid]['id'],
-                "unitid": config.connectors[API_CONNECTOR]['sensors'][_sid]['unitid'],
-                "binding-path": f"/{sensor}",
-                "level": config.connectors[API_CONNECTOR]['sensors'][_sid]['level']
-            }
-
-            parameters.append(_pjson)
-            components.append(_cjson)
-        # Add timestamp as long
-        parameters.append({
-            'name': 'date',
-            'type': 'long',
-            'doc': 'Date of measurement'
-            })
-
-        # Add the converter (we need to push as input-format)
-        converters = [{
-            "input-type": "string",
-            "output-type": "StringEpochTime",
-            "target-path": "/date",
-            "input-args": {
-                "input-format": "yyyy-MM-ddTHH:mm:ssZ"
-            }
-        }]
-
-        mapping = [{
-            "name": "Timestamp",
-            "target-path": "/date"
-        }]
-
-        payload['parameters'] = parameters
-        payload['components'] = components
-        payload['converters'] = converters
-        payload['mapping'] = mapping
-
-        if dry_run:
-            std_out(f'Dry run request to: {API_BASE_URL}sensors/configure')
-            print(dumps(payload, indent = 2))
-            return False
-
-        response = post(f'{API_BASE_URL}sensors/configure',
-                        data = dumps(payload), headers = headers)
-
-
-        if response.status_code == 200 or response.status_code == 201:
-            if 'sensorid' in response.json():
-                platform_id = str(response.json()['sensorid'])
-                platform_url = "https://sensors.nilu.no/api/sensors/" + platform_id
-                std_out(f'Device created with: \n{platform_url}', 'SUCCESS')
-                return response.json()
-            else:
-                std_out('Response does not contain sensorid field')
-        else:
-            std_out(f'{API_BASE_URL} reported {response.status_code}:\n{response.json()}', 'ERROR')
-            return False
-
-    def get_device_json(self, update = False):
-        '''
-            https://sensors.nilu.no/api/doc#get--sensor-by-id
-        '''
-        if 'NILU_BEARER' in environ:
-            std_out('Auth Bearer found, using it', 'SUCCESS')
-            headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
-        else:
-            std_out('Cannot request without bearer', 'ERROR')
-            return None
-
-        if self.devicejson is None or update:
-            try:
-                deviceR = get(f'{self.API_BASE_URL}sensors/{self.id}')
-                if deviceR.status_code == 429:
-                    std_out('API reported {}. Retrying once'.format(deviceR.status_code),
-                            'WARNING')
-                    sleep(30)
-                    deviceR = get(f'{self.API_BASE_URL}sensors/{self.id}', headers = headers)
-
-                if deviceR.status_code == 200 or deviceR.status_code == 201:
-                    self.devicejson = deviceR.json()
-                else:
-                    std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
-            except:
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-        return self.devicejson
-
-    def get_device_description(self, update = False):
-        if self.get_device_json(update) is not None:
-            return self.get_device_json()['description']
-        return None
-
-    def get_device_lat_long(self, update = False):
-
-        if self.lat is None or self.long is None or update:
-            if self.get_device_json(update) is not None:
-                latidude = longitude = None
-                if 'location' in self.devicejson.keys():
-                    latitude, longitude = self.devicejson['location']['latitude'], self.devicejson['location']['longitude']
-
-                self.lat = latitude
-                self.long = longitude
-
-        std_out ('Device {} is located at {}, {}'.format(self.id, self.lat, self.long))
-
-        return (self.lat, self.long)
-
-    def get_device_alt(self, update = False):
-
-        if self.lat is None or self.long is None:
-            self.get_device_lat_long(update)
-
-        if self.alt is None or update:
-            self.alt = get_elevation(_lat = self.lat, _long = self.long)
-
-        std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
-
-        return self.alt
-
-    def get_device_added_at(self, update = False):
-
-        if 'NILU_BEARER' in environ:
-            std_out('Auth Bearer found, using it', 'SUCCESS')
-            headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
-        else:
-            std_out('Cannot request without bearer', 'ERROR')
-            return None
-
-        if self.added_at is None or update:
-            try:
-                response = get(f'{self.API_BASE_URL}data/id/{self.id}/minutc', headers = headers)
-                if response.status_code == 429:
-                    std_out('API reported {}. Retrying once'.format(response.status_code),
-                            'WARNING')
-                    sleep(30)
-                    response = get(f'{self.API_BASE_URL}data/id/{self.id}/minutc', headers = headers)
-
-                if response.status_code == 200 or response.status_code == 201:
-                    last_json = response.json()
-                    first_readings = []
-                    for item in last_json:
-                        if 'timestamp_from_epoch' in item: first_readings.append(item['timestamp_from_epoch'])
-
-                    self.added_at = localise_date(datetime.fromtimestamp(max(list(set(first_readings)))), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-                else:
-                    std_out(f'API reported {response.status_code}: {response.json()}', 'ERROR')
-            except:
-                print_exc()
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-        std_out ('Device {} has last reading at {}'.format(self.id, self.added_at))
-
-        return self.added_at
-
-    def get_device_last_reading(self, update = False):
-        if 'NILU_BEARER' in environ:
-            std_out('Auth Bearer found, using it', 'SUCCESS')
-            headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
-        else:
-            std_out('Cannot request without bearer', 'ERROR')
-            return None
-
-        if self.last_reading_at is None or update:
-            try:
-                response = get(f'{self.API_BASE_URL}data/id/{self.id}/maxutc', headers = headers)
-                if response.status_code == 429:
-                    std_out('API reported {}. Retrying once'.format(response.status_code),
-                            'WARNING')
-                    sleep(30)
-                    response = get(f'{self.API_BASE_URL}data/id/{self.id}/maxutc', headers = headers)
-
-                if response.status_code == 200 or response.status_code == 201:
-                    last_json = response.json()
-                    last_readings = []
-                    for item in last_json:
-                        if 'timestamp_from_epoch' in item: last_readings.append(item['timestamp_from_epoch'])
-
-                    self.last_reading_at = localise_date(datetime.fromtimestamp(max(list(set(last_readings)))), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-                else:
-                    std_out(f'API reported {response.status_code}: {response.json()}', 'ERROR')
-            except:
-                print_exc()
-                std_out('Failed request. Probably no connection', 'ERROR')
-                pass
-
-        std_out ('Device {} has last reading at {}'.format(self.id, self.last_reading_at))
-
-        return self.last_reading_at
-
-    def get_device_timezone(self, update = False):
-
-        if self.timezone is None or update:
-            latitude, longitude = self.get_device_lat_long(update)
-            # Localize it
-            if latitude is not None and longitude is not None:
-                # self.timezone = tz_where.tzNameAt(latitude, longitude, forceTZ=True)
-                self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
-
-        std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
-
-        return self.timezone
-
-    def get_device_sensors(self, update = False):
-
-        if self.sensors is None or update:
-            if self.get_device_json(update) is not None:
-                # Get available sensors
-                sensors = self.devicejson['components']
-                # Put the ids and the names in lists
-                self.sensors = dict()
-                for sensor in sensors:
-                    self.sensors[sensor['id']] = sensor['binding-path'][1:]
-
-        return self.sensors
-
-    def get_device_data(self, min_date = None, max_date = None, frequency = '1Min', clean_na = None, resample = True):
-        '''
-            From
-            https://sensors.nilu.no/api/doc#get--data-from-utc-timestamp-by-id
-            From-to
-            https://sensors.nilu.no/api/doc#get--data-from-utc-timestamp-range-by-id
-        '''
-
-        if 'NILU_BEARER' in environ:
-            std_out('Auth Bearer found, using it', 'SUCCESS')
-            headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
-        else:
-            std_out('Cannot request without bearer', 'ERROR')
-            return None
-
-        std_out(f'Requesting data from {self.API_BASE_URL}')
-        std_out(f'Device ID: {self.id}')
-
-        # Make sure we have the everything we need beforehand
-        self.get_device_sensors()
-        self.get_device_timezone()
-        # This is not available yet
-        # self.get_device_added_at()
-        self.get_device_last_reading()
-
-        if self.timezone is None:
-            std_out('Device does not have timezone set, skipping', 'WARNING')
-            return None
-
-        # Check start date and end date
-        if min_date is not None:
-            min_date = localise_date(to_datetime(min_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-            std_out (f'Min Date: {min_date}')
-        else:
-            std_out(f"No min_date specified, requesting all", 'WARNING')
-            # min_date = localise_date(to_datetime(self.added_at), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-
-        if max_date is not None:
-            max_date = localise_date(to_datetime(max_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-            std_out (f'Max Date: {max_date}')
-        else:
-            std_out(f"No max_date specified")
-
-        # Trim based on actual data available
-        if min_date is not None and self.last_reading_at is not None:
-            if min_date > self.last_reading_at:
-                std_out(f'Device request would yield empty data (min_date). Returning', 'WARNING')
-                return None
-
-        if max_date is not None and self.added_at is not None:
-            if max_date < self.added_at:
-                std_out(f'Device request would yield empty data (max_date). Returning', 'WARNING')
-                return None
-
-        if max_date is not None and self.last_reading_at is not None:
-            if max_date > self.last_reading_at:
-                std_out('Trimming max_date to last reading', 'WARNING')
-                max_date = self.last_reading_at
-
-        # Print stuff
-        std_out(f'Device timezone: {self.timezone}')
-        if not self.sensors.keys():
-            std_out(f'Device is empty')
-            return None
-        else: std_out(f'Sensor IDs: {list(self.sensors.keys())}')
-
-        df = DataFrame()
-
-        # Request sensor per ID
-        request = f'{self.API_BASE_URL}data/id/{self.id}/'
-
-        if min_date is not None: request += f'fromutc/{min_date}/'
-        if max_date is not None: request += f'toutc/{max_date}'
-
-        # Make request
-        response = get(request, headers = headers)
-
-        # Retry once in case of 429 after 30s
-        if response.status_code == 429:
-            std_out('Too many requests, waiting for 1 more retry', 'WARNING')
-            sleep (30)
-            response = get(request, headers = headers)
-
-        df = DataFrame(response.json()).pivot(index='timestamp_from_epoch', columns='component', values='value')
-        df.columns.name = None
-        df.index = localise_date(to_datetime(df.index, unit='s'), self.timezone)
-        df = df.reindex(df.index.rename('TIME'))
-
-        # Drop unnecessary columns
-        df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
-        # Check for weird things in the data
-        df = df.apply(to_numeric, errors='coerce')
-        # Resample
-        if (resample):
-            df = df.resample(frequency).mean()
-        df = clean(df, clean_na, how = 'all')
-
-        # Rename columns
-        d = {}
-        for component in self.devicejson['components']:
-            if 'name' in component: d[component['name']]=self.sensors[component['id']]
-        df = df.rename(columns=d)
-
-        self.data = df
-
-        std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
-        return self.data
-
-    def post_data_to_device(self, df, clean_na = 'drop', chunk_size = None, dry_run = False, max_retries = 2):
-        '''
-            POST external data in the IFLINK API, following
-            https://sensors.nilu.no/api/doc#push--sensor-data-by-id
-            Parameters
-            ----------
-                df: pandas DataFrame
-                    Contains data in a DataFrame format.
-                    Data is posted using the column name of the dataframe
-                    Data is posted in UTC TZ so dataframe needs to have located
-                    timestamp
-                clean_na: string, optional
-                    'drop'
-                    'drop', 'fill'
-                chunk_size: None (not used?)
-                    chunk size to split resulting pandas DataFrame for posting readings
-                dry_run: boolean
-                    False
-                    Post the payload to the API or just return it
-                max_retries: int
-                    2
-                    Maximum number of retries per chunk
-            Returns
-            -------
-                True if the data was posted succesfully
-        '''
-
-        if 'NILU_BEARER' not in environ:
-            std_out('Cannot post without Auth Bearer', 'ERROR')
-            return False
-
-        headers = {'Authorization':'Bearer ' + environ['NILU_BEARER'],
-            'Content-type': 'application/json'}
-
-        # Clean df of nans
-        df = clean(df, clean_na, how = 'all')
-
-        std_out(f'Posting columns to {self.API_BASE_URL}.')
-        std_out(f'Rest in schema are empty: {list(df.columns)}')
-
-        # Fill with declared schema to avoid rejection by the API
-        self.get_device_sensors()
-        for sensor in self.sensors:
-            if self.sensors[sensor] not in df.columns:
-                df[self.sensors[sensor]] = nan
-
-        # Split the dataframe in chunks
-        std_out(f'Splitting post in chunks of size {chunk_size}')
-
-        for i in trange(len(df.index), file=sys.stdout,
-                        desc=f"Posting data for {self.id}..."):
-
-            row = DataFrame(df.loc[df.index[i],:]).T
-            # Prepare json post
-            payload = {}
-            payload['date'] = localise_date(df.index[i], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
-
-            for column in row.columns:
-                payload[column] = row.loc[df.index[i], column]
-
-            if dry_run:
-                std_out(f'Dry run request to: {self.API_BASE_URL}sensors/{self.id}/inbound')
-                return dumps(payload, indent = 2, cls = NpEncoder)
-
-            post_ok = False
-            retries = 0
-
-            while post_ok == False and retries < max_retries:
-
-                response = post(f'{self.API_BASE_URL}sensors/{self.id}/inbound',
-                            data = dumps(payload, cls = NpEncoder), headers = headers)
-
-                if response.status_code == 200 or response.status_code == 201:
-                    post_ok = True
-                    break
-                else:
-                    retries += 1
-                    std_out (f'Chunk ({i+1}/{len(df.index)}) post failed. \
-                           API responded {response.status_code}.\
-                            Retrying ({retries}/{max_retries}', 'WARNING')
-
-            if (not post_ok) or (retries == max_retries):
-                std_out (f'Chunk ({i+1}/{len(df.index)}) post failed. \
-                       API responded {response.status_code}.\
-                        Reached max_retries', 'ERROR')
-                return False
+#         self.id = did # the number after https://smartcitizen.me/kits/######
+#         self.kit_id = None # the number that defines the type of blueprint
+#         self.mac = None
+#         self.last_reading_at = None
+#         self.added_at = None
+#         self.timezone = None
+#         self.lat = None
+#         self.long = None
+#         self.alt = None
+#         self.data = None
+#         self.sensors = None
+#         self.devicejson = None
+#         self.postprocessing = None
+#         self._url = f'https://smartcitizen.me/kits/{self.id}'
+#         self._api_url = f'{self.API_BASE_URL}{self.id}'
+
+#     @property
+#     def url(self):
+#         return self._url
+
+#     @property
+#     def api_url(self):
+#         return self._api_url
+
+#     @staticmethod
+#     # def new_device(name, kit_id = 26, location = None, exposure = 'indoor', user_tags = 'Lab, Research, Experimental', dry_run = False):
+#     def new_device(name, location = {}, dry_run = False, **kwargs):
+#         '''
+#             Creates a new device in the Smart Citizen Platform provided a name
+#             Parameters
+#             ----------
+#                 name: string
+#                     Device name
+#                 location: dict, optional
+#                     None
+#                     location = {
+#                                 'longitude': longitude (double) – sensor east-west position,
+#                                 'latitude': latitude (double) – sensor north-south position,
+#                                 'altitude': altitude (double) – sensor height above sea level
+#                                 }
+#                 dry_run: boolean
+#                     False
+#                     Post the payload to the API or just return it
+#                 **kwargs
+#                 ------
+#                 kit_id: int, optional
+#                     26 (SCK 2.1)
+#                     Kit ID - related to blueprint
+#                 exposure: string, optional
+#                     'indoor'
+#                     Type of exposure ('indoor', 'outdoor')
+#                 user_tags: string
+#                     'Lab, Research, Experimental'
+#                     User tags, comma separated
+#                 -----
+#             Returns
+#             -------
+#                 If dry_run, prints out a dict containing the payload and
+#                 returns False
+#                 If not, either False in case of error or a
+#                 dictionary containing:
+#                     id (int) – sensor identifier
+#                     message (string) – HTTP status text
+#                     http-status-code (int) – HTTP status code
+#         '''
+
+#         API_BASE_URL = 'https://api.smartcitizen.me/v0/devices'
+
+#         if 'SC_ADMIN_BEARER' not in environ:
+#             std_out('Cannot post without Auth Bearer', 'ERROR')
+#             return
+
+#         headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'], 'Content-type': 'application/json'}
+
+#         # Set defaults
+#         if 'kit_id' not in kwargs:
+#             kit_id = 26
+#         else: kit_id = kwargs['kit_id']
+
+#         if 'exposure' not in kwargs:
+#             exposure = 'indoor'
+#         else: exposure = kwargs['exposure']
+
+#         if 'user_tags' not in kwargs:
+#             user_tags = 'Lab, Research, Experimental'
+#         else: user_tags = kwargs['user_tags']
+
+#         payload = {}
+#         try:
+#             payload['name'] = name
+#         except:
+#             std_out('Your device needs a name!', 'ERROR')
+#             sys.exit()
+
+#         payload['device_token'] = binascii.b2a_hex(urandom(3)).decode('utf-8')
+#         payload['description'] = ''
+#         payload['kit_id'] = kit_id
+#         payload['latitude'] = location['latitude']
+#         payload['longitude'] = location['longitude']
+#         payload['exposure'] = exposure
+#         payload['user_tags'] = user_tags
+
+#         if dry_run:
+#             std_out(f'Dry run request to: {API_BASE_URL}sensors/configure')
+#             print(dumps(payload, indent = 2))
+#             return False
+
+#         response = post(API_BASE_URL, data=dumps(payload), headers=headers)
+
+#         if response.status_code == 200 or response.status_code == 201:
+#             if 'id' in response.json():
+#                 platform_id = str(response.json()['id'])
+#                 platform_url = "https://smartcitizen.me/kits/" + platform_id
+#                 std_out(f'Device created with: \n{platform_url}', 'SUCCESS')
+#                 return response.json()
+#             else:
+#                 std_out('Response does not contain id field')
+
+#         std_out(f'Error while creating new device, platform returned {response.status_code}', 'ERROR')
+#         return False
+
+#     @staticmethod
+#     def global_search(value = None, full = False):
+#         """
+#         Gets devices from Smart Citizen API based on basic search query values,
+#         searching both Users and Devices at the same time.
+#         Global search documentation: https://developer.smartcitizen.me/#global-search
+#         Parameters
+#         ----------
+#             value: string
+#                 None
+#                 Query to fit
+#                 For null, not_null values, use 'null' or 'not_null'
+#             full: bool
+#                 False
+#                 Returns a list with if False, or the whole dataframe if True
+#         Returns
+#         -------
+#             A list of kit IDs that comply with the requirements, or the full df, depending on full.
+#         """
+
+#         API_BASE_URL = "https://api.smartcitizen.me/v0/search?q="
+
+#         # Value check
+#         if value is None: std_out(f'Value needs a value, {value} supplied', 'ERROR'); return None
+
+#         url = API_BASE_URL  + f'{value}'
+
+#         df = DataFrame()
+#         isn = True
+#         while isn:
+#             try:
+#                 r = get(url)
+#                 # If status code OK, retrieve data
+#                 if r.status_code == 200 or r.status_code == 201:
+#                     h = process_headers(r.headers)
+#                     df = df.combine_first(DataFrame(r.json()).set_index('id'))
+#                 else:
+#                     std_out('API reported {}'.format(r.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#             if 'next' in h:
+#                 if h['next'] == url: isn = False
+#                 elif h['next'] != url: url = h['next']
+#             else:
+#                 isn = False
+
+#         if full: return df
+#         else: return list(df.index)
+
+#     @staticmethod
+#     def search_by_query(key = '', value = None, full = False):
+#         """
+#         Gets devices from Smart Citizen API based on ransack parameters
+#         Basic query documentation: https://developer.smartcitizen.me/#basic-searching
+#         Parameters
+#         ----------
+#             key: string
+#                 ''
+#                 Query key according to the basic query documentation. Some (not all) parameters are:
+#                 ['id', 'owner_id', 'name', 'description', 'mac_address', 'created_at',
+#                 'updated_at', 'kit_id', 'geohash', 'last_recorded_at', 'uuid', 'state',
+#                 'postprocessing_id', 'hardware_info']
+#             value: string
+#                 None
+#                 Query to fit
+#                 For null, not_null values, use 'null' or 'not_null'
+#             full: bool
+#                 False
+#                 Returns a list with if False, or the whole dataframe if True
+#         Returns
+#         -------
+#             A list of kit IDs that comply with the requirements, or the full df, depending on full.
+#         """
+
+#         API_BASE_URL = "https://api.smartcitizen.me/v0/devices/"
+
+#         # Value check
+#         if value is None: std_out(f'Value needs a value, {value} supplied', 'ERROR'); return None
+
+#         if value == 'null' or value == 'not_null':
+#              url = API_BASE_URL  + f'?q[{key}_{value}]=1'
+#         else:
+#              url = API_BASE_URL  + f'?q[{key}]={value}'
+
+#         df = DataFrame()
+#         isn = True
+#         while isn:
+#             try:
+#                 r = get(url)
+#                 # If status code OK, retrieve data
+#                 if r.status_code == 200 or r.status_code == 201:
+#                     h = process_headers(r.headers)
+#                     df = df.combine_first(DataFrame(r.json()).set_index('id'))
+#                 else:
+#                     std_out('API reported {}'.format(r.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#             if 'next' in h:
+#                 if h['next'] == url: isn = False
+#                 elif h['next'] != url: url = h['next']
+#             else:
+#                 isn = False
+
+#         if full: return df
+#         else: return list(df.index)
+
+#     @staticmethod
+#     def get_world_map(min_date = None, max_date = None, city = None, within = None, tags = None, tag_method = 'any', full = False):
+#         """
+#         Gets devices from Smart Citizen API with certain requirements
+#         Parameters
+#         ----------
+#             min_date: string, datetime-like object, optional
+#                 None
+#                 Minimum date to filter out the devices. Device started posted before min_date
+#             max_date: string, datetime-like object, optional
+#                 None
+#                 Maximum date to filter out the devices. Device posted after max_date
+#             city: string, optional
+#                 Empty string
+#                 City
+#             within: tuple
+#                 Empty tuple
+#                 Gets the devices within a circle center on lat, long with a radius_meters
+#                 within = tuple(lat, long, radius_meters)
+#             tags: list of strings
+#                 None
+#                 Tags for the device (system or user). Default system wide are: indoor, outdoor, online, and offline
+#             tag_method: string
+#                 'any'
+#                 'any' or 'all'. Checks if 'all' the tags are to be included in the tags or it could be any
+#             full: bool
+#                 False
+#                 Returns a list with if False, or the whole dataframe if True
+#         Returns
+#         -------
+#             A list of kit IDs that comply with the requirements, or the full df, depending on full.
+#             If no requirements are set, returns all of them
+#         """
+
+#         def is_within_circle(x, within):
+#             if isnan(x['latitude']): return False
+#             if isnan(x['longitude']): return False
+
+#             return distance((within[0], within[1]), (x['latitude'], x['longitude'])).m<within[2]
+
+#         world_map = get('https://api.smartcitizen.me/v0/devices/world_map')
+
+#         df = DataFrame(world_map.json()).set_index('id')
+
+#         # Filter out dates
+#         if min_date is not None: df=df[(min_date > df['added_at'])]
+#         if max_date is not None: df=df[(max_date < df['last_reading_at'])]
+
+#         # Location
+#         if city is not None: df=df[(df['city']==city)]
+#         if within is not None:
+
+#             df['within'] = df.apply(lambda x: is_within_circle(x, within), axis=1)
+#             df=df[(df['within']==True)]
+
+#         # Tags
+#         if tags is not None:
+#             if tag_method == 'any':
+#                 df['has_tags'] = df.apply(lambda x: any(tag in x['system_tags']+x['user_tags'] for tag in tags), axis=1)
+#             elif tag_method == 'all':
+#                 df['has_tags'] = df.apply(lambda x: all(tag in x['system_tags']+x['user_tags'] for tag in tags), axis=1)
+#             df=df[(df['has_tags']==True)]
+
+#         if full: return df
+#         else: return list(df.index)
+
+#     def get_mac(self, update = False):
+#         if self.mac is None or update:
+#             std_out(f'Requesting MAC from API for device {self.id}')
+#             # Get device
+#             try:
+#                 deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
+
+#                 # If status code OK, retrieve data
+#                 if deviceR.status_code == 200 or deviceR.status_code == 201:
+#                     if 'hardware_info' in deviceR.json().keys(): self.mac = deviceR.json()['hardware_info']['mac']
+#                     std_out ('Device {} is has this MAC {}'.format(self.id, self.mac))
+#                 else:
+#                     std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#         return self.mac
+
+#     def get_device_json(self, update = False):
+#         if self.devicejson is None or update:
+#             try:
+#                 deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
+#                 if deviceR.status_code == 429:
+#                     std_out('API reported {}. Retrying once'.format(deviceR.status_code),
+#                             'WARNING')
+#                     sleep(30)
+#                     deviceR = get(self.API_BASE_URL + '{}/'.format(self.id))
+
+#                 if deviceR.status_code == 200 or deviceR.status_code == 201:
+#                     self.devicejson = deviceR.json()
+#                 else:
+#                     std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+#         return self.devicejson
+
+#     def get_device_description(self, update = False):
+#         if self.get_device_json(update) is not None:
+#             return self.get_device_json()['kit']['description']
+#         return None
+
+#     def get_kit_ID(self, update = False):
+
+#         if self.kit_id is None or update:
+#             if self.get_device_json(update) is not None:
+#                 self.kit_id = self.devicejson['kit']['id']
+
+#         return self.kit_id
+
+#     def post_kit_ID(self):
+#         '''
+#             Posts kit id to platform
+#         '''
+
+#         if 'SC_ADMIN_BEARER' not in environ:
+#             std_out('Cannot post without Auth Admin Bearer', 'ERROR')
+#             return
+
+#         headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'], 'Content-type': 'application/json'}
+
+#         if self.kit_id is not None:
+
+#             payload = {'kit_id': self.kit_id}
+
+#             payload_json = dumps(payload)
+#             response = patch(f'{self.API_BASE_URL}{self.id}',
+#                         data = payload_json, headers = headers)
+
+#             if response.status_code == 200 or response.status_code == 201:
+#                 std_out(f'Kit ID for device {self.id} was updated to {self.kit_id}', 'SUCCESS')
+#                 return True
+
+#         std_out(f'Problem while updating kit ID for device {self.id}')
+
+#         return False
+
+#     def get_device_last_reading(self, update = False):
+
+#         if self.last_reading_at is None or update:
+#             if self.get_device_json(update) is not None and self.get_device_json(update)['state'] != 'never_published':
+#                 self.last_reading_at = localise_date(self.devicejson['last_reading_at'], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+
+#         std_out ('Device {} has last reading at {}'.format(self.id, self.last_reading_at))
+
+#         return self.last_reading_at
+
+#     def get_device_added_at(self, update = False):
+
+#         if self.added_at is None or update:
+#             if self.get_device_json(update) is not None:
+#                 self.added_at = localise_date(self.devicejson['added_at'], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+
+#         std_out ('Device {} was added at {}'.format(self.id, self.added_at))
+
+#         return self.added_at
+
+#     def get_device_postprocessing(self, update = False):
+
+#         if self.postprocessing is None or update:
+#             if self.get_device_json(update) is not None:
+#                 self.postprocessing = self.devicejson['postprocessing']
+
+#                 if self.postprocessing is not None:
+#                     # Check the url in hardware
+#                     if 'hardware_url' in self.postprocessing:
+#                         urls = url_checker(self.postprocessing['hardware_url'])
+#                         # If URL is empty, try prepending base url from config
+#                         if not urls:
+#                             tentative_url = f"{config._base_postprocessing_url}hardware/{self.postprocessing['hardware_url']}.{config._default_file_type}"
+#                         else:
+#                             if len(urls)>1: std_out('URLs for postprocessing recipe are more than one, trying first', 'WARNING')
+#                             tentative_url = urls[0]
+
+#                         self.postprocessing['hardware_url'] = tentative_url
+
+#                     std_out ('Device {} has postprocessing information:\n{}'.format(self.id, self.postprocessing))
+#                 else:
+#                     std_out (f'Device {self.id} has no postprocessing information')
+
+#         return self.postprocessing
+
+#     def get_device_timezone(self, update = False):
+
+#         if self.timezone is None or update:
+#             latitude, longitude = self.get_device_lat_long(update)
+#             # Localize it
+
+#             if latitude is not None and longitude is not None:
+#                 # self.timezone = tz_where.tzNameAt(latitude, longitude, forceTZ=True)
+#                 self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
+#         std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
+
+#         return self.timezone
+
+#     def get_device_lat_long(self, update = False):
+
+#         if self.lat is None or self.long is None or update:
+#             if self.get_device_json(update) is not None:
+#                 latidude = longitude = None
+#                 if 'location' in self.devicejson.keys():
+#                     latitude, longitude = self.devicejson['location']['latitude'], self.devicejson['location']['longitude']
+#                 elif 'data' in self.devicejson.keys():
+#                     if 'location' in self.devicejson['data'].keys():
+#                         latitude, longitude = self.devicejson['data']['location']['latitude'], self.devicejson['data']['location']['longitude']
+
+#                 self.lat = latitude
+#                 self.long = longitude
+
+#         std_out ('Device {} is located at {}, {}'.format(self.id, self.lat, self.long))
+
+#         return (self.lat, self.long)
+
+#     def get_device_alt(self, update = False):
+
+#         if self.lat is None or self.long is None:
+#             self.get_device_lat_long(update)
+
+#         if self.alt is None or update:
+#             self.alt = get_elevation(_lat = self.lat, _long = self.long)
+
+#         std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
+
+#         return self.alt
+
+#     def get_device_sensors(self, update = False):
+
+#         if self.sensors is None or update:
+#             if self.get_device_json(update) is not None:
+#                 # Get available sensors in platform
+#                 sensors = self.devicejson['data']['sensors']
+
+#                 # Put the ids and the names in lists
+#                 self.sensors = dict()
+#                 for sensor in sensors:
+#                     for key in config.names['sc_sensor_names']:
+#                         if str(config.names['sc_sensor_names'][key]['id']) == str(sensor['id']):
+#                             # IDs are unique
+#                             if key in config._sc_ignore_keys: continue
+#                             self.sensors[sensor['id']] = key
+
+#         return self.sensors
+
+#     def convert_rollup(self, frequency):
+#         # Convert frequency from pandas to API's
+#         for index, letter in enumerate(frequency):
+#             try:
+#                 aux = int(letter)
+#             except:
+#                 index_first = index
+#                 letter_first = letter
+#                 rollup_value = frequency[:index_first]
+#                 frequency_unit = frequency[index_first:]
+#                 break
+
+#         for item in config._freq_conv_lut:
+#             if item[1] == frequency_unit:
+#                 rollup_unit = item[0]
+#                 break
+
+#         rollup = rollup_value + rollup_unit
+#         return rollup
+
+#     def get_device_data(self, min_date = None, max_date = None, frequency = '1Min', clean_na = None, resample = True):
+
+#         if 'SC_ADMIN_BEARER' in environ:
+#             std_out('Admin Bearer found, using it', 'SUCCESS')
+
+#             headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER']}
+#         else:
+#             headers = None
+#             std_out('Admin Bearer not found', 'WARNING')
+
+#         std_out(f'Requesting data from SC API')
+#         std_out(f'Device ID: {self.id}')
+
+#         rollup = self.convert_rollup(frequency)
+#         std_out(f'Using rollup: {rollup}')
+
+#         # Make sure we have the everything we need beforehand
+#         self.get_device_sensors()
+#         self.get_device_timezone()
+#         self.get_device_last_reading()
+#         self.get_device_added_at()
+#         self.get_kit_ID()
+
+#         if self.timezone is None:
+#             std_out('Device does not have timezone set, skipping', 'WARNING')
+#             return None
+
+#         # Check start date and end date
+#         # Converting to UTC by passing None
+#         # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.dt.tz_convert.html
+#         if min_date is not None:
+#             min_date = localise_date(to_datetime(min_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
+#             std_out (f'Min Date: {min_date}')
+#         else:
+#             min_date = localise_date(to_datetime('2001-01-01'), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
+#             std_out(f"No min_date specified")
+
+#         if max_date is not None:
+#             max_date = localise_date(to_datetime(max_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%S')
+#             std_out (f'Max Date: {max_date}')
+
+#         # Trim based on actual data available
+#         if min_date is not None and self.last_reading_at is not None:
+#             if min_date > self.last_reading_at:
+#                 std_out(f'Device request would yield empty data (min_date). Returning', 'WARNING')
+#                 return None
+
+#         if max_date is not None and self.added_at is not None:
+#             if max_date < self.added_at:
+#                 std_out(f'Device request would yield empty data (max_date). Returning', 'WARNING')
+#                 return None
+
+#         if max_date is not None and self.last_reading_at is not None:
+#             if max_date > self.last_reading_at:
+#                 std_out('Trimming max_date to last reading', 'WARNING')
+#                 max_date = self.last_reading_at
+
+#         # Print stuff
+#         std_out('Kit ID: {}'.format(self.kit_id))
+#         std_out(f'Device timezone: {self.timezone}')
+#         if not self.sensors.keys():
+#             std_out(f'Device is empty')
+#             return None
+#         else: std_out(f'Sensor IDs: {list(self.sensors.keys())}')
+
+#         df = DataFrame()
+#         std_out(f'Requesting from {min_date} to {max_date}')
+
+#         # Get devices in the sensor first
+#         for sensor_id in self.sensors.keys():
+
+#             # Request sensor per ID
+#             request = self.API_BASE_URL + '{}/readings?'.format(self.id)
+
+#             if min_date is not None: request += f'from={min_date}'
+#             if max_date is not None: request += f'&to={max_date}'
+
+#             request += f'&rollup={rollup}'
+#             request += f'&sensor_id={sensor_id}'
+#             request += '&function=avg'
+
+#             # Make request
+#             response = get(request, headers = headers)
+
+#             # Retry once in case of 429 after 30s
+#             if response.status_code == 429:
+#                 std_out('Too many requests, waiting for 1 more retry', 'WARNING')
+#                 sleep (30)
+#                 response = get(request, headers = headers)
+
+#             flag_error = False
+#             try:
+#                 sensorjson = response.json()
+#             except:
+#                 std_out(f'Problem with json data from API, {response.status_code}', 'ERROR')
+#                 flag_error = True
+#                 pass
+#                 continue
+
+#             if 'readings' not in sensorjson.keys():
+#                 std_out(f'No readings key in request for sensor: {sensor_id} ({self.sensors[sensor_id]})', 'ERROR')
+#                 flag_error = True
+#                 continue
+
+#             elif sensorjson['readings'] == []:
+#                 std_out(f'No data in request for sensor: {sensor_id} ({self.sensors[sensor_id]})', 'WARNING')
+#                 flag_error = True
+#                 continue
+
+#             if flag_error: continue
+
+#             try:
+#                 dfsensor = DataFrame(sensorjson['readings']).set_index(0)
+#                 dfsensor.columns = [self.sensors[sensor_id]]
+#                 dfsensor.index = localise_date(dfsensor.index, self.timezone)
+#                 dfsensor.sort_index(inplace=True)
+#                 dfsensor = dfsensor[~dfsensor.index.duplicated(keep='first')]
+
+#                 # Drop unnecessary columns
+#                 dfsensor.drop([i for i in dfsensor.columns if 'Unnamed' in i], axis=1, inplace=True)
+#                 # Check for weird things in the data
+#                 dfsensor = dfsensor.astype(float, errors='ignore')
+#                 # dfsensor = dfsensor.apply(to_numeric, errors='coerce')
+#                 # Resample
+#                 if (resample):
+#                     dfsensor = dfsensor.resample(frequency).mean()
+#                 df = df.combine_first(dfsensor)
+#             except:
+#                 print_exc()
+#                 std_out('Problem with sensor data from API', 'ERROR')
+#                 flag_error = True
+#                 pass
+#                 continue
+
+#             try:
+#                 df = df.reindex(df.index.rename('TIME'))
+#                 df = clean(df, clean_na, how = 'all')
+#                 self.data = df
+
+#             except:
+#                 std_out('Problem closing up the API dataframe', 'ERROR')
+#                 pass
+#                 return None
+
+#         if flag_error == False: std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
+#         return self.data
+
+#     def post_device_data(self, clean_na = 'drop', chunk_size = 500):
+#         '''
+#             POST self.data in the SmartCitizen API
+#             Parameters
+#             ----------
+#                 clean_na: string, optional
+#                     'drop'
+#                     'drop', 'fill'
+#                 chunk_size: integer
+#                     chunk size to split resulting pandas DataFrame for posting readings
+#             Returns
+#             -------
+#                 True if the data was posted succesfully
+#         '''
+#         if self.data is None:
+#             std_out('No data to post, ignoring', 'ERROR')
+#             return False
+
+#         if 'SC_BEARER' not in environ:
+#             std_out('Cannot post without Auth Bearer', 'ERROR')
+#             return False
+
+#         if 'SC_ADMIN_BEARER' in environ:
+#             std_out('Using admin Bearer')
+#             bearer = environ['SC_ADMIN_BEARER']
+#         else:
+#             bearer = environ['SC_BEARER']
+
+#         headers = {'Authorization':'Bearer ' + bearer, 'Content-type': 'application/json'}
+#         post_ok = True
+
+#         for sensor_id in self.sensors:
+#             df = DataFrame(self.data[self.sensors[sensor]]).copy()
+#             post_ok &= self.post_data_to_device(df, clean_na = clean_na, chunk_size = chunk_size)
+
+#         return post_ok
+
+#     def post_data_to_device(self, df, clean_na = 'drop', chunk_size = 500, dry_run = False, max_retries = 2):
+#         '''
+#             POST external pandas.DataFrame to the SmartCitizen API
+#             Parameters
+#             ----------
+#                 df: pandas DataFrame
+#                     Contains data in a DataFrame format.
+#                     Data is posted using the column names of the dataframe
+#                     Data is posted in UTC TZ so dataframe needs to have located
+#                     timestamp
+#                 clean_na: string, optional
+#                     'drop'
+#                     'drop', 'fill'
+#                 chunk_size: integer
+#                     chunk size to split resulting pandas DataFrame for posting readings
+#                 dry_run: boolean
+#                     False
+#                     Post the payload to the API or just return it
+#                 max_retries: int
+#                     2
+#                     Maximum number of retries per chunk
+#             Returns
+#             -------
+#                 True if the data was posted succesfully
+#         '''
+#         if 'SC_BEARER' not in environ:
+#             std_out('Cannot post without Auth Bearer', 'ERROR')
+#             return False
+
+#         if 'SC_ADMIN_BEARER' in environ:
+#             std_out('Using admin Bearer')
+#             bearer = environ['SC_ADMIN_BEARER']
+#         else:
+#             bearer = environ['SC_BEARER']
+
+#         headers = {'Authorization':'Bearer ' + bearer, 'Content-type': 'application/json'}
+
+#         # Clean df of nans
+#         df = clean(df, clean_na, how = 'all')
+#         std_out(f'Posting columns to {self.API_BASE_URL}')
+#         std_out(f'{list(df.columns)}')
+#         df.index.name = 'recorded_at'
+
+#         # Split the dataframe in chunks
+#         std_out(f'Splitting post in chunks of size {chunk_size}')
+#         chunked_dfs = [df[i:i+chunk_size] for i in range(0, df.shape[0], chunk_size)]
+
+#         for i in trange(len(chunked_dfs), file=sys.stdout,
+#                         desc=f"Posting data for {self.id}..."):
+
+#             chunk = chunked_dfs[i].copy()
+
+#             # Prepare json post
+#             payload = {"data":[]}
+#             for item in chunk.index:
+#                 payload["data"].append(
+#                     {
+#                         "recorded_at": localise_date(item, 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ'),
+#                         "sensors": [{
+#                             "id": column,
+#                             "value": chunk.loc[item, column]
+#                         } for column in chunk.columns if not isnan(chunk.loc[item, column])]
+#                     }
+#                 )
+
+#             if dry_run:
+#                 std_out(f'Dry run request to: {self.API_BASE_URL}{self.id}/readings for chunk ({i+1}/{len(chunked_dfs)})')
+#                 return dumps(payload, indent = 2, cls = NpEncoder)
+
+#             post_ok = False
+#             retries = 0
+
+#             while post_ok == False and retries < max_retries:
+#                 response = post(f'{self.API_BASE_URL}{self.id}/readings',
+#                             data = dumps(payload, cls = NpEncoder), headers = headers)
+
+#                 if response.status_code == 200 or response.status_code == 201:
+#                     post_ok = True
+#                     break
+#                 else:
+#                     retries += 1
+#                     std_out (f'Chunk ({i+1}/{len(chunked_dfs)}) post failed. \
+#                            API responded {response.status_code}.\
+#                             Retrying ({retries}/{max_retries}', 'WARNING')
+
+#             if (not post_ok) or (retries == max_retries):
+#                 std_out (f'Chunk ({i+1}/{len(chunked_dfs)}) post failed. \
+#                        API responded {response.status_code}.\
+#                         Reached max_retries', 'ERROR')
+#                 return False
+
+#         return True
+
+#     def patch_postprocessing(self, dry_run = False):
+#         '''
+#             POST postprocessing info into the device in the SmartCitizen API
+#             Updates all the post info. Changes need to be made info the keys of the postprocessing outside of here
+
+#             # Example postprocessing:
+#             # {
+#             #   "blueprint_url": "https://github.com/fablabbcn/smartcitizen-data/blob/master/blueprints/sc_21_station_module.json",
+#             #   "hardware_url": "https://raw.githubusercontent.com/fablabbcn/smartcitizen-data/master/hardware/SCAS210001.json",
+#             #   "latest_postprocessing": "2020-10-29T08:35:23Z"
+#             # }
+#         '''
+
+#         if 'SC_ADMIN_BEARER' not in environ:
+#             std_out('Cannot post without Admin Auth Bearer', 'ERROR')
+#             return
+
+#         headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER'],
+#                    'Content-type': 'application/json'}
+
+#         post = {"postprocessing_attributes": self.postprocessing}
+#         post_json = dumps(post)
+
+#         if dry_run:
+#             std_out(f'Dry run request to: {self.API_BASE_URL}{self.id}/')
+#             return dumps(post_json, indent = 2)
+
+#         std_out(f'Posting postprocessing_attributes:\n {post_json}')
+#         response = patch(f'{self.API_BASE_URL}{self.id}/',
+#                          data = post_json, headers = headers)
+
+#         if response.status_code == 200 or response.status_code == 201:
+#             std_out(f"Postprocessing posted", "SUCCESS")
+#             return True
+#         else:
+#             std_out(f"API responded with {response.status_code}")
+
+#         return False
+
+# class MuvApiDevice:
+
+#     API_BASE_URL='https://data.waag.org/api/muv/'
+
+#     def __init__ (self, did):
+#         self.id = did
+#         self.timezone = None
+#         self.data = None
+#         self.sensors = None
+
+#     def get_device_timezone(self):
+#         self.timezone = 'Europe/Madrid'
+#         return self.timezone
+
+#     def get_device_sensors(self):
+#         if self.sensors is None:
+#             self.sensors = dict()
+#             for key in config.blueprints:
+#                 if 'muv' not in key: continue
+#                 if 'sensors' in config.blueprints[key]:
+#                     for sensor_name in config.blueprints[key]['sensors'].keys():
+#                         # IDs are unique
+#                         self.sensors[config.blueprints[key]['sensors'][sensor_name]['id']] = sensor_name
+#         return self.sensors
+
+#     def get_device_data(self, min_date = None, max_date = None, frequency = '3Min', clean_na = None, resample = True):
+
+#         if min_date is not None: days_ago = (to_datetime(date.today())-to_datetime(min_date)).days
+#         else: days_ago = 365 # One year of data
+
+#         std_out(f'Requesting data from MUV API')
+#         std_out(f'Device ID: {self.id}')
+#         self.get_device_timezone()
+#         self.get_device_sensors()
+
+#         # Get devices
+#         try:
+#             if days_ago == -1: url = f'{self.API_BASE_URL}getSensorData?sensor_id={self.id}'
+#             else: url = f'{self.API_BASE_URL}getSensorData?sensor_id={self.id}&days={days_ago}'
+#             df = DataFrame(get(url).json())
+#         except:
+#             print_exc()
+#             std_out('Failed sensor request request. Probably no connection', 'ERROR')
+#             pass
+#             return None
+
+#         try:
+#             # Rename columns
+#             df.rename(columns = self.sensors, inplace = True)
+#             df = df.set_index('time')
+
+#             df.index = localise_date(df.index, self.timezone)
+#             df = df[~df.index.duplicated(keep='first')]
+#             # Drop unnecessary columns
+#             df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
+#             df.drop('id', axis=1, inplace=True)
+#             # Check for weird things in the data
+#             df = df.apply(to_numeric, errors='coerce')
+#             # # Resample
+#             if (resample):
+#                 df = df.resample(frequency).mean()
+#             df = df.reindex(df.index.rename('TIME'))
+
+#             df = clean(df, clean_na, how = 'all')
+
+#             self.data = df
+
+#         except:
+#             print_exc()
+#             std_out('Problem closing up the API dataframe', 'ERROR')
+#             pass
+#             return None
+
+#         std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
+#         return self.data
+
+# class DadesObertesApiDevice:
+
+#     API_BASE_URL="https://analisi.transparenciacatalunya.cat/resource/tasf-thgu.json"
+
+#     def __init__ (self, did = None, within = None):
+#         if did is None and within is None:
+#             std_out('Specify either station id (=codi_eoi) or within (=(lat, long, radius_meters))')
+#             return
+
+#         if did is not None: self.id = did
+#         if within is not None: self.id = self.get_id_from_within(within)
+
+#         self.timezone = None
+#         self.data = None
+#         self.sensors = None
+#         self.devicejson = None
+#         self.lat = None
+#         self.long = None
+#         self.alt = None
+#         self.timezone = None
+
+#     @staticmethod
+#     def get_world_map(city = None, within = None, station_type = None, area_type = None, full = False):
+#         """
+#         Gets devices from Dades Obertes API with certain requirements
+#         Parameters
+#         ----------
+#             city: string, optional
+#                 Empty string
+#                 City
+#             within: tuple
+#                 Empty tuple
+#                 Gets the devices within a circle center on lat, long with a radius_meters
+#                 within = tuple(lat, long, radius_meters)
+#             station_type: string
+#                 None
+#                 Type of station, to choose from: 'background', nan or 'traffic'
+#             area_type: string
+#                 None
+#                 Type of area, to choose from:  nan, 'peri-urban', 'rural', 'suburban', 'urban'
+#             full: bool
+#                 False
+#                 Return full dataframe or not
+#         Returns
+#         -------
+#             A list of eoi codes that comply with the requirements. If no requirements are set, returns all of them
+#         """
+#         def is_within_circle(x, within):
+#             if isnan(x['latitud']): return False
+#             if isnan(x['longitud']): return False
+
+#             return distance(location_A=(within[0], within[1]), location_B=(x['latitude'], x['longitude'])).m < within[2]
+
+#         world_map = get("https://analisi.transparenciacatalunya.cat/resource/tasf-thgu.json")
+#         df = read_json(StringIO(world_map.content.decode('utf-8'))).set_index('codi_eoi')
+
+#         # Location
+#         if city is not None: df=df[(df['municipi']==city)]
+#         if within is not None:
+
+#             df['within'] = df.apply(lambda x: is_within_circle(x, within), axis=1)
+#             df=df[(df['within']==True)]
+
+#         # Station type
+#         if station_type is not None: df=df[(df['tipus_estacio']==station_type)]
+#         # Area type
+#         if area_type is not None: df=df[(df['area_urbana']==area_type)]
+
+#         if full: return df
+#         return list(set(list(df.index)))
+
+#     def get_id_from_within(self, within):
+#         '''
+#             Gets the stations within a radius in meters.
+#             within = tuple(lat, long, radius_meters)
+#         '''
+#         request = self.API_BASE_URL
+#         request += f'$where=within_circle(geocoded_column,{within[0]},{within[1]},{within[2]})'
+
+#         try:
+#             s = get(request)
+#         except:
+#             std_out('Problem with request from API', 'ERROR')
+#             return None
+
+#         if s.status_code == 200 or s.status_code == 201:
+#             df = read_json(StringIO(s.content.decode('utf-8')))
+#         else:
+#             std_out('API reported {}'.format(s.status_code), 'ERROR')
+#             return None
+
+#         if 'codi_eoi' in df.columns:
+#             ids = list(set(df.codi_eoi.values))
+#             if ids == []: std_out('No stations within range', 'ERROR')
+#             elif len(ids) > 1:
+#                 for ptid in ids:
+#                     municipi = next(iter(set(df[df.codi_eoi==ptid].municipi.values)))
+#                     nom_estacio = next(iter(set(df[df.codi_eoi==ptid].nom_estacio.values)))
+#                     area_urbana = next(iter(set(df[df.codi_eoi==ptid].area_urbana.values)))
+#                     tipus_estacio = next(iter(set(df[df.codi_eoi==ptid].tipus_estacio.values)))
+
+#                     std_out(f'{ids.index(ptid)+1} /- {ptid} --- {municipi} - {nom_estacio} - Type: {area_urbana} - {tipus_estacio}')
+
+#                 wptid = int(input('Multiple stations found, please select one: ')) - 1
+
+#                 devid = ids[wptid]
+#                 std_out(f'Selected station in {next(iter(set(df[df.codi_eoi==devid].municipi.values)))} with codi_eoi={devid}')
+#             else:
+#                 devid = ids[0]
+#                 municipi = next(iter(set(df[df.codi_eoi==devid].municipi.values)))
+#                 nom_estacio = next(iter(set(df[df.codi_eoi==devid].nom_estacio.values)))
+#                 area_urbana = next(iter(set(df[df.codi_eoi==devid].area_urbana.values)))
+#                 tipus_estacio = next(iter(set(df[df.codi_eoi==devid].tipus_estacio.values)))
+#                 std_out(f'Found station in {next(iter(set(df[df.codi_eoi==devid].municipi.values)))} with codi_eoi={devid}')
+#                 std_out(f'Found station in {municipi} - {nom_estacio} - {devid} - Type: {area_urbana} - {tipus_estacio}')
+
+#         else:
+#             std_out('Data is empty', 'ERROR')
+#             return None
+
+#         return devid
+
+#     def get_device_sensors(self):
+
+#         if self.sensors is None:
+#             if self.get_device_json() is not None:
+#                 # Get available sensors
+#                 sensors = list(set(self.devicejson.contaminant))
+
+#                 # Put the ids and the names in lists
+#                 self.sensors = dict()
+#                 for sensor in sensors:
+#                     for key in config.blueprints:
+#                         if not search("csic_station",key): continue
+#                         if 'sensors' in config.blueprints[key]:
+#                             for sensor_name in config.blueprints[key]['sensors'].keys():
+#                                 if config.blueprints[key]['sensors'][sensor_name]['id'] == str(sensor):
+#                                     # IDs are unique
+#                                     self.sensors[sensor] = sensor_name
+
+#         return self.sensors
+
+#     def get_device_json(self):
+
+#         if self.devicejson is None:
+#             try:
+#                 s = get(self.API_BASE_URL + f'/?codi_eoi={self.id}')
+#                 if s.status_code == 200 or s.status_code == 201:
+#                     self.devicejson = read_json(StringIO(s.content.decode('utf-8')))
+#                 else:
+#                     std_out('API reported {}'.format(s.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#         return self.devicejson
+
+#     def get_device_timezone(self):
+
+#         if self.timezone is None:
+#             latitude, longitude = self.get_device_lat_long()
+#             # Localize it
+#             # self.timezone = tz_where.tzNameAt(latitude, longitude)
+#             self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
+
+#         std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
+
+#         return self.timezone
+
+#     def get_device_alt(self, update = False):
+
+#         if self.lat is None or self.long is None:
+#             self.get_device_lat_long(update)
+
+#         if self.alt is None or update:
+#             self.alt = get_elevation(_lat = self.lat, _long = self.long)
+
+#         std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
+
+#         return self.alt
+
+#     def get_device_lat_long(self):
+
+#         if self.lat is None or self.long is None:
+#             if self.get_device_json() is not None:
+#                 latitude = longitude = None
+#                 if 'latitud' in self.devicejson.columns:
+#                     latitude = next(iter(set(self.devicejson.latitud)))
+#                     longitude = next(iter(set(self.devicejson.longitud)))
+
+#                 self.lat = latitude
+#                 self.long = longitude
+
+#             std_out ('Device {} is located at {}, {}'.format(self.id, latitude, longitude))
+
+#         return (self.lat, self.long)
+
+#     def get_device_data(self, min_date = None, max_date = None, frequency = '1H', clean_na = None, resample = True):
+#         '''
+#         Based on code snippet from Marc Roig:
+#         # I2CAT RESEARCH CENTER - BARCELONA - MARC ROIG (marcroig@i2cat.net)
+#         '''
+
+#         std_out(f'Requesting data from Dades Obertes API')
+#         std_out(f'Device ID: {self.id}')
+#         self.get_device_sensors()
+#         self.get_device_timezone()
+
+#         request = self.API_BASE_URL
+#         request += f'/?codi_eoi={self.id}'
+
+#         if min_date is not None and max_date is not None:
+#             request += "&$where=data between " + to_datetime(min_date).strftime("'%Y-%m-%dT%H:%M:%S'") \
+#                     + " and " + to_datetime(max_date).strftime("'%Y-%m-%dT%H:%M:%S'")
+#         elif min_date is not None:
+#             request += "&$where=data >= " + to_datetime(min_date).strftime("'%Y-%m-%dT%H:%M:%S'")
+#         elif max_date is not None:
+#             request += "&$where=data < " + to_datetime(max_date).strftime("'%Y-%m-%dT%H:%M:%S'")
+
+#         try:
+#             s = get(request)
+#         except:
+#             print_exc()
+#             std_out('Problem with sensor data from API', 'ERROR')
+#             pass
+#             return None
+
+#         if s.status_code == 200 or s.status_code == 201:
+#             df = read_json(StringIO(s.content.decode('utf-8')))
+#         else:
+#             std_out('API reported {}'.format(s.status_code), 'ERROR')
+#             pass
+#             return None
+
+#         # Filter columns
+#         measures = ['h0' + str(i) for i in range(1,10)]
+#         measures += ['h' + str(i) for i in range(10,25)]
+#         # validations = ['v0' + str(i) for i in range(1,10)]
+#         # validations  += ['v' + str(i) for i in range(10,25)]
+#         new_measures_names = list(range(1,25))
+
+#         columns = ['contaminant', 'data'] + measures# + validations
+#         try:
+#             df_subset = df[columns]
+#             df_subset.columns  = ['contaminant', 'date'] + new_measures_names
+#         except:
+#             print_exc()
+#             std_out('Problem while filtering columns', 'Error')
+#             return None
+#         else:
+#             std_out('Successful filtering', 'SUCCESS')
+
+#         # Pivot
+#         try:
+#             df = DataFrame([])
+#             for contaminant in self.sensors.keys():
+#                 if contaminant not in df_subset['contaminant'].values:
+#                     std_out(f'{contaminant} not in columns. Skipping', 'WARNING')
+#                     continue
+#                 df_temp= df_subset.loc[df_subset['contaminant']==contaminant].drop('contaminant', 1).set_index('date').unstack().reset_index()
+#                 df_temp.columns = ['hours', 'date', contaminant]
+#                 df_temp['date'] = to_datetime(df_temp['date'])
+#                 timestamp_lambda = lambda x: x['date'] + DateOffset(hours=int(x['hours']))
+#                 df_temp['date'] = df_temp.apply( timestamp_lambda, axis=1)
+#                 df_temp = df_temp.set_index('date')
+#                 df[contaminant] = df_temp[contaminant]
+#         except:
+#             # print_exc()
+#             std_out('Problem while filtering columns', 'Error')
+#             pass
+#             return None
+#         else:
+#             std_out('Successful pivoting', 'SUCCESS')
+
+#         df.index = to_datetime(df.index).tz_localize('UTC').tz_convert(self.timezone)
+#         df.sort_index(inplace=True)
+
+#         # Rename
+#         try:
+#             df.rename(columns=self.sensors, inplace=True)
+#         except:
+#             # print_exc()
+#             std_out('Problem while renaming columns', 'Error')
+#             pass
+#             return None
+#         else:
+#             std_out('Successful renaming', 'SUCCESS')
+
+#         # Clean
+#         df = df[~df.index.duplicated(keep='first')]
+#         # Drop unnecessary columns
+#         df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
+#         # Check for weird things in the data
+#         df = df.apply(to_numeric, errors='coerce')
+#         # Resample
+#         if (resample):
+#             df = df.resample(frequency).mean()
+
+#         try:
+#             df = df.reindex(df.index.rename('TIME'))
+#             df = clean(df, clean_na, how = 'all')
+#             self.data = df
+#         except:
+#             std_out('Problem closing up the API dataframe', 'ERROR')
+#             pass
+#             return None
+
+#         std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
+#         return self.data
+
+# class NiluApiDevice(object):
+#     """docstring for IflinkDevice"""
+#     API_BASE_URL='https://sensors.nilu.no/api/'
+#     API_CONNECTOR='sensors.nilu.no'
+
+#     # Docs
+#     # https://sensors.nilu.no/api/doc#configure-sensor-schema
+#     # https://sensors.nilu.no/api/doc#push--sensor-data-by-id
+
+#     def __init__ (self, did):
+
+#         self.id = did
+#         self.timezone = None
+#         self.lat = None
+#         self.long = None
+#         self.alt = None
+#         self.data = None
+#         self.sensors = None
+#         self.devicejson = None
+#         self.last_reading_at = None
+#         self.added_at = None
+#         self._api_url = self.API_BASE_URL + f'sensors/{self.id}'
+
+#     @property
+#     def api_url(self):
+#         return self._api_url
+
+#     @staticmethod
+#     # def new_device(name, description = '', resolution = '1Min', epsg = config._epsg, enabled = True, location = None, sensors = None, dry_run = False):
+#     def new_device(name, location = {}, dry_run = False, **kwargs):
+
+#         '''
+#             Configures the device as a new sensor schema.
+#             This is a one-time configuration and shouldn't be necessary in a recursive way.
+#             More information at: https://sensors.nilu.no/api/doc#configure-sensor-schema
+
+#             Parameters
+#             ----------
+#                 name: string
+#                     Device name
+#                 location: dict
+#                     None
+#                     sensor location. If sensor is moving (i.e. position is not fixed),
+#                     then location must explicitly be set to an empty object: {} when configured. Also see this section.
+#                     location = {
+#                                 'longitude': longitude (double) – sensor east-west position,
+#                                 'latitude': latitude (double) – sensor north-south position,
+#                                 'altitude': altitude (double) – sensor height above sea level
+#                                 }
+#                 dry_run: boolean
+#                     False
+#                     Post the payload to the API or just return it
+#                 **kwargs
+#                 ------
+#                 description: string, optional
+#                     ''
+#                     sensor description
+#                 frequency: string, optional
+#                     '1Min'
+#                     pandas formatted frequency
+#                 epsg: int, optional
+#                     4326
+#                     SRS EPSG code. Defaults to 4326 (WGS84). More info https://spatialreference.org/
+#                 enabled: boolean, optional
+#                     True
+#                     flag indicating if sensor is enabled for data transfer
+
+#                 sensors: dict()
+#                     Dictionary containing necessary information of the sensors to be stored. scdata format:
+#                     {
+#                         'SHORT_NAME': {
+#                                         'desc': 'Channel description',
+#                                         'id': 'sensor SC platform id',
+#                                         'units': 'sensor_recording_units'
+#                                     },
+#                         ...
+#                     }
+#                 ------
+
+#             Returns
+#             -------
+#                 If dry_run, prints out a dict containing the payload and
+#                 returns False
+#                 If not, either False in case of error or a
+#                 dictionary containing:
+#                     sensorid (int) – sensor identifier
+#                     message (string) – HTTP status text
+#                     http-status-code (int) – HTTP status code
+#                     atom (string) – atom URL to sensor
+#         '''
+
+#         API_BASE_URL='https://sensors.nilu.no/api/'
+#         API_CONNECTOR='nilu'
+
+#         if API_CONNECTOR not in config.connectors:
+#             std_out(f'No connector for {API_CONNECTOR}', 'ERROR')
+#             return False
+
+#         if 'NILU_BEARER' not in environ:
+#             std_out('Cannot configure without Auth Bearer', 'ERROR')
+#             return False
+
+#         headers = {'Authorization':'Bearer ' + environ['NILU_BEARER'], 'Content-type': 'application/json'}
+
+#         if name is None:
+#             std_out('Need a name to create a new sensor', 'ERROR')
+#             return False
+#         std_out (f'Configuring IFLINK device named {name}')
+
+#         # Verify inputs
+#         flag_error = False
+
+#         dft_input_params = ['epsg', 'description', 'frequency', 'enabled', 'sensors']
+#         if any([x not in kwargs for x in dft_input_params]):
+#             std_out('Input params not ok for NiluApiDevice', 'ERROR')
+#             return False
+
+#         # EPSG int type
+#         try:
+#             epsg = int(kwargs['epsg'])
+#         except:
+#             std_out('Could not convert epsg to int', 'ERROR')
+#             flag_error = True
+#             pass
+
+#         # Resolution in seconds
+#         if not flag_error:
+#             try:
+#                 resolution_seconds = to_timedelta(kwargs['frequency']).seconds
+#             except:
+#                 std_out('Could not convert resolution to seconds', 'ERROR')
+#                 flag_error = True
+#                 pass
+
+#         # Location
+#         if not flag_error:
+#             try:
+#                 location['longitude']
+#                 location['latitude']
+#                 location['altitude']
+#             except KeyError:
+#                 std_out('Need latitude, longitude and altitude in location dict', 'ERROR')
+#                 flag_error = True
+#                 pass
+
+#         if flag_error: return False
+
+#         # Construct payload
+#         payload = {
+#             "name": name,
+#             "description": kwargs['description'],
+#             "resolution": resolution_seconds,
+#             "srs": {
+#                 "epsg": epsg
+#             },
+#             "enabled": kwargs['enabled']
+#         }
+
+#         payload['location'] = location
+
+#         parameters = []
+#         components = []
+
+#         # Construct
+#         sensors = kwargs['sensors']
+#         for sensor in sensors.keys():
+#             # Check if it's in the configured connectors
+#             _sid = str(sensors[sensor]['id'])
+
+#             if _sid is None:
+#                 std_out(f"Sensor {sensor} id is None. Ignoring", "WARNING")
+#                 return False
+
+#             if _sid not in config.connectors[API_CONNECTOR]['sensors']:
+#                 if config._strict:
+#                     std_out(f"Sensor {sensor} not found in connectors list", "ERROR")
+#                     return False
+#                 std_out(f"Sensor {sensor} not found in connectors list", "WARNING")
+#                 continue
+
+#             units = sensors[sensor]['units']
+
+#             _pjson = {
+#                 "name": sensor,
+#                 "type": "double",
+#                 "doc": f"{sensors[sensor]['desc']} in {units}"
+#             }
+
+#             _cjson = {
+#                 "componentid": config.connectors[API_CONNECTOR]['sensors'][_sid]['id'],
+#                 "unitid": config.connectors[API_CONNECTOR]['sensors'][_sid]['unitid'],
+#                 "binding-path": f"/{sensor}",
+#                 "level": config.connectors[API_CONNECTOR]['sensors'][_sid]['level']
+#             }
+
+#             parameters.append(_pjson)
+#             components.append(_cjson)
+#         # Add timestamp as long
+#         parameters.append({
+#             'name': 'date',
+#             'type': 'long',
+#             'doc': 'Date of measurement'
+#             })
+
+#         # Add the converter (we need to push as input-format)
+#         converters = [{
+#             "input-type": "string",
+#             "output-type": "StringEpochTime",
+#             "target-path": "/date",
+#             "input-args": {
+#                 "input-format": "yyyy-MM-ddTHH:mm:ssZ"
+#             }
+#         }]
+
+#         mapping = [{
+#             "name": "Timestamp",
+#             "target-path": "/date"
+#         }]
+
+#         payload['parameters'] = parameters
+#         payload['components'] = components
+#         payload['converters'] = converters
+#         payload['mapping'] = mapping
+
+#         if dry_run:
+#             std_out(f'Dry run request to: {API_BASE_URL}sensors/configure')
+#             print(dumps(payload, indent = 2))
+#             return False
+
+#         response = post(f'{API_BASE_URL}sensors/configure',
+#                         data = dumps(payload), headers = headers)
+
+
+#         if response.status_code == 200 or response.status_code == 201:
+#             if 'sensorid' in response.json():
+#                 platform_id = str(response.json()['sensorid'])
+#                 platform_url = "https://sensors.nilu.no/api/sensors/" + platform_id
+#                 std_out(f'Device created with: \n{platform_url}', 'SUCCESS')
+#                 return response.json()
+#             else:
+#                 std_out('Response does not contain sensorid field')
+#         else:
+#             std_out(f'{API_BASE_URL} reported {response.status_code}:\n{response.json()}', 'ERROR')
+#             return False
+
+#     def get_device_json(self, update = False):
+#         '''
+#             https://sensors.nilu.no/api/doc#get--sensor-by-id
+#         '''
+#         if 'NILU_BEARER' in environ:
+#             std_out('Auth Bearer found, using it', 'SUCCESS')
+#             headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
+#         else:
+#             std_out('Cannot request without bearer', 'ERROR')
+#             return None
+
+#         if self.devicejson is None or update:
+#             try:
+#                 deviceR = get(f'{self.API_BASE_URL}sensors/{self.id}')
+#                 if deviceR.status_code == 429:
+#                     std_out('API reported {}. Retrying once'.format(deviceR.status_code),
+#                             'WARNING')
+#                     sleep(30)
+#                     deviceR = get(f'{self.API_BASE_URL}sensors/{self.id}', headers = headers)
+
+#                 if deviceR.status_code == 200 or deviceR.status_code == 201:
+#                     self.devicejson = deviceR.json()
+#                 else:
+#                     std_out('API reported {}'.format(deviceR.status_code), 'ERROR')
+#             except:
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+#         return self.devicejson
+
+#     def get_device_description(self, update = False):
+#         if self.get_device_json(update) is not None:
+#             return self.get_device_json()['description']
+#         return None
+
+#     def get_device_lat_long(self, update = False):
+
+#         if self.lat is None or self.long is None or update:
+#             if self.get_device_json(update) is not None:
+#                 latidude = longitude = None
+#                 if 'location' in self.devicejson.keys():
+#                     latitude, longitude = self.devicejson['location']['latitude'], self.devicejson['location']['longitude']
+
+#                 self.lat = latitude
+#                 self.long = longitude
+
+#         std_out ('Device {} is located at {}, {}'.format(self.id, self.lat, self.long))
+
+#         return (self.lat, self.long)
+
+#     def get_device_alt(self, update = False):
+
+#         if self.lat is None or self.long is None:
+#             self.get_device_lat_long(update)
+
+#         if self.alt is None or update:
+#             self.alt = get_elevation(_lat = self.lat, _long = self.long)
+
+#         std_out ('Device {} altitude is {}m'.format(self.id, self.alt))
+
+#         return self.alt
+
+#     def get_device_added_at(self, update = False):
+
+#         if 'NILU_BEARER' in environ:
+#             std_out('Auth Bearer found, using it', 'SUCCESS')
+#             headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
+#         else:
+#             std_out('Cannot request without bearer', 'ERROR')
+#             return None
+
+#         if self.added_at is None or update:
+#             try:
+#                 response = get(f'{self.API_BASE_URL}data/id/{self.id}/minutc', headers = headers)
+#                 if response.status_code == 429:
+#                     std_out('API reported {}. Retrying once'.format(response.status_code),
+#                             'WARNING')
+#                     sleep(30)
+#                     response = get(f'{self.API_BASE_URL}data/id/{self.id}/minutc', headers = headers)
+
+#                 if response.status_code == 200 or response.status_code == 201:
+#                     last_json = response.json()
+#                     first_readings = []
+#                     for item in last_json:
+#                         if 'timestamp_from_epoch' in item: first_readings.append(item['timestamp_from_epoch'])
+
+#                     self.added_at = localise_date(datetime.fromtimestamp(max(list(set(first_readings)))), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+#                 else:
+#                     std_out(f'API reported {response.status_code}: {response.json()}', 'ERROR')
+#             except:
+#                 print_exc()
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#         std_out ('Device {} has last reading at {}'.format(self.id, self.added_at))
+
+#         return self.added_at
+
+#     def get_device_last_reading(self, update = False):
+#         if 'NILU_BEARER' in environ:
+#             std_out('Auth Bearer found, using it', 'SUCCESS')
+#             headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
+#         else:
+#             std_out('Cannot request without bearer', 'ERROR')
+#             return None
+
+#         if self.last_reading_at is None or update:
+#             try:
+#                 response = get(f'{self.API_BASE_URL}data/id/{self.id}/maxutc', headers = headers)
+#                 if response.status_code == 429:
+#                     std_out('API reported {}. Retrying once'.format(response.status_code),
+#                             'WARNING')
+#                     sleep(30)
+#                     response = get(f'{self.API_BASE_URL}data/id/{self.id}/maxutc', headers = headers)
+
+#                 if response.status_code == 200 or response.status_code == 201:
+#                     last_json = response.json()
+#                     last_readings = []
+#                     for item in last_json:
+#                         if 'timestamp_from_epoch' in item: last_readings.append(item['timestamp_from_epoch'])
+
+#                     self.last_reading_at = localise_date(datetime.fromtimestamp(max(list(set(last_readings)))), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+#                 else:
+#                     std_out(f'API reported {response.status_code}: {response.json()}', 'ERROR')
+#             except:
+#                 print_exc()
+#                 std_out('Failed request. Probably no connection', 'ERROR')
+#                 pass
+
+#         std_out ('Device {} has last reading at {}'.format(self.id, self.last_reading_at))
+
+#         return self.last_reading_at
+
+#     def get_device_timezone(self, update = False):
+
+#         if self.timezone is None or update:
+#             latitude, longitude = self.get_device_lat_long(update)
+#             # Localize it
+#             if latitude is not None and longitude is not None:
+#                 # self.timezone = tz_where.tzNameAt(latitude, longitude, forceTZ=True)
+#                 self.timezone = tf.timezone_at(lng=longitude, lat=latitude)
+
+#         std_out ('Device {} timezone is {}'.format(self.id, self.timezone))
+
+#         return self.timezone
+
+#     def get_device_sensors(self, update = False):
+
+#         if self.sensors is None or update:
+#             if self.get_device_json(update) is not None:
+#                 # Get available sensors
+#                 sensors = self.devicejson['components']
+#                 # Put the ids and the names in lists
+#                 self.sensors = dict()
+#                 for sensor in sensors:
+#                     self.sensors[sensor['id']] = sensor['binding-path'][1:]
+
+#         return self.sensors
+
+#     def get_device_data(self, min_date = None, max_date = None, frequency = '1Min', clean_na = None, resample = True):
+#         '''
+#             From
+#             https://sensors.nilu.no/api/doc#get--data-from-utc-timestamp-by-id
+#             From-to
+#             https://sensors.nilu.no/api/doc#get--data-from-utc-timestamp-range-by-id
+#         '''
+
+#         if 'NILU_BEARER' in environ:
+#             std_out('Auth Bearer found, using it', 'SUCCESS')
+#             headers = {'Authorization':'Bearer ' + environ['NILU_BEARER']}
+#         else:
+#             std_out('Cannot request without bearer', 'ERROR')
+#             return None
+
+#         std_out(f'Requesting data from {self.API_BASE_URL}')
+#         std_out(f'Device ID: {self.id}')
+
+#         # Make sure we have the everything we need beforehand
+#         self.get_device_sensors()
+#         self.get_device_timezone()
+#         # This is not available yet
+#         # self.get_device_added_at()
+#         self.get_device_last_reading()
+
+#         if self.timezone is None:
+#             std_out('Device does not have timezone set, skipping', 'WARNING')
+#             return None
+
+#         # Check start date and end date
+#         if min_date is not None:
+#             min_date = localise_date(to_datetime(min_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+#             std_out (f'Min Date: {min_date}')
+#         else:
+#             std_out(f"No min_date specified, requesting all", 'WARNING')
+#             # min_date = localise_date(to_datetime(self.added_at), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+
+#         if max_date is not None:
+#             max_date = localise_date(to_datetime(max_date), 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+#             std_out (f'Max Date: {max_date}')
+#         else:
+#             std_out(f"No max_date specified")
+
+#         # Trim based on actual data available
+#         if min_date is not None and self.last_reading_at is not None:
+#             if min_date > self.last_reading_at:
+#                 std_out(f'Device request would yield empty data (min_date). Returning', 'WARNING')
+#                 return None
+
+#         if max_date is not None and self.added_at is not None:
+#             if max_date < self.added_at:
+#                 std_out(f'Device request would yield empty data (max_date). Returning', 'WARNING')
+#                 return None
+
+#         if max_date is not None and self.last_reading_at is not None:
+#             if max_date > self.last_reading_at:
+#                 std_out('Trimming max_date to last reading', 'WARNING')
+#                 max_date = self.last_reading_at
+
+#         # Print stuff
+#         std_out(f'Device timezone: {self.timezone}')
+#         if not self.sensors.keys():
+#             std_out(f'Device is empty')
+#             return None
+#         else: std_out(f'Sensor IDs: {list(self.sensors.keys())}')
+
+#         df = DataFrame()
+
+#         # Request sensor per ID
+#         request = f'{self.API_BASE_URL}data/id/{self.id}/'
+
+#         if min_date is not None: request += f'fromutc/{min_date}/'
+#         if max_date is not None: request += f'toutc/{max_date}'
+
+#         # Make request
+#         response = get(request, headers = headers)
+
+#         # Retry once in case of 429 after 30s
+#         if response.status_code == 429:
+#             std_out('Too many requests, waiting for 1 more retry', 'WARNING')
+#             sleep (30)
+#             response = get(request, headers = headers)
+
+#         df = DataFrame(response.json()).pivot(index='timestamp_from_epoch', columns='component', values='value')
+#         df.columns.name = None
+#         df.index = localise_date(to_datetime(df.index, unit='s'), self.timezone)
+#         df = df.reindex(df.index.rename('TIME'))
+
+#         # Drop unnecessary columns
+#         df.drop([i for i in df.columns if 'Unnamed' in i], axis=1, inplace=True)
+#         # Check for weird things in the data
+#         df = df.apply(to_numeric, errors='coerce')
+#         # Resample
+#         if (resample):
+#             df = df.resample(frequency).mean()
+#         df = clean(df, clean_na, how = 'all')
+
+#         # Rename columns
+#         d = {}
+#         for component in self.devicejson['components']:
+#             if 'name' in component: d[component['name']]=self.sensors[component['id']]
+#         df = df.rename(columns=d)
+
+#         self.data = df
+
+#         std_out(f'Device {self.id} loaded successfully from API', 'SUCCESS')
+#         return self.data
+
+#     def post_data_to_device(self, df, clean_na = 'drop', chunk_size = None, dry_run = False, max_retries = 2):
+#         '''
+#             POST external data in the IFLINK API, following
+#             https://sensors.nilu.no/api/doc#push--sensor-data-by-id
+#             Parameters
+#             ----------
+#                 df: pandas DataFrame
+#                     Contains data in a DataFrame format.
+#                     Data is posted using the column name of the dataframe
+#                     Data is posted in UTC TZ so dataframe needs to have located
+#                     timestamp
+#                 clean_na: string, optional
+#                     'drop'
+#                     'drop', 'fill'
+#                 chunk_size: None (not used?)
+#                     chunk size to split resulting pandas DataFrame for posting readings
+#                 dry_run: boolean
+#                     False
+#                     Post the payload to the API or just return it
+#                 max_retries: int
+#                     2
+#                     Maximum number of retries per chunk
+#             Returns
+#             -------
+#                 True if the data was posted succesfully
+#         '''
+
+#         if 'NILU_BEARER' not in environ:
+#             std_out('Cannot post without Auth Bearer', 'ERROR')
+#             return False
+
+#         headers = {'Authorization':'Bearer ' + environ['NILU_BEARER'],
+#             'Content-type': 'application/json'}
+
+#         # Clean df of nans
+#         df = clean(df, clean_na, how = 'all')
+
+#         std_out(f'Posting columns to {self.API_BASE_URL}.')
+#         std_out(f'Rest in schema are empty: {list(df.columns)}')
+
+#         # Fill with declared schema to avoid rejection by the API
+#         self.get_device_sensors()
+#         for sensor in self.sensors:
+#             if self.sensors[sensor] not in df.columns:
+#                 df[self.sensors[sensor]] = nan
+
+#         # Split the dataframe in chunks
+#         std_out(f'Splitting post in chunks of size {chunk_size}')
+
+#         for i in trange(len(df.index), file=sys.stdout,
+#                         desc=f"Posting data for {self.id}..."):
+
+#             row = DataFrame(df.loc[df.index[i],:]).T
+#             # Prepare json post
+#             payload = {}
+#             payload['date'] = localise_date(df.index[i], 'UTC').strftime('%Y-%m-%dT%H:%M:%SZ')
+
+#             for column in row.columns:
+#                 payload[column] = row.loc[df.index[i], column]
+
+#             if dry_run:
+#                 std_out(f'Dry run request to: {self.API_BASE_URL}sensors/{self.id}/inbound')
+#                 return dumps(payload, indent = 2, cls = NpEncoder)
+
+#             post_ok = False
+#             retries = 0
+
+#             while post_ok == False and retries < max_retries:
+
+#                 response = post(f'{self.API_BASE_URL}sensors/{self.id}/inbound',
+#                             data = dumps(payload, cls = NpEncoder), headers = headers)
+
+#                 if response.status_code == 200 or response.status_code == 201:
+#                     post_ok = True
+#                     break
+#                 else:
+#                     retries += 1
+#                     std_out (f'Chunk ({i+1}/{len(df.index)}) post failed. \
+#                            API responded {response.status_code}.\
+#                             Retrying ({retries}/{max_retries}', 'WARNING')
+
+#             if (not post_ok) or (retries == max_retries):
+#                 std_out (f'Chunk ({i+1}/{len(df.index)}) post failed. \
+#                        API responded {response.status_code}.\
+#                         Reached max_retries', 'ERROR')
+#                 return False
 
-        return True
+#         return True
```

### Comparing `scdata-0.9.1/scdata/test/__init__.py` & `scdata-1.0.0/scdata/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,434 +1,326 @@
 """ Main implementation of the class Test """
 
 from os import makedirs
 from os.path import join, exists
 from shutil import copyfile, rmtree, make_archive
 from traceback import print_exc
-from datetime import datetime
+from datetime import datetime, timedelta
 import yaml
 import json
 import folium
+import asyncio
 from re import sub
+from pydantic import TypeAdapter, BaseModel, ConfigDict, model_serializer
+from typing import Optional, List, Dict, Any
 
-from scdata.utils import std_out, get_tests_log
-from scdata.io import read_csv_file
+from scdata.tools.custom_logger import logger
+from scdata.tools.date import localise_date
+from scdata.tools.find import find_by_field
+from scdata.io import read_csv_file, export_csv_file
 from scdata._config import config
-from scdata.device import Device
-from scdata.test.plot.plot_tools import to_png_b64
+from scdata import Device
+from scdata.models import TestOptions
 
-class Test(object):
+class Test(BaseModel):
 
-    from .plot import (ts_plot, ts_iplot, device_metric_map, path_plot,
-                        scatter_plot, scatter_iplot, ts_scatter,
-                        heatmap_plot, heatmap_iplot,
-                        box_plot, ts_dendrogram,
-                        ts_dispersion_plot, ts_dispersion_grid,
-                        scatter_dispersion_grid)
-                        #, report_plot, cat_plot, violin_plot)
+    from .plot import (ts_plot, device_metric_map, path_plot,
+        scatter_plot, ts_scatter,
+        # ts_iplot, scatter_iplot, heatmap_iplot,
+        heatmap_plot,
+        box_plot, ts_dendrogram,
+        ts_dispersion_plot, ts_dispersion_grid,
+        scatter_dispersion_grid)
+        #, report_plot, cat_plot, violin_plot)
 
     if config._ipython_avail:
         from .plot import ts_uplot, ts_dispersion_uplot
     from .export import to_csv, to_html
-    from .load import load
-    from .utils import (combine, prepare, dispersion_analysis,
-                        dispersion_summary, get_common_channels,
-                        gaps_check)
-
-    def __init__(self, name):
-
-        self.options = {
-                        'cached_data_margin': config.data['cached_data_margin'],
-                        'load_cached_api': config.data['load_cached_api'],
-                        'store_cached_api': config.data['store_cached_api'],
-                        'clean_na': config.data['clean_na']
-                        }
-
-        if self.__check_tname__(name): self.__set_tname__(name)
-
-        self.details = dict()
-        self.devices = dict()
-        self.descriptor = {'id': self.full_name}
-
-        self._default_fields = {
-                                'id': '',
-                                'comment': '',
-                                'notes': '',
-                                'project': '',
-                                'author': '',
-                                'commit': '',
-                                'devices': dict(),
-                                'report': '',
-                                'type_test': ''
-                                }
+    from .tools import combine, prepare, history
+    from .dispersion import dispersion_analysis, dispersion_summary
+    from .checks import get_common_channels, gaps_check
+
+    model_config = ConfigDict(arbitrary_types_allowed = True)
+    name: str
+    path: str = ''
+    devices: List[Device] = []
+    options: TestOptions = TestOptions()
+    # TODO - Define test types based on enum
+    # dev
+    # deployment...
+    type: str = 'dev'
+    new: bool = False
+    loaded: bool = False
+    force_recreate: bool = False
+    # results: List[TestResult] = []
+
+    def model_post_init(self, __context) -> None:
+
+        if self.__check_tname__(self.name):
+            self.__set_tname__(self.name)
+
+        if self.new or self.force_recreate:
+            logger.info('New test')
+            self.create()
+        else:
+            with open(join(self.path, 'test.json'), 'r') as file:
+                tj = json.load(file)
 
-        # Dict for report
-        self.content = dict()
+            self.devices = TypeAdapter(List[Device]).validate_python(tj['devices'])
+            self.options = TypeAdapter(TestOptions).validate_python(tj['options'])
+            print (tj['meta'])
+            self.type = tj['meta']['type']
+            if self.name != tj['meta']['name']:
+                raise ValueError('Name not matching')
 
-        # Dispersion analysis
-        self.dispersion_df = None
-        self._dispersion_summary = None
-        self.common_channels = None
+            if self.path != tj['meta']['path']:
+                raise ValueError('Path not matching')
 
-    def __str__(self):
-        return self.full_name
+        # TODO
+        # Dispersion analysis
+        # self.dispersion_df = None
+        # self._dispersion_summary = None
+        # self.common_channels = None
 
+        logger.info(f'Test {self.name} initialized')
 
-    @property
-    def default_fields(self):
-        return self._default_fields
-
-    def __set_options__(self, options):
-
-        test_options = [
-            'load_cached_api',
-            'store_cached_api',
-            'clean_na',
-            'frequency',
-            'min_date',
-            'max_date',
-            'resample'
-        ]
-
-        for option in test_options:
-            if option in options.keys():
-                self.options[option] = options[option]
+    def __str__(self):
+        return self.__full_name__
 
     def __set_tname__(self, name):
         current_date = datetime.now()
-        self.full_name = f'{current_date.year}_{str(current_date.month).zfill(2)}_{name}'
+        self.name = f'{current_date.year}_{str(current_date.month).zfill(2)}_{name}'
         self.path = join(config.paths['processed'], str(current_date.year), \
-                str(current_date.month).zfill(2), self.full_name)
-        std_out (f'Full Name: {self.full_name}')
+                str(current_date.month).zfill(2), self.name)
+
+        logger.info (f'Full Name: {self.name}')
 
     def __check_tname__(self, name):
-        test_log = get_tests_log()
+        test_log = self.history()
         test_logn = list(test_log.keys())
 
         if not any([name in tlog for tlog in test_logn]):
+            logger.info ('Test is new')
+            self.new = True
             return name
         else:
+            self.new = False
             undef_test = True
-
             while undef_test:
-
                 # Wait for input
-                poss_names = list()
-                std_out ('Possible tests found', force = True)
+                possible_names = list()
+                logger.info ('Possible tests found:')
                 for ctest in test_logn:
                     if name in ctest:
-                        poss_names.append(test_logn.index(ctest) + 1)
-                        std_out (str(test_logn.index(ctest) + 1) + ' --- ' + ctest, force = True)
-                std_out ('// --- \\\\', force = True)
-                if len(poss_names) == 1:
-                    which_test = str(poss_names[0])
+                        possible_names.append(test_logn.index(ctest) + 1)
+                        logger.info (str(test_logn.index(ctest) + 1) + ' --- ' + ctest)
+                logger.info ('// --- \\\\')
+                if len(possible_names) == 1:
+                    which_test = str(possible_names[0])
                 else:
                     which_test = input('Similar tests found, please select one or input other name [New]: ')
 
                 if which_test == 'New':
                     new_name = input('Enter new name: ')
                     break
                 elif which_test.isdigit():
-                    if int(which_test) in poss_names:
-                        self.full_name = test_logn[int(which_test)-1]
-                        self.path = test_log[self.full_name]['path']
-                        std_out(f'Test full name, {self.full_name}', force = True)
+                    if int(which_test) in possible_names:
+                        self.name = test_logn[int(which_test)-1]
+                        self.path = test_log[self.name]['path']
+                        logger.info(f'Test full name, {self.name}')
                         return False
                     else:
-                        std_out("Type 'New' for other name, or test number in possible tests", 'ERROR')
+                        logger.error("Type 'New' for other name, or test number in possible tests")
                 else:
-                    std_out("Type 'New' for other name, or test number", 'ERROR')
-            if self.__check_tname__(new_name): self.__set_tname__(new_name)
+                    logger.error("Type 'New' for other name, or test number")
 
-    def create(self, force = False):
+            if self.__check_tname__(new_name):
+                self.__set_tname__(new_name)
+
+    def create(self):
         # Create folder structure under data subdir
         if not exists(self.path):
-            std_out('Creating new test')
+            logger.info('Creating new test')
             makedirs(self.path)
         else:
-            if not force:
-                std_out (f'Test already exists with this name. Full name: {self.full_name}. Maybe force = True?', 'ERROR')
+            if not self.force_recreate:
+                logger.error (f'Test already exists with this name. \
+                    Full name: {self.name}. Maybe force_recreate = True?')
                 return None
             else:
-                std_out (f'Overwriting test. Full name: {self.full_name}')
+                logger.info (f'Overwriting test. Full name: {self.name}')
 
-        self.__update_descriptor__()
-        self.__preprocess__()
+        # TODO Remove
+        # self.__preprocess__()
+        self.__dump__()
 
-        std_out (f'Test creation finished. Name: {self.full_name}', 'SUCCESS')
-        return self.full_name
+        logger.info (f'Test creation finished. Name: {self.name}')
+        return self.name
 
     def purge(self):
         # Check if the folder structure exists
         if not exists(self.path):
-            std_out('Test folder doesnt exist', 'ERROR')
+            logger.error('Test folder doesnt exist')
         else:
-            std_out (f'Purging cached directory in: {self.path}')
+            logger.info (f'Purging cached directory in: {self.path}')
             try:
                 rmtree(join(self.path, 'cached'))
             except:
-                std_out('Error while purging directory', 'ERROR')
+                logger.error('Error while purging directory')
                 pass
             else:
-                std_out (f'Purged cached folder', 'SUCCESS')
+                logger.info (f'Purged cached folder')
                 return True
         return False
 
-    def add_details(self, details):
-        '''
-            details: a dict containing the information about the test. Minimum of:
-                - project
-                - commit
-                - author
-                - test_type
-                - report
-                - comment
-        '''
-
-        for detail in details.keys(): self.details[detail] = details[detail]
-
-    def add_devices_list(self, devices_list, blueprint):
-        '''
-            Convenience method to add devices from a list of api devices with a certain blueprint
-            Params:
-                devices_list: list
-                Contains devices ids (str or int)
-
-                blueprint: String
-                Blueprint name
-        '''
-        if blueprint is None: return False
-
-        if blueprint not in config.blueprints.keys():
-            std_out(f'Blueprint {blueprint} not in blueprints', 'ERROR')
-            return False
-
-        for device in devices_list:
-            self.add_device(Device(blueprint = blueprint , descriptor = {'source': 'api',
-                                                                            'id': str(device)
-                                                                            }
-                                    )
-            )
-        return True
-
-    def add_device(self, device):
-        '''
-            Adds a device to the test. The device has to be an instance of 'scdata.device.Device'
-        '''
-        if device.id not in self.devices.keys():
-            self.devices[device.id] = device
-            return True
-        else:
-            std_out(f'Device {device.id} is duplicated', 'WARNING')
-            return False
-
-    def add_content(self, title, figure = None, text = None, iframe = None, show_title = True, force = False):
-        '''
-            Adds content for the rendered flask template of the test. Content is a dict()
-            which contains a key per title (replacing ' ' with '_') and the content in it.
-
-            Parameters
-            ----------
-            title
-                None
-                Content title. Needs to not be None
-            figure
-                None
-                matplotlib or similar figure that can be converted to base64
-            text
-                None
-                Text to be converted to <p> html tag with additional inner html (jinja2 safe rendered)
-            iframe
-                None
-                HTML iframe contanining anything
-            show_title
-                True
-                show title in HTML <h3> tag
-            force
-                If already added content with this title
-
-            Returns
-            ----------
-            True if content added, false otherwise
-
-        '''
-
-        title_cor = sub('\W|^(?=\d)','_', title)
-
-        if title_cor not in self.content or force:
-            self.content[title_cor] = dict()
-
-            if title is not None:
-                self.content[title_cor]['title'] = title
-            if figure is not None:
-                self.content[title_cor]['image'] = to_png_b64(figure)
-            if text is not None:
-                self.content[title_cor]['text'] = text
-            if iframe is not None:
-                self.content[title_cor]['iframe'] = iframe
-
-            self.content[title_cor]['show_title'] = show_title
-
-            std_out('Item added', 'SUCCESS')
-            return True
-
-        else:
-            std_out('Item not added as its already in content', 'ERROR')
-            return False
+    def get_device(self, device_id):
+        did = find_by_field(self.devices, device_id, 'id')
+        if did is None:
+            logger.error(f'Device {device_id} is not in test')
+        return did
 
+    # TODO - Do we want this with asyncio?
     def process(self, only_new = False):
         '''
         Calculates all the metrics in each of the devices
         Returns True if done OK
         '''
         process_ok = True
-        for device in self.devices: process_ok &= self.devices[device].process(only_new = only_new)
+        for device in self.devices:
+            process_ok &= device.process(only_new = only_new)
 
         # Cosmetic output
-        if process_ok: std_out(f'Test {self.full_name} processed', 'SUCCESS')
-        else: std_out(f'Test {self.full_name} not processed', 'ERROR')
+        if process_ok: logger.info(f'Test {self.name} processed')
+        else: logger.error(f'Test {self.name} not processed')
 
         return process_ok
 
-    def __preprocess__(self):
-        '''
-            Processes the files for one test, given that the devices and details have been added
-        '''
-
-        std_out('Processing files')
-
-        def get_raw_files():
-                list_raw_files = []
-                for device in self.devices.keys():
-                    if self.devices[device].source == 'csv':
-                        list_raw_files.append(self.devices[device].raw_data_file)
-
-                return list_raw_files
-
-        def copy_raw_files(_raw_src_path, _raw_dst_path, _list_raw_files):
-            try:
-
-                for item in _list_raw_files:
-                    s = join(_raw_src_path, item)
-                    d = join(_raw_dst_path, item.split('/')[-1])
-                    copyfile(s, d)
-
-                std_out('Copy raw files: OK', 'SUCCESS')
-
-                return True
-
-            except:
-                std_out('Problem copying raw files', 'ERROR')
-                print_exc()
-                return False
-
-        def date_parser(s, a):
-            return parser.parse(s).replace(microsecond=int(a[-3:])*1000)
-
-        # Define paths
-        raw_src_path = join(config.paths['data'], 'raw')
-        raw_dst_path = join(self.path, 'raw')
+    # # TODO - CHECK FOR CSV FILES
+    # def __preprocess__(self):
+    #     '''
+    #     Processes the files for one test, given that the devices and details have been added
+    #     '''
+
+    #     logger.info('Processing files...')
+    #     def get_raw_files():
+    #             list_raw_files = []
+    #             for device in self.devices:
+    #                 if device.source.type == 'sd-csv':
+    #                     list_raw_files.append(device.source.files.raw_data_file)
+
+    #             return list_raw_files
+
+    #     def copy_raw_files(_raw_src_path, _raw_dst_path, _list_raw_files):
+    #         try:
+
+    #             for item in _list_raw_files:
+    #                 s = join(_raw_src_path, item)
+    #                 d = join(_raw_dst_path, item.split('/')[-1])
+    #                 copyfile(s, d)
+
+    #             logger.info('Copy raw files: OK')
+
+    #             return True
+
+    #         except:
+    #             logger.error('Problem copying raw files')
+    #             print_exc()
+    #             return False
+
+    #     def date_parser(s, a):
+    #         return parser.parse(s).replace(microsecond=int(a[-3:])*1000)
+
+    #     # Define paths
+    #     raw_src_path = join(config.paths['data'], 'raw')
+    #     raw_dst_path = join(self.path, 'raw')
 
-        # Create path
-        if not exists(raw_dst_path): makedirs(raw_dst_path)
+    #     # Create path
+    #     if not exists(raw_dst_path): makedirs(raw_dst_path)
 
         # Get raw files
-        list_raw_files = get_raw_files()
+        # list_raw_files = get_raw_files()
 
         # Copy raw files and process data
-        if len(list_raw_files):
-            if copy_raw_files(raw_src_path, raw_dst_path, list_raw_files):
-
-                # Process devices
-                for device_name in self.devices.keys():
-
-                    device = self.devices[device_name]
-
-                    if device.source == 'csv':
-
-                        std_out ('Processing csv from device {}'.format(device.id))
-                        src_path = join(raw_src_path, device.raw_data_file)
-                        dst_path = join(self.path, device.processed_data_file)
-
-                        # Load csv file, only localising and removing
-                        df = read_csv_file(file_path = src_path,
-                                            timezone = device.timezone,
-                                            frequency = device.frequency,
-                                            clean_na = None,
-                                            index_name = device.sources[device.source]['index'],
-                                            skiprows = device.sources[device.source]['header_skip'],
-                                            sep = device.sources[device.source]['sep'],
-                                            tzaware = device.sources[device.source]['tz-aware'],
-                                            resample = device.resample
-                                            )
-                        df.index.rename(config._csv_defaults['index_name'], inplace=True)
-                        df.to_csv(dst_path, sep=config._csv_defaults['sep'])
-
-            std_out('Files preprocessed')
-        std_out(f'Test {self.full_name} path: {self.path}')
-
-    def __update_descriptor__(self):
-        if self.descriptor == {}: self.std_out('No descriptor file to update')
-
-        for field in self._default_fields:
-            if field not in self.descriptor.keys(): self.descriptor[field] = self._default_fields[field]
-
-        # Add details to descriptor, or update them if there is anything in details
-        for detail in self.details.keys(): self.descriptor[detail] = self.details[detail]
-        # Add devices to descriptor
-        for device_name in self.devices.keys():
+        # if len(list_raw_files):
+        #     if copy_raw_files(raw_src_path, raw_dst_path, list_raw_files):
 
-            device = self.devices[device_name]
-
-            if device.source == 'csv':
-                device.processed_data_file = self.full_name + '_' + str(device.id) + '.csv'
-
-            dvars = vars(device).copy()
-            for discvar in config._discvars:
-                if discvar in dvars:
-                    dvars.pop(discvar)
-
-            self.descriptor['devices'][device.id] = dvars
-
-        # Create yaml with test description
-        with open(join(self.path, 'test_description.yaml'), 'w') as yaml_file:
-            yaml.dump(self.descriptor, yaml_file)
-
-        std_out ('Descriptor file updated')
+        #         # Process devices
+        #         for device in self.devices:
+        #             ## Make this for CSV devices
+        #             if device.source.type == 'sd-csv':
+
+        #                 logger.info (f'Processing csv from device {device.id}...')
+        #                 src_path = join(raw_src_path, device.raw_data_file)
+        #                 dst_path = join(self.path, device.processed_data_file)
+
+        #                 # Load csv file, only localising and removing
+        #                 df = read_csv_file(file_path = src_path,
+        #                                     timezone = device.timezone,
+        #                                     frequency = device.frequency,
+        #                                     clean_na = None,
+        #                                     index_name = device.sources[device.source]['index'],
+        #                                     skiprows = device.sources[device.source]['header_skip'],
+        #                                     sep = device.sources[device.source]['sep'],
+        #                                     tzaware = device.sources[device.source]['tz-aware'],
+        #                                     resample = device.resample
+        #                                     )
+        #                 df.index.rename(config._csv_defaults['index_name'], inplace=True)
+        #                 df.to_csv(dst_path, sep=config._csv_defaults['sep'])
+
+            # logger.info('Files preprocessed')
+        # logger.info(f'Test {self.name} path: {self.path}')
+
+    @model_serializer
+    def ser_model(self) -> Dict[str, Any]:
+
+        return {
+            'meta': {
+                'name': self.name,
+                'path': self.path,
+                'type': self.type
+            },
+            'options': self.options.model_dump(),
+            'devices': [{'params': device.params.model_dump(),
+                         'metrics': [metric.model_dump() for metric in device.metrics],
+                         'source': device.source.model_dump(),
+                         'blueprint': device.blueprint}
+                         for device in self.devices]
+        }
+
+    def __dump__(self):
+        with open(join(self.path, 'test.json'), 'w') as file:
+            json.dump(self.ser_model(), file, indent=4)
 
     def compress(self, cformat = 'zip', selection = 'full'):
         '''
-            Compress the test folder (or selected folder) into a defined
-            format in the test.path directory
-
-            Parameters
-            ----------
-            cformat
-                'zip'
-                String. Valid shutil.make_archive input: 'zip', 'tar',
-                'gztar', 'bztar', 'xztar'
-            selection
-                'full'
-                String. Selection of folders to compress. Either 'full',
-                'cached' or 'raw'. If 'full', compresses the whole test,
-                including test_description.yaml
-
-            Returns
-            ----------
-            True if all good, False otherwise
+        Compress the test folder (or selected folder) into a defined
+        format in the test.path directory
 
+        Parameters
+        ----------
+        cformat
+            'zip'
+            String. Valid shutil.make_archive input: 'zip', 'tar',
+            'gztar', 'bztar', 'xztar'
+        selection
+            'full'
+            String. Selection of folders to compress. Either 'full',
+            'cached' or 'raw'. If 'full', compresses the whole test,
+            including test_description.yaml
+
+        Returns
+        ----------
+        True if all good, False otherwise
         '''
-
-
         if cformat not in ['zip', 'tar', 'gztar', 'bztar', 'xztar']:
-            std_out('Invalid format', 'ERROR')
+            logger.error('Invalid format')
             return False
 
         if selection not in ['full', 'cached', 'raw']:
-            std_out('Invalid selection (valid options: full, cached, raw', 'ERROR')
+            logger.error('Invalid selection (valid options: full, cached, raw')
             return False
 
         if selection == 'full':
             _root_dir = self.path
         elif selection == 'cached':
             _root_dir = join(self.path, 'cached')
         elif selection == 'raw':
@@ -437,7 +329,47 @@
         fname_t = join(self.path.strip(f'{self.full_name}')[:-1], self.full_name + f'_{selection}')
         make_archive(fname_t, cformat, root_dir=_root_dir)
 
         fname = fname_t + '.' + cformat
         if not exists(fname): return False
 
         return fname
+
+    def cache(self):
+        logger.info(f'Caching files...')
+        for device in self.devices:
+            logger.info(f'Caching files for {device.id}...')
+
+            cached_file_path = join(self.path, 'cached')
+            if not exists(cached_file_path):
+                logger.info('Creating path for exporting cached data')
+                makedirs(cached_file_path)
+
+            if device.export(cached_file_path, forced_overwrite = True, file_format = 'csv'):
+                logger.info(f'Device {device.id} cached')
+
+        return all([exists(join(self.path, 'cached', f'{d.id}.csv')) for d in self.devices])
+
+    async def load(self):
+        '''
+        Loads the test data and the different devices.
+
+        Returns
+        ----------
+            None
+        '''
+        logger.info('Loading test...')
+
+        for device in self.devices:
+            # Check for cached data
+            cached_file_path = ''
+            if self.options.cache:
+                tentative_path = join(self.path, 'cached', f'{device.id}.csv')
+                if exists(tentative_path): cached_file_path = tentative_path
+            # Load device (no need to go async, it's fast enough)
+            await device.load(cache=cached_file_path)
+
+        logger.info('Test load done')
+        if self.options.cache: self.cache()
+
+        self.loaded = all([d.loaded for d in self.devices])
+        return self.loaded
```

### Comparing `scdata-0.9.1/scdata/test/export/templates/sc_template.html` & `scdata-1.0.0/scdata/test/export/templates/sc_template.html`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/test/export/to_file.py` & `scdata-1.0.0/scdata/test/export/to_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ''' Implementation of csv and html export for devices in test '''
 
 from os.path import join, dirname, exists
 from os import makedirs
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 import flask
 from re import sub
 
 def to_csv(self, path = None, forced_overwrite = False):
     """
     Exports devices in test to desired path
     Parameters
@@ -16,26 +16,28 @@
             The path (directory) to export the csv(s) into. If None, exports to test_path/processed/
         forced_overwrite: boolean
         	False
             To overwrite existing files
     Returns
     -------
         True if export successul
-    """	
+    """
     export_ok = True
 
     if path is None: epath = join(self.path, 'processed')
     else: epath = path
 
     # Export to csv
-    for device in self.devices.keys():
-        export_ok &= self.devices[device].export(epath, forced_overwrite = forced_overwrite)
+    for device in self.devices:
+        export_ok &= device.export(epath, forced_overwrite = forced_overwrite)
 
-    if export_ok: std_out(f'Test {self.full_name} exported successfully', 'SUCCESS')
-    else: std_out(f'Test {self.full_name} not exported successfully', 'ERROR')
+    if export_ok:
+        logger.info(f'Test {self.name} exported successfully')
+    else:
+        logger.error(f'Error while exporting test: {self.name}')
 
     return export_ok
 
 def to_html(self, title = 'Your title here', template = 'sc_template.html', path = None,
             details = True, devices_summary = True, full = True, header = True):
     '''
     Generates an html description for the test
@@ -61,30 +63,32 @@
             True
             Whether to return a full html or not
         header: bool
             True
             Whether to include a header or not
     Returns
     ----------
-        rendered: 
+        rendered:
             flask rendered template
     '''
+    # TODO - Update or remove
+    raise NotImplementedError
 
     # Find the path to the html templates directory
     template_folder = join(dirname(__file__), 'templates')
 
     if path is None: path = join(self.path, 'export')
 
-    if not exists(path): 
-        std_out('Creating folder for test export')
+    if not exists(path):
+        logger.info('Creating folder for test export')
         makedirs(path)
 
-    filename = join(path, f'{self.full_name}.html')
-    
-    docname = sub('.','_', self.full_name)
+    filename = join(path, f'{self.name}.html')
+
+    docname = sub('.','_', self.name)
     app = flask.Flask(docname, template_folder = template_folder)
 
     with app.app_context():
         rendered = flask.render_template(
             template,
             title = title,
             descriptor = self.descriptor,
@@ -93,11 +97,11 @@
             devices_summary = devices_summary,
             full = full,
             header = header
         )
 
     with open(filename, 'w') as handle:
         handle.write(rendered)
-        
-    std_out (f'File saved to: {filename}', 'SUCCESS')
+
+    logger.info (f'File saved to: {filename}')
 
     return filename, rendered
```

### Comparing `scdata-0.9.1/scdata/test/plot/__init__.py` & `scdata-1.0.0/scdata/test/plot/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .ts_plot import ts_plot
-from .ts_iplot import ts_iplot
+# from .ts_iplot import ts_iplot
 from scdata._config import config
 if config._ipython_avail:
     from .ts_uplot import ts_uplot
     from .ts_dispersion_uplot import ts_dispersion_uplot
 from .scatter_plot import scatter_plot
-from .scatter_iplot import scatter_iplot
+# from .scatter_iplot import scatter_iplot
 from .ts_scatter import ts_scatter
 from .heatmap_plot import heatmap_plot
-from .heatmap_iplot import heatmap_iplot
+# from .heatmap_iplot import heatmap_iplot
 from .box_plot import box_plot
 from .ts_dendrogram import ts_dendrogram
 from .maps import device_metric_map, path_plot
 from .ts_dispersion_plot import ts_dispersion_plot
 from .ts_dispersion_grid import ts_dispersion_grid
 from .scatter_dispersion_grid import scatter_dispersion_grid
 # from .tools import (target_diagram, scatter_diagram)
```

### Comparing `scdata-0.9.1/scdata/test/plot/box_plot.py` & `scdata-1.0.0/scdata/test/plot/box_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from matplotlib import style
 from seaborn import set_palette, boxplot
 # import seaborn as sns
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data, groupby_session
 
 def box_plot(self, **kwargs):
     """
     Plots heatmap in seaborn plot, based on period binning
     Parameters
@@ -27,31 +28,32 @@
         formatting: dict
             Name of auxiliary electrode found in dataframe. Defaults in config._boxplot_def_fmt
     Returns
     -------
         Matplotlib figure
     """
 
-    if config.framework == 'jupyterlab': plt.ioff();
-    plt.clf();
+    if config.framework == 'jupyterlab':
+        plt.ioff()
+    plt.clf()
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._boxplot_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._boxplot_def_fmt['mpl'], kwargs['formatting'])
 
     # if 'fontsize' in formatting:
     #     sns.set(rc = {'font.size': formatting['fontsize']})
```

### Comparing `scdata-0.9.1/scdata/test/plot/heatmap_iplot.py` & `scdata-1.0.0/scdata/test/plot/heatmap_iplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from plotly.graph_objs import Heatmap, Layout, Figure
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data, groupby_session
 from plotly.offline import iplot
 
 def heatmap_iplot(self, **kwargs):
     """
     Plots heatmap in plotly interactive plot
     Parameters
     ----------
         traces: dict
             Data for the plot, with the format:
             "traces":  {"1": {"devices": '8019043',
                              "channel" : "PM_10"}
-                        }      
-        options: dict 
+                        }
+        options: dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Name of auxiliary electrode found in dataframe. Defaults in config._heatmap_def_fmt
     Returns
     -------
         Plotly figure
     """
     if config.framework == 'jupyterlab': renderers.default = config.framework
 
-    if 'traces' not in kwargs: 
-        std_out('No traces defined', 'ERROR')
+    if 'traces' not in kwargs:
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._heatmap_def_fmt['plotly']
     else:
         formatting = dict_fmerge(config._heatmap_def_fmt['plotly'], kwargs['formatting'])
 
     # Make it standard
     for trace in traces:
         if 'subplot' not in trace: traces[trace]['subplot'] = 1
 
     # Get dataframe
     df, subplots = prepare_data(self, traces, options)
     n_subplots = len(subplots)
 
-    gskwags = {'frequency_hours': formatting['frequency_hours']}    
+    gskwags = {'frequency_hours': formatting['frequency_hours']}
 
     dfgb, labels, yaxis, channel = groupby_session(df, **gskwags)
     xticks = [i.strftime("%Y-%m-%d") for i in dfgb.resample(formatting['session']).mean().index]
 
      # Data
     data = [
         Heatmap(
```

### Comparing `scdata-0.9.1/scdata/test/plot/heatmap_plot.py` & `scdata-1.0.0/scdata/test/plot/heatmap_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from matplotlib import style
 from seaborn import set_palette, heatmap
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data, groupby_session
 
 def heatmap_plot(self, **kwargs):
     """
     Plots heatmap in seaborn plot, based on period binning
     Parameters
@@ -21,31 +22,32 @@
         formatting: dict
             Name of auxiliary electrode found in dataframe. Defaults in config._heatmap_def_fmt
     Returns
     -------
         Matplotlib figure
     """
 
-    if config.framework == 'jupyterlab': plt.ioff();
-    plt.clf();
+    if config.framework == 'jupyterlab':
+        plt.ioff()
+    plt.clf()
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._heatmap_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._heatmap_def_fmt['mpl'], kwargs['formatting'])
 
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
```

### Comparing `scdata-0.9.1/scdata/test/plot/maps.py` & `scdata-1.0.0/scdata/test/plot/maps.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from folium import (Map, Marker, Circle, GeoJson, DivIcon,
                     GeoJsonTooltip, GeoJsonPopup)
 
 from folium.plugins import MiniMap, TimestampedGeoJson
 from math import isnan, floor, ceil
 from traceback import print_exc
 from pandas import cut, date_range
-from scdata.utils import dict_fmerge, clean, std_out
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.cleaning import clean
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 from numpy import linspace, nan
 from branca import element
 from jinja2 import Template, FileSystemLoader, Environment
 import json
 from os.path import dirname, join
 
@@ -241,15 +243,15 @@
 
         # Get lat, long
         try:
             self.devices[str(device)].api_device.get_device_lat_long()
             _lat = self.devices[str(device)].api_device.lat
             _long = self.devices[str(device)].api_device.long
         except AttributeError:
-            std_out(f'Cannot retrieve [lat, long] from device {device}', 'WARNING')
+            logger.warning(f'Cannot retrieve [lat, long] from device {device}')
             pass
             continue
 
         if _lat is None or _long is None: continue
 
         # Resample
         try:
@@ -369,32 +371,32 @@
     features = []
     if devices == 'all':
         mdev = self.devices
     else:
         mdev = list()
         for device in devices:
             if device in self.devices: mdev.append(device)
-            else: std_out(f'Device {device} not found, ignoring', 'WARNING')
+            else: logger.warning(f'Device {device} not found, ignoring')
 
     if len(mdev) == 0:
-        std_out('Requested devices not in test', 'ERROR')
+        logger.error('Requested devices not in test')
         return None
 
     for device in mdev:
         chs = ['GPS_LAT','GPS_LONG']
         if channel is not None:
             if channel not in self.devices[str(device)].readings.columns:
-                std_out(f'Channel {channel} not in columns: {self.devices[str(device)].readings.columns}', 'ERROR')
+                logger.error(f'Channel {channel} not in columns: {self.devices[str(device)].readings.columns}')
                 return None
 
             # Get bins
             minmax = False
             if not options['minmax']:
                 if all([key not in channel for key in config._channel_bins]):
-                    std_out(f'Requested channel {channel} not in config mapped bins {config._channel_bins.keys()}.Using min/max mapping', 'WARNING')
+                    logger.warning(f'Requested channel {channel} not in config mapped bins {config._channel_bins.keys()}.Using min/max mapping')
                     minmax = True
             else:
                 minmax = True
 
             if minmax:
                 bins = linspace(self.devices[str(device)].readings[channel].min(),
                     self.devices[str(device)].readings[channel].max(),
@@ -433,16 +435,16 @@
         for date in dfc.index:
             if date == dfc.index[-1]: break
             times = []
 
             color = str(dfc.loc[date, 'COLOR'])
             if color == 'nan' or isnan(dfc.loc[date, 'GPS_LONG'])\
             or isnan(dfc.loc[date, 'GPS_LAT']):
-                std_out(f'Skipping point {date}', 'WARNING'); continue
-
+                logger.warning(f'Skipping point {date}')
+                continue
             geometry = {
                 'type': 'LineString',
                 'coordinates': [[dfc.loc[date, 'GPS_LONG'],
                     dfc.loc[date, 'GPS_LAT']],
                     [dfc.loc[date+dfc.index.freq, 'GPS_LONG']
                     ,dfc.loc[date+dfc.index.freq, 'GPS_LAT']]],
                 }
@@ -539,15 +541,15 @@
             style="""
                 background-color: #F0EFEF;
                 border: 1px solid gray;
                 border-radius: 1px;
                 box-shadow: 2px;
             """,
             max_width=800,
-        );
+        )
 
         GeoJson(featurecol,
             tooltip=tooltip,
             popup=popup,
             style_function=lambda x: {
                 'color': x['properties']['style']['color'],
                 'weight': x['properties']['style']['stroke-width'],
@@ -563,15 +565,15 @@
             loop=False,
             max_speed=options['max_speed'],
             loop_button=True,
             time_slider_drag_update=True
         ).add_to(m)
 
     else:
-        std_out(f'Not supported map type {map_type}', 'ERROR')
+        logger.error(f'Not supported map type {map_type}')
         return None
 
     if options['minimap']:
         minimap = MiniMap(toggle_display=True, tile_layer=options['tiles'])
         minimap.add_to(m)
 
     if options['legend'] and not legend_labels is None:
```

### Comparing `scdata-0.9.1/scdata/test/plot/plot_tools.py` & `scdata-1.0.0/scdata/test/plot/plot_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from numpy import arange
 from pandas import cut, DataFrame, to_datetime, option_context, to_numeric
 import io
 import base64
 
 '''
 Available styles
@@ -63,83 +63,82 @@
     pngImageB64String = "data:image/png;base64,"
     pngImageB64String += base64.b64encode(output.getvalue()).decode('utf8')
 
     return pngImageB64String
 
 def prepare_data(test, traces, options):
 
-    std_out('Preparing data for plot')
+    logger.info('Preparing data for plot')
 
     # Dataframe to return
     df = DataFrame()
 
     # Check if there are different subplots
     n_subplots = 1
 
     for trace in traces:
         if 'subplot' in traces[trace].keys():
             n_subplots = max(n_subplots, traces[trace]['subplot'])
         else:
-            std_out (f'Trace {trace} not assigned to subplot. Skipping', 'WARNING')
+            logger.warning (f'Trace {trace} not assigned to subplot. Skipping')
 
-    std_out (f'Making {n_subplots} subplots')
+    logger.info (f'Making {n_subplots} subplots')
 
     # Generate list of subplots
     subplots = [[] for x in range(n_subplots)]
 
     # Put data in the df
     for trace in traces.keys():
 
         if 'subplot' not in traces[trace].keys():
-            std_out(f'The trace {traces[trace]} was not placed in any subplot. Assuming subplot #1', 'WARNING')
+            logger.warning(f'The trace {traces[trace]} was not placed in any subplot. Assuming subplot #1')
             traces[trace]['subplot'] = 1
 
         ndevs = traces[trace]['devices']
         nchans = traces[trace]['channel']
 
         # Make them lists always
-        if ndevs == 'all': devices = list(test.devices.keys())
+        if ndevs == 'all': devices = [device.id for device in test.devices]
         elif type(ndevs) == str or type(ndevs) == int: devices = [ndevs]
         else: devices = ndevs
+        print (devices)
 
-        for device in devices:
-
-            ndev = str(device)
+        for ndev in devices:
 
             # Make them lists always
-            if nchans == 'all': channels = list(test.devices[ndev].readings.columns)
+            if nchans == 'all': channels = list(test.get_device(ndev).data.columns)
             elif type(nchans) == str: channels = [nchans]
             else: channels = nchans
 
             for channel in channels:
                 # Check if device is in columns
-                if channel not in test.devices[ndev].readings.columns:
-                    std_out(f'The device {ndev} does not contain {channel}. Ignoring', 'WARNING')
+                if channel not in test.get_device(ndev).data.columns:
+                    logger.warning(f'The device {ndev} does not contain {channel}. Ignoring')
                     continue
 
                 # Put channel in subplots
-                subplots[traces[trace]['subplot']-1].append(channel + '_' + ndev)
+                subplots[traces[trace]['subplot']-1].append(f'{channel}_{ndev}')
 
                 column_orig = [channel]
-                columns_add = [channel + '_' + ndev]
+                columns_add = [f'{channel}_{ndev}']
 
                 # Add filtering name to dfdev
                 if 'filter' in traces[trace]:
                     col_name = traces[trace]['filter']['col']
 
-                    if col_name not in test.devices[ndev].readings.columns:
-                        std_out(f'Column {col_name} not in dataframe. Ignoring filtering', 'WARNING')
+                    if col_name not in test.get_device(ndev).data.columns:
+                        logger.warning(f'Column {col_name} not in dataframe. Ignoring filtering')
                     else:
                         column_orig.append(col_name)
                         columns_add.append(col_name)
 
                 # Device dataframe
-                dfdev = DataFrame(test.devices[ndev].readings[column_orig].values,
+                dfdev = DataFrame(test.get_device(ndev).data[column_orig].values,
                                     columns = columns_add,
-                                    index = test.devices[ndev].readings.index)
+                                    index = test.get_device(ndev).data.index)
 
                 # Add filtering function
                 if 'filter' in traces[trace]:
                     value = traces[trace]['filter']['value']
                     relationship = traces[trace]['filter']['relationship']
 
                     if col_name in dfdev.columns:
@@ -150,15 +149,15 @@
                         elif relationship == '>=':
                             dfdev.loc[dfdev[col_name]>=value]
                         elif relationship == '<':
                             dfdev.loc[dfdev[col_name]<value]
                         elif relationship == '>':
                             dfdev.loc[dfdev[col_name]>value]
                         else:
-                            std_out(f"Not valid relationship. Valid options: '==', '<=', '>=', '<', '>'", 'ERROR')
+                            logger.error(f"Not valid relationship. Valid options: '==', '<=', '>=', '<', '>'")
                             continue
                         # Remove column for filtering from dfdev
                         dfdev.drop(columns=[col_name], inplace = True)
 
                 # Combine it in the df
                 df = df.combine_first(dfdev)
         # Add average or other extras
@@ -166,15 +165,15 @@
         # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.core.resample.Resampler.aggregate.html
         if 'extras' in traces[trace]:
             for extra in traces[trace]['extras']:
 
                 nextras = list()
                 for device in traces[trace]['devices']:
                     for channel in traces[trace]['channel']:
-                        nextras.append(channel + '_' + str(device))
+                        nextras.append(f'{channel}_{ndev}')
 
                 if extra == 'bands':
                     ubn = channel + f"-{trace}-{'UPPER-BAND'}"
                     lbn = channel + f"-{trace}-{'LOWER-BAND'}"
 
                     df[ubn] = df.loc[:, nextras].mean(axis = 1) + 2*df.loc[:, nextras].std(axis = 1)
                     df[lbn] = df.loc[:, nextras].mean(axis = 1) - 2*df.loc[:, nextras].std(axis = 1)
@@ -203,19 +202,19 @@
 
     # Make sure everything is numeric before resampling
     # https://stackoverflow.com/questions/34257069/resampling-pandas-dataframe-is-deleting-column#34270422
     # df = df.apply(to_numeric, errors='coerce')
     df = df.astype(float, errors='ignore')
 
     if df.empty:
-        std_out('Empty dataframe for plot', 'ERROR')
+        logger.error('Empty dataframe for plot')
         return None, None
     # Resample it
     if options['frequency'] is not None:
-        std_out(f"Resampling at {options['frequency']}", "INFO")
+        logger.info(f"Resampling at {options['frequency']}")
 
         if 'resample' in options:
 
             if options['resample'] == 'max': df = df.resample(options['frequency']).max()
             if options['resample'] == 'min': df = df.resample(options['frequency']).min()
             if options['resample'] == 'mean': df = df.resample(options['frequency']).mean()
 
@@ -225,15 +224,15 @@
     # Clean na
     if options['clean_na'] is not None:
         if options['clean_na'] == 'fill':
             df = df.fillna(method='ffill')
         if options['clean_na'] == 'drop':
             df.dropna(axis = 0, how='any')
 
-    if df.empty: std_out('Dataframe for selected options is empty', 'WARNING')
+    if df.empty: logger.warning('Dataframe for selected options is empty')
 
     return df, subplots
 
 def groupby_session(dataframe, **kwargs):
     '''
     Prepares datafram with groupby options for plots in heatmap or boxplots.
     Parameters
```

### Comparing `scdata-0.9.1/scdata/test/plot/scatter_dispersion_grid.py` & `scdata-1.0.0/scdata/test/plot/scatter_dispersion_grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from math import ceil
 from matplotlib import gridspec
 
-plt.style.use('seaborn-white')
+plt.style.use(config._plot_style)
 
 def scatter_dispersion_grid(self, **kwargs):
     '''
     Plots disperison timeseries in matplotlib plot
     Parameters
     ----------
         channels: list
             Channel
-        options: dict 
+        options: dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Formatting dict. Defaults in config._ts_plot_def_fmt
     Returns
     -------
         Matplotlib figure
     '''
     if self.common_channels == []: self.get_common_channels()
 
     if 'channels' not in kwargs:
-        std_out('Using common channels')
+        logger.info('Using common channels')
         channels = self.common_channels
     else:
         channels = kwargs['channels']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['mpl']
     else:
-        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])        
+        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])
 
     if self.dispersion_df is None:
-        std_out('Perform dispersion analysis first!', 'ERROR')
+        logger.error('Perform dispersion analysis first!')
         return None
 
     if len(self.devices)>30:
         distribution = 'normal'
-        std_out('Using normal distribution')
-        std_out(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
+        logger.info('Using normal distribution')
+        logger.info(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
     else:
         distribution = 't-student'
-        std_out(f'Using t-student distribution.')
-    
+        logger.info(f'Using t-student distribution.')
+
     # Number of subplots
-    number_of_subplots = len(channels) 
+    number_of_subplots = len(channels)
     if number_of_subplots % 2 == 0: cols = 2
     else: cols = 2
     rows = int(ceil(number_of_subplots / cols))
 
     # Create grid
     gs = gridspec.GridSpec(rows, cols, wspace=0.9, hspace=0.4)
     figure = plt.figure(figsize=(cols*10,rows*5))
     figure.tight_layout()
 
     n = 0
 
     for channel in channels:
 
         if channel not in self.common_channels:
-            std_out(f'Channel {channel} not in common_channels')
+            logger.info(f'Channel {channel} not in common_channels')
             continue
         if channel in config._dispersion['ignore_channels']:
-            std_out(f'Channel {channel} ignored per config')
-            continue       
-        
+            logger.info(f'Channel {channel} ignored per config')
+            continue
+
         ax = figure.add_subplot(gs[n])
         n += 1
-        
+
         dispersion_avg = self._dispersion_summary[channel]
-     
+
         if distribution:
             limit_confidence = config._dispersion['limit_confidence_sigma']
 
             # Calculate upper and lower bounds
             if (config._dispersion['instantatenous_dispersion']):
                 # For sensors with high variability in the measurements, it's better to use this
                 upper_bound = self.dispersion_df[channel + '_AVG']\
@@ -96,41 +96,41 @@
                             + limit_confidence * dispersion_avg
                 lower_bound = self.dispersion_df[channel + '_AVG']\
                             - abs(limit_confidence * dispersion_avg)
         else:
             limit_confidence = t.interval(config._dispersion['t_confidence_level']/100.0, len(self.devices),
                                             loc=self.dispersion_df[channel + '_AVG'], scale=dispersion_avg)
             upper_bound = limit_confidence[1]
-            lower_bound = limit_confidence[0]   
-            
+            lower_bound = limit_confidence[0]
+
         for device in list(self.devices):
             color = cm.viridis.colors[round(list(self.devices).index(device)\
                                       *len(cm.viridis.colors)/len(list(self.devices)))]
 
-            plt.scatter(self.dispersion_df[channel + '_AVG'], 
-                          self.dispersion_df[channel + '-' + device], 
+            plt.scatter(self.dispersion_df[channel + '_AVG'],
+                          self.dispersion_df[channel + '-' + device],
                           label = device, alpha = 0.3, color = color)
-     
-        plt.plot([min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])], 
-                  [min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])], 
+
+        plt.plot([min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])],
+                  [min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])],
                   'r', label = 'AVG', alpha = 0.9, linewidth = 1.5)
 
         plt.plot([min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])],
-                  [min(lower_bound), max(lower_bound)], 
+                  [min(lower_bound), max(lower_bound)],
                   'g', label = 'AVG ± σSTD', alpha = 0.8, linewidth = 1.5)
-        
+
         plt.plot([min(self.dispersion_df[channel + '_AVG']), max(self.dispersion_df[channel + '_AVG'])],
-                  [min(upper_bound), 
-                   max(upper_bound)], 
+                  [min(upper_bound),
+                   max(upper_bound)],
                   'g', alpha = 0.8, linewidth = 1.5)
-        
+
         plt.legend(bbox_to_anchor=(1, 0.4), fancybox=True, loc='center left', ncol = 2)
         plt.xlabel('Refererence (avg. of test)')
         plt.ylabel('Individual device (-)')
         plt.title(f"Dispersion analysis for {channel} sensor - STD = {round(self.dispersion_df[channel + '_STD'].mean(), 2)}")
         plt.grid()
-    
+
     plt.subplots_adjust(top = formatting['suptitle_factor']);
 
     if options['show']: plt.show()
 
     return figure
```

### Comparing `scdata-0.9.1/scdata/test/plot/scatter_iplot.py` & `scdata-1.0.0/scdata/test/plot/scatter_iplot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from .scatter_plot import scatter_plot
 from scdata._config import config
 from plotly.io import renderers
 import plotly.tools as tls
 
 def scatter_iplot(self, **kwargs):
     """
@@ -12,52 +13,51 @@
         traces: dict
             Data for the plot, with the format:
             traces = {
                         "1": {"devices": "10751",
                               "channel": "EXT_PM_A_1"},
                         "2": {"devices": "10751",
                               "channel": "EXT_PM_A_10"
-                              }    
-                    }     
-        options: dict 
+                              }
+                    }
+        options: dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Name of auxiliary electrode found in dataframe. Defaults in config._corr_plot_def_fmt
     Returns
     -------
         Plotly figure
     """
-    std_out ('Not yet working', 'ERROR')
-    return None
+    raise NotImplementedError
     if config.framework == 'jupyterlab': renderers.default = config.framework
 
-    if 'traces' not in kwargs: 
-        std_out('No traces defined', 'ERROR')
+    if 'traces' not in kwargs:
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._scatter_plot_def_fmt['plotly']
     else:
         formatting = dict_fmerge(config._scatter_plot_def_fmt['plotly'], kwargs['formatting'])
 
     # Set options to not show in scatter_plot
     toshow = options['show']
     options['show'] = False
-    
+
     # Make sns plot
     mfig = scatter_plot(self, traces = traces, options = options, formatting = formatting)
     options['show'] = toshow
-    
+
     pfig = tls.mpl_to_plotly(mfig);
 
-    if options['show']: pfig.show();	        
+    if options['show']: pfig.show();
 
     return pfig
```

### Comparing `scdata-0.9.1/scdata/test/plot/scatter_plot.py` & `scdata-1.0.0/scdata/test/plot/scatter_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from matplotlib import style
 from seaborn import set_palette, regplot, scatterplot, relplot
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data, colors
 from numpy import array
 from math import floor, ceil
 
 def scatter_plot(self, **kwargs):
     """
@@ -33,31 +34,32 @@
         formatting: dict
             Formatting dict. Defaults in config._scatter_plot_def_fmt
     Returns
     -------
         Matplotlib figure and axes
     """
 
-    if config.framework == 'jupyterlab': plt.ioff();
-    plt.clf();
+    if config.framework == 'jupyterlab':
+        plt.ioff()
+    plt.clf()
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._scatter_plot_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._scatter_plot_def_fmt['mpl'], kwargs['formatting'])
 
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
@@ -169,25 +171,25 @@
                 if formatting['legend']:
                     ax.set_title(f'{i[2*j+1]} vs. {i[2*j]}', fontsize = formatting['title_fontsize'])
 
             if formatting['ylabel'] is not None:
                 try:
                     ax.set_ylabel(formatting['ylabel']);
                 except:
-                    std_out (f'y_label for subplot {subplots.index(i)} not set', 'WARNING')
+                    logger.warning (f'y_label for subplot {subplots.index(i)} not set')
                     ax.set_ylabel('')
                     pass
             else:
                 ax.set_ylabel('')
 
             if formatting['xlabel'] is not None:
                 try:
                     ax.set_xlabel(formatting['xlabel']);
                 except:
-                    std_out (f'x_label for subplot {subplots.index(i)} not set', 'WARNING')
+                    logger.warning (f'x_label for subplot {subplots.index(i)} not set')
                     ax.set_xlabel('')
                     pass
             else:
                 ax.set_xlabel('')
 
             y_axes.append(ax.get_ylim())
             x_axes.append(ax.get_xlim())
@@ -204,25 +206,25 @@
                 ax = axes[subplots.index(i)]
 
             # Set y axis limit
             if formatting['yrange'] is not None and not formatting['sharey']:
                 try:
                     ax.set_ylim(formatting['yrange']);
                 except:
-                    std_out (f'yrange for subplot {subplots.index(i)} not set', 'WARNING')
+                    logger.warning (f'yrange for subplot {subplots.index(i)} not set')
                     pass
             elif formatting['sharey']:
                 ax.set_ylim(min([yl[0] for yl in y_axes]), max([yl[1] for yl in y_axes]))
 
             # Set x axis limit
             if formatting['xrange'] is not None and not formatting['sharex']:
                 try:
                     ax.set_xlim(formatting['xrange']);
                 except:
-                    std_out (f'xrange for subplot {subplots.index(i)} not set', 'WARNING')
+                    logger.warning (f'xrange for subplot {subplots.index(i)} not set')
                     pass
             elif formatting['sharex']:
                 ax.set_xlim(min([xl[0] for xl in x_axes]), max([xl[1] for xl in x_axes]))
 
             if formatting['legend']:
                 ax.legend(loc='best')
             else:
```

### Comparing `scdata-0.9.1/scdata/test/plot/target_diagram.py` & `scdata-1.0.0/scdata/test/plot/target_diagram.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/test/plot/ts_dendrogram.py` & `scdata-1.0.0/scdata/test/plot/ts_dendrogram.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from scipy.cluster import hierarchy as hc
 from pandas import DataFrame
-from scdata.utils import std_out, dict_fmerge, clean
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.cleaning import clean
 from scdata._config import config
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from matplotlib import style
 
 def ts_dendrogram(self, **kwargs):
     """
-    Plots dendrogram of devices and channels in matplotlib plot. Takes all the channels 
+    Plots dendrogram of devices and channels in matplotlib plot. Takes all the channels
     in channels that are in the test `devices`
     Parameters
     ----------
         devices: list or string
             'all'
             If 'all', uses all devices in the test
         channels: list
@@ -26,87 +28,87 @@
         'options': dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Name of auxiliary electrode found in dataframe. Defaults in config._dendrogram_def_fmt
     Returns
     -------
         Dendrogram matrix, shows plot
-    """    
+    """
     if 'metric' not in kwargs: metric = 'correlation'
     else: metric = kwargs['metric']
-        
+
     if 'method' not in kwargs: method = 'single'
     else: method = kwargs['method']
-    
+
     if 'devices' not in kwargs: devices = list(self.devices.keys())
     else: devices = kwargs['devices']
-    
+
     if 'channels' not in kwargs: channels = 'all'
     else: channels = kwargs['channels']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._dendrogram_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._dendrogram_def_fmt['mpl'], kwargs['formatting'])
 
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
-    
+
     # Palette
     if formatting['palette'] is not None: set_palette(formatting['palette'])
 
     # Size sanity check
-    if formatting['width'] > 50: 
+    if formatting['width'] > 50:
 
-        std_out('Reducing width to 12')
+        logger.info('Reducing width to 12')
         formatting['width'] = 12
-    
-    if formatting['height'] > 50: 
 
-        std_out('Reducing height to 10')
-        formatting['height'] = 10    
+    if formatting['height'] > 50:
+
+        logger.info('Reducing height to 10')
+        formatting['height'] = 10
 
     # Font size
     if formatting['fontsize'] is not None:
             rcParams.update({'font.size': formatting['fontsize']});
-        
+
     df = DataFrame()
-    
+
     for device in devices:
         dfd = self.devices[device].readings.copy()
         dfd = dfd.resample(options['frequency']).mean()
-        
-        if channels != 'all': 
+
+        if channels != 'all':
             for channel in channels:
                 if channel in dfd.columns: df = df.append(dfd[channel].rename(device+'_'+channel))
         else: df = df.append(dfd)
 
     if options['clean_na'] is not None:
         if options['clean_na'] == 'drop': df.dropna(axis = 1, inplace=True)
         if options['clean_na'] == 'fill': df = df.fillna(method='ffill')
-    
+
     Z = hc.linkage(df, method = method, metric = metric)
 
     # Plot dendogram
     plt.figure(figsize=(formatting['width'], formatting['height']))
     plt.title(formatting['title'], fontsize = formatting['title_fontsize'])
     plt.subplots_adjust(top = formatting['suptitle_factor']);
     plt.xlabel(formatting['xlabel'])
     plt.ylabel(formatting['ylabel'])
     hc.dendrogram(
         Z,
         orientation=formatting['orientation'],
         leaf_font_size=formatting['fontsize'],  # font size for the x axis labels
         labels=df.index
     )
-    
+
     plt.show()
-    
+
     return Z
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_dispersion_grid.py` & `scdata-1.0.0/scdata/test/plot/ts_dispersion_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from math import ceil
 from matplotlib import gridspec
 
-plt.style.use('seaborn-white')
+plt.style.use(config._plot_style)
 
 def ts_dispersion_grid(self, **kwargs):
     '''
     Plots disperison timeseries in matplotlib plot
     Parameters
     ----------
         channels: list
             Channel
-        options: dict 
+        options: dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Formatting dict. Defaults in config._ts_plot_def_fmt
     Returns
     -------
         Matplotlib figure
     '''
     if self.common_channels == []: self.get_common_channels()
 
     if 'channels' not in kwargs:
-        std_out('Using common channels')
+        logger.info('Using common channels')
         channels = self.common_channels
     else:
         channels = kwargs['channels']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['mpl']
     else:
-        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])        
+        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])
 
     if self.dispersion_df is None:
-        std_out('Perform dispersion analysis first!', 'ERROR')
+        logger.info('Perform dispersion analysis first!', 'ERROR')
         return None
 
     if len(self.devices)>30:
         distribution = 'normal'
-        std_out('Using normal distribution')
-        std_out(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
+        logger.info('Using normal distribution')
+        logger.info(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
     else:
         distribution = 't-student'
-        std_out(f'Using t-student distribution.')
-    
+        logger.info(f'Using t-student distribution.')
+
     # Number of subplots
-    number_of_subplots = len(channels) 
+    number_of_subplots = len(channels)
     if number_of_subplots % 2 == 0: cols = 2
     else: cols = 2
     rows = int(ceil(number_of_subplots / cols))
 
     # Time series plot
     gs = gridspec.GridSpec(rows, cols, wspace=0.9, hspace=0.3)
     figure = plt.figure(figsize=(cols*10,rows*5))
     figure.tight_layout()
 
     n = 0
 
     for channel in channels:
 
         if channel not in self.common_channels:
-            std_out(f'Channel {channel} not in common_channels')
+            logger.info(f'Channel {channel} not in common_channels')
             continue
         if channel in config._dispersion['ignore_channels']:
-            std_out(f'Channel {channel} ignored per config')
-            continue     
-        
+            logger.info(f'Channel {channel} ignored per config')
+            continue
+
         ax = figure.add_subplot(gs[n])
         n += 1
-        
+
         dispersion_avg = self._dispersion_summary[channel]
-     
+
         if distribution:
             limit_confidence = config._dispersion['limit_confidence_sigma']
 
             # Calculate upper and lower bounds
             if (config._dispersion['instantatenous_dispersion']):
                 # For sensors with high variability in the measurements, it's better to use this
                 upper_bound = self.dispersion_df[channel + '_AVG']\
@@ -96,31 +96,31 @@
                             + limit_confidence * dispersion_avg
                 lower_bound = self.dispersion_df[channel + '_AVG']\
                             - abs(limit_confidence * dispersion_avg)
         else:
             limit_confidence = t.interval(config._dispersion['t_confidence_level']/100.0, len(self.devices),
                                             loc=self.dispersion_df[channel + '_AVG'], scale=dispersion_avg)
             upper_bound = limit_confidence[1]
-            lower_bound = limit_confidence[0]   
-            
+            lower_bound = limit_confidence[0]
+
         for device in list(self.devices):
             color = cm.viridis.colors[round(list(self.devices).index(device)\
                                       *len(cm.viridis.colors)/len(list(self.devices)))]
 
-            plt.plot(self.dispersion_df.index, 
-                      self.dispersion_df[channel + '-' + device], 
+            plt.plot(self.dispersion_df.index,
+                      self.dispersion_df[channel + '-' + device],
                       label = device, alpha = 0.3, color = color)
- 
+
         plt.plot(self.dispersion_df.index, self.dispersion_df[channel + '_AVG'],
                 'r', label = 'AVG', alpha = 0.9, linewidth = 1.5)
 
-        plt.plot(self.dispersion_df.index, lower_bound, 
+        plt.plot(self.dispersion_df.index, lower_bound,
                 'g', label = 'AVG ± σSTD', alpha = 0.8, linewidth = 1.5)
 
-        plt.plot(self.dispersion_df.index, upper_bound, 
+        plt.plot(self.dispersion_df.index, upper_bound,
                 'g', alpha = 0.8, linewidth = 1.5)
 
         plt.legend(bbox_to_anchor=(1, 0.5), fancybox=True, loc='center left', ncol = 2)
         plt.xlabel('Refererence (avg. of test)')
         plt.ylabel('Individual device (-)')
         plt.title(f"Dispersion analysis for {channel} sensor - STD = {round(self.dispersion_df[channel + '_STD'].mean(), 2)}")
         plt.grid()
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_dispersion_plot.py` & `scdata-1.0.0/scdata/test/plot/ts_dispersion_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 import matplotlib.pyplot as plt
 import matplotlib.colors
 from matplotlib import rcParams
 from matplotlib import style
 from seaborn import set_palette
 from scipy.stats import t
@@ -11,80 +11,80 @@
 def ts_dispersion_plot(self, **kwargs):
     '''
     Plots disperison timeseries in matplotlib plot
     Parameters
     ----------
         channel: string
             Channel
-        options: dict 
+        options: dict
             Options including data processing prior to plot. Defaults in config._plot_def_opt
         formatting: dict
             Formatting dict. Defaults in config._ts_plot_def_fmt
     Returns
     -------
         Matplotlib figure
     '''
 
     if 'channel' not in kwargs:
-        std_out('Needs at least one channel to plot')
+        logger.info('Needs at least one channel to plot')
         return None
     else:
         channel = kwargs['channel']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['mpl']
     else:
-        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])        
+        formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])
 
     if self.dispersion_df is None:
-        std_out('Perform dispersion analysis first!', 'ERROR')
+        logger.error('Perform dispersion analysis first!')
         return None
 
     if self.common_channels == []: self.get_common_channels()
     if channel not in self.common_channels:
-        std_out(f'Channel {channel} not in common_channels')
+        logger.info(f'Channel {channel} not in common_channels')
         return None
     if channel in config._dispersion['ignore_channels']:
-        std_out(f'Channel {channel} ignored per config')
+        logger.info(f'Channel {channel} ignored per config')
         return None
 
     if len(self.devices)>config._dispersion['nt_threshold']:
         distribution = 'normal'
-        std_out('Using normal distribution')
-        std_out(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
+        logger.info('Using normal distribution')
+        logger.info(f"Using limit for sigma confidence: {config._dispersion['limit_confidence_sigma']}")
     else:
         distribution = 't-student'
-        std_out(f'Using t-student distribution.')
+        logger.info(f'Using t-student distribution.')
 
     # Size sanity check
-    if formatting['width'] > 50: 
-        std_out('Reducing width to 12')
+    if formatting['width'] > 50:
+        logger.info('Reducing width to 12')
         formatting['width'] = 12
     if formatting['height'] > 50:
-        std_out('Reducing height to 10')
-        formatting['height'] = 10        
+        logger.info('Reducing height to 10')
+        formatting['height'] = 10
 
     # Make subplot
-    figure, (ax_tbr, ax_ok) = plt.subplots(nrows = 2, 
+    figure, (ax_tbr, ax_ok) = plt.subplots(nrows = 2,
                                 sharex = formatting['sharex'],
                                 figsize = (formatting['width'],
                                            formatting['height'])
                                 );
     # cmap = plt.cm.Reds
-    norm = matplotlib.colors.Normalize(vmin=0, 
+    norm = matplotlib.colors.Normalize(vmin=0,
             vmax=config._dispersion['limit_errors']/2)
     ch_index = self.common_channels.index(channel)+1
-    
+
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
     # Font size
     if formatting['fontsize'] is not None:
             rcParams.update({'font.size': formatting['fontsize']});
 
@@ -102,21 +102,21 @@
                         - abs(limit_confidence * self.dispersion_df[channel + '_STD'])
         else:
             upper_bound = self.dispersion_df[channel + '_AVG']\
                         + limit_confidence * dispersion_avg
             lower_bound = self.dispersion_df[channel + '_AVG']\
                         - abs(limit_confidence * dispersion_avg)
     else:
-        limit_confidence = t.interval(config._dispersion['t_confidence_level']/100.0, len(self.devices), 
+        limit_confidence = t.interval(config._dispersion['t_confidence_level']/100.0, len(self.devices),
                                         loc=self.dispersion_df[channel + '_AVG'], scale=dispersion_avg)
         upper_bound = limit_confidence[1]
         lower_bound = limit_confidence[0]
 
     for device in self.devices:
-        ncol = channel + '-' + device 
+        ncol = channel + '-' + device
         if ncol in self.dispersion_df.columns:
 
             # Count how many times we go above the upper bound or below the lower one
             count_problems_up = self.dispersion_df[ncol] > upper_bound
             count_problems_down =  self.dispersion_df[ncol] < lower_bound
 
             # Count them
@@ -124,27 +124,27 @@
                                 else 0 for i in range(len(count_problems_up))]
 
             # Add the trace in either
             number_errors = np.sum(count_problems)
             max_number_errors = len(count_problems)
 
             if number_errors/max_number_errors > config._dispersion['limit_errors']/100:
-                std_out (f"Device {device} out of {config._dispersion['limit_errors']}% limit\
-                         - {np.round(number_errors/max_number_errors*100, 1)}% out", 'WARNING')
+                logger.warning (f"Device {device} out of {config._dispersion['limit_errors']}% limit\
+                         - {np.round(number_errors/max_number_errors*100, 1)}% out")
                 alpha = 1
-                ax_tbr.plot(self.dispersion_df.index, 
-                         self.dispersion_df[ncol], 
+                ax_tbr.plot(self.dispersion_df.index,
+                         self.dispersion_df[ncol],
                          color = 'r',
                          label = device, alpha = alpha)
             else:
                 alpha = 1
                 color = 'g'
-                ax_ok.plot(self.dispersion_df.index, 
-                         self.dispersion_df[ncol], 
-                         color = color, 
+                ax_ok.plot(self.dispersion_df.index,
+                         self.dispersion_df[ncol],
+                         color = color,
                          label = device, alpha = alpha)
 
     # Add upper and low bound bound to subplot 1
     ax_tbr.plot(self.dispersion_df.index, self.dispersion_df[channel + '_AVG'],
             'b', label = 'Average', alpha = 0.6)
     ax_tbr.plot(self.dispersion_df.index, upper_bound,
             'k', label = 'Upper-Bound', alpha = 0.6)
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_dispersion_uplot.py` & `scdata-1.0.0/scdata/test/plot/ts_dispersion_uplot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+
 from scdata._config import config
 from .plot_tools import colors
 from scipy.stats import t
 import numpy as np
 
 # uPlot
 from IPython.display import HTML
@@ -54,64 +56,64 @@
             }
 
             u = new uPlot(options, data, document.getElementById("plot{{subplot}}"))
         </script>
         '''
 
     if 'channel' not in kwargs:
-        std_out('Needs at least one channel to plot')
+        logger.info('Needs at least one channel to plot')
         return None
     else:
         channel = kwargs['channel']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['uplot']
     else:
         formatting = dict_fmerge(config._ts_plot_def_fmt['uplot'],
                                  kwargs['formatting'])
 
     # Size sanity check
     if formatting['width'] < 100:
-        std_out('Setting width to 800')
+        logger.info('Setting width to 800')
         formatting['width'] = 800
     if formatting['height'] < 100:
-        std_out('Reducing height to 600')
+        logger.info('Reducing height to 600')
         formatting['height'] = 600
 
     if 'html' not in options:
         options['html'] = False
 
     if self.dispersion_df is None:
-        std_out('Perform dispersion analysis first!', 'ERROR')
+        logger.error('Perform dispersion analysis first!')
         return None
 
     if self.common_channels == []: self.get_common_channels()
 
     if channel not in self.common_channels:
-        std_out(f'Channel {channel} not in common_channels')
+        logger.info(f'Channel {channel} not in common_channels')
         return None
     if channel in config._dispersion['ignore_channels']:
-        std_out(f'Channel {channel} ignored per config')
+        logger.info(f'Channel {channel} ignored per config')
         return None
 
     if len(self.devices)>config._dispersion['nt_threshold']:
         distribution = 'normal'
-        std_out('Using normal distribution')
-        std_out(f"Using limit for sigma confidence:\
+        logger.info('Using normal distribution')
+        logger.info(f"Using limit for sigma confidence:\
                 {config._dispersion['limit_confidence_sigma']}")
     else:
         distribution = 't-student'
-        std_out(f'Using t-student distribution.')
+        logger.info(f'Using t-student distribution.')
 
     ch_index = self.common_channels.index(channel)+1
     total_number = len(self.common_channels)
     h = Template(head_template).render(title = f'({ch_index}/{total_number}) - {channel}')
 
     dispersion_avg = self._dispersion_summary[channel]
 
@@ -165,16 +167,16 @@
 
             # Add the trace in either
             number_errors = np.sum(count_problems)
             max_number_errors = len(count_problems)
 
             # TBR
             if number_errors/max_number_errors > config._dispersion['limit_errors']/100:
-                std_out (f"Device {device} out of {config._dispersion['limit_errors']}% limit\
-                         - {np.round(number_errors/max_number_errors*100, 1)}% out", 'WARNING')
+                logger.warning (f"Device {device} out of {config._dispersion['limit_errors']}% limit\
+                         - {np.round(number_errors/max_number_errors*100, 1)}% out")
                 subplots[0].append(ncol)
             #OK
             else:
                 subplots[n_subplots-1].append(ncol)
 
     # Add upper and low bound bound to subplot 0
     subplots[0].append(channel + '_AVG')
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_iplot.py` & `scdata-1.0.0/scdata/test/plot/ts_iplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data
 
 # Plotly
 import plotly.tools as tls
 from plotly.subplots import make_subplots
 # import plotly.graph_objs as go
@@ -32,27 +33,27 @@
     -------
         Plotly figure
     """
 
     if config.framework == 'jupyterlab': renderers.default = config.framework
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options', 'WARNING')
+        logger.warning('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting', 'WARNING')
+        logger.warning('Using default formatting')
         formatting = config._ts_plot_def_fmt['plotly']
     else:
         formatting = dict_fmerge(config._ts_plot_def_fmt['plotly'], kwargs['formatting'])
 
     # Get dataframe
     df, subplots = prepare_data(self, traces, options)
 
@@ -60,18 +61,18 @@
     if df is None:
         return None
 
     n_subplots = len(subplots)
 
     # Size sanity check
     if formatting['width'] < 100:
-        std_out('Setting width to 800')
+        logger.info('Setting width to 800')
         formatting['width'] = 800
     if formatting['height'] < 100:
-        std_out('Reducing height to 600')
+        logger.info('Reducing height to 600')
         formatting['height'] = 600
 
     figure = make_subplots(rows = n_subplots, cols=1,
                            shared_xaxes = formatting['sharex'])
 
     # Add traces
     for isbplt in range(n_subplots):
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_plot.py` & `scdata-1.0.0/scdata/test/plot/ts_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+
 from scdata._config import config
 from .plot_tools import prepare_data
 from pandas import to_datetime
 
 # Matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
@@ -30,31 +32,32 @@
         formatting: dict
             Formatting dict. Defaults in config._ts_plot_def_fmt
     Returns
     -------
         Matplotlib figure
     """
 
-    if config.framework == 'jupyterlab': plt.ioff();
-    plt.clf();
+    if config.framework == 'jupyterlab':
+        plt.ioff()
+    plt.clf()
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._ts_plot_def_fmt['mpl'], kwargs['formatting'])
 
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
@@ -73,18 +76,18 @@
     if df is None:
         return None
 
     n_subplots = len(subplots)
 
     # Size sanity check
     if formatting['width'] > 50:
-        std_out('Reducing width to 12')
+        logger.info('Reducing width to 12')
         formatting['width'] = 12
     if formatting['height'] > 50:
-        std_out('Reducing height to 10')
+        logger.info('Reducing height to 10')
         formatting['height'] = 10
 
     # Plot
     figure, axes = plt.subplots(n_subplots, 1,
                                 sharex = formatting['sharex'],
                                 figsize = (formatting['width'],
                                            formatting['height'])
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_scatter.py` & `scdata-1.0.0/scdata/test/plot/ts_scatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
 from scdata._config import config
 from .plot_tools import prepare_data
 
 # Matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from matplotlib import gridspec
@@ -32,31 +33,32 @@
         formatting: dict
             Name of auxiliary electrode found in dataframe
     Returns
     -------
         Matplotlib figure containing timeseries and scatter plot with correlation
         coefficients on it
     """
-    if config.framework == 'jupyterlab': plt.ioff();
-    plt.clf();
+    if config.framework == 'jupyterlab':
+        plt.ioff()
+    plt.clf()
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.error('No traces defined')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_scatter_def_fmt['mpl']
     else:
         formatting = dict_fmerge(config._ts_scatter_def_fmt['mpl'], kwargs['formatting'])
 
     # Style
     if formatting['style'] is not None: style.use(formatting['style'])
     else: style.use(config._plot_style)
@@ -92,17 +94,17 @@
     feature_trace = subplots[0][0]
     ref_trace = subplots[0][1]
 
     # Calculate basic metrics
     pearsonCorr = list(df.corr('pearson')[list(df.columns)[0]])[-1]
     rmse = sqrt(mean_squared_error(df[feature_trace].fillna(0), df[ref_trace].fillna(0)))
 
-    std_out (f'Pearson correlation coefficient: {pearsonCorr}')
-    std_out (f'Coefficient of determination R²: {pearsonCorr*pearsonCorr}')
-    std_out (f'RMSE: {rmse}')
+    logger.info (f'Pearson correlation coefficient: {pearsonCorr}')
+    logger.info (f'Coefficient of determination R²: {pearsonCorr*pearsonCorr}')
+    logger.info (f'RMSE: {rmse}')
 
     # Time Series plot
     ax1.plot(df.index, df[feature_trace], color = 'g', label = feature_trace, linewidth = 1, alpha = 0.9)
     ax1.plot(df.index, df[ref_trace], color = 'k', label = ref_trace, linewidth = 1, alpha = 0.7)
     ax1.axis('tight')
 
     # Correlation plot
```

### Comparing `scdata-0.9.1/scdata/test/plot/ts_uplot.py` & `scdata-1.0.0/scdata/test/plot/ts_uplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from scdata.utils import std_out, dict_fmerge
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+
 from scdata._config import config
 from .plot_tools import prepare_data, colors
 
 # uPlot
 from IPython.display import HTML
 import json
 from jinja2 import Template
@@ -64,37 +66,37 @@
             }
 
             u = new uPlot(options, data, document.getElementById("plot{{subplot}}"))
         </script>
         '''
 
     if 'traces' not in kwargs:
-        std_out('No traces defined', 'ERROR')
+        logger.info('No traces defined', 'ERROR')
         return None
     else:
         traces = kwargs['traces']
 
     if 'options' not in kwargs:
-        std_out('Using default options')
+        logger.info('Using default options')
         options = config._plot_def_opt
     else:
         options = dict_fmerge(config._plot_def_opt, kwargs['options'])
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._ts_plot_def_fmt['uplot']
     else:
         formatting = dict_fmerge(config._ts_plot_def_fmt['uplot'], kwargs['formatting'])
 
     # Size sanity check
     if formatting['width'] < 100:
-        std_out('Setting width to 800')
+        logger.info('Setting width to 800')
         formatting['width'] = 800
     if formatting['height'] < 100:
-        std_out('Reducing height to 600')
+        logger.info('Reducing height to 600')
         formatting['height'] = 600
 
     if 'html' not in options:
         options['html'] = False
 
     h = Template(head_template).render(title=formatting['title'])
```

### Comparing `scdata-0.9.1/scdata/test/utils/checks.py` & `scdata-1.0.0/scdata/test/checks/checks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 import matplotlib.pyplot as plt
 import missingno as msno
 from pandas import to_datetime, DataFrame
 from scdata.test.plot.plot_tools import prepare_data
 from scdata._config import config
-from scdata.utils.dictmerge import dict_fmerge
+from scdata.tools.dictmerge import dict_fmerge
 
 def gaps_check(self, devices = None, channels = None, groupby = 'channel', **kwargs):
     if config.framework == 'jupyterlab': plt.ioff();
     plt.clf();
 
     if 'formatting' not in kwargs:
-        std_out('Using default formatting')
+        logger.info('Using default formatting')
         formatting = config._missingno_def_fmt
     else:
         formatting = dict_fmerge(config._missingno_def_fmt, kwargs['formatting'])
 
 	# Get list of devices
     if devices is None:
         _devices = list(self.devices.keys())
     else:
         _devices = devices
 
     if channels is None:
-        std_out('Need some channels to check gaps for', 'ERROR')
+        logger.error('Need some channels to check gaps for')
         return
 
     if groupby == 'device':
 
         for device in _devices:
             if device not in self.devices:
-                std_out('Device not found in test', 'WARNING')
+                logger.warning('Device not found in test')
                 continue
             msno.matrix(self.devices[device].readings)
 
     elif groupby == 'channel':
 
         for channel in channels:
             traces = {"1": {"devices": _devices, "channel": channel, "subplot": 1}}
             options = config._plot_def_opt
             df, _ = prepare_data(self, traces, options)
             fig, ax = plt.subplots(1, len(_devices), figsize=(formatting['width'], formatting['height']))
             for device in _devices:
                 if device not in self.devices:
-                    std_out('Device not found in test', 'WARNING')
+                    logger.warning('Device not found in test')
                     continue
                 msno.matrix(df = DataFrame(df[f'{channel}_{device}']), sparkline=False, ax = ax[_devices.index(device)], fontsize=formatting['fontsize'])
                 ax[_devices.index(device)].set_yticks([i for i in range(len(df))], [i for i in df.index.values])
             plt.show()
 
 def get_common_channels(self, devices = None, ignore_missing_channels = False, pop_zero_readings_devices = False, detailed = False, verbose = True):
     '''
@@ -91,44 +91,43 @@
             # We don't reduce the list in case the new list is smaller
             list_channels = list(set(list_channels) | set(self.devices[device].readings.columns))
         else:
             # We reduce it
             list_channels = list(set(list_channels) & set(self.devices[device].readings.columns))
 
         channels_devices[device] = {len(self.devices[device].readings.columns)}
-        std_out ('Device {}'.format(device), force = verbose)
-        std_out (f'Min reading at {self.devices[device].readings.index[0]}', force = verbose)
-        std_out (f'Max reading at {self.devices[device].readings.index[-1]}', force = verbose)
-        std_out (f'Number of dataframe points {len(self.devices[device].readings.index)}', force = verbose)
+        logger.info (f'Device {device}')
+        logger.info (f'Min reading at {self.devices[device].readings.index[0]}')
+        logger.info (f'Max reading at {self.devices[device].readings.index[-1]}')
+        logger.info (f'Number of dataframe points {len(self.devices[device].readings.index)}')
         if detailed:
             for column in list_channels:
-                std_out ('\tColumn {}'.format(column), force = verbose)
+                logger.info ('\tColumn {}'.format(column))
                 nas = self.devices[device].readings[column].isna()
-                std_out ('\tNumber of nas {}'.format(nas.sum()), force = verbose)
+                logger.info ('\tNumber of nas {}'.format(nas.sum()))
 
         ## Eliminate devices with no points
         if (len(self.devices[device].readings.index) == 0):
-            std_out (f'Device {device} for insufficient data points', 'WARNING')
+            logger.warning (f'Device {device} for insufficient data points')
             if pop_zero_readings_devices: self.devices.pop(device)
         # Check the number of channels
         elif len_channels != len(self.devices[device].readings.columns):
-            std_out(f"Device {device} has {len(self.devices[device].readings.columns)}. Current common channel length is {len_channels}", 'WARNING')
+            logger.warning(f"Device {device} has {len(self.devices[device].readings.columns)}. Current common channel length is {len_channels}")
             len_channels = len(list_channels)
             show_warning = True
-            if ignore_missing_channels: std_out ("Ignoring missing channels", 'WARNING')
-        std_out ('---------', force = verbose)
-
+            if ignore_missing_channels: logger.warning ("Ignoring missing channels")
+        logger.error ('---------')
 
     if return_all:
 
         self.common_channels = list_channels
-    
-        std_out(f'Final list of channels:\n {self.common_channels}')
+
+        logger.info(f'Final list of channels:\n {self.common_channels}')
         if show_warning:
-            std_out (f'Some devices show less amount of sensors', 'WARNING')
+            logger.warning (f'Some devices show less amount of sensors')
             print (channels_devices)
 
         return self.common_channels
 
     else:
 
         return list_channels
```

### Comparing `scdata-0.9.1/scdata/test/utils/combine.py` & `scdata-1.0.0/scdata/test/tools/combine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 from pandas import DataFrame
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata.device import Device
 
 def combine(self, devices = None, readings = None):
     """
-    Combines devices from a test into a new dataframe, following the 
+    Combines devices from a test into a new dataframe, following the
     naming as follows: DEVICE-NAME_READING-NAME
     Parameters
     ----------
         devices: list or None
             None
             If None, includes all the devices in self.devices
         readings: list or None
             None
             If None, includes all the readings in self.readings
     Returns
     -------
         Dataframe if successful or False otherwise
-    """ 
+    """
 
     dfc = DataFrame()
 
     if devices is None:
         dl = list(self.devices.keys())
-    else: 
+    else:
         # Only pick the ones that are actually present
         dl = list(set(devices).intersection(list(self.devices.keys())))
         if len(dl) != len(devices):
-            std_out('Requested devices are not all present in devices', 'WARNING')
-            std_out(f'Discarding {set(devices).difference(list(self.devices.keys()))}')
+            logger.warning('Requested devices are not all present in devices')
+            logger.info(f'Discarding {set(devices).difference(list(self.devices.keys()))}')
 
     for device in dl:
         new_names = list()
 
         if readings is None:
             rl = list(self.devices[device].readings.columns)
-        else: 
+        else:
             # Only pick the ones that are actually present
             rl = list(set(readings).intersection(list(self.devices[device].readings.columns)))
 
             if any([reading not in rl for reading in readings]):
-                std_out(f'Requested readings are not all present in readings for device {device}', 'WARNING')
-                std_out(f'Discarding {list(set(readings).difference(list(self.devices[device].readings.columns)))}', 'WARNING')
-        
+                logger.warning(f'Requested readings are not all present in readings for device {device}')
+                logger.warning(f'Discarding {list(set(readings).difference(list(self.devices[device].readings.columns)))}')
+
         rename = dict()
 
         for reading in rl:
             rename[reading] = reading + '_' + self.devices[device].id
-        
+
         df = self.devices[device].readings[rl].copy()
         df.rename(columns = rename, inplace = True)
         dfc = dfc.combine_first(df)
-    
+
     if dfc.empty:
-        std_out('Error ocurred while combining data. Review data', 'ERROR')
+        logger.error('Error ocurred while combining data. Review data')
         return False
     else:
-        std_out('Data combined successfully', 'SUCCESS')
+        logger.info('Data combined successfully')
         return dfc
```

### Comparing `scdata-0.9.1/scdata/test/utils/dispersion.py` & `scdata-1.0.0/scdata/test/dispersion/dispersion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from scdata.utils import std_out, localise_date
+from scdata.tools.custom_logger import logger
+from scdata.tools.date import localise_date
 from pandas import DataFrame
 from scdata._config import config
 
 def dispersion_analysis(self, devices = None, min_date = None, max_date = None, timezone = 'Europe/Madrid', smooth_window = 5):
     '''
         Creates channels on a new dataframe for each device/channel combination, and makes the average/std of each
         in a point-by-point fashion
@@ -62,31 +63,31 @@
                     channel_new = self.devices[device].readings[channel].bfill().rolling(window=smooth_window).mean()
                     dispersion_df[channel + '-' + device] = channel_new[channel_new > 0]
                 else:
                     dispersion_df[channel + '-' + device] = self.devices[device].readings[channel].resample('1Min').bfill()
 
                 columns.append(channel + '-' + device)
             else:
-                std_out(f'Device {device} does not contain {channel}</p>', 'WARNING')
+                logger.warning(f'Device {device} does not contain {channel}</p>')
                 warning = True
 
         dispersion_df.index = localise_date(dispersion_df.index, timezone)
 
         # Trim dataset to min and max dates (normally these tests are carried out with _minutes_ of differences)
         if min_date is not None: dispersion_df = dispersion_df[dispersion_df.index > min_date]
         if max_date is not None: dispersion_df = dispersion_df[dispersion_df.index < max_date]
 
         # Calculate Metrics
         dispersion_df[channel + '_AVG'] = dispersion_df.loc[:,columns].mean(skipna=True, axis = 1)
         dispersion_df[channel + '_STD'] = dispersion_df.loc[:,columns].std(skipna=True, axis = 1)
 
     if not warning:
-        std_out(f'All devices have the provided channels list recorded')
+        logger.info(f'All devices have the provided channels list recorded')
     else:
-        std_out(f'Missing channels, review data', 'WARNING')
+        logger.warning(f'Missing channels, review data')
 
     if devices is None:
         self.dispersion_df = dispersion_df
         return self.dispersion_summary
 
     group_dispersion_summary = dict()
 
@@ -98,15 +99,15 @@
     return group_dispersion_summary
 
 @property
 def dispersion_summary(self):
     self._dispersion_summary = dict()
 
     if self.dispersion_df is None:
-        std_out('Perform dispersion analysis first!', 'ERROR')
+        logger.error('Perform dispersion analysis first!')
         return None
     for channel in self.common_channels:
         if channel in config._dispersion['ignore_channels']: continue
-        # Calculate 
+        # Calculate
         self._dispersion_summary[channel] = self.dispersion_df[channel + '_STD'].mean()
 
     return self._dispersion_summary
```

### Comparing `scdata-0.9.1/scdata/test/utils/prepare.py` & `scdata-1.0.0/scdata/test/tools/prepare.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from scdata.utils import std_out, dict_fmerge, clean
+from scdata.tools.custom_logger import logger
+from scdata.tools.dictmerge import dict_fmerge
+from scdata.tools.cleaning import  clean
 from scdata._config import config
 from numpy import array
 from pandas import DataFrame
 
 def prepare(self, measurand, inputs, options = dict()):
     """
     Prepares a test for a regression model
@@ -36,15 +38,15 @@
         df = df.combine_first(combined_df)
 
     if options['common_avg']:
 
         common_channels = inputs[list(inputs.keys())[0]]
         for input_device in inputs.keys():
             common_channels = list(set(common_channels).intersection(set(inputs[input_device])))
-        std_out(f'Performing avg in common columns {common_channels}')
+        logger.info(f'Performing avg in common columns {common_channels}')
         for channel in common_channels:
             columns_list = [channel + '_' + device for device in list(inputs.keys())]
             df[channel + '_AVG'] = df[columns_list].mean(axis = 1)
 
         df = df.loc[:, df.columns.str.contains("_AVG")| df.columns.str.contains(measurand_name)]
 
     if options['clean_na'] is not None:
```

### Comparing `scdata-0.9.1/scdata/utils/cleaning.py` & `scdata-1.0.0/scdata/tools/cleaning.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/date.py` & `scdata-1.0.0/scdata/tools/date.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/dictmerge.py` & `scdata-1.0.0/scdata/tools/dictmerge.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/interim/example.csv` & `scdata-1.0.0/scdata/tools/interim/example.csv`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,1013 +1,1013 @@
-TIME,TEMP,HUM,BATT,LIGHT,NOISE_A,PRESS,CCS811_VOCS,CCS811_ECO2,ADC_48_0,ADC_48_1,ADC_48_2,ADC_48_3,PM_1,PM_25,PM_10
-ISO 8601,C,%,%,Lux,dBA,kPa,ppb,ppm,V,V,V,V,ug/m3,ug/m3,ug/m3
-Time,Temperature,Humidity,Battery,Light,Noise dBA,Barometric pressure,VOC Gas CCS811,eCO2 Gas CCS811,ADS1x15 ADC 0x48 Ch0,ADS1x15 ADC 0x48 Ch1,ADS1x15 ADC 0x48 Ch2,ADS1x15 ADC 0x48 Ch3,PM 1.0,PM 2.5,PM 10.0
-,55,56,10,14,53,58,113,112,0,0,0,0,89,87,88
-2020-09-02T15:35:19Z,26.92,61.17,-1,5,43.34,101.53,null,null,0.204281,0.212750,0.218586,0.209000,null,null,null
-2020-09-02T15:35:49Z,26.90,61.18,100,8,46.94,101.55,null,null,0.202578,0.212055,0.219797,0.208891,null,null,null
-2020-09-02T15:36:19Z,26.92,61.17,100,7,47.10,101.54,null,null,0.204656,0.212156,0.221180,0.210086,null,null,null
-2020-09-02T15:36:49Z,27.00,61.17,100,7,40.23,101.54,null,null,0.202375,0.211820,0.217867,0.208695,null,null,null
-2020-09-02T15:37:19Z,27.02,61.19,99,6,50.44,101.53,null,null,0.204305,0.214047,0.220977,0.209359,null,null,null
-2020-09-02T15:37:49Z,27.06,60.90,99,8,55.43,101.53,null,null,0.204508,0.213484,0.220422,0.209727,null,null,null
-2020-09-02T15:38:19Z,27.13,60.77,99,7,61.21,101.53,null,null,0.204820,0.213289,0.219609,0.209453,null,null,null
-2020-09-02T15:38:49Z,27.10,60.56,99,8,43.58,101.53,null,null,0.204367,0.212547,0.221062,0.208687,null,null,null
-2020-09-02T15:39:19Z,27.07,60.51,99,6,42.34,101.53,null,null,0.205031,0.213109,0.220453,0.209469,null,null,null
-2020-09-02T15:39:49Z,27.05,60.52,99,6,37.82,101.54,null,null,0.205609,0.213156,0.219805,0.209508,null,null,null
-2020-09-02T15:40:19Z,27.06,60.58,99,7,32.72,101.54,0.00,400.00,0.205016,0.212984,0.220570,0.209367,null,null,null
-2020-09-02T15:40:49Z,27.06,60.53,99,7,34.22,101.54,0.00,400.00,0.204414,0.213031,0.222000,0.209312,null,null,null
-2020-09-02T15:41:19Z,27.03,60.60,99,7,32.29,101.54,0.00,400.00,0.205383,0.213047,0.220727,0.209586,null,null,null
-2020-09-02T15:41:49Z,27.03,60.59,99,7,34.32,101.54,0.00,400.00,0.203547,0.212711,0.220375,0.209641,null,null,null
-2020-09-02T15:42:19Z,26.99,60.62,99,7,40.97,101.54,0.00,400.00,0.205852,0.212242,0.221188,0.209469,null,null,null
-2020-09-02T15:42:49Z,27.02,60.63,99,7,46.62,101.54,0.00,400.00,0.205102,0.212969,0.222883,0.209883,null,null,null
-2020-09-02T15:43:19Z,26.99,60.69,99,7,42.23,101.54,0.00,400.00,0.205695,0.213742,0.221531,0.209570,null,null,null
-2020-09-02T15:43:49Z,27.00,60.64,99,7,41.76,101.54,0.00,400.00,0.205141,0.213445,0.220516,0.209219,null,null,null
-2020-09-02T15:44:19Z,26.99,60.59,99,7,41.79,101.54,0.00,400.00,0.204203,0.212109,0.220719,0.209148,null,null,null
-2020-09-02T15:44:49Z,26.97,60.61,99,7,40.08,101.54,0.00,400.00,0.205586,0.213641,0.222227,0.210219,null,null,null
-2020-09-02T15:45:19Z,26.97,60.65,99,6,43.69,101.54,0.00,400.00,0.204383,0.214031,0.221844,0.209500,null,null,null
-2020-09-02T15:45:49Z,26.95,60.66,99,7,32.34,101.55,0.00,400.00,0.205406,0.213484,0.221477,0.210125,null,null,null
-2020-09-02T15:46:19Z,26.97,60.66,99,7,34.11,101.55,0.00,400.00,0.204430,0.212977,0.221914,0.210531,null,null,null
-2020-09-02T15:46:49Z,26.99,60.56,99,7,43.35,101.54,0.00,400.00,0.205375,0.212883,0.221539,0.210187,null,null,null
-2020-09-02T15:47:19Z,26.97,60.57,99,7,33.25,101.54,0.00,400.00,0.205734,0.213000,0.220844,0.211203,null,null,null
-2020-09-02T15:47:49Z,26.99,60.58,99,7,32.76,101.54,0.00,400.00,0.205445,0.214086,0.220055,0.210250,null,null,null
-2020-09-02T15:48:19Z,27.00,60.54,99,7,37.54,101.54,0.00,400.00,0.204984,0.213172,0.220219,0.209500,null,null,null
-2020-09-02T15:48:49Z,27.00,60.48,99,7,35.26,101.54,0.00,400.00,0.206883,0.213398,0.222523,0.210008,null,null,null
-2020-09-02T15:49:19Z,27.00,60.50,99,7,36.43,101.54,0.00,400.00,0.205828,0.213250,0.221758,0.209422,null,null,null
-2020-09-02T15:49:49Z,26.96,60.57,99,7,32.70,101.55,0.00,400.00,0.205359,0.212797,0.220406,0.209586,null,null,null
-2020-09-02T15:50:19Z,27.00,60.57,99,7,35.76,101.54,0.00,400.00,0.204961,0.213039,0.221594,0.209375,null,null,null
-2020-09-02T15:50:49Z,26.95,60.57,99,8,42.94,101.55,0.00,400.00,0.206383,0.213766,0.221234,0.210000,null,null,null
-2020-09-02T15:51:19Z,26.96,60.59,99,7,38.18,101.55,0.00,400.00,0.204117,0.212852,0.221930,0.210906,null,null,null
-2020-09-02T15:51:49Z,26.95,60.61,99,6,38.26,101.55,0.00,400.00,0.207234,0.213297,0.222516,0.211008,null,null,null
-2020-09-02T15:52:19Z,26.95,60.61,99,5,32.14,101.55,0.00,400.00,0.205336,0.212898,0.221781,0.210836,null,null,null
-2020-09-02T15:52:49Z,26.97,60.57,99,8,30.17,101.55,0.00,400.00,0.204727,0.212508,0.222797,0.210336,null,null,null
-2020-09-02T15:53:19Z,26.97,60.55,99,8,37.34,101.55,0.00,400.00,0.206938,0.212891,0.222500,0.210984,null,null,null
-2020-09-02T15:53:49Z,26.99,60.53,99,7,32.21,101.55,0.00,400.00,0.205258,0.212023,0.221672,0.211008,null,null,null
-2020-09-02T15:54:19Z,26.99,60.64,99,7,32.19,101.55,0.00,400.00,0.206125,0.214664,0.222227,0.210727,null,null,null
-2020-09-02T15:54:49Z,26.99,60.60,99,8,43.76,101.55,0.00,400.00,0.204906,0.213086,0.222469,0.210547,null,null,null
-2020-09-02T15:55:19Z,26.96,60.58,99,8,34.39,101.55,0.00,400.00,0.204617,0.212484,0.222930,0.211391,null,null,null
-2020-09-02T15:55:49Z,26.99,60.58,99,8,36.21,101.54,0.00,400.00,0.205656,0.213414,0.222344,0.210797,null,null,null
-2020-09-02T15:56:19Z,27.02,60.52,99,8,48.76,101.54,0.00,400.00,0.205133,0.212633,0.222352,0.210305,null,null,null
-2020-09-02T15:56:49Z,26.97,60.53,99,8,36.52,101.54,0.00,400.00,0.205109,0.212516,0.221766,0.210484,null,null,null
-2020-09-02T15:57:19Z,26.99,60.60,99,7,37.21,101.54,0.00,400.00,0.206148,0.213695,0.221531,0.211094,null,null,null
-2020-09-02T15:57:49Z,26.99,60.55,99,8,31.64,101.54,0.00,400.00,0.206313,0.212711,0.223742,0.210859,null,null,null
-2020-09-02T15:58:19Z,27.00,60.56,99,8,34.39,101.55,0.00,400.00,0.204586,0.212961,0.222344,0.210281,null,null,null
-2020-09-02T15:58:49Z,27.00,60.59,99,8,41.08,101.54,0.00,400.00,0.207320,0.214797,0.222914,0.209898,null,null,null
-2020-09-02T15:59:19Z,26.97,60.59,99,8,34.42,101.55,0.00,400.00,0.205398,0.212945,0.222797,0.210688,null,null,null
-2020-09-02T15:59:49Z,27.03,60.56,99,7,32.98,101.54,0.00,400.00,0.205836,0.214078,0.223273,0.210930,null,null,null
-2020-09-02T16:00:19Z,27.02,60.47,99,7,45.93,101.55,0.00,400.00,0.206547,0.213687,0.221992,0.210367,null,null,null
-2020-09-02T16:00:49Z,27.03,60.56,99,7,45.68,101.55,0.00,400.00,0.206117,0.213086,0.223102,0.210484,null,null,null
-2020-09-02T16:01:19Z,27.03,60.51,99,7,36.86,101.55,0.00,400.00,0.206289,0.212992,0.222922,0.210445,null,null,null
-2020-09-02T16:01:49Z,27.03,60.46,99,8,40.82,101.55,0.00,400.00,0.206078,0.213062,0.223320,0.211375,null,null,null
-2020-09-02T16:02:19Z,27.02,60.50,99,7,39.18,101.54,0.00,400.00,0.205875,0.213367,0.223180,0.211406,null,null,null
-2020-09-02T16:02:49Z,27.00,60.52,99,7,45.35,101.54,0.00,400.00,0.206047,0.214047,0.222969,0.210422,null,null,null
-2020-09-02T16:03:19Z,27.00,60.51,99,7,34.89,101.55,0.00,400.00,0.206711,0.213508,0.223648,0.211547,null,null,null
-2020-09-02T16:03:49Z,27.03,60.47,99,7,32.08,101.54,0.00,400.00,0.204516,0.213039,0.222047,0.210570,null,null,null
-2020-09-02T16:04:19Z,27.06,60.48,99,7,31.69,101.55,0.00,400.00,0.205422,0.213477,0.223508,0.210727,null,null,null
-2020-09-02T16:04:49Z,27.07,60.41,99,7,36.52,101.54,0.00,400.00,0.205445,0.212398,0.223117,0.211187,null,null,null
-2020-09-02T16:05:19Z,27.05,60.43,99,7,35.50,101.54,0.00,400.00,0.206125,0.212609,0.221875,0.211305,null,null,null
-2020-09-02T16:05:49Z,27.07,60.42,99,8,32.35,101.54,0.00,400.00,0.207102,0.214508,0.223023,0.211469,null,null,null
-2020-09-02T16:06:19Z,27.05,60.49,99,7,36.51,101.55,0.00,400.00,0.206742,0.213922,0.223125,0.209969,null,null,null
-2020-09-02T16:06:49Z,27.02,60.53,99,7,36.01,101.54,0.00,400.00,0.207289,0.214484,0.224398,0.211156,null,null,null
-2020-09-02T16:07:19Z,26.99,60.60,99,7,35.25,101.54,0.00,400.00,0.205820,0.213930,0.223703,0.211555,null,null,null
-2020-09-02T16:07:49Z,26.97,60.65,99,7,34.31,101.55,0.00,400.00,0.206648,0.213461,0.223125,0.211383,null,null,null
-2020-09-02T16:08:19Z,26.96,60.73,99,7,38.52,101.56,0.00,400.00,0.204992,0.212555,0.221437,0.210734,null,null,null
-2020-09-02T16:08:49Z,26.97,60.74,99,7,35.89,101.55,0.00,400.00,0.205734,0.213273,0.223063,0.211195,null,null,null
-2020-09-02T16:09:19Z,26.93,60.78,99,7,33.21,101.55,0.00,400.00,0.207563,0.213555,0.223133,0.210875,null,null,null
-2020-09-02T16:09:49Z,26.93,60.80,99,7,36.80,101.55,0.00,400.00,0.205469,0.213523,0.222320,0.211680,null,null,null
-2020-09-02T16:10:19Z,26.87,60.95,99,7,36.63,101.55,0.00,400.00,0.206687,0.213414,0.222430,0.210742,null,null,null
-2020-09-02T16:10:49Z,26.87,61.00,99,8,46.74,101.55,0.00,400.00,0.207016,0.214195,0.223289,0.211391,null,null,null
-2020-09-02T16:11:19Z,26.86,61.04,99,7,35.17,101.55,0.00,400.00,0.207609,0.214445,0.224172,0.211297,null,null,null
-2020-09-02T16:11:49Z,26.85,61.08,99,7,42.57,101.55,0.00,400.00,0.205437,0.215094,0.223805,0.211781,null,null,null
-2020-09-02T16:12:19Z,26.83,61.16,99,7,44.69,101.54,0.00,400.00,0.207391,0.213977,0.223180,0.211430,null,null,null
-2020-09-02T16:12:49Z,26.82,61.16,99,7,47.68,101.55,0.00,400.00,0.207133,0.213227,0.223523,0.211562,null,null,null
-2020-09-02T16:13:19Z,26.83,61.16,99,7,32.53,101.55,0.00,400.00,0.205820,0.214117,0.223766,0.211578,null,null,null
-2020-09-02T16:13:49Z,26.79,61.20,99,7,31.89,101.55,0.00,400.00,0.205664,0.214711,0.222969,0.211195,null,null,null
-2020-09-02T16:14:19Z,26.80,61.15,99,7,37.32,101.55,0.00,400.00,0.206281,0.214453,0.222570,0.211367,null,null,null
-2020-09-02T16:14:49Z,26.82,61.18,99,7,32.34,101.55,0.00,400.00,0.206930,0.213391,0.224461,0.211672,null,null,null
-2020-09-02T16:15:19Z,26.83,61.12,99,7,45.62,101.55,0.00,400.00,0.207438,0.214492,0.224328,0.211078,null,null,null
-2020-09-02T16:15:49Z,26.80,61.18,99,7,41.62,101.55,0.00,400.00,0.206062,0.214328,0.222820,0.211266,null,null,null
-2020-09-02T16:16:19Z,26.82,61.16,99,7,34.80,101.55,0.00,400.00,0.205984,0.214695,0.223203,0.211453,null,null,null
-2020-09-02T16:16:49Z,26.79,61.14,99,6,35.80,101.54,0.00,400.00,0.208359,0.214234,0.223711,0.211437,null,null,null
-2020-09-02T16:17:19Z,26.80,61.27,99,6,36.20,101.55,0.00,400.00,0.206930,0.213594,0.224242,0.212016,null,null,null
-2020-09-02T16:17:49Z,26.78,61.22,99,7,33.81,101.55,0.00,400.00,0.205547,0.213945,0.223125,0.211508,null,null,null
-2020-09-02T16:18:19Z,26.80,61.23,99,6,38.43,101.55,0.00,400.00,0.207672,0.214211,0.223344,0.211891,null,null,null
-2020-09-02T16:18:49Z,26.79,61.27,99,1,45.28,101.55,0.00,400.00,0.206477,0.214055,0.224125,0.211414,null,null,null
-2020-09-02T16:19:19Z,26.76,61.28,99,0,43.63,101.54,0.00,400.00,0.206469,0.213453,0.223391,0.211852,null,null,null
-2020-09-02T16:19:49Z,26.75,61.32,99,0,41.21,101.55,0.00,400.00,0.205992,0.213898,0.224203,0.211570,null,null,null
-2020-09-02T16:20:19Z,26.75,61.33,99,1,44.33,101.55,0.00,400.00,0.205758,0.213734,0.222344,0.211898,null,null,null
-2020-09-02T16:20:49Z,26.75,61.36,99,4,40.12,101.55,0.00,400.00,0.206813,0.214000,0.222297,0.211492,null,null,null
-2020-09-02T16:21:19Z,26.75,61.37,99,6,40.87,101.55,0.00,400.00,0.205852,0.214367,0.223797,0.211672,null,null,null
-2020-09-02T16:21:49Z,26.75,61.41,99,7,32.16,101.55,0.00,400.00,0.205320,0.213961,0.221609,0.210898,null,null,null
-2020-09-02T16:22:19Z,26.75,61.40,99,6,39.42,101.55,0.00,400.00,0.207672,0.214813,0.221852,0.212117,null,null,null
-2020-09-02T16:22:49Z,26.76,61.41,99,6,36.05,101.55,0.00,400.00,0.206008,0.214141,0.224672,0.211570,null,null,null
-2020-09-02T16:23:19Z,26.76,61.31,99,6,32.24,101.55,0.00,400.00,0.205016,0.213344,0.223203,0.211680,null,null,null
-2020-09-02T16:23:49Z,26.76,61.31,99,7,39.06,101.55,0.00,400.00,0.207695,0.214789,0.223805,0.211625,null,null,null
-2020-09-02T16:24:19Z,26.78,61.33,99,7,35.99,101.54,0.00,400.00,0.207047,0.214836,0.224828,0.211477,null,null,null
-2020-09-02T16:24:49Z,26.75,61.37,99,8,40.18,101.55,0.00,400.00,0.205586,0.212586,0.223281,0.212070,null,null,null
-2020-09-02T16:25:19Z,26.75,61.36,99,7,40.32,101.54,0.00,400.00,0.206703,0.215062,0.224242,0.211539,null,null,null
-2020-09-02T16:25:49Z,26.76,61.35,99,7,39.47,101.54,0.00,400.00,0.207305,0.214164,0.224664,0.212141,null,null,null
-2020-09-02T16:26:19Z,26.78,61.34,99,2,59.45,101.55,0.00,400.00,0.206602,0.214422,0.224352,0.212078,null,null,null
-2020-09-02T16:26:49Z,26.80,61.31,99,6,46.54,101.55,0.00,400.00,0.207609,0.215031,0.224180,0.212102,null,null,null
-2020-09-02T16:27:19Z,26.79,61.22,99,7,46.24,101.55,0.00,400.00,0.206320,0.213844,0.224227,0.212094,null,null,null
-2020-09-02T16:27:49Z,26.76,61.28,99,7,43.74,101.55,0.00,400.00,0.209039,0.216055,0.224859,0.211500,null,null,null
-2020-09-02T16:28:19Z,26.78,61.31,99,6,46.79,101.55,0.00,402.00,0.207641,0.214789,0.223727,0.211203,null,null,null
-2020-09-02T16:28:49Z,26.80,61.30,99,6,43.63,101.55,0.00,402.00,0.206953,0.214203,0.224023,0.212062,null,null,null
-2020-09-02T16:29:19Z,26.76,61.28,99,5,35.82,101.55,0.00,400.00,0.206859,0.214570,0.222891,0.211195,null,null,null
-2020-09-02T16:29:49Z,26.79,61.31,99,5,41.48,101.55,0.00,400.00,0.206852,0.214547,0.224055,0.212008,null,null,null
-2020-09-02T16:30:19Z,26.75,61.35,99,7,44.71,101.55,0.00,400.00,0.205484,0.213828,0.225242,0.212727,null,null,null
-2020-09-02T16:30:49Z,26.78,61.35,99,5,45.54,101.55,0.00,400.00,0.205508,0.213180,0.224031,0.211352,null,null,null
-2020-09-02T16:31:19Z,26.79,61.35,99,7,45.54,101.55,0.00,400.00,0.207469,0.213523,0.223875,0.211805,null,null,null
-2020-09-02T16:31:49Z,26.78,61.41,99,6,56.88,101.55,0.00,400.00,0.207703,0.214992,0.222477,0.211820,null,null,null
-2020-09-02T16:32:19Z,26.76,61.36,99,6,43.66,101.54,0.00,400.00,0.206664,0.213047,0.223742,0.212445,null,null,null
-2020-09-02T16:32:49Z,26.78,61.38,99,6,56.30,101.55,0.00,400.00,0.206516,0.212938,0.223891,0.211516,null,null,null
-2020-09-02T16:33:19Z,26.78,61.41,99,5,53.03,101.54,0.00,400.00,0.206992,0.214039,0.223867,0.212344,null,null,null
-2020-09-02T16:33:49Z,26.79,61.42,99,5,52.41,101.55,0.00,400.00,0.207719,0.214008,0.224258,0.211375,null,null,null
-2020-09-02T16:34:19Z,26.76,61.41,99,5,43.36,101.55,0.00,400.00,0.206750,0.215180,0.224078,0.212000,null,null,null
-2020-09-02T16:34:49Z,26.78,61.41,99,5,51.47,101.54,0.00,400.00,0.207023,0.214602,0.222633,0.212039,null,null,null
-2020-09-02T16:35:19Z,26.76,61.42,99,5,53.53,101.55,0.00,400.00,0.205953,0.213906,0.225008,0.211875,null,null,null
-2020-09-02T16:35:49Z,26.80,61.42,99,5,46.54,101.55,0.00,400.00,0.206281,0.213094,0.226086,0.212117,null,null,null
-2020-09-02T16:36:19Z,26.78,61.43,99,6,34.88,101.55,0.00,400.00,0.206578,0.214500,0.224703,0.212031,null,null,null
-2020-09-02T16:36:49Z,26.75,61.36,99,5,65.30,101.55,0.00,400.00,0.207359,0.214445,0.223805,0.212047,null,null,null
-2020-09-02T16:37:19Z,26.82,61.37,99,5,46.50,101.55,0.00,400.00,0.206766,0.214336,0.224883,0.212305,null,null,null
-2020-09-02T16:37:49Z,26.79,61.35,99,4,34.38,101.55,0.00,400.00,0.208000,0.214156,0.223797,0.213313,null,null,null
-2020-09-02T16:38:19Z,26.78,61.39,99,5,48.38,101.55,0.00,400.00,0.205398,0.213492,0.224906,0.213117,null,null,null
-2020-09-02T16:38:49Z,26.75,61.42,99,6,34.31,101.55,0.00,400.00,0.207773,0.214586,0.223102,0.212688,null,null,null
-2020-09-02T16:39:19Z,26.75,61.43,99,5,50.82,101.55,0.00,400.00,0.208859,0.215453,0.225828,0.212836,null,null,null
-2020-09-02T16:39:49Z,26.78,61.45,99,7,47.49,101.55,0.00,400.00,0.207188,0.213484,0.224836,0.211977,null,null,null
-2020-09-02T16:40:19Z,26.76,61.45,99,6,46.84,101.55,0.00,400.00,0.206727,0.214508,0.223656,0.212164,null,null,null
-2020-09-02T16:40:49Z,26.79,61.45,99,5,48.08,101.55,0.00,400.00,0.208398,0.214859,0.224211,0.212328,null,null,null
-2020-09-02T16:41:19Z,26.78,61.47,99,5,48.27,101.55,0.00,400.00,0.205586,0.214328,0.224258,0.212211,null,null,null
-2020-09-02T16:41:49Z,26.80,61.43,99,5,35.00,101.55,0.00,400.00,0.206742,0.213648,0.224172,0.211906,null,null,null
-2020-09-02T16:42:19Z,26.78,61.45,99,6,51.34,101.55,0.00,400.00,0.207219,0.215109,0.223820,0.212094,null,null,null
-2020-09-02T16:42:49Z,26.79,61.43,99,7,59.59,101.55,0.00,400.00,0.206422,0.213898,0.223500,0.211391,null,null,null
-2020-09-02T16:43:19Z,26.79,61.38,99,6,53.25,101.55,0.00,400.00,0.206484,0.213695,0.223320,0.212234,null,null,null
-2020-09-02T16:43:49Z,26.76,61.39,99,5,51.15,101.55,0.00,400.00,0.207797,0.214617,0.224539,0.212711,null,null,null
-2020-09-02T16:44:19Z,26.78,61.44,99,6,61.55,101.55,0.00,400.00,0.207305,0.215000,0.225336,0.212219,null,null,null
-2020-09-02T16:44:49Z,26.78,61.46,99,7,55.02,101.55,0.00,400.00,0.207531,0.214461,0.223234,0.211562,null,null,null
-2020-09-02T16:45:19Z,26.79,61.46,99,6,54.41,101.55,0.00,400.00,0.206820,0.214336,0.224805,0.212578,null,null,null
-2020-09-02T16:45:49Z,26.78,61.38,99,5,44.06,101.55,0.00,400.00,0.207352,0.214844,0.225031,0.212148,null,null,null
-2020-09-02T16:46:19Z,26.76,61.41,99,5,45.74,101.55,1.00,408.00,0.206211,0.213234,0.224695,0.212711,null,null,null
-2020-09-02T16:46:49Z,26.78,61.40,99,5,43.05,101.55,1.00,408.00,0.206156,0.215219,0.224086,0.212523,null,null,null
-2020-09-02T16:47:19Z,26.78,61.36,99,7,46.29,101.55,0.00,403.00,0.208367,0.215367,0.223906,0.212164,null,null,null
-2020-09-02T16:47:49Z,26.76,61.37,99,6,38.83,101.55,0.00,403.00,0.207602,0.213984,0.226141,0.212297,null,null,null
-2020-09-02T16:48:19Z,26.80,61.46,99,6,49.41,101.56,1.00,408.00,0.208641,0.215797,0.224578,0.212383,null,null,null
-2020-09-02T16:48:49Z,26.76,61.42,99,7,54.37,101.56,1.00,408.00,0.207320,0.215383,0.225570,0.213031,null,null,null
-2020-09-02T16:49:19Z,26.78,61.42,99,7,38.22,101.56,0.00,400.00,0.207773,0.215164,0.224750,0.212375,null,null,null
-2020-09-02T16:49:49Z,26.78,61.40,99,5,48.10,101.55,0.00,400.00,0.207055,0.214469,0.225086,0.212930,null,null,null
-2020-09-02T16:50:19Z,26.80,61.41,99,6,47.12,101.56,0.00,400.00,0.206586,0.214000,0.226313,0.212727,null,null,null
-2020-09-02T16:50:49Z,26.78,61.43,99,6,39.72,101.56,0.00,400.00,0.208609,0.214609,0.223703,0.211812,null,null,null
-2020-09-02T16:51:19Z,26.80,61.43,99,5,32.02,101.56,0.00,400.00,0.208852,0.215758,0.223945,0.212617,null,null,null
-2020-09-02T16:51:49Z,26.82,61.39,99,7,50.12,101.56,0.00,400.00,0.207805,0.216219,0.225094,0.212555,null,null,null
-2020-09-02T16:52:19Z,26.82,61.37,99,7,40.76,101.56,0.00,400.00,0.207328,0.214469,0.224203,0.211898,null,null,null
-2020-09-02T16:52:49Z,26.80,61.40,99,5,32.03,101.56,0.00,400.00,0.206922,0.214133,0.226516,0.213156,null,null,null
-2020-09-02T16:53:19Z,26.79,61.39,99,5,47.70,101.56,0.00,400.00,0.205969,0.213117,0.224906,0.213055,null,null,null
-2020-09-02T16:53:49Z,26.82,61.39,99,6,34.54,101.56,0.00,400.00,0.207937,0.214273,0.224992,0.212563,null,null,null
-2020-09-02T16:54:19Z,26.78,61.41,99,11,44.06,101.56,0.00,400.00,0.209273,0.215672,0.224336,0.211969,null,null,null
-2020-09-02T16:54:49Z,26.79,61.40,99,5,46.32,101.56,0.00,400.00,0.207891,0.215250,0.223969,0.212836,null,null,null
-2020-09-02T16:55:19Z,26.79,61.41,99,5,43.35,101.56,0.00,400.00,0.206594,0.213719,0.225914,0.212344,null,null,null
-2020-09-02T16:55:49Z,26.79,61.41,99,6,42.66,101.55,0.00,400.00,0.208258,0.215445,0.225977,0.212969,null,null,null
-2020-09-02T16:56:19Z,26.79,61.39,99,7,34.32,101.56,0.00,400.00,0.207937,0.214820,0.225680,0.212367,null,null,null
-2020-09-02T16:56:49Z,26.80,61.39,99,6,34.39,101.56,0.00,400.00,0.206648,0.214336,0.224789,0.212453,null,null,null
-2020-09-02T16:57:19Z,26.82,61.39,99,5,39.51,101.56,0.00,400.00,0.207695,0.215461,0.224430,0.212563,null,null,null
-2020-09-02T16:57:49Z,26.80,61.37,99,6,30.78,101.56,0.00,400.00,0.206250,0.214492,0.224578,0.212461,null,null,null
-2020-09-02T16:58:19Z,26.80,61.38,99,5,34.31,101.56,0.00,400.00,0.207297,0.214250,0.223734,0.212477,null,null,null
-2020-09-02T16:58:49Z,26.80,61.34,99,5,33.83,101.56,0.00,400.00,0.206297,0.213625,0.226031,0.212625,null,null,null
-2020-09-02T16:59:19Z,26.80,61.37,99,6,34.66,101.56,0.00,400.00,0.207500,0.214289,0.226539,0.213430,null,null,null
-2020-09-02T16:59:49Z,26.80,61.33,99,6,35.41,101.56,0.00,400.00,0.206578,0.214547,0.225102,0.212742,null,null,null
-2020-09-02T17:00:19Z,26.78,61.37,99,5,28.19,101.56,0.00,400.00,0.207625,0.214445,0.223641,0.212352,null,null,null
-2020-09-02T17:00:49Z,26.79,61.37,99,5,33.32,101.56,0.00,400.00,0.207430,0.215664,0.224883,0.212625,null,null,null
-2020-09-02T17:01:19Z,26.79,61.32,99,5,30.39,101.56,0.00,400.00,0.206867,0.214656,0.224719,0.212437,null,null,null
-2020-09-02T17:01:49Z,26.79,61.32,99,3,36.65,101.56,0.00,400.00,0.207539,0.214023,0.225898,0.212711,null,null,null
-2020-09-02T17:02:19Z,26.80,61.28,99,3,39.84,101.56,0.00,400.00,0.207164,0.214500,0.224578,0.213398,null,null,null
-2020-09-02T17:02:49Z,26.82,61.33,99,5,36.84,101.56,0.00,400.00,0.208219,0.215352,0.224742,0.212859,null,null,null
-2020-09-02T17:03:19Z,26.79,61.33,99,2,39.69,101.56,0.00,400.00,0.206375,0.213859,0.224219,0.212672,null,null,null
-2020-09-02T17:03:49Z,26.80,61.29,99,2,38.25,101.56,0.00,400.00,0.206648,0.214117,0.226453,0.212969,null,null,null
-2020-09-02T17:04:19Z,26.82,61.32,99,1,32.85,101.56,0.00,400.00,0.207672,0.214719,0.225938,0.212609,null,null,null
-2020-09-02T17:04:49Z,26.80,61.29,99,1,33.37,101.56,0.00,400.00,0.206445,0.215312,0.224758,0.212484,null,null,null
-2020-09-02T17:05:19Z,26.85,61.30,99,0,28.27,101.56,0.00,400.00,0.206352,0.213633,0.224727,0.213109,null,null,null
-2020-09-02T17:05:49Z,26.82,61.33,99,0,34.98,101.57,0.00,400.00,0.206633,0.214422,0.224797,0.212570,null,null,null
-2020-09-02T17:06:19Z,26.82,61.34,99,0,35.85,101.56,0.00,400.00,0.207031,0.214281,0.226344,0.212852,null,null,null
-2020-09-02T17:06:49Z,26.82,61.33,99,0,38.67,101.56,0.00,400.00,0.207961,0.215492,0.226727,0.213148,null,null,null
-2020-09-02T17:07:19Z,26.80,61.31,99,0,37.07,101.56,0.00,400.00,0.207680,0.214039,0.224375,0.213039,null,null,null
-2020-09-02T17:07:49Z,26.80,61.34,99,0,30.61,101.56,0.00,400.00,0.207180,0.215070,0.225367,0.212367,null,null,null
-2020-09-02T17:08:19Z,26.82,61.29,99,0,38.02,101.56,0.00,400.00,0.206391,0.213844,0.225328,0.212437,null,null,null
-2020-09-02T17:08:49Z,26.79,61.31,99,0,31.37,101.56,0.00,400.00,0.207438,0.213516,0.226172,0.213125,null,null,null
-2020-09-02T17:09:19Z,26.80,61.37,99,0,29.62,101.57,0.00,402.00,0.207156,0.215523,0.224172,0.212820,null,null,null
-2020-09-02T17:09:49Z,26.80,61.38,99,0,31.27,101.56,0.00,402.00,0.209031,0.214883,0.223305,0.212711,null,null,null
-2020-09-02T17:10:19Z,26.80,61.36,99,0,29.51,101.56,0.00,400.00,0.207000,0.214344,0.226164,0.212883,null,null,null
-2020-09-02T17:10:49Z,26.83,61.31,99,0,29.40,101.57,0.00,400.00,0.206687,0.214961,0.226812,0.213250,null,null,null
-2020-09-02T17:11:19Z,26.82,61.30,99,0,36.35,101.57,0.00,400.00,0.208094,0.214586,0.224703,0.212531,null,null,null
-2020-09-02T17:11:49Z,26.85,61.26,99,0,32.61,101.57,0.00,400.00,0.206211,0.214477,0.225570,0.211906,null,null,null
-2020-09-02T17:12:19Z,26.82,61.24,99,0,33.21,101.57,0.00,400.00,0.206820,0.215023,0.225984,0.213922,null,null,null
-2020-09-02T17:12:49Z,26.82,61.21,99,0,29.61,101.57,0.00,400.00,0.208477,0.214820,0.225648,0.212555,null,null,null
-2020-09-02T17:13:19Z,26.83,61.26,99,0,42.91,101.57,0.00,400.00,0.208016,0.214961,0.226070,0.213828,null,null,null
-2020-09-02T17:13:49Z,26.80,61.28,99,0,41.18,101.57,0.00,400.00,0.208328,0.214945,0.226492,0.213047,null,null,null
-2020-09-02T17:14:19Z,26.78,61.31,99,0,43.03,101.57,0.00,400.00,0.207469,0.215141,0.226500,0.212641,null,null,null
-2020-09-02T17:14:49Z,26.83,61.28,99,0,43.33,101.57,0.00,400.00,0.205742,0.212578,0.224055,0.213188,null,null,null
-2020-09-02T17:15:19Z,26.80,61.20,99,0,41.11,101.57,0.00,400.00,0.208203,0.214227,0.224867,0.212961,null,null,null
-2020-09-02T17:15:49Z,26.79,61.27,99,0,30.39,101.57,0.00,400.00,0.207789,0.215219,0.225117,0.213117,null,null,null
-2020-09-02T17:16:19Z,26.79,61.27,99,0,36.02,101.57,0.00,401.00,0.207438,0.215047,0.225133,0.212414,null,null,null
-2020-09-02T17:16:49Z,26.80,61.27,99,0,29.92,101.57,0.00,401.00,0.209359,0.215578,0.226820,0.212984,null,null,null
-2020-09-02T17:17:19Z,26.80,61.24,99,0,36.32,101.57,0.00,401.00,0.206336,0.215016,0.225812,0.213211,null,null,null
-2020-09-02T17:17:49Z,26.80,61.22,99,0,35.67,101.57,0.00,401.00,0.207609,0.214648,0.225125,0.212867,null,null,null
-2020-09-02T17:18:19Z,26.80,61.21,99,0,32.17,101.57,0.00,400.00,0.207242,0.214820,0.224914,0.213305,null,null,null
-2020-09-02T17:18:49Z,26.82,61.21,99,0,31.75,101.57,0.00,400.00,0.206938,0.214094,0.224031,0.213023,null,null,null
-2020-09-02T17:19:19Z,26.78,61.18,99,0,40.38,101.57,0.00,405.00,0.207727,0.214953,0.225906,0.213195,null,null,null
-2020-09-02T17:19:49Z,26.80,61.18,99,0,31.25,101.57,0.00,405.00,0.207297,0.214617,0.226156,0.213406,null,null,null
-2020-09-02T17:20:19Z,26.78,61.15,99,0,38.03,101.57,0.00,405.00,0.208445,0.214695,0.225328,0.212898,null,null,null
-2020-09-02T17:20:49Z,26.80,61.21,99,0,32.58,101.57,0.00,405.00,0.206430,0.213727,0.225602,0.212633,null,null,null
-2020-09-02T17:21:19Z,26.79,61.15,99,0,41.62,101.57,0.00,402.00,0.207336,0.214969,0.226250,0.213156,null,null,null
-2020-09-02T17:21:49Z,26.82,61.15,99,0,29.18,101.57,0.00,402.00,0.205812,0.213859,0.226742,0.213500,null,null,null
-2020-09-02T17:22:19Z,26.79,61.14,99,0,31.99,101.57,0.00,400.00,0.208039,0.214164,0.224547,0.213305,null,null,null
-2020-09-02T17:22:49Z,26.79,61.15,99,0,44.61,101.57,0.00,400.00,0.207211,0.215258,0.226445,0.213117,null,null,null
-2020-09-02T17:23:19Z,26.82,61.18,99,0,29.50,101.57,0.00,400.00,0.208937,0.216547,0.225172,0.212922,null,null,null
-2020-09-02T17:23:49Z,26.80,61.15,99,0,33.33,101.57,0.00,400.00,0.206695,0.215125,0.224625,0.212555,null,null,null
-2020-09-02T17:24:19Z,26.79,61.11,99,0,36.83,101.57,0.00,400.00,0.207914,0.214547,0.225984,0.212883,null,null,null
-2020-09-02T17:24:49Z,26.79,61.13,99,0,30.81,101.57,0.00,400.00,0.207391,0.215375,0.225789,0.213109,null,null,null
-2020-09-02T17:25:19Z,26.80,61.12,99,0,29.84,101.57,0.00,400.00,0.207805,0.214430,0.224906,0.212852,null,null,null
-2020-09-02T17:25:49Z,26.79,61.17,99,0,37.42,101.57,0.00,400.00,0.208203,0.215703,0.225734,0.213227,null,null,null
-2020-09-02T17:26:19Z,26.82,61.20,99,0,31.45,101.57,0.00,400.00,0.206477,0.214359,0.226523,0.213570,null,null,null
-2020-09-02T17:26:49Z,26.80,61.15,99,0,30.40,101.57,0.00,400.00,0.206437,0.214586,0.227227,0.213367,null,null,null
-2020-09-02T17:27:19Z,26.82,61.08,99,0,35.69,101.57,0.00,400.00,0.207172,0.215352,0.225313,0.213094,null,null,null
-2020-09-02T17:27:49Z,26.82,61.10,99,0,31.87,101.57,0.00,400.00,0.208070,0.214516,0.227023,0.213719,null,null,null
-2020-09-02T17:28:19Z,26.83,61.08,99,0,32.04,101.57,0.00,400.00,0.207203,0.215719,0.225180,0.212648,null,null,null
-2020-09-02T17:28:49Z,26.82,61.15,99,0,33.93,101.57,0.00,400.00,0.206672,0.214234,0.224414,0.212617,null,null,null
-2020-09-02T17:29:19Z,26.85,61.15,99,0,43.52,101.57,0.00,400.00,0.208273,0.215297,0.224484,0.212656,null,null,null
-2020-09-02T17:29:49Z,26.83,61.09,99,0,37.06,101.57,0.00,400.00,0.208102,0.215359,0.225805,0.213477,null,null,null
-2020-09-02T17:30:19Z,26.79,61.14,99,0,40.34,101.57,0.00,400.00,0.208469,0.215320,0.227023,0.213234,null,null,null
-2020-09-02T17:30:49Z,26.82,61.13,99,0,42.09,101.57,0.00,400.00,0.207797,0.214680,0.224344,0.213211,null,null,null
-2020-09-02T17:31:19Z,26.79,61.12,99,0,29.60,101.57,0.00,400.00,0.207219,0.215008,0.227078,0.213750,null,null,null
-2020-09-02T17:31:49Z,26.82,61.13,99,0,34.32,101.57,0.00,400.00,0.206805,0.214695,0.226555,0.213117,null,null,null
-2020-09-02T17:32:19Z,26.80,60.99,99,0,42.81,101.57,0.00,400.00,0.207398,0.214031,0.226453,0.213094,null,null,null
-2020-09-02T17:32:49Z,26.85,60.99,99,0,34.25,101.58,0.00,400.00,0.208008,0.215836,0.226562,0.213969,null,null,null
-2020-09-02T17:33:19Z,26.82,61.00,99,0,34.73,101.57,0.00,400.00,0.207828,0.215539,0.224977,0.212836,null,null,null
-2020-09-02T17:33:49Z,26.85,61.05,99,0,36.24,101.58,0.00,400.00,0.209148,0.215375,0.224445,0.212453,null,null,null
-2020-09-02T17:34:19Z,26.85,61.08,99,0,34.10,101.58,0.00,400.00,0.206523,0.215633,0.224898,0.212664,null,null,null
-2020-09-02T17:34:49Z,26.83,61.04,99,0,32.62,101.58,0.00,400.00,0.207820,0.215023,0.226039,0.213086,null,null,null
-2020-09-02T17:35:19Z,26.82,61.07,99,0,32.95,101.58,0.00,400.00,0.208031,0.215641,0.223375,0.212648,null,null,null
-2020-09-02T17:35:49Z,26.85,61.09,99,0,33.98,101.58,0.00,400.00,0.208555,0.215687,0.225195,0.213344,null,null,null
-2020-09-02T17:36:19Z,26.85,61.07,99,0,30.12,101.58,0.00,400.00,0.207297,0.215039,0.224789,0.213172,null,null,null
-2020-09-02T17:36:49Z,26.82,61.12,99,0,28.95,101.58,0.00,400.00,0.206867,0.214625,0.224875,0.213484,null,null,null
-2020-09-02T17:37:19Z,26.83,61.07,99,0,32.12,101.58,0.00,400.00,0.207930,0.214156,0.226383,0.213789,null,null,null
-2020-09-02T17:37:49Z,26.83,61.05,99,0,35.35,101.58,0.00,400.00,0.207297,0.214711,0.225391,0.213367,null,null,null
-2020-09-02T17:38:19Z,26.83,61.06,99,0,33.84,101.58,0.00,400.00,0.208477,0.215180,0.226562,0.213336,null,null,null
-2020-09-02T17:38:49Z,26.85,60.99,99,0,37.91,101.59,0.00,400.00,0.207633,0.215625,0.226664,0.213656,null,null,null
-2020-09-02T17:39:19Z,26.85,61.07,99,0,43.89,101.58,0.00,400.00,0.207828,0.215562,0.224906,0.213344,null,null,null
-2020-09-02T17:39:49Z,26.83,61.06,99,0,42.91,101.58,0.00,400.00,0.207914,0.214680,0.227258,0.213211,null,null,null
-2020-09-02T17:40:19Z,26.83,61.10,99,0,33.79,101.58,0.00,400.00,0.208562,0.216000,0.227531,0.214320,null,null,null
-2020-09-02T17:40:49Z,26.86,61.05,99,0,31.88,101.59,0.00,400.00,0.208992,0.215375,0.225039,0.213617,null,null,null
-2020-09-02T17:41:19Z,26.85,61.02,99,0,34.28,101.59,0.00,400.00,0.207523,0.215930,0.226875,0.213266,null,null,null
-2020-09-02T17:41:49Z,26.86,61.01,99,0,33.50,101.59,0.00,400.00,0.208242,0.215047,0.227148,0.214398,null,null,null
-2020-09-02T17:42:19Z,26.83,61.06,99,0,29.00,101.59,0.00,400.00,0.207320,0.215672,0.225102,0.212563,null,null,null
-2020-09-02T17:42:49Z,26.83,61.07,99,0,30.12,101.59,0.00,400.00,0.207125,0.215648,0.226063,0.213820,null,null,null
-2020-09-02T17:43:19Z,26.83,61.03,99,0,29.49,101.59,0.00,400.00,0.207336,0.214719,0.227195,0.214188,null,null,null
-2020-09-02T17:43:49Z,26.85,61.04,99,0,44.31,101.59,0.00,400.00,0.206977,0.214227,0.225695,0.213695,null,null,null
-2020-09-02T17:44:19Z,26.83,61.02,99,0,31.26,101.60,0.00,400.00,0.208461,0.215945,0.226203,0.213570,null,null,null
-2020-09-02T17:44:49Z,26.82,61.08,99,0,33.97,101.59,0.00,400.00,0.207609,0.214680,0.226430,0.212859,null,null,null
-2020-09-02T17:45:19Z,26.83,61.11,99,0,39.32,101.60,0.00,400.00,0.207164,0.214086,0.223922,0.212602,null,null,null
-2020-09-02T17:45:49Z,26.82,61.10,99,0,28.84,101.60,0.00,400.00,0.208148,0.215562,0.226313,0.213766,null,null,null
-2020-09-02T17:46:19Z,26.83,61.13,99,0,31.38,101.59,0.00,400.00,0.209219,0.216477,0.225461,0.213250,null,null,null
-2020-09-02T17:46:49Z,26.83,61.16,99,0,32.88,101.60,0.00,400.00,0.207563,0.214914,0.225438,0.214102,null,null,null
-2020-09-02T17:47:19Z,26.83,61.13,99,0,31.17,101.60,0.00,400.00,0.208469,0.215414,0.225305,0.213469,null,null,null
-2020-09-02T17:47:49Z,26.82,61.15,99,0,32.94,101.60,0.00,400.00,0.208312,0.214789,0.226484,0.213141,null,null,null
-2020-09-02T17:48:19Z,26.83,61.14,99,0,31.19,101.60,0.00,400.00,0.207297,0.215547,0.226523,0.214016,null,null,null
-2020-09-02T17:48:49Z,26.83,61.19,99,0,54.83,101.60,0.00,400.00,0.207125,0.214742,0.225156,0.214203,null,null,null
-2020-09-02T17:49:19Z,26.82,61.14,99,0,30.29,101.61,0.00,400.00,0.208383,0.216188,0.225477,0.213758,null,null,null
-2020-09-02T17:49:49Z,26.82,61.16,99,0,31.22,101.61,0.00,400.00,0.208242,0.216039,0.225266,0.213188,null,null,null
-2020-09-02T17:50:19Z,26.80,61.16,99,0,42.41,101.61,0.00,400.00,0.206961,0.214297,0.227336,0.213930,null,null,null
-2020-09-02T17:50:49Z,26.83,61.20,99,0,41.23,101.61,0.00,400.00,0.208117,0.215891,0.227539,0.213500,null,null,null
-2020-09-02T17:51:19Z,26.80,61.16,99,0,34.44,101.61,0.00,400.00,0.206086,0.214273,0.224820,0.212812,null,null,null
-2020-09-02T17:51:49Z,26.82,61.20,99,0,29.99,101.61,0.00,400.00,0.206734,0.215133,0.225102,0.213625,null,null,null
-2020-09-02T17:52:19Z,26.80,61.20,99,0,31.04,101.61,0.00,400.00,0.207594,0.214844,0.226750,0.213242,null,null,null
-2020-09-02T17:52:49Z,26.80,61.18,99,0,31.11,101.61,0.00,400.00,0.209164,0.215289,0.225453,0.213305,null,null,null
-2020-09-02T17:53:19Z,26.80,61.20,99,0,33.92,101.61,0.00,400.00,0.208508,0.214977,0.226141,0.213523,null,null,null
-2020-09-02T17:53:49Z,26.82,61.20,99,0,31.50,101.61,0.00,400.00,0.209414,0.216289,0.226586,0.213383,null,null,null
-2020-09-02T17:54:19Z,26.78,61.19,99,0,34.70,101.61,0.00,400.00,0.208727,0.216258,0.225695,0.213508,null,null,null
-2020-09-02T17:54:49Z,26.79,61.21,99,0,38.10,101.61,0.00,400.00,0.208438,0.215266,0.226523,0.214234,null,null,null
-2020-09-02T17:55:19Z,26.79,61.27,99,0,31.31,101.61,0.00,400.00,0.207766,0.215102,0.227242,0.213273,null,null,null
-2020-09-02T17:55:49Z,26.80,61.23,99,0,28.57,101.61,0.00,400.00,0.207312,0.215086,0.226367,0.213734,null,null,null
-2020-09-02T17:56:19Z,26.80,61.27,99,0,38.48,101.61,0.00,400.00,0.206273,0.214898,0.225859,0.212992,null,null,null
-2020-09-02T17:56:49Z,26.82,61.23,99,0,28.91,101.61,0.00,400.00,0.207320,0.214898,0.225812,0.213867,null,null,null
-2020-09-02T17:57:19Z,26.79,61.24,99,0,31.91,101.61,0.00,400.00,0.208906,0.215352,0.225930,0.214086,null,null,null
-2020-09-02T17:57:49Z,26.79,61.24,99,0,29.27,101.61,0.00,400.00,0.209273,0.215547,0.226656,0.213781,null,null,null
-2020-09-02T17:58:19Z,26.80,61.22,99,0,30.29,101.61,0.00,400.00,0.207945,0.215062,0.226000,0.213766,null,null,null
-2020-09-02T17:58:49Z,26.80,61.22,99,0,29.99,101.62,0.00,400.00,0.208750,0.215805,0.226633,0.213461,null,null,null
-2020-09-02T17:59:19Z,26.78,61.20,99,0,30.26,101.61,0.00,400.00,0.207391,0.215125,0.226633,0.213820,null,null,null
-2020-09-02T17:59:49Z,26.79,61.25,99,0,34.72,101.61,0.00,400.00,0.208008,0.215148,0.226562,0.213680,null,null,null
-2020-09-02T18:00:19Z,26.79,61.28,99,0,31.31,101.61,0.00,400.00,0.205984,0.214539,0.227500,0.213695,null,null,null
-2020-09-02T18:00:49Z,26.78,61.29,99,0,27.02,101.62,0.00,400.00,0.205453,0.214266,0.225539,0.213867,null,null,null
-2020-09-02T18:01:19Z,26.80,61.27,99,0,29.32,101.62,0.00,400.00,0.209055,0.216070,0.226313,0.212906,null,null,null
-2020-09-02T18:01:49Z,26.78,61.26,99,0,35.63,101.62,0.00,400.00,0.209156,0.215953,0.226430,0.213547,null,null,null
-2020-09-02T18:02:19Z,26.78,61.26,99,0,38.88,101.62,0.00,400.00,0.208336,0.215242,0.225914,0.213461,null,null,null
-2020-09-02T18:02:49Z,26.79,61.28,99,0,39.33,101.62,0.00,400.00,0.209094,0.216242,0.226711,0.213844,null,null,null
-2020-09-02T18:03:19Z,26.79,61.25,99,0,31.27,101.62,0.00,400.00,0.209000,0.215570,0.224812,0.213062,null,null,null
-2020-09-02T18:03:49Z,26.78,61.24,99,0,34.29,101.62,0.00,400.00,0.207891,0.215133,0.227961,0.214086,null,null,null
-2020-09-02T18:04:19Z,26.78,61.24,99,0,46.69,101.62,0.00,400.00,0.207148,0.215133,0.226242,0.213227,null,null,null
-2020-09-02T18:04:49Z,26.79,61.23,99,0,40.83,101.62,0.00,400.00,0.209305,0.215648,0.226727,0.213383,null,null,null
-2020-09-02T18:05:19Z,26.78,61.26,99,0,37.27,101.62,0.00,400.00,0.208336,0.215516,0.226258,0.212992,null,null,null
-2020-09-02T18:05:49Z,26.76,61.28,99,0,31.74,101.62,0.00,400.00,0.208133,0.215266,0.226125,0.213766,null,null,null
-2020-09-02T18:06:19Z,26.79,61.21,99,0,32.77,101.63,0.00,400.00,0.206531,0.215484,0.225531,0.213570,null,null,null
-2020-09-02T18:06:49Z,26.78,61.27,99,0,29.96,101.63,0.00,400.00,0.208000,0.216195,0.225664,0.213602,null,null,null
-2020-09-02T18:07:19Z,26.79,61.22,99,0,29.92,101.63,0.00,400.00,0.208273,0.214320,0.226359,0.214008,null,null,null
-2020-09-02T18:07:49Z,26.79,61.25,99,0,42.11,101.63,0.00,400.00,0.206781,0.214570,0.226320,0.213273,null,null,null
-2020-09-02T18:08:19Z,26.76,61.27,99,0,32.64,101.63,0.00,400.00,0.206328,0.214781,0.226922,0.213500,null,null,null
-2020-09-02T18:08:49Z,26.78,61.21,99,0,37.51,101.63,0.00,400.00,0.207547,0.215531,0.224961,0.212906,null,null,null
-2020-09-02T18:09:19Z,26.79,61.26,99,0,47.01,101.63,0.00,400.00,0.208859,0.216266,0.227125,0.213547,null,null,null
-2020-09-02T18:09:49Z,26.79,61.26,99,0,40.44,101.63,0.00,400.00,0.209438,0.216672,0.227109,0.213492,null,null,null
-2020-09-02T18:10:19Z,26.76,61.24,99,0,33.06,101.63,0.00,400.00,0.208305,0.214883,0.226398,0.213570,null,null,null
-2020-09-02T18:10:49Z,26.76,61.30,99,0,36.35,101.63,0.00,400.00,0.207516,0.216461,0.227477,0.214453,null,null,null
-2020-09-02T18:11:19Z,26.79,61.27,99,0,29.37,101.63,0.00,405.00,0.207602,0.215523,0.226008,0.213500,null,null,null
-2020-09-02T18:11:49Z,26.76,61.24,99,0,32.70,101.64,0.00,405.00,0.210156,0.216102,0.225844,0.213703,null,null,null
-2020-09-02T18:12:19Z,26.78,61.22,99,0,47.85,101.63,0.00,400.00,0.207945,0.215914,0.228008,0.214234,null,null,null
-2020-09-02T18:12:49Z,26.78,61.25,99,0,28.51,101.63,0.00,400.00,0.208289,0.215875,0.225547,0.213523,null,null,null
-2020-09-02T18:13:19Z,26.82,61.26,99,0,29.62,101.63,0.00,405.00,0.207180,0.215836,0.224617,0.213211,null,null,null
-2020-09-02T18:13:49Z,26.75,61.27,99,0,35.93,101.63,0.00,405.00,0.207570,0.214719,0.226805,0.213992,null,null,null
-2020-09-02T18:14:19Z,26.79,61.22,99,0,33.99,101.64,0.00,400.00,0.207914,0.215258,0.226094,0.213336,null,null,null
-2020-09-02T18:14:49Z,26.75,61.31,99,0,27.99,101.63,0.00,400.00,0.208227,0.215547,0.226789,0.213125,null,null,null
-2020-09-02T18:15:19Z,26.75,61.25,99,0,27.64,101.64,0.00,400.00,0.206961,0.215555,0.226195,0.213352,null,null,null
-2020-09-02T18:15:49Z,26.75,61.29,99,0,33.47,101.64,0.00,400.00,0.208852,0.214234,0.226945,0.213898,null,null,null
-2020-09-02T18:16:19Z,26.78,61.27,99,0,32.46,101.64,0.00,400.00,0.207594,0.215039,0.226313,0.213531,null,null,null
-2020-09-02T18:16:49Z,26.78,61.26,99,0,29.94,101.64,0.00,400.00,0.208383,0.216273,0.224961,0.213820,null,null,null
-2020-09-02T18:17:19Z,26.78,61.29,99,0,42.46,101.64,0.00,400.00,0.207695,0.215734,0.227016,0.214023,null,null,null
-2020-09-02T18:17:49Z,26.78,61.26,99,0,27.38,101.64,0.00,400.00,0.207555,0.215578,0.228430,0.213961,null,null,null
-2020-09-02T18:18:19Z,26.78,61.27,99,0,29.92,101.64,0.00,405.00,0.206836,0.215930,0.226547,0.213516,null,null,null
-2020-09-02T18:18:49Z,26.78,61.28,99,0,37.84,101.64,0.00,405.00,0.208227,0.216953,0.226766,0.214031,null,null,null
-2020-09-02T18:19:19Z,26.79,61.27,99,0,41.44,101.64,0.00,400.00,0.206914,0.214219,0.226734,0.213859,null,null,null
-2020-09-02T18:19:49Z,26.78,61.29,99,0,33.56,101.64,0.00,400.00,0.207414,0.214789,0.225984,0.213211,null,null,null
-2020-09-02T18:20:19Z,26.78,61.33,99,0,36.98,101.64,0.00,400.00,0.207742,0.215391,0.226984,0.213609,null,null,null
-2020-09-02T18:20:49Z,26.76,61.26,99,0,26.48,101.64,0.00,400.00,0.207398,0.215438,0.225844,0.212789,null,null,null
-2020-09-02T18:21:19Z,26.75,61.32,99,0,29.26,101.64,0.00,400.00,0.208070,0.215531,0.227680,0.214367,null,null,null
-2020-09-02T18:21:49Z,26.76,61.37,99,0,30.91,101.65,0.00,400.00,0.208383,0.215148,0.224602,0.213570,null,null,null
-2020-09-02T18:22:19Z,26.76,61.31,99,0,36.29,101.64,0.00,400.00,0.208523,0.216562,0.226672,0.214070,null,null,null
-2020-09-02T18:22:49Z,26.76,61.27,99,0,37.99,101.65,0.00,400.00,0.207383,0.215617,0.227297,0.213555,null,null,null
-2020-09-02T18:23:19Z,26.78,61.29,99,0,33.18,101.65,0.00,400.00,0.207125,0.215805,0.226336,0.213523,null,null,null
-2020-09-02T18:23:49Z,26.78,61.29,99,0,30.20,101.65,0.00,400.00,0.208586,0.215055,0.226227,0.213391,null,null,null
-2020-09-02T18:24:19Z,26.78,61.27,99,0,30.31,101.65,0.00,400.00,0.208523,0.214687,0.227078,0.213961,null,null,null
-2020-09-02T18:24:49Z,26.76,61.26,99,0,27.77,101.65,0.00,400.00,0.208766,0.216109,0.226539,0.214453,null,null,null
-2020-09-02T18:25:19Z,26.76,61.26,99,0,33.83,101.65,0.00,400.00,0.208695,0.215516,0.226117,0.213570,null,null,null
-2020-09-02T18:25:49Z,26.78,61.34,99,0,29.15,101.66,0.00,400.00,0.208547,0.215914,0.226250,0.213828,null,null,null
-2020-09-02T18:26:19Z,26.79,61.27,99,0,28.52,101.65,0.00,400.00,0.208648,0.216148,0.226797,0.213336,null,null,null
-2020-09-02T18:26:49Z,26.76,61.27,99,0,47.22,101.65,0.00,400.00,0.208234,0.214750,0.224734,0.213680,null,null,null
-2020-09-02T18:27:19Z,26.76,61.27,99,0,29.17,101.66,0.00,400.00,0.208711,0.214930,0.226719,0.213422,null,null,null
-2020-09-02T18:27:49Z,26.76,61.25,99,0,30.46,101.66,0.00,400.00,0.209859,0.216984,0.226430,0.214062,null,null,null
-2020-09-02T18:28:19Z,26.78,61.27,99,0,45.85,101.66,0.00,400.00,0.207664,0.214719,0.225945,0.214094,null,null,null
-2020-09-02T18:28:49Z,26.76,61.29,99,0,26.93,101.66,0.00,400.00,0.208391,0.215578,0.226617,0.214039,null,null,null
-2020-09-02T18:29:19Z,26.76,61.29,99,0,32.36,101.66,0.00,400.00,0.209102,0.215094,0.227070,0.214461,null,null,null
-2020-09-02T18:29:49Z,26.75,61.26,99,0,29.56,101.66,0.00,400.00,0.207273,0.215445,0.224539,0.212883,null,null,null
-2020-09-02T18:30:19Z,26.78,61.28,99,0,33.74,101.66,0.00,400.00,0.208852,0.215359,0.226555,0.214344,null,null,null
-2020-09-02T18:30:49Z,26.75,61.25,99,0,30.80,101.66,0.00,400.00,0.207281,0.215141,0.227406,0.214633,null,null,null
-2020-09-02T18:31:19Z,26.75,61.29,99,0,29.90,101.66,0.00,400.00,0.208984,0.216766,0.227352,0.213742,null,null,null
-2020-09-02T18:31:49Z,26.76,61.26,99,0,29.49,101.67,0.00,400.00,0.209164,0.216781,0.227758,0.214719,null,null,null
-2020-09-02T18:32:19Z,26.76,61.24,99,0,29.27,101.67,0.00,400.00,0.208836,0.214898,0.226906,0.213727,null,null,null
-2020-09-02T18:32:49Z,26.76,61.25,99,0,29.91,101.67,0.00,400.00,0.209156,0.214914,0.227164,0.214172,null,null,null
-2020-09-02T18:33:19Z,26.75,61.28,99,0,32.42,101.67,0.00,400.00,0.207914,0.216281,0.226773,0.214305,null,null,null
-2020-09-02T18:33:49Z,26.78,61.26,99,0,31.13,101.67,0.00,400.00,0.209984,0.216039,0.227273,0.214016,null,null,null
-2020-09-02T18:34:19Z,26.73,61.27,99,0,31.28,101.67,0.00,400.00,0.208273,0.215367,0.225359,0.213055,null,null,null
-2020-09-02T18:34:49Z,26.76,61.26,99,0,40.61,101.67,0.00,400.00,0.208305,0.216266,0.227422,0.214148,null,null,null
-2020-09-02T18:35:19Z,26.75,61.28,99,0,28.73,101.67,0.00,400.00,0.208766,0.215195,0.228961,0.213695,null,null,null
-2020-09-02T18:35:49Z,26.73,61.29,99,0,27.68,101.68,0.00,400.00,0.209477,0.217234,0.226734,0.213352,null,null,null
-2020-09-02T18:36:19Z,26.78,61.27,99,0,28.02,101.68,0.00,400.00,0.208367,0.216430,0.227234,0.213820,null,null,null
-2020-09-02T18:36:49Z,26.73,61.26,99,0,30.34,101.68,0.00,400.00,0.209187,0.215570,0.225688,0.213070,null,null,null
-2020-09-02T18:37:19Z,26.72,61.28,99,0,37.77,101.68,0.00,400.00,0.208414,0.216391,0.227422,0.214031,null,null,null
-2020-09-02T18:37:49Z,26.75,61.28,99,0,26.21,101.68,0.00,400.00,0.208414,0.216891,0.226617,0.214930,null,null,null
-2020-09-02T18:38:19Z,26.79,61.27,99,0,38.24,101.68,0.00,400.00,0.208586,0.216391,0.225461,0.213406,null,null,null
-2020-09-02T18:38:49Z,26.75,61.29,99,0,29.46,101.68,0.00,400.00,0.207320,0.215211,0.227219,0.213734,null,null,null
-2020-09-02T18:39:19Z,26.76,61.30,99,0,37.09,101.68,0.00,400.00,0.206867,0.215633,0.226758,0.213602,null,null,null
-2020-09-02T18:39:49Z,26.75,61.26,99,0,30.16,101.69,0.00,400.00,0.210242,0.216117,0.226633,0.214711,null,null,null
-2020-09-02T18:40:19Z,26.73,61.27,99,0,27.77,101.69,0.00,400.00,0.208867,0.214953,0.227055,0.214586,null,null,null
-2020-09-02T18:40:49Z,26.75,61.25,99,0,27.22,101.69,0.00,400.00,0.209523,0.215617,0.227500,0.214414,null,null,null
-2020-09-02T18:41:19Z,26.75,61.25,99,0,29.97,101.68,0.00,405.00,0.209852,0.215898,0.224711,0.213484,null,null,null
-2020-09-02T18:41:49Z,26.75,61.26,99,0,27.99,101.69,0.00,405.00,0.207992,0.215234,0.226500,0.214250,null,null,null
-2020-09-02T18:42:19Z,26.75,61.27,99,0,30.08,101.69,0.00,400.00,0.208867,0.216133,0.226320,0.214195,null,null,null
-2020-09-02T18:42:49Z,26.72,61.25,99,0,33.02,101.69,0.00,400.00,0.207281,0.215211,0.227578,0.214430,null,null,null
-2020-09-02T18:43:19Z,26.73,61.25,99,0,31.84,101.69,0.00,400.00,0.209703,0.215805,0.227187,0.214305,null,null,null
-2020-09-02T18:43:49Z,26.75,61.25,99,0,28.54,101.69,0.00,400.00,0.208570,0.215844,0.225898,0.213648,null,null,null
-2020-09-02T18:44:19Z,26.75,61.20,99,0,38.93,101.69,0.00,400.00,0.208312,0.214719,0.226117,0.214219,null,null,null
-2020-09-02T18:44:49Z,26.76,61.25,99,0,27.77,101.70,0.00,400.00,0.208406,0.216195,0.226453,0.214148,null,null,null
-2020-09-02T18:45:19Z,26.73,61.23,99,0,34.12,101.69,0.00,405.00,0.208578,0.216422,0.227313,0.214695,null,null,null
-2020-09-02T18:45:49Z,26.75,61.25,99,0,29.40,101.70,0.00,405.00,0.207789,0.216102,0.226875,0.213625,null,null,null
-2020-09-02T18:46:19Z,26.75,61.26,99,0,30.90,101.69,0.00,400.00,0.209133,0.215531,0.227687,0.214227,null,null,null
-2020-09-02T18:46:49Z,26.75,61.22,99,0,27.44,101.70,0.00,400.00,0.206750,0.216047,0.226164,0.213781,null,null,null
-2020-09-02T18:47:19Z,26.75,61.25,99,0,38.95,101.70,0.00,400.00,0.207664,0.216188,0.228406,0.214914,null,null,null
-2020-09-02T18:47:49Z,26.73,61.25,99,0,33.23,101.70,0.00,400.00,0.209711,0.215750,0.226922,0.214820,null,null,null
-2020-09-02T18:48:19Z,26.73,61.25,99,0,32.01,101.70,0.00,405.00,0.207844,0.215961,0.228203,0.213945,null,null,null
-2020-09-02T18:48:49Z,26.73,61.27,99,0,27.87,101.70,0.00,405.00,0.208102,0.215062,0.227203,0.214445,null,null,null
-2020-09-02T18:49:19Z,26.73,61.26,99,0,32.92,101.70,0.00,405.00,0.208531,0.215820,0.228031,0.214180,null,null,null
-2020-09-02T18:49:49Z,26.73,61.26,99,0,32.59,101.71,0.00,405.00,0.207992,0.215906,0.226844,0.213859,null,null,null
-2020-09-02T18:50:19Z,26.75,61.26,99,0,40.72,101.70,0.00,400.00,0.207211,0.215242,0.226789,0.214375,null,null,null
-2020-09-02T18:50:49Z,26.75,61.24,99,0,40.23,101.70,0.00,400.00,0.207531,0.215547,0.226648,0.214227,null,null,null
-2020-09-02T18:51:19Z,26.73,61.27,99,0,30.17,101.71,0.00,400.00,0.207633,0.215539,0.227961,0.214891,null,null,null
-2020-09-02T18:51:49Z,26.73,61.21,99,0,30.91,101.71,0.00,400.00,0.208555,0.215312,0.227430,0.214430,null,null,null
-2020-09-02T18:52:19Z,26.73,61.21,99,0,30.26,101.71,0.00,401.00,0.208586,0.214648,0.227031,0.213469,null,null,null
-2020-09-02T18:52:49Z,26.75,61.22,99,0,28.14,101.71,0.00,401.00,0.208500,0.215797,0.225703,0.213398,null,null,null
-2020-09-02T18:53:19Z,26.73,61.24,99,0,30.46,101.71,0.00,401.00,0.208813,0.216625,0.226781,0.214289,null,null,null
-2020-09-02T18:53:49Z,26.73,61.20,99,0,27.59,101.71,0.00,401.00,0.208531,0.215703,0.228148,0.215211,null,null,null
-2020-09-02T18:54:19Z,26.73,61.20,99,0,37.89,101.71,0.00,401.00,0.209328,0.215859,0.227102,0.213992,null,null,null
-2020-09-02T18:54:49Z,26.75,61.23,99,0,40.86,101.71,0.00,401.00,0.208273,0.215250,0.226867,0.214109,null,null,null
-2020-09-02T18:55:19Z,26.76,61.19,99,0,35.40,101.71,0.00,400.00,0.208445,0.215703,0.227430,0.214023,null,null,null
-2020-09-02T18:55:49Z,26.76,61.19,99,0,36.41,101.72,0.00,400.00,0.208781,0.216008,0.228672,0.214703,null,null,null
-2020-09-02T18:56:19Z,26.73,61.20,99,0,27.30,101.71,0.00,400.00,0.209266,0.216594,0.227289,0.213922,null,null,null
-2020-09-02T18:56:49Z,26.75,61.23,99,0,41.40,101.72,0.00,400.00,0.208148,0.216844,0.227375,0.214312,null,null,null
-2020-09-02T18:57:19Z,26.76,61.23,99,0,29.22,101.72,0.00,402.00,0.208781,0.215844,0.228539,0.214969,null,null,null
-2020-09-02T18:57:49Z,26.73,61.22,99,0,35.73,101.72,0.00,402.00,0.207961,0.215141,0.226492,0.214250,null,null,null
-2020-09-02T18:58:19Z,26.72,61.22,99,0,33.97,101.72,0.00,400.00,0.207508,0.216484,0.227437,0.214305,null,null,null
-2020-09-02T18:58:49Z,26.72,61.22,99,0,41.50,101.72,0.00,400.00,0.207633,0.214781,0.226172,0.214133,null,null,null
-2020-09-02T18:59:19Z,26.72,61.21,99,0,31.43,101.72,0.00,403.00,0.208055,0.216680,0.226180,0.214281,null,null,null
-2020-09-02T18:59:49Z,26.72,61.20,99,0,28.45,101.72,0.00,403.00,0.209336,0.215477,0.226133,0.214273,null,null,null
-2020-09-02T19:00:19Z,26.75,61.20,99,0,43.51,101.72,0.00,400.00,0.209430,0.214883,0.226656,0.214344,null,null,null
-2020-09-02T19:00:49Z,26.76,61.19,99,0,38.56,101.72,0.00,400.00,0.209023,0.216289,0.227930,0.214211,null,null,null
-2020-09-02T19:01:19Z,26.72,61.20,99,0,35.51,101.73,0.00,400.00,0.208687,0.216219,0.228031,0.214578,null,null,null
-2020-09-02T19:01:49Z,26.73,61.16,99,0,26.41,101.72,0.00,400.00,0.208734,0.215594,0.226086,0.214523,null,null,null
-2020-09-02T19:02:19Z,26.73,61.18,99,0,28.89,101.73,0.00,402.00,0.206742,0.215289,0.228719,0.214961,null,null,null
-2020-09-02T19:02:49Z,26.73,61.18,99,0,30.12,101.73,0.00,402.00,0.208836,0.216117,0.227758,0.214422,null,null,null
-2020-09-02T19:03:19Z,26.75,61.20,99,0,29.28,101.73,0.00,402.00,0.208312,0.215180,0.225102,0.213750,null,null,null
-2020-09-02T19:03:49Z,26.75,61.21,99,0,27.66,101.73,0.00,402.00,0.207914,0.216258,0.226883,0.214719,null,null,null
-2020-09-02T19:04:19Z,26.75,61.18,99,0,38.16,101.73,0.00,400.00,0.209586,0.215836,0.226617,0.213625,null,null,null
-2020-09-02T19:04:49Z,26.72,61.19,99,0,29.47,101.73,0.00,400.00,0.208914,0.216391,0.225938,0.214047,null,null,null
-2020-09-02T19:05:19Z,26.73,61.20,99,0,31.08,101.73,0.00,400.00,0.210820,0.216688,0.228750,0.213953,null,null,null
-2020-09-02T19:05:49Z,26.72,61.18,99,0,35.06,101.74,0.00,400.00,0.208773,0.215727,0.227148,0.214141,null,null,null
-2020-09-02T19:06:19Z,26.73,61.18,99,0,28.42,101.74,0.00,400.00,0.208117,0.216281,0.227703,0.214352,null,null,null
-2020-09-02T19:06:49Z,26.75,61.15,99,0,27.49,101.74,0.00,400.00,0.207750,0.213992,0.227258,0.213805,null,null,null
-2020-09-02T19:07:19Z,26.73,61.17,99,0,36.86,101.74,0.00,400.00,0.208312,0.215906,0.228266,0.214836,null,null,null
-2020-09-02T19:07:49Z,26.73,61.20,99,0,28.06,101.74,0.00,400.00,0.209633,0.215805,0.226617,0.213766,null,null,null
-2020-09-02T19:08:19Z,26.73,61.15,99,0,42.98,101.74,0.00,400.00,0.210172,0.216727,0.228547,0.214898,null,null,null
-2020-09-02T19:08:49Z,26.73,61.17,99,0,30.73,101.74,0.00,400.00,0.207820,0.214781,0.226391,0.214711,null,null,null
-2020-09-02T19:09:19Z,26.73,61.18,99,0,35.31,101.74,0.00,400.00,0.207383,0.215742,0.226445,0.214203,null,null,null
-2020-09-02T19:09:49Z,26.76,61.15,99,0,34.41,101.74,0.00,400.00,0.209133,0.217023,0.228531,0.214789,null,null,null
-2020-09-02T19:10:19Z,26.75,61.13,99,0,36.97,101.74,0.00,400.00,0.207867,0.215758,0.227914,0.214320,null,null,null
-2020-09-02T19:10:49Z,26.73,61.15,99,0,32.75,101.74,0.00,400.00,0.207359,0.216828,0.225031,0.214047,null,null,null
-2020-09-02T19:11:19Z,26.73,61.15,99,0,31.48,101.75,0.00,400.00,0.211180,0.216969,0.226984,0.214141,null,null,null
-2020-09-02T19:11:49Z,26.72,61.15,99,0,30.40,101.74,0.00,400.00,0.207883,0.215539,0.225555,0.214570,null,null,null
-2020-09-02T19:12:19Z,26.72,61.13,99,0,31.59,101.75,0.00,400.00,0.208633,0.215477,0.227258,0.214594,null,null,null
-2020-09-02T19:12:49Z,26.72,61.15,99,0,32.65,101.75,0.00,400.00,0.208211,0.216227,0.226656,0.213992,null,null,null
-2020-09-02T19:13:19Z,26.75,61.15,99,0,28.17,101.75,0.00,400.00,0.208289,0.216242,0.224648,0.213953,null,null,null
-2020-09-02T19:13:49Z,26.73,61.17,99,0,36.33,101.75,0.00,400.00,0.207992,0.214500,0.227320,0.214906,null,null,null
-2020-09-02T19:14:19Z,26.72,61.15,99,0,44.19,101.75,0.00,400.00,0.208992,0.216086,0.227281,0.214273,null,null,null
-2020-09-02T19:14:49Z,26.75,61.17,99,0,36.57,101.75,0.00,400.00,0.209508,0.215539,0.228555,0.214687,null,null,null
-2020-09-02T19:15:19Z,26.73,61.18,99,0,36.84,101.76,0.00,400.00,0.208555,0.215594,0.227305,0.213594,null,null,null
-2020-09-02T19:15:49Z,26.75,61.17,99,0,28.63,101.75,0.00,400.00,0.209430,0.216312,0.226422,0.214844,null,null,null
-2020-09-02T19:16:19Z,26.72,61.16,99,0,28.77,101.75,0.00,400.00,0.207195,0.214891,0.226852,0.213633,null,null,null
-2020-09-02T19:16:49Z,26.73,61.18,99,0,29.79,101.76,0.00,400.00,0.209078,0.216320,0.227492,0.215070,null,null,null
-2020-09-02T19:17:19Z,26.73,61.15,99,0,28.77,101.76,0.00,402.00,0.209844,0.216219,0.227695,0.214211,null,null,null
-2020-09-02T19:17:49Z,26.72,61.18,99,0,37.14,101.75,0.00,402.00,0.209602,0.216633,0.226195,0.214195,null,null,null
-2020-09-02T19:18:19Z,26.72,61.12,99,0,31.29,101.76,0.00,400.00,0.208078,0.214867,0.226586,0.214156,null,null,null
-2020-09-02T19:18:49Z,26.72,61.13,99,0,30.90,101.76,0.00,400.00,0.210484,0.215547,0.226625,0.213875,null,null,null
-2020-09-02T19:19:19Z,26.71,61.18,99,0,27.06,101.76,0.00,400.00,0.209312,0.215961,0.227117,0.214852,null,null,null
-2020-09-02T19:19:49Z,26.75,61.15,99,0,35.30,101.76,0.00,400.00,0.208586,0.215047,0.227508,0.214859,null,null,null
-2020-09-02T19:20:19Z,26.72,61.16,99,0,29.25,101.76,0.00,400.00,0.208758,0.216391,0.227141,0.214039,null,null,null
-2020-09-02T19:20:49Z,26.72,61.15,99,0,33.06,101.76,0.00,400.00,0.210187,0.217539,0.227633,0.214508,null,null,null
-2020-09-02T19:21:19Z,26.72,61.16,99,0,27.36,101.77,1.00,407.00,0.209203,0.216867,0.228094,0.214367,null,null,null
-2020-09-02T19:21:49Z,26.73,61.12,99,0,28.17,101.76,1.00,407.00,0.207211,0.215719,0.226469,0.214008,null,null,null
-2020-09-02T19:22:19Z,26.72,61.14,99,0,31.75,101.76,0.00,401.00,0.208859,0.214992,0.227453,0.214547,null,null,null
-2020-09-02T19:22:49Z,26.73,61.13,99,0,44.82,101.77,0.00,401.00,0.209383,0.216555,0.225953,0.214094,null,null,null
-2020-09-02T19:23:19Z,26.72,61.15,99,0,30.23,101.77,0.00,400.00,0.208227,0.216797,0.224031,0.214469,null,null,null
-2020-09-02T19:23:49Z,26.73,61.08,99,0,29.87,101.77,0.00,400.00,0.210055,0.216406,0.228734,0.215203,null,null,null
-2020-09-02T19:24:19Z,26.72,61.14,99,0,31.47,101.77,0.00,400.00,0.208570,0.215250,0.226945,0.214836,null,null,null
-2020-09-02T19:24:49Z,26.72,61.13,99,0,26.08,101.77,0.00,400.00,0.209266,0.216805,0.226688,0.214211,null,null,null
-2020-09-02T19:25:19Z,26.73,61.12,99,0,27.26,101.77,0.00,403.00,0.210539,0.216656,0.228633,0.213938,null,null,null
-2020-09-02T19:25:49Z,26.72,61.15,99,0,29.54,101.77,0.00,403.00,0.208594,0.215609,0.228172,0.214258,null,null,null
-2020-09-02T19:26:19Z,26.73,61.13,99,0,41.14,101.77,0.00,402.00,0.209805,0.216180,0.226695,0.214781,null,null,null
-2020-09-02T19:26:49Z,26.72,61.11,99,0,30.75,101.77,0.00,402.00,0.208922,0.215813,0.227367,0.214984,null,null,null
-2020-09-02T19:27:19Z,26.72,61.12,99,0,27.42,101.77,0.00,402.00,0.209492,0.216594,0.226859,0.214328,null,null,null
-2020-09-02T19:27:49Z,26.72,61.12,99,0,31.28,101.78,0.00,402.00,0.208586,0.216078,0.228703,0.215109,null,null,null
-2020-09-02T19:28:19Z,26.72,61.12,99,0,29.96,101.77,0.00,403.00,0.210742,0.216578,0.227352,0.214328,null,null,null
-2020-09-02T19:28:49Z,26.72,61.11,99,0,28.04,101.77,0.00,403.00,0.209211,0.216742,0.227797,0.214094,null,null,null
-2020-09-02T19:29:19Z,26.72,61.08,99,0,32.06,101.77,0.00,403.00,0.208898,0.216133,0.227258,0.214687,null,null,null
-2020-09-02T19:29:49Z,26.73,61.10,99,0,30.08,101.77,0.00,403.00,0.208508,0.215664,0.226266,0.214383,null,null,null
-2020-09-02T19:30:19Z,26.73,61.11,99,0,33.14,101.77,0.00,402.00,0.209266,0.217000,0.226633,0.213750,null,null,null
-2020-09-02T19:30:49Z,26.73,61.05,99,0,35.19,101.77,0.00,402.00,0.208992,0.217000,0.228211,0.214492,null,null,null
-2020-09-02T19:31:19Z,26.73,61.09,99,0,31.43,101.77,0.00,400.00,0.206219,0.215203,0.226859,0.214414,null,null,null
-2020-09-02T19:31:49Z,26.73,61.11,99,0,31.24,101.77,0.00,400.00,0.209922,0.217273,0.228141,0.214930,null,null,null
-2020-09-02T19:32:19Z,26.71,61.09,99,0,35.33,101.78,0.00,400.00,0.209187,0.215852,0.226734,0.213547,null,null,null
-2020-09-02T19:32:49Z,26.75,61.11,99,0,43.97,101.78,0.00,400.00,0.209039,0.215898,0.227070,0.214805,null,null,null
-2020-09-02T19:33:19Z,26.73,61.09,99,0,29.88,101.78,0.00,400.00,0.208133,0.216219,0.226102,0.213961,null,null,null
-2020-09-02T19:33:49Z,26.71,61.10,99,0,37.48,101.78,0.00,400.00,0.209000,0.215672,0.228547,0.214820,null,null,null
-2020-09-02T19:34:19Z,26.72,61.06,99,0,28.64,101.78,0.00,400.00,0.208531,0.216672,0.226977,0.214070,null,null,null
-2020-09-02T19:34:49Z,26.72,61.06,99,0,30.42,101.78,0.00,400.00,0.210453,0.216281,0.227266,0.214234,null,null,null
-2020-09-02T19:35:19Z,26.72,61.07,99,0,25.29,101.78,0.00,400.00,0.208602,0.216523,0.226047,0.214016,null,null,null
-2020-09-02T19:35:49Z,26.72,61.06,99,0,30.02,101.78,0.00,400.00,0.207039,0.215164,0.228352,0.214531,null,null,null
-2020-09-02T19:36:19Z,26.72,61.09,99,0,28.19,101.78,0.00,401.00,0.208906,0.216453,0.226234,0.214039,null,null,null
-2020-09-02T19:36:49Z,26.72,61.07,99,0,34.66,101.78,0.00,401.00,0.210266,0.216648,0.228641,0.214914,null,null,null
-2020-09-02T19:37:19Z,26.73,61.07,99,0,29.86,101.78,0.00,400.00,0.209242,0.215672,0.227664,0.215188,null,null,null
-2020-09-02T19:37:49Z,26.72,61.05,99,0,27.82,101.78,0.00,400.00,0.209320,0.215430,0.227703,0.214813,null,null,null
-2020-09-02T19:38:19Z,26.73,61.05,99,0,26.21,101.78,0.00,400.00,0.207930,0.216156,0.228523,0.213687,null,null,null
-2020-09-02T19:38:49Z,26.73,61.06,99,0,34.64,101.79,0.00,400.00,0.207711,0.215438,0.227367,0.214633,null,null,null
-2020-09-02T19:39:19Z,26.73,61.05,99,0,32.47,101.78,0.00,401.00,0.208922,0.216617,0.226977,0.214766,null,null,null
-2020-09-02T19:39:49Z,26.73,61.07,99,0,28.92,101.79,0.00,401.00,0.208641,0.215219,0.225398,0.214609,null,null,null
-2020-09-02T19:40:19Z,26.72,61.05,99,0,31.59,101.79,0.00,400.00,0.209734,0.215773,0.226555,0.215227,null,null,null
-2020-09-02T19:40:49Z,26.71,61.07,99,0,32.36,101.78,0.00,400.00,0.208141,0.215984,0.227422,0.215039,null,null,null
-2020-09-02T19:41:19Z,26.73,61.02,99,0,33.23,101.78,0.00,401.00,0.208539,0.215383,0.225555,0.213961,null,null,null
-2020-09-02T19:41:49Z,26.75,61.02,99,0,30.48,101.78,0.00,401.00,0.208516,0.215727,0.229008,0.214937,null,null,null
-2020-09-02T19:42:19Z,26.72,60.99,99,0,31.95,101.78,0.00,400.00,0.208586,0.216219,0.227234,0.214102,null,null,null
-2020-09-02T19:42:49Z,26.72,61.02,99,0,33.64,101.78,0.00,400.00,0.208711,0.216086,0.227516,0.214656,null,null,null
-2020-09-02T19:43:19Z,26.72,61.04,99,0,32.90,101.78,0.00,402.00,0.209523,0.217117,0.228117,0.214523,null,null,null
-2020-09-02T19:43:49Z,26.73,61.04,99,0,38.04,101.79,0.00,402.00,0.209102,0.216203,0.225562,0.214602,null,null,null
-2020-09-02T19:44:19Z,26.73,61.02,99,0,33.80,101.79,0.00,400.00,0.209352,0.217016,0.227367,0.214781,null,null,null
-2020-09-02T19:44:49Z,26.73,61.05,99,0,28.67,101.79,0.00,400.00,0.209398,0.216508,0.227289,0.214539,null,null,null
-2020-09-02T19:45:19Z,26.72,61.02,99,0,29.05,101.79,0.00,402.00,0.208375,0.216047,0.227687,0.214789,null,null,null
-2020-09-02T19:45:49Z,26.72,61.04,99,0,30.29,101.78,0.00,402.00,0.208500,0.216844,0.226883,0.214180,null,null,null
-2020-09-02T19:46:19Z,26.72,60.94,99,0,28.88,101.79,0.00,400.00,0.210805,0.216906,0.227031,0.214188,null,null,null
-2020-09-02T19:46:49Z,26.72,61.02,99,0,39.67,101.79,0.00,400.00,0.208797,0.215414,0.227211,0.214461,null,null,null
-2020-09-02T19:47:19Z,26.73,60.99,99,0,27.24,101.79,0.00,400.00,0.209086,0.216398,0.228719,0.214836,null,null,null
-2020-09-02T19:47:49Z,26.72,61.00,99,0,36.90,101.79,0.00,400.00,0.207734,0.216430,0.226711,0.214648,null,null,null
-2020-09-02T19:48:19Z,26.73,61.02,99,0,42.65,101.79,0.00,400.00,0.208961,0.216078,0.226164,0.214445,null,null,null
-2020-09-02T19:48:49Z,26.72,60.99,99,0,28.71,101.79,0.00,400.00,0.210117,0.216656,0.226047,0.214586,null,null,null
-2020-09-02T19:49:19Z,26.73,61.00,99,0,26.67,101.79,0.00,400.00,0.209680,0.216477,0.228797,0.215273,null,null,null
-2020-09-02T19:49:49Z,26.73,60.99,99,0,26.26,101.79,0.00,400.00,0.208844,0.215125,0.227336,0.213883,null,null,null
-2020-09-02T19:50:19Z,26.73,61.02,99,0,30.18,101.79,0.00,400.00,0.208875,0.215711,0.229062,0.214758,null,null,null
-2020-09-02T19:50:49Z,26.73,60.98,99,0,32.47,101.79,0.00,400.00,0.210289,0.216914,0.228328,0.214437,null,null,null
-2020-09-02T19:51:19Z,26.73,60.99,99,0,29.72,101.80,0.00,400.00,0.210445,0.216781,0.226961,0.214133,null,null,null
-2020-09-02T19:51:49Z,26.72,60.98,99,0,26.24,101.79,0.00,400.00,0.209125,0.215875,0.228062,0.214906,null,null,null
-2020-09-02T19:52:19Z,26.69,61.02,99,0,28.40,101.80,0.00,400.00,0.209844,0.215930,0.228250,0.215586,null,null,null
-2020-09-02T19:52:49Z,26.73,60.99,99,0,30.34,101.80,0.00,400.00,0.210797,0.216227,0.228031,0.214625,null,null,null
-2020-09-02T19:53:19Z,26.73,60.96,99,0,41.29,101.80,0.00,400.00,0.208445,0.215883,0.228297,0.214914,null,null,null
-2020-09-02T19:53:49Z,26.72,60.98,99,0,32.49,101.80,0.00,400.00,0.209016,0.215977,0.227836,0.215023,null,null,null
-2020-09-02T19:54:19Z,26.72,61.00,99,0,28.91,101.81,0.00,400.00,0.208625,0.216523,0.227391,0.215000,null,null,null
-2020-09-02T19:54:49Z,26.72,60.96,99,0,36.37,101.80,0.00,400.00,0.208898,0.215711,0.226359,0.214102,null,null,null
-2020-09-02T19:55:19Z,26.75,60.99,99,0,27.78,101.80,0.00,400.00,0.207586,0.216156,0.227930,0.214445,null,null,null
-2020-09-02T19:55:49Z,26.75,60.94,99,0,44.31,101.81,0.00,400.00,0.209305,0.215813,0.227625,0.214344,null,null,null
-2020-09-02T19:56:19Z,26.75,60.97,99,0,27.36,101.81,0.00,403.00,0.209766,0.214867,0.228437,0.215383,null,null,null
-2020-09-02T19:56:49Z,26.72,60.95,99,0,28.84,101.81,0.00,403.00,0.208273,0.217391,0.228758,0.214922,null,null,null
-2020-09-02T19:57:19Z,26.71,60.97,99,0,27.47,101.81,0.00,406.00,0.207148,0.216805,0.225938,0.214055,null,null,null
-2020-09-02T19:57:49Z,26.73,60.96,99,0,27.28,101.80,0.00,406.00,0.209609,0.217586,0.226398,0.214344,null,null,null
-2020-09-02T19:58:19Z,26.71,60.94,99,0,44.64,101.81,0.00,403.00,0.208664,0.215680,0.227039,0.213852,null,null,null
-2020-09-02T19:58:49Z,26.73,60.98,99,0,27.30,101.81,0.00,403.00,0.207133,0.215258,0.228625,0.214625,null,null,null
-2020-09-02T19:59:19Z,26.72,60.94,99,0,29.94,101.81,0.00,400.00,0.206852,0.216414,0.227031,0.215234,null,null,null
-2020-09-02T19:59:49Z,26.73,60.95,99,0,33.01,101.81,0.00,400.00,0.210625,0.215703,0.228250,0.215406,null,null,null
-2020-09-02T20:00:19Z,26.72,60.92,99,0,26.53,101.81,0.00,400.00,0.208539,0.216047,0.227789,0.214516,null,null,null
-2020-09-02T20:00:49Z,26.72,60.97,99,0,27.06,101.82,0.00,400.00,0.209844,0.216258,0.227305,0.214672,null,null,null
-2020-09-02T20:01:19Z,26.71,60.91,99,0,27.60,101.81,0.00,400.00,0.209445,0.216047,0.229070,0.214672,null,null,null
-2020-09-02T20:01:49Z,26.73,60.93,99,0,26.31,101.81,0.00,400.00,0.210234,0.216734,0.228094,0.215344,null,null,null
-2020-09-02T20:02:19Z,26.75,60.97,99,0,28.51,101.81,0.00,400.00,0.209734,0.216594,0.228234,0.214008,null,null,null
-2020-09-02T20:02:49Z,26.75,60.99,99,0,45.60,101.82,0.00,400.00,0.207891,0.216836,0.227781,0.214742,null,null,null
-2020-09-02T20:03:19Z,26.75,60.98,99,0,29.01,101.82,0.00,400.00,0.208687,0.217141,0.228234,0.214742,null,null,null
-2020-09-02T20:03:49Z,26.72,60.98,99,0,30.45,101.81,0.00,400.00,0.209125,0.216953,0.226594,0.213859,null,null,null
-2020-09-02T20:04:19Z,26.73,60.92,99,0,33.90,101.82,0.00,400.00,0.208414,0.215578,0.228984,0.214078,null,null,null
-2020-09-02T20:04:49Z,26.72,60.94,99,0,27.08,101.82,0.00,400.00,0.209055,0.216078,0.227500,0.214578,null,null,null
-2020-09-02T20:05:19Z,26.72,60.93,99,0,28.19,101.82,0.00,401.00,0.209688,0.216609,0.227383,0.215016,null,null,null
-2020-09-02T20:05:49Z,26.72,60.91,99,0,41.74,101.81,0.00,401.00,0.207523,0.215937,0.227836,0.214648,null,null,null
-2020-09-02T20:06:19Z,26.71,60.96,99,0,27.77,101.81,0.00,401.00,0.209844,0.216797,0.228242,0.214437,null,null,null
-2020-09-02T20:06:49Z,26.72,60.89,99,0,27.14,101.82,0.00,401.00,0.210273,0.215914,0.227437,0.214023,null,null,null
-2020-09-02T20:07:19Z,26.72,60.97,99,0,25.87,101.82,0.00,400.00,0.209000,0.217609,0.228516,0.215273,null,null,null
-2020-09-02T20:07:49Z,26.71,60.95,99,0,25.90,101.82,0.00,400.00,0.207648,0.215945,0.227742,0.214883,null,null,null
-2020-09-02T20:08:19Z,26.73,60.93,99,0,38.44,101.82,0.00,400.00,0.208672,0.215625,0.227586,0.214445,null,null,null
-2020-09-02T20:08:49Z,26.72,60.93,99,0,35.06,101.82,0.00,400.00,0.209961,0.216820,0.226867,0.214305,null,null,null
-2020-09-02T20:09:19Z,26.72,60.92,99,0,30.11,101.82,0.00,406.00,0.208977,0.216375,0.226375,0.215188,null,null,null
-2020-09-02T20:09:49Z,26.72,60.91,99,0,30.43,101.82,0.00,406.00,0.208594,0.215836,0.228047,0.214531,null,null,null
-2020-09-02T20:10:19Z,26.71,60.92,99,0,28.47,101.82,0.00,400.00,0.209602,0.216273,0.227609,0.214352,null,null,null
-2020-09-02T20:10:49Z,26.75,60.89,99,0,40.78,101.82,0.00,400.00,0.207406,0.215320,0.227633,0.214664,null,null,null
-2020-09-02T20:11:19Z,26.72,60.92,99,0,30.17,101.82,0.00,401.00,0.208102,0.215625,0.228914,0.215398,null,null,null
-2020-09-02T20:11:49Z,26.72,60.91,99,0,27.28,101.83,0.00,401.00,0.208875,0.217078,0.227594,0.214922,null,null,null
-2020-09-02T20:12:19Z,26.72,60.91,99,0,33.95,101.82,0.00,400.00,0.209516,0.216602,0.225930,0.214094,null,null,null
-2020-09-02T20:12:49Z,26.72,60.90,99,0,28.70,101.82,0.00,400.00,0.209172,0.216602,0.227500,0.214734,null,null,null
-2020-09-02T20:13:19Z,26.73,60.88,99,0,32.72,101.82,0.00,400.00,0.210141,0.217063,0.227445,0.214437,null,null,null
-2020-09-02T20:13:49Z,26.72,60.90,99,0,29.81,101.82,0.00,400.00,0.208922,0.216328,0.226336,0.214813,null,null,null
-2020-09-02T20:14:19Z,26.71,60.93,99,0,39.12,101.82,0.00,401.00,0.207750,0.216102,0.228313,0.214945,null,null,null
-2020-09-02T20:14:49Z,26.69,60.90,99,0,27.64,101.83,0.00,401.00,0.209070,0.217688,0.228039,0.215008,null,null,null
-2020-09-02T20:15:19Z,26.71,60.93,99,0,29.67,101.83,0.00,400.00,0.207094,0.214750,0.227289,0.213914,null,null,null
-2020-09-02T20:15:49Z,26.72,60.90,99,0,40.85,101.83,0.00,400.00,0.210734,0.217531,0.228398,0.215156,null,null,null
-2020-09-02T20:16:19Z,26.73,60.91,99,0,27.77,101.82,0.00,401.00,0.209141,0.217055,0.227281,0.215172,null,null,null
-2020-09-02T20:16:49Z,26.71,60.87,99,0,23.86,101.82,0.00,401.00,0.209164,0.216312,0.229008,0.214773,null,null,null
-2020-09-02T20:17:19Z,26.71,60.86,99,0,30.70,101.82,0.00,400.00,0.209219,0.216211,0.228492,0.215328,null,null,null
-2020-09-02T20:17:49Z,26.73,60.89,99,0,29.73,101.83,0.00,400.00,0.208250,0.216148,0.226797,0.214250,null,null,null
-2020-09-02T20:18:19Z,26.72,60.90,99,0,28.14,101.82,0.00,400.00,0.207445,0.215258,0.228203,0.214586,null,null,null
-2020-09-02T20:18:49Z,26.72,60.89,99,0,27.64,101.83,0.00,400.00,0.209352,0.215477,0.226992,0.215195,null,null,null
-2020-09-02T20:19:19Z,26.72,60.89,99,0,28.87,101.83,0.00,400.00,0.210508,0.216562,0.228383,0.214594,null,null,null
-2020-09-02T20:19:49Z,26.72,60.90,99,0,25.70,101.83,0.00,400.00,0.210453,0.216445,0.229555,0.215039,null,null,null
-2020-09-02T20:20:19Z,26.72,60.91,99,0,32.08,101.83,0.00,400.00,0.208945,0.215383,0.227867,0.214406,null,null,null
-2020-09-02T20:20:49Z,26.71,60.91,99,0,29.68,101.83,0.00,400.00,0.210258,0.217352,0.228109,0.214687,null,null,null
-2020-09-02T20:21:19Z,26.73,60.94,99,0,33.66,101.83,0.00,402.00,0.209352,0.217094,0.226156,0.214367,null,null,null
-2020-09-02T20:21:49Z,26.75,60.89,99,0,27.08,101.83,0.00,402.00,0.208281,0.216930,0.227008,0.214867,null,null,null
-2020-09-02T20:22:19Z,26.72,60.90,99,0,29.51,101.83,0.00,400.00,0.207797,0.216586,0.226531,0.214414,null,null,null
-2020-09-02T20:22:49Z,26.72,60.91,99,0,30.89,101.83,0.00,400.00,0.208062,0.215070,0.228359,0.215055,null,null,null
-2020-09-02T20:23:19Z,26.71,60.89,99,0,34.23,101.83,0.00,400.00,0.209438,0.217312,0.227891,0.214852,null,null,null
-2020-09-02T20:23:49Z,26.73,60.84,99,0,30.14,101.83,0.00,400.00,0.207469,0.215680,0.225773,0.214289,null,null,null
-2020-09-02T20:24:19Z,26.72,60.90,99,0,29.21,101.83,0.00,400.00,0.207766,0.215969,0.227336,0.214758,null,null,null
-2020-09-02T20:24:49Z,26.72,60.85,99,0,33.50,101.83,0.00,400.00,0.209133,0.216391,0.227906,0.215250,null,null,null
-2020-09-02T20:25:19Z,26.71,60.84,99,0,29.21,101.83,0.00,400.00,0.207195,0.214781,0.228898,0.214914,null,null,null
-2020-09-02T20:25:49Z,26.72,60.82,99,0,35.26,101.83,0.00,400.00,0.209805,0.215680,0.227406,0.214180,null,null,null
-2020-09-02T20:26:19Z,26.73,60.87,99,0,31.19,101.83,0.00,400.00,0.208602,0.215266,0.227898,0.214398,null,null,null
-2020-09-02T20:26:49Z,26.71,60.89,99,0,30.56,101.83,0.00,400.00,0.208844,0.216164,0.228016,0.214516,null,null,null
-2020-09-02T20:27:19Z,26.68,60.86,99,0,26.03,101.83,0.00,400.00,0.209297,0.216789,0.229500,0.215094,null,null,null
-2020-09-02T20:27:49Z,26.71,60.92,99,0,25.19,101.83,0.00,400.00,0.209813,0.217055,0.228391,0.214469,null,null,null
-2020-09-02T20:28:19Z,26.71,60.90,99,0,45.17,101.83,0.00,400.00,0.208562,0.216398,0.229164,0.215367,null,null,null
-2020-09-02T20:28:49Z,26.71,60.87,99,0,29.61,101.83,0.00,400.00,0.208453,0.215805,0.227367,0.215555,null,null,null
-2020-09-02T20:29:19Z,26.72,60.87,99,0,27.42,101.83,0.00,400.00,0.209445,0.215852,0.228492,0.215266,null,null,null
-2020-09-02T20:29:49Z,26.72,60.86,99,0,27.22,101.83,0.00,400.00,0.209422,0.216438,0.227320,0.214648,null,null,null
-2020-09-02T20:30:19Z,26.71,60.84,99,0,30.30,101.83,0.00,400.00,0.209531,0.216945,0.227938,0.214484,null,null,null
-2020-09-02T20:30:49Z,26.69,60.84,99,0,27.30,101.83,0.00,400.00,0.208594,0.216195,0.227477,0.214703,null,null,null
-2020-09-02T20:31:19Z,26.72,60.91,99,0,26.62,101.83,0.00,400.00,0.208344,0.216523,0.227305,0.214563,null,null,null
-2020-09-02T20:31:49Z,26.72,60.90,99,0,33.72,101.83,0.00,400.00,0.210180,0.216438,0.226359,0.214687,null,null,null
-2020-09-02T20:32:19Z,26.69,60.87,99,0,28.06,101.84,0.00,400.00,0.209359,0.216172,0.226508,0.214648,null,null,null
-2020-09-02T20:32:49Z,26.71,60.90,99,0,29.05,101.83,0.00,400.00,0.208773,0.215508,0.227828,0.214375,null,null,null
-2020-09-02T20:33:19Z,26.71,60.86,99,0,32.30,101.84,0.00,400.00,0.208945,0.216680,0.227453,0.214312,null,null,null
-2020-09-02T20:33:49Z,26.69,60.86,99,0,28.70,101.84,0.00,400.00,0.209430,0.215680,0.227375,0.214883,null,null,null
-2020-09-02T20:34:19Z,26.72,60.89,99,0,27.28,101.84,0.00,400.00,0.209906,0.216570,0.226617,0.215273,null,null,null
-2020-09-02T20:34:49Z,26.71,60.89,99,0,27.06,101.84,0.00,400.00,0.209203,0.216609,0.226758,0.214398,null,null,null
-2020-09-02T20:35:19Z,26.72,60.87,99,0,29.41,101.84,0.00,402.00,0.209562,0.217453,0.230320,0.215547,null,null,null
-2020-09-02T20:35:49Z,26.72,60.86,99,0,27.84,101.84,0.00,402.00,0.209391,0.217219,0.228008,0.215422,null,null,null
-2020-09-02T20:36:19Z,26.72,60.86,99,0,50.97,101.84,0.00,402.00,0.206375,0.216906,0.227016,0.215305,null,null,null
-2020-09-02T20:36:49Z,26.73,60.85,99,0,29.50,101.84,0.00,402.00,0.209367,0.216805,0.226953,0.214859,null,null,null
-2020-09-02T20:37:19Z,26.72,60.86,99,0,26.46,101.84,0.00,400.00,0.211102,0.217266,0.228188,0.214352,null,null,null
-2020-09-02T20:37:49Z,26.71,60.83,99,0,33.62,101.84,0.00,400.00,0.208930,0.216508,0.227820,0.214750,null,null,null
-2020-09-02T20:38:19Z,26.73,60.83,99,0,26.99,101.84,0.00,400.00,0.208984,0.217039,0.227930,0.215289,null,null,null
-2020-09-02T20:38:49Z,26.69,60.89,99,0,28.27,101.84,0.00,400.00,0.210859,0.217164,0.227961,0.214766,null,null,null
-2020-09-02T20:39:19Z,26.71,60.90,99,0,36.91,101.84,0.00,400.00,0.209672,0.217797,0.226773,0.214539,null,null,null
-2020-09-02T20:39:49Z,26.71,60.82,99,0,28.17,101.85,0.00,400.00,0.210820,0.216688,0.228062,0.215234,null,null,null
-2020-09-02T20:40:19Z,26.72,60.82,99,0,28.68,101.84,0.00,400.00,0.208773,0.215687,0.228391,0.214852,null,null,null
-2020-09-02T20:40:49Z,26.72,60.84,99,0,24.65,101.84,0.00,400.00,0.209891,0.217719,0.228789,0.215484,null,null,null
-2020-09-02T20:41:19Z,26.73,60.87,99,0,27.28,101.84,0.00,400.00,0.209023,0.215859,0.228336,0.214813,null,null,null
-2020-09-02T20:41:49Z,26.72,60.86,99,0,26.16,101.84,0.00,400.00,0.210164,0.216266,0.229102,0.215047,null,null,null
-2020-09-02T20:42:19Z,26.71,60.85,99,0,25.73,101.84,0.00,400.00,0.208805,0.216625,0.226430,0.214305,null,null,null
-2020-09-02T20:42:49Z,26.72,60.80,99,0,32.94,101.85,0.00,400.00,0.209641,0.216531,0.227906,0.214727,null,null,null
-2020-09-02T20:43:19Z,26.71,60.84,99,0,28.50,101.85,0.00,403.00,0.209344,0.216477,0.227984,0.214648,null,null,null
-2020-09-02T20:43:49Z,26.73,60.83,99,0,27.49,101.84,0.00,403.00,0.210047,0.217344,0.227742,0.215656,null,null,null
-2020-09-02T20:44:19Z,26.73,60.86,99,0,32.37,101.85,0.00,403.00,0.208148,0.215344,0.225977,0.213734,null,null,null
-2020-09-02T20:44:49Z,26.72,60.85,99,0,38.05,101.85,0.00,403.00,0.207078,0.215781,0.227391,0.214719,null,null,null
-2020-09-02T20:45:19Z,26.72,60.82,99,0,39.45,101.85,0.00,403.00,0.209148,0.216172,0.227555,0.214422,null,null,null
-2020-09-02T20:45:49Z,26.73,60.81,99,0,41.65,101.85,0.00,403.00,0.210391,0.216945,0.228977,0.215148,null,null,null
-2020-09-02T20:46:19Z,26.69,60.82,99,0,26.26,101.85,0.00,403.00,0.208656,0.216180,0.227305,0.214805,null,null,null
-2020-09-02T20:46:49Z,26.72,60.81,99,0,27.16,101.85,0.00,403.00,0.210250,0.217086,0.227367,0.215172,null,null,null
-2020-09-02T20:47:19Z,26.72,60.82,99,0,27.60,101.85,4.00,428.00,0.208734,0.216484,0.225766,0.215125,null,null,null
-2020-09-02T20:47:49Z,26.73,60.83,99,0,26.46,101.85,4.00,428.00,0.209453,0.215844,0.227570,0.214766,null,null,null
-2020-09-02T20:48:19Z,26.73,60.83,99,0,31.35,101.85,3.00,424.00,0.209156,0.216312,0.226680,0.214906,null,null,null
-2020-09-02T20:48:49Z,26.72,60.85,99,0,29.84,101.85,3.00,424.00,0.211070,0.217180,0.228211,0.214602,null,null,null
-2020-09-02T20:49:19Z,26.72,60.85,99,0,27.62,101.85,4.00,428.00,0.208430,0.216359,0.228625,0.214648,null,null,null
-2020-09-02T20:49:49Z,26.73,60.82,99,0,26.55,101.85,4.00,428.00,0.209445,0.217406,0.226711,0.215219,null,null,null
-2020-09-02T20:50:19Z,26.71,60.83,99,0,26.60,101.85,3.00,424.00,0.207867,0.216000,0.229125,0.214992,null,null,null
-2020-09-02T20:50:49Z,26.72,60.83,99,0,37.48,101.85,3.00,424.00,0.208078,0.216781,0.227867,0.214664,null,null,null
-2020-09-02T20:51:19Z,26.71,60.82,99,0,28.60,101.85,4.00,428.00,0.209992,0.217281,0.228188,0.215469,null,null,null
-2020-09-02T20:51:49Z,26.72,60.83,99,0,27.08,101.85,4.00,428.00,0.208359,0.215680,0.227625,0.213656,null,null,null
-2020-09-02T20:52:19Z,26.72,60.83,99,0,36.21,101.85,3.00,424.00,0.210328,0.216695,0.229320,0.215328,null,null,null
-2020-09-02T20:52:49Z,26.72,60.83,99,0,27.42,101.85,3.00,424.00,0.207312,0.216500,0.226906,0.214336,null,null,null
-2020-09-02T20:53:19Z,26.72,60.81,99,0,27.66,101.85,3.00,424.00,0.209922,0.216953,0.227305,0.215297,null,null,null
-2020-09-02T20:53:49Z,26.71,60.77,99,0,33.46,101.85,3.00,424.00,0.208406,0.215875,0.226953,0.214578,null,null,null
-2020-09-02T20:54:19Z,26.71,60.80,99,0,25.03,101.85,3.00,424.00,0.209172,0.216344,0.227211,0.215562,null,null,null
-2020-09-02T20:54:49Z,26.72,60.85,99,0,25.19,101.86,3.00,424.00,0.208687,0.216734,0.228547,0.215453,null,null,null
-2020-09-02T20:55:19Z,26.72,60.81,99,0,27.40,101.85,4.00,428.00,0.208719,0.216984,0.228844,0.215438,null,null,null
-2020-09-02T20:55:49Z,26.71,60.82,99,0,29.01,101.85,4.00,428.00,0.209250,0.216391,0.227633,0.215578,null,null,null
-2020-09-02T20:56:19Z,26.71,60.86,99,0,33.32,101.85,4.00,428.00,0.209195,0.216422,0.227094,0.214477,null,null,null
-2020-09-02T20:56:49Z,26.72,60.79,99,0,37.93,101.85,4.00,428.00,0.208703,0.215625,0.227727,0.215156,null,null,null
-2020-09-02T20:57:19Z,26.71,60.81,99,0,39.76,101.85,3.00,422.00,0.209484,0.216797,0.229594,0.214586,null,null,null
-2020-09-02T20:57:49Z,26.72,60.81,99,0,30.31,101.85,3.00,422.00,0.210117,0.216461,0.226156,0.214461,null,null,null
-2020-09-02T20:58:19Z,26.71,60.79,99,0,29.90,101.85,5.00,434.00,0.210781,0.217242,0.226008,0.214352,null,null,null
-2020-09-02T20:58:49Z,26.71,60.80,99,0,41.31,101.85,5.00,434.00,0.208844,0.216859,0.227313,0.214781,null,null,null
-2020-09-02T20:59:19Z,26.72,60.85,99,0,26.55,101.85,3.00,424.00,0.210781,0.216820,0.227695,0.214539,null,null,null
-2020-09-02T20:59:49Z,26.72,60.82,99,0,27.42,101.85,3.00,424.00,0.208500,0.216930,0.227023,0.215062,null,null,null
-2020-09-02T21:00:19Z,26.69,60.80,99,0,33.66,101.85,5.00,434.00,0.210219,0.218047,0.229445,0.214852,null,null,null
-2020-09-02T21:00:49Z,26.71,60.80,99,0,32.42,101.85,5.00,434.00,0.208930,0.216469,0.228906,0.215227,null,null,null
-2020-09-02T21:01:19Z,26.73,60.81,99,0,28.51,101.85,3.00,424.00,0.210773,0.217406,0.228117,0.214570,null,null,null
-2020-09-02T21:01:49Z,26.69,60.78,99,0,31.35,101.85,3.00,424.00,0.208805,0.215969,0.227836,0.215000,null,null,null
-2020-09-02T21:02:19Z,26.72,60.80,99,0,42.70,101.85,3.00,424.00,0.209734,0.217578,0.228734,0.214953,null,null,null
-2020-09-02T21:02:49Z,26.72,60.83,99,0,32.68,101.85,3.00,424.00,0.208703,0.217203,0.227398,0.214547,null,null,null
-2020-09-02T21:03:19Z,26.71,60.80,99,0,27.80,101.85,3.00,424.00,0.210406,0.217266,0.227875,0.214367,null,null,null
-2020-09-02T21:03:49Z,26.71,60.81,99,0,27.62,101.85,3.00,424.00,0.210406,0.217273,0.227281,0.214945,null,null,null
-2020-09-02T21:04:19Z,26.71,60.82,99,0,26.71,101.85,5.00,434.00,0.209523,0.216102,0.227484,0.215016,null,null,null
-2020-09-02T21:04:49Z,26.73,60.80,99,0,27.26,101.85,5.00,434.00,0.210336,0.217250,0.230086,0.215625,null,null,null
-2020-09-02T21:05:19Z,26.71,60.79,99,0,28.28,101.86,5.00,434.00,0.208586,0.216070,0.228906,0.215023,null,null,null
-2020-09-02T21:05:49Z,26.69,60.80,99,0,27.94,101.85,5.00,434.00,0.210008,0.216484,0.228000,0.215547,null,null,null
-2020-09-02T21:06:19Z,26.69,60.75,99,0,31.34,101.86,4.00,428.00,0.208969,0.216523,0.228062,0.215742,null,null,null
-2020-09-02T21:06:49Z,26.71,60.83,99,0,27.42,101.85,4.00,428.00,0.208531,0.216906,0.229031,0.215687,null,null,null
-2020-09-02T21:07:19Z,26.73,60.77,99,0,27.77,101.85,4.00,428.00,0.209531,0.216289,0.226242,0.214336,null,null,null
-2020-09-02T21:07:49Z,26.73,60.81,99,0,27.71,101.85,4.00,428.00,0.209320,0.216523,0.228078,0.214781,null,null,null
-2020-09-02T21:08:19Z,26.72,60.80,99,0,30.29,101.85,4.00,428.00,0.209586,0.217227,0.228758,0.215984,null,null,null
-2020-09-02T21:08:49Z,26.71,60.83,99,0,27.89,101.85,4.00,428.00,0.208047,0.216711,0.226234,0.214109,null,null,null
-2020-09-02T21:09:19Z,26.72,60.81,99,0,30.78,101.86,3.00,424.00,0.208961,0.216227,0.227047,0.215047,null,null,null
-2020-09-02T21:09:49Z,26.69,60.79,99,0,28.17,101.86,3.00,424.00,0.209047,0.216422,0.228453,0.215461,null,null,null
-2020-09-02T21:10:19Z,26.71,60.80,99,0,28.78,101.86,3.00,424.00,0.211406,0.216227,0.228172,0.215148,null,null,null
-2020-09-02T21:10:49Z,26.71,60.81,99,0,29.04,101.86,3.00,424.00,0.208586,0.217023,0.226703,0.215445,null,null,null
-2020-09-02T21:11:19Z,26.71,60.81,99,0,31.60,101.86,3.00,424.00,0.209258,0.215844,0.229563,0.215312,null,null,null
-2020-09-02T21:11:49Z,26.72,60.79,99,0,30.42,101.86,3.00,424.00,0.208750,0.216406,0.230023,0.215008,null,null,null
-2020-09-02T21:12:19Z,26.71,60.78,99,0,27.96,101.86,3.00,424.00,0.208203,0.216570,0.227266,0.215141,null,null,null
-2020-09-02T21:12:49Z,26.72,60.76,99,0,24.03,101.86,3.00,424.00,0.208914,0.216508,0.229438,0.215852,null,null,null
-2020-09-02T21:13:19Z,26.68,60.81,99,0,27.38,101.87,5.00,434.00,0.209688,0.217211,0.225828,0.214367,null,null,null
-2020-09-02T21:13:49Z,26.72,60.81,99,0,29.13,101.86,5.00,434.00,0.210945,0.218211,0.226859,0.214703,null,null,null
-2020-09-02T21:14:19Z,26.71,60.79,99,0,26.55,101.87,5.00,434.00,0.208641,0.216477,0.228437,0.215047,null,null,null
-2020-09-02T21:14:49Z,26.69,60.76,99,0,25.95,101.87,5.00,434.00,0.209164,0.216117,0.229430,0.215953,null,null,null
-2020-09-02T21:15:19Z,26.69,60.82,99,0,27.08,101.87,4.00,428.00,0.208258,0.215453,0.228148,0.214977,null,null,null
-2020-09-02T21:15:49Z,26.69,60.79,99,0,27.14,101.87,4.00,428.00,0.209891,0.216805,0.227414,0.214406,null,null,null
-2020-09-02T21:16:19Z,26.71,60.78,99,0,27.99,101.87,4.00,428.00,0.209531,0.216609,0.228680,0.214914,null,null,null
-2020-09-02T21:16:49Z,26.71,60.83,99,0,27.90,101.87,4.00,428.00,0.210383,0.217398,0.228133,0.215492,null,null,null
-2020-09-02T21:17:19Z,26.73,60.80,99,0,28.23,101.87,4.00,428.00,0.209609,0.217461,0.228414,0.214711,null,null,null
-2020-09-02T21:17:49Z,26.71,60.74,99,0,30.60,101.87,4.00,428.00,0.209398,0.217570,0.228617,0.215484,null,null,null
-2020-09-02T21:18:19Z,26.72,60.76,99,0,25.09,101.87,4.00,428.00,0.210609,0.218133,0.228352,0.215406,null,null,null
-2020-09-02T21:18:49Z,26.71,60.79,99,0,29.28,101.87,4.00,428.00,0.210406,0.217242,0.227141,0.214617,null,null,null
-2020-09-02T21:19:19Z,26.72,60.77,99,0,28.66,101.87,4.00,428.00,0.208750,0.216516,0.228781,0.215258,null,null,null
-2020-09-02T21:19:49Z,26.71,60.77,99,0,27.32,101.87,4.00,428.00,0.210320,0.216891,0.225883,0.214766,null,null,null
-2020-09-02T21:20:19Z,26.69,60.79,99,0,26.00,101.87,4.00,428.00,0.210047,0.216914,0.226914,0.213961,null,null,null
-2020-09-02T21:20:49Z,26.69,60.76,99,0,30.44,101.87,4.00,428.00,0.210648,0.217586,0.228555,0.215055,null,null,null
-2020-09-02T21:21:19Z,26.72,60.84,99,0,28.15,101.87,3.00,424.00,0.209094,0.216937,0.230297,0.215656,null,null,null
-2020-09-02T21:21:49Z,26.69,60.84,99,0,33.63,101.87,3.00,424.00,0.209172,0.215789,0.229375,0.214828,null,null,null
-2020-09-02T21:22:19Z,26.69,60.81,99,0,28.55,101.87,4.00,428.00,0.209063,0.216359,0.229414,0.215477,null,null,null
-2020-09-02T21:22:49Z,26.71,60.81,99,0,31.48,101.87,4.00,428.00,0.209273,0.216805,0.229102,0.215672,null,null,null
-2020-09-02T21:23:19Z,26.71,60.80,99,0,27.85,101.87,5.00,434.00,0.207617,0.217320,0.228563,0.215086,null,null,null
-2020-09-02T21:23:49Z,26.72,60.83,99,0,32.42,101.87,5.00,434.00,0.210203,0.216320,0.229734,0.215492,null,null,null
-2020-09-02T21:24:19Z,26.71,60.80,99,0,26.95,101.88,4.00,428.00,0.208570,0.215867,0.227070,0.214961,null,null,null
-2020-09-02T21:24:49Z,26.73,60.77,99,0,29.68,101.88,4.00,428.00,0.210734,0.216664,0.227867,0.215297,null,null,null
-2020-09-02T21:25:19Z,26.69,60.80,99,0,37.26,101.88,3.00,424.00,0.210680,0.217359,0.228766,0.215531,null,null,null
-2020-09-02T21:25:49Z,26.73,60.77,99,0,26.60,101.88,3.00,424.00,0.209813,0.216750,0.226734,0.214414,null,null,null
-2020-09-02T21:26:19Z,26.72,60.76,99,0,26.82,101.88,5.00,434.00,0.210063,0.217367,0.226305,0.214922,null,null,null
-2020-09-02T21:26:49Z,26.72,60.75,99,0,32.89,101.88,5.00,434.00,0.209266,0.217148,0.228641,0.215547,null,null,null
-2020-09-02T21:27:19Z,26.71,60.77,99,0,29.72,101.88,5.00,434.00,0.208555,0.217250,0.228813,0.215453,null,null,null
-2020-09-02T21:27:49Z,26.69,60.76,99,0,30.57,101.88,5.00,434.00,0.208219,0.215531,0.228813,0.215570,null,null,null
-2020-09-02T21:28:19Z,26.72,60.71,99,0,28.25,101.88,4.00,428.00,0.209672,0.217891,0.226797,0.214680,null,null,null
-2020-09-02T21:28:49Z,26.71,60.78,99,0,28.89,101.88,4.00,428.00,0.209094,0.216102,0.228398,0.215273,null,null,null
-2020-09-02T21:29:19Z,26.69,60.75,99,0,31.28,101.88,4.00,428.00,0.208773,0.215445,0.230203,0.214898,null,null,null
-2020-09-02T21:29:49Z,26.69,60.76,99,0,26.57,101.88,4.00,428.00,0.210477,0.217000,0.228477,0.215234,null,null,null
-2020-09-02T21:30:19Z,26.71,60.77,99,0,25.92,101.88,5.00,434.00,0.211031,0.216781,0.229969,0.215898,null,null,null
-2020-09-02T21:30:49Z,26.68,60.76,99,0,39.18,101.88,5.00,434.00,0.209180,0.216648,0.227250,0.214297,null,null,null
-2020-09-02T21:31:19Z,26.71,60.77,99,0,26.38,101.88,5.00,435.00,0.209648,0.216930,0.226812,0.214437,null,null,null
-2020-09-02T21:31:49Z,26.71,60.79,99,0,27.62,101.88,5.00,435.00,0.208414,0.216141,0.228563,0.215961,null,null,null
-2020-09-02T21:32:19Z,26.71,60.74,99,0,31.86,101.88,4.00,428.00,0.209562,0.216703,0.228445,0.214828,null,null,null
-2020-09-02T21:32:49Z,26.71,60.77,99,0,29.30,101.88,4.00,428.00,0.211258,0.217500,0.227461,0.215195,null,null,null
-2020-09-02T21:33:19Z,26.69,60.76,99,0,27.99,101.88,5.00,434.00,0.209516,0.217305,0.227273,0.214992,null,null,null
-2020-09-02T21:33:49Z,26.71,60.80,99,0,40.89,101.88,5.00,434.00,0.210719,0.217477,0.228188,0.214844,null,null,null
-2020-09-02T21:34:19Z,26.71,60.76,99,0,26.57,101.88,5.00,435.00,0.209367,0.216680,0.228406,0.214836,null,null,null
-2020-09-02T21:34:49Z,26.71,60.76,99,0,28.20,101.88,5.00,435.00,0.210562,0.216984,0.228836,0.215117,null,null,null
-2020-09-02T21:35:19Z,26.71,60.78,99,0,36.26,101.88,5.00,435.00,0.208242,0.217219,0.228391,0.215328,null,null,null
-2020-09-02T21:35:49Z,26.66,60.77,99,0,29.00,101.88,5.00,435.00,0.210344,0.217023,0.229211,0.215664,null,null,null
-2020-09-02T21:36:19Z,26.71,60.78,99,0,27.10,101.88,5.00,434.00,0.208148,0.216906,0.227922,0.215195,null,null,null
-2020-09-02T21:36:49Z,26.71,60.76,99,0,31.85,101.88,5.00,434.00,0.209898,0.216844,0.228437,0.215352,null,null,null
-2020-09-02T21:37:19Z,26.71,60.75,99,0,40.83,101.88,5.00,434.00,0.208562,0.216023,0.228117,0.214656,null,null,null
-2020-09-02T21:37:49Z,26.71,60.77,99,0,27.73,101.88,5.00,434.00,0.210164,0.216195,0.225977,0.214102,null,null,null
-2020-09-02T21:38:19Z,26.69,60.71,99,0,29.49,101.88,5.00,434.00,0.209969,0.217586,0.226977,0.214469,null,null,null
-2020-09-02T21:38:49Z,26.71,60.73,99,0,28.91,101.88,5.00,434.00,0.210773,0.218117,0.229070,0.215805,null,null,null
-2020-09-02T21:39:19Z,26.73,60.77,99,0,27.49,101.88,5.00,439.00,0.209586,0.216328,0.228672,0.215430,null,null,null
-2020-09-02T21:39:49Z,26.68,60.72,99,0,30.47,101.88,5.00,439.00,0.207914,0.215719,0.229281,0.216125,null,null,null
-2020-09-02T21:40:19Z,26.68,60.79,99,0,33.80,101.88,5.00,439.00,0.210109,0.217117,0.227617,0.214148,null,null,null
-2020-09-02T21:40:49Z,26.68,60.80,99,0,27.84,101.88,5.00,439.00,0.210531,0.217484,0.227023,0.214617,null,null,null
-2020-09-02T21:41:19Z,26.69,60.74,99,0,39.36,101.88,5.00,434.00,0.210523,0.217430,0.227328,0.215312,null,null,null
-2020-09-02T21:41:49Z,26.69,60.79,99,0,29.36,101.88,5.00,434.00,0.210328,0.216242,0.226469,0.215148,null,null,null
-2020-09-02T21:42:19Z,26.72,60.75,99,0,28.01,101.88,6.00,441.00,0.208766,0.216797,0.228047,0.214281,null,null,null
-2020-09-02T21:42:49Z,26.69,60.80,99,0,27.30,101.89,6.00,441.00,0.211063,0.217719,0.227578,0.215039,null,null,null
-2020-09-02T21:43:19Z,26.68,60.80,99,0,27.08,101.88,6.00,445.00,0.210133,0.216781,0.228164,0.215367,null,null,null
-2020-09-02T21:43:49Z,26.71,60.76,99,0,28.71,101.88,6.00,445.00,0.207891,0.216984,0.228523,0.215570,null,null,null
-2020-09-02T21:44:19Z,26.71,60.81,99,0,27.02,101.88,5.00,434.00,0.210016,0.217023,0.227383,0.215094,null,null,null
-2020-09-02T21:44:49Z,26.69,60.77,99,0,26.73,101.88,5.00,434.00,0.209156,0.217047,0.228914,0.215078,null,null,null
-2020-09-02T21:45:19Z,26.72,60.74,99,0,26.43,101.88,6.00,445.00,0.207906,0.215086,0.228148,0.215148,null,null,null
-2020-09-02T21:45:49Z,26.72,60.79,99,0,27.77,101.88,6.00,445.00,0.209883,0.216758,0.228352,0.215086,null,null,null
-2020-09-02T21:46:19Z,26.69,60.75,99,0,28.61,101.88,6.00,445.00,0.209453,0.217055,0.228563,0.215453,null,null,null
-2020-09-02T21:46:49Z,26.68,60.70,99,0,28.84,101.88,6.00,445.00,0.207742,0.216172,0.228570,0.215867,null,null,null
-2020-09-02T21:47:19Z,26.72,60.73,99,0,26.89,101.89,7.00,450.00,0.209187,0.216078,0.229625,0.215641,null,null,null
-2020-09-02T21:47:49Z,26.71,60.73,99,0,26.31,101.88,7.00,450.00,0.210086,0.217344,0.228250,0.215266,null,null,null
-2020-09-02T21:48:19Z,26.72,60.77,99,0,34.83,101.89,7.00,450.00,0.209766,0.216289,0.226805,0.214516,null,null,null
-2020-09-02T21:48:49Z,26.69,60.76,99,0,26.34,101.89,7.00,450.00,0.208891,0.217172,0.228258,0.214602,null,null,null
-2020-09-02T21:49:19Z,26.71,60.75,99,0,27.22,101.89,7.00,448.00,0.210727,0.216117,0.228156,0.215086,null,null,null
-2020-09-02T21:49:49Z,26.71,60.74,99,0,37.59,101.89,7.00,448.00,0.210125,0.217508,0.227812,0.214953,null,null,null
-2020-09-02T21:50:19Z,26.72,60.77,99,0,26.41,101.89,7.00,448.00,0.210797,0.216391,0.227445,0.214813,null,null,null
-2020-09-02T21:50:49Z,26.69,60.74,99,0,24.93,101.89,7.00,448.00,0.211836,0.217844,0.229445,0.215453,null,null,null
-2020-09-02T21:51:19Z,26.69,60.70,99,0,26.43,101.89,7.00,448.00,0.208781,0.216539,0.229383,0.215305,null,null,null
-2020-09-02T21:51:49Z,26.69,60.73,99,0,28.51,101.89,7.00,448.00,0.209336,0.216750,0.229484,0.216102,null,null,null
-2020-09-02T21:52:19Z,26.71,60.71,99,0,25.59,101.88,8.00,454.00,0.208258,0.215625,0.227094,0.214195,null,null,null
-2020-09-02T21:52:49Z,26.72,60.75,99,0,26.97,101.89,8.00,454.00,0.209141,0.217258,0.228109,0.215203,null,null,null
-2020-09-02T21:53:19Z,26.72,60.77,99,0,26.82,101.89,8.00,459.00,0.208961,0.217633,0.229586,0.215766,null,null,null
-2020-09-02T21:53:49Z,26.69,60.72,99,0,27.51,101.89,8.00,459.00,0.208930,0.215953,0.228047,0.215453,null,null,null
-2020-09-02T21:54:19Z,26.71,60.73,99,0,32.14,101.89,7.00,448.00,0.209414,0.216836,0.227266,0.215023,null,null,null
-2020-09-02T21:54:49Z,26.69,60.75,99,0,36.11,101.89,7.00,448.00,0.210180,0.216734,0.228109,0.215180,null,null,null
-2020-09-02T21:55:19Z,26.69,60.76,99,0,26.87,101.89,8.00,459.00,0.209195,0.216609,0.227617,0.215219,null,null,null
-2020-09-02T21:55:49Z,26.71,60.75,99,0,28.76,101.89,8.00,459.00,0.209484,0.216695,0.228836,0.215562,null,null,null
-2020-09-02T21:56:19Z,26.69,60.73,99,0,26.57,101.89,8.00,454.00,0.209742,0.216594,0.228266,0.215320,null,null,null
-2020-09-02T21:56:49Z,26.71,60.74,99,0,26.82,101.89,8.00,454.00,0.209203,0.217055,0.229375,0.215414,null,null,null
-2020-09-02T21:57:19Z,26.71,60.73,99,0,30.16,101.89,8.00,459.00,0.209344,0.216367,0.228719,0.215633,null,null,null
-2020-09-02T21:57:49Z,26.69,60.72,99,0,27.45,101.89,8.00,459.00,0.208070,0.216656,0.226906,0.214633,null,null,null
-2020-09-02T21:58:19Z,26.68,60.82,99,0,26.93,101.89,8.00,459.00,0.211234,0.217672,0.227516,0.215062,null,null,null
-2020-09-02T21:58:49Z,26.68,60.79,99,0,26.57,101.89,8.00,459.00,0.208953,0.217063,0.225406,0.214070,null,null,null
-2020-09-02T21:59:19Z,26.71,60.75,99,0,29.04,101.89,8.00,459.00,0.209734,0.216711,0.226766,0.215727,null,null,null
-2020-09-02T21:59:49Z,26.68,60.69,99,0,26.14,101.89,8.00,459.00,0.208102,0.216297,0.227891,0.215172,null,null,null
-2020-09-02T22:00:19Z,26.69,60.70,99,0,28.06,101.89,8.00,454.00,0.208664,0.216945,0.228172,0.215539,null,null,null
-2020-09-02T22:00:49Z,26.69,60.76,99,0,28.47,101.90,8.00,454.00,0.209937,0.216781,0.227812,0.215352,null,null,null
-2020-09-02T22:01:19Z,26.71,60.71,99,0,25.76,101.90,8.00,459.00,0.209484,0.216273,0.227742,0.215133,null,null,null
-2020-09-02T22:01:49Z,26.69,60.71,99,0,26.31,101.90,8.00,459.00,0.210492,0.216813,0.228008,0.214398,null,null,null
-2020-09-02T22:02:19Z,26.69,60.70,99,0,25.59,101.90,10.00,470.00,0.209852,0.216961,0.228055,0.215398,null,null,null
-2020-09-02T22:02:49Z,26.66,60.69,99,0,39.59,101.90,10.00,470.00,0.208813,0.216156,0.227500,0.214398,null,null,null
-2020-09-02T22:03:19Z,26.69,60.69,99,0,28.34,101.90,10.00,470.00,0.209211,0.217102,0.228813,0.215023,null,null,null
-2020-09-02T22:03:49Z,26.71,60.67,99,0,28.39,101.90,10.00,470.00,0.208891,0.216898,0.227812,0.215258,null,null,null
-2020-09-02T22:04:19Z,26.69,60.74,99,0,28.25,101.90,10.00,470.00,0.209094,0.217211,0.229312,0.215641,null,null,null
-2020-09-02T22:04:49Z,26.69,60.70,99,0,27.55,101.90,10.00,470.00,0.208430,0.216609,0.227109,0.215406,null,null,null
-2020-09-02T22:05:19Z,26.69,60.70,99,0,29.03,101.90,8.00,459.00,0.209453,0.216734,0.227820,0.215172,null,null,null
-2020-09-02T22:05:49Z,26.69,60.71,99,0,29.16,101.90,8.00,459.00,0.209898,0.217867,0.229469,0.215367,null,null,null
-2020-09-02T22:06:19Z,26.71,60.77,99,0,27.85,101.90,10.00,470.00,0.209906,0.218539,0.227883,0.215125,null,null,null
-2020-09-02T22:06:49Z,26.69,60.77,99,0,28.61,101.90,10.00,470.00,0.208055,0.216484,0.229133,0.214883,null,null,null
-2020-09-02T22:07:19Z,26.69,60.67,99,0,27.92,101.90,10.00,470.00,0.209047,0.217141,0.228258,0.215680,null,null,null
-2020-09-02T22:07:49Z,26.68,60.72,99,0,27.30,101.90,10.00,470.00,0.208203,0.217414,0.227477,0.215016,null,null,null
-2020-09-02T22:08:19Z,26.69,60.71,99,0,31.69,101.90,10.00,470.00,0.209539,0.217055,0.228766,0.214312,null,null,null
-2020-09-02T22:08:49Z,26.65,60.68,99,0,26.24,101.90,10.00,470.00,0.208547,0.215984,0.227078,0.215297,null,null,null
-2020-09-02T22:09:19Z,26.68,60.70,99,0,30.99,101.91,10.00,470.00,0.209133,0.217523,0.226437,0.215289,null,null,null
-2020-09-02T22:09:49Z,26.68,60.75,99,0,26.53,101.91,10.00,470.00,0.208367,0.216242,0.229148,0.215422,null,null,null
-2020-09-02T22:10:19Z,26.71,60.75,99,0,26.21,101.91,10.00,470.00,0.210984,0.217852,0.228164,0.214383,null,null,null
-2020-09-02T22:10:49Z,26.69,60.73,99,0,27.89,101.90,10.00,470.00,0.209648,0.216813,0.228414,0.214883,null,null,null
-2020-09-02T22:11:19Z,26.71,60.70,99,0,25.87,101.91,10.00,470.00,0.208813,0.216109,0.227617,0.215547,null,null,null
-2020-09-02T22:11:49Z,26.72,60.71,99,0,25.73,101.91,10.00,470.00,0.210805,0.218906,0.227070,0.215500,null,null,null
-2020-09-02T22:12:19Z,26.69,60.68,99,0,29.58,101.91,12.00,480.00,0.211086,0.217594,0.228734,0.215109,null,null,null
-2020-09-02T22:12:49Z,26.65,60.70,99,0,26.11,101.91,12.00,480.00,0.208602,0.217836,0.227336,0.215188,null,null,null
-2020-09-02T22:13:19Z,26.68,60.66,99,0,26.55,101.91,12.00,480.00,0.210109,0.217336,0.226055,0.214492,null,null,null
-2020-09-02T22:13:49Z,26.69,60.71,99,0,27.34,101.91,12.00,480.00,0.209508,0.217734,0.229578,0.215469,null,null,null
-2020-09-02T22:14:19Z,26.69,60.68,99,0,26.11,101.91,12.00,480.00,0.210570,0.216562,0.229656,0.215148,null,null,null
-2020-09-02T22:14:49Z,26.68,60.73,99,0,26.95,101.91,12.00,480.00,0.210133,0.216711,0.228578,0.215344,null,null,null
-2020-09-02T22:15:19Z,26.66,60.68,99,0,27.75,101.91,11.00,476.00,0.209609,0.216727,0.226453,0.215625,null,null,null
-2020-09-02T22:15:49Z,26.71,60.66,99,0,26.87,101.91,11.00,476.00,0.209234,0.216836,0.228039,0.214906,null,null,null
-2020-09-02T22:16:19Z,26.71,60.70,99,0,31.86,101.91,12.00,480.00,0.208727,0.215531,0.226562,0.214953,null,null,null
-2020-09-02T22:16:49Z,26.71,60.68,99,0,28.17,101.91,12.00,480.00,0.208813,0.216977,0.228969,0.215359,null,null,null
-2020-09-02T22:17:19Z,26.71,60.69,99,0,28.37,101.91,12.00,480.00,0.209695,0.217492,0.227719,0.214977,null,null,null
-2020-09-02T22:17:49Z,26.69,60.71,99,0,29.62,101.91,12.00,480.00,0.210750,0.216617,0.227141,0.214695,null,null,null
-2020-09-02T22:18:19Z,26.66,60.72,99,0,29.31,101.91,11.00,476.00,0.209656,0.216758,0.228047,0.215227,null,null,null
-2020-09-02T22:18:49Z,26.71,60.67,99,0,25.65,101.91,11.00,476.00,0.209766,0.217383,0.228352,0.215414,null,null,null
-2020-09-02T22:19:19Z,26.69,60.70,99,0,28.12,101.91,13.00,486.00,0.209391,0.216391,0.227969,0.215023,null,null,null
-2020-09-02T22:19:49Z,26.68,60.68,99,0,27.73,101.92,13.00,486.00,0.210109,0.216555,0.229258,0.214828,null,null,null
-2020-09-02T22:20:19Z,26.71,60.68,99,0,27.28,101.92,13.00,486.00,0.208453,0.218070,0.228180,0.215484,null,null,null
-2020-09-02T22:20:49Z,26.68,60.72,99,0,26.99,101.92,13.00,486.00,0.209656,0.217625,0.230500,0.215047,null,null,null
-2020-09-02T22:21:19Z,26.68,60.70,99,0,28.15,101.92,13.00,486.00,0.209039,0.217766,0.227891,0.215172,null,null,null
-2020-09-02T22:21:49Z,26.68,60.74,99,0,26.91,101.92,13.00,486.00,0.209344,0.216258,0.228672,0.215406,null,null,null
-2020-09-02T22:22:19Z,26.71,60.76,99,0,28.15,101.92,14.00,492.00,0.208703,0.215820,0.226844,0.215273,null,null,null
-2020-09-02T22:22:49Z,26.69,60.73,99,0,25.59,101.92,14.00,492.00,0.209711,0.216805,0.229898,0.215891,null,null,null
-2020-09-02T22:23:19Z,26.68,60.74,99,0,24.83,101.92,13.00,486.00,0.209609,0.217336,0.227633,0.215391,null,null,null
-2020-09-02T22:23:49Z,26.68,60.74,99,0,29.32,101.92,13.00,486.00,0.209734,0.216461,0.227750,0.215273,null,null,null
-2020-09-02T22:24:19Z,26.68,60.67,99,0,27.64,101.92,12.00,480.00,0.209250,0.216992,0.228719,0.215828,null,null,null
-2020-09-02T22:24:49Z,26.68,60.71,99,0,27.16,101.93,12.00,480.00,0.210305,0.217852,0.226891,0.215211,null,null,null
-2020-09-02T22:25:19Z,26.66,60.72,99,0,27.32,101.92,14.00,492.00,0.211047,0.217781,0.227984,0.215258,null,null,null
-2020-09-02T22:25:49Z,26.69,60.71,99,0,27.78,101.92,14.00,492.00,0.210375,0.219086,0.227789,0.214805,null,null,null
-2020-09-02T22:26:19Z,26.65,60.71,99,0,29.27,101.92,14.00,492.00,0.209602,0.216922,0.228352,0.214898,null,null,null
-2020-09-02T22:26:49Z,26.68,60.72,99,0,33.66,101.92,14.00,492.00,0.209695,0.216055,0.228414,0.214547,null,null,null
-2020-09-02T22:27:19Z,26.66,60.71,99,0,25.82,101.93,14.00,492.00,0.209391,0.217125,0.227695,0.214758,null,null,null
-2020-09-02T22:27:49Z,26.69,60.71,99,0,29.82,101.93,14.00,492.00,0.208820,0.216820,0.228008,0.216102,null,null,null
-2020-09-02T22:28:19Z,26.68,60.75,99,0,37.01,101.93,13.00,486.00,0.211055,0.218023,0.229836,0.216578,null,null,null
-2020-09-02T22:28:49Z,26.66,60.73,99,0,26.87,101.93,13.00,486.00,0.211430,0.216727,0.226930,0.214273,null,null,null
-2020-09-02T22:29:19Z,26.66,60.72,99,0,27.36,101.93,13.00,486.00,0.209805,0.217195,0.227016,0.215227,null,null,null
-2020-09-02T22:29:49Z,26.69,60.73,99,0,27.20,101.92,13.00,486.00,0.210203,0.217375,0.227859,0.214742,null,null,null
-2020-09-02T22:30:19Z,26.66,60.73,99,0,28.63,101.93,14.00,492.00,0.208922,0.216977,0.227750,0.215195,null,null,null
-2020-09-02T22:30:49Z,26.69,60.73,99,0,27.40,101.93,14.00,492.00,0.207891,0.216906,0.228617,0.215039,null,null,null
-2020-09-02T22:31:19Z,26.69,60.75,99,0,27.32,101.93,13.00,486.00,0.210688,0.217711,0.228695,0.215273,null,null,null
-2020-09-02T22:31:49Z,26.66,60.70,99,0,29.89,101.93,13.00,486.00,0.209781,0.216703,0.228352,0.215297,null,null,null
-2020-09-02T22:32:19Z,26.69,60.73,99,0,26.84,101.93,14.00,496.00,0.211375,0.217141,0.227609,0.215000,null,null,null
-2020-09-02T22:32:49Z,26.69,60.73,99,0,30.55,101.93,14.00,496.00,0.210227,0.216609,0.227516,0.215695,null,null,null
-2020-09-02T22:33:19Z,26.68,60.69,99,0,24.93,101.93,14.00,496.00,0.210625,0.217258,0.229266,0.215594,null,null,null
-2020-09-02T22:33:49Z,26.68,60.70,99,0,27.12,101.93,14.00,496.00,0.210648,0.217648,0.229281,0.215609,null,null,null
-2020-09-02T22:34:19Z,26.69,60.75,99,0,29.17,101.93,14.00,492.00,0.210047,0.217117,0.227961,0.215359,null,null,null
-2020-09-02T22:34:49Z,26.68,60.71,99,0,29.26,101.93,14.00,492.00,0.206883,0.216078,0.227375,0.215195,null,null,null
-2020-09-02T22:35:19Z,26.66,60.72,99,0,27.96,101.93,14.00,496.00,0.211797,0.218156,0.227328,0.215547,null,null,null
-2020-09-02T22:35:49Z,26.66,60.77,99,0,28.22,101.93,14.00,496.00,0.209617,0.215672,0.228617,0.215500,null,null,null
-2020-09-02T22:36:19Z,26.66,60.73,99,0,26.71,101.93,14.00,492.00,0.209187,0.216680,0.227836,0.214687,null,null,null
-2020-09-02T22:36:49Z,26.68,60.74,99,0,28.34,101.93,14.00,492.00,0.210086,0.216102,0.228945,0.214281,null,null,null
-2020-09-02T22:37:19Z,26.69,60.72,99,0,26.06,101.93,14.00,496.00,0.209211,0.216445,0.227789,0.215953,null,null,null
-2020-09-02T22:37:49Z,26.69,60.72,99,0,26.78,101.93,14.00,496.00,0.209531,0.216750,0.228406,0.215258,null,null,null
-2020-09-02T22:38:19Z,26.65,60.72,99,0,26.53,101.93,14.00,492.00,0.210703,0.218203,0.227531,0.215117,null,null,null
-2020-09-02T22:38:49Z,26.68,60.69,99,0,27.12,101.93,14.00,492.00,0.209187,0.217438,0.228719,0.215523,null,null,null
-2020-09-02T22:39:19Z,26.68,60.72,99,0,27.75,101.93,14.00,496.00,0.210562,0.217141,0.229133,0.215273,null,null,null
-2020-09-02T22:39:49Z,26.69,60.75,99,0,25.84,101.93,14.00,496.00,0.209305,0.217078,0.226930,0.214914,null,null,null
-2020-09-02T22:40:19Z,26.68,60.69,99,0,24.58,101.93,14.00,492.00,0.210828,0.218484,0.227117,0.215141,null,null,null
-2020-09-02T22:40:49Z,26.68,60.69,99,0,27.59,101.93,14.00,492.00,0.210945,0.217406,0.228258,0.214961,null,null,null
-2020-09-02T22:41:19Z,26.66,60.70,99,0,28.02,101.93,15.00,501.00,0.209359,0.217391,0.228844,0.215344,null,null,null
-2020-09-02T22:41:49Z,26.68,60.69,99,0,28.52,101.93,15.00,501.00,0.208195,0.217023,0.227984,0.214734,null,null,null
-2020-09-02T22:42:19Z,26.68,60.71,99,0,26.67,101.94,15.00,501.00,0.208758,0.217242,0.228375,0.215602,null,null,null
-2020-09-02T22:42:49Z,26.66,60.71,99,0,29.03,101.93,15.00,501.00,0.209234,0.217672,0.228828,0.215406,null,null,null
-2020-09-02T22:43:19Z,26.68,60.75,99,0,26.41,101.94,15.00,501.00,0.210289,0.218187,0.227461,0.214867,null,null,null
-2020-09-02T22:43:49Z,26.66,60.69,99,0,28.06,101.94,15.00,501.00,0.208734,0.217023,0.228125,0.215633,null,null,null
-2020-09-02T22:44:19Z,26.68,60.66,99,0,28.14,101.94,15.00,501.00,0.209844,0.216773,0.229305,0.214813,null,null,null
-2020-09-02T22:44:49Z,26.66,60.69,99,0,25.67,101.94,15.00,501.00,0.211477,0.217195,0.227055,0.214414,null,null,null
-2020-09-02T22:45:19Z,26.66,60.73,99,0,25.79,101.94,15.00,501.00,0.209555,0.217297,0.229672,0.215469,null,null,null
-2020-09-02T22:45:49Z,26.68,60.72,99,0,30.96,101.94,15.00,501.00,0.208406,0.216109,0.228586,0.216133,null,null,null
-2020-09-02T22:46:19Z,26.68,60.69,99,0,26.95,101.94,15.00,501.00,0.209531,0.216266,0.227398,0.214500,null,null,null
-2020-09-02T22:46:49Z,26.66,60.71,99,0,25.38,101.94,15.00,501.00,0.208922,0.216742,0.230086,0.215562,null,null,null
-2020-09-02T22:47:19Z,26.66,60.71,99,0,28.09,101.94,15.00,501.00,0.209680,0.216422,0.228086,0.215406,null,null,null
-2020-09-02T22:47:49Z,26.69,60.75,99,0,26.48,101.94,15.00,501.00,0.208609,0.216891,0.228391,0.214594,null,null,null
-2020-09-02T22:48:19Z,26.66,60.70,99,0,27.45,101.94,16.00,508.00,0.208438,0.216617,0.227898,0.215672,null,null,null
-2020-09-02T22:48:49Z,26.68,60.72,99,0,30.01,101.94,16.00,508.00,0.209992,0.217289,0.227445,0.215070,null,null,null
-2020-09-02T22:49:19Z,26.66,60.67,99,0,26.57,101.94,16.00,508.00,0.210305,0.217266,0.229086,0.215625,null,null,null
-2020-09-02T22:49:49Z,26.66,60.74,99,0,24.65,101.94,16.00,508.00,0.210164,0.217187,0.227625,0.215156,null,null,null
-2020-09-02T22:50:19Z,26.68,60.73,99,0,27.32,101.94,16.00,508.00,0.208195,0.216258,0.228938,0.214891,null,null,null
-2020-09-02T22:50:49Z,26.68,60.72,99,0,26.78,101.94,16.00,508.00,0.209930,0.217453,0.227187,0.214195,null,null,null
-2020-09-02T22:51:19Z,26.66,60.68,99,0,26.14,101.94,15.00,502.00,0.210367,0.217727,0.228289,0.215031,null,null,null
-2020-09-02T22:51:49Z,26.65,60.71,99,0,28.07,101.94,15.00,502.00,0.210000,0.217234,0.227828,0.215469,null,null,null
-2020-09-02T22:52:19Z,26.68,60.77,99,0,27.73,101.94,16.00,508.00,0.210547,0.217492,0.228406,0.215641,null,null,null
-2020-09-02T22:52:49Z,26.66,60.70,99,0,26.82,101.94,16.00,508.00,0.208789,0.217195,0.231500,0.215281,null,null,null
-2020-09-02T22:53:19Z,26.68,60.74,99,0,26.11,101.94,16.00,508.00,0.210367,0.218484,0.229672,0.215453,null,null,null
-2020-09-02T22:53:49Z,26.66,60.70,99,0,26.97,101.94,16.00,508.00,0.209305,0.218273,0.227852,0.215813,null,null,null
-2020-09-02T22:54:19Z,26.66,60.70,99,0,26.26,101.94,16.00,508.00,0.210555,0.217609,0.229609,0.215406,null,null,null
-2020-09-02T22:54:49Z,26.68,60.69,99,0,27.30,101.94,16.00,508.00,0.209148,0.217391,0.228125,0.215164,null,null,null
-2020-09-02T22:55:19Z,26.68,60.72,99,0,25.38,101.94,16.00,508.00,0.209906,0.217391,0.228516,0.215172,null,null,null
-2020-09-02T22:55:49Z,26.65,60.70,99,0,25.82,101.95,16.00,508.00,0.210648,0.217328,0.230391,0.215906,null,null,null
-2020-09-02T22:56:19Z,26.66,60.67,99,0,26.73,101.95,16.00,508.00,0.210703,0.217344,0.228602,0.215297,null,null,null
-2020-09-02T22:56:49Z,26.68,60.67,99,0,29.61,101.95,16.00,508.00,0.210328,0.217945,0.228617,0.215023,null,null,null
-2020-09-02T22:57:19Z,26.68,60.67,99,0,24.72,101.95,17.00,518.00,0.210195,0.217063,0.228313,0.215242,null,null,null
-2020-09-02T22:57:49Z,26.65,60.71,99,0,29.16,101.94,17.00,518.00,0.209602,0.217836,0.227305,0.214625,null,null,null
-2020-09-02T22:58:19Z,26.66,60.67,99,0,25.98,101.94,16.00,508.00,0.209891,0.217609,0.229578,0.215359,null,null,null
-2020-09-02T22:58:49Z,26.68,60.69,99,0,41.57,101.94,16.00,508.00,0.209531,0.217445,0.228758,0.215219,null,null,null
-2020-09-02T22:59:19Z,26.66,60.70,99,0,26.84,101.94,16.00,508.00,0.208758,0.216633,0.227641,0.215328,null,null,null
-2020-09-02T22:59:49Z,26.65,60.67,99,0,27.68,101.95,16.00,508.00,0.209867,0.217133,0.227273,0.215766,null,null,null
-2020-09-02T23:00:19Z,26.65,60.71,99,0,31.87,101.94,16.00,508.00,0.209781,0.218070,0.228906,0.215234,null,null,null
-2020-09-02T23:00:49Z,26.68,60.68,99,0,27.59,101.94,16.00,508.00,0.210320,0.217328,0.227914,0.215641,null,null,null
-2020-09-02T23:01:19Z,26.68,60.74,99,0,26.64,101.95,16.00,508.00,0.210695,0.216930,0.229383,0.216133,null,null,null
-2020-09-02T23:01:49Z,26.66,60.74,99,0,31.88,101.94,16.00,508.00,0.209727,0.218219,0.226961,0.214930,null,null,null
-2020-09-02T23:02:19Z,26.66,60.69,99,0,26.00,101.94,16.00,508.00,0.211766,0.218242,0.229461,0.215141,null,null,null
-2020-09-02T23:02:49Z,26.66,60.76,99,0,27.47,101.94,16.00,508.00,0.209648,0.216602,0.227094,0.215367,null,null,null
-2020-09-02T23:03:19Z,26.68,60.70,99,0,32.38,101.95,16.00,508.00,0.209711,0.216875,0.229508,0.215312,null,null,null
-2020-09-02T23:03:49Z,26.66,60.69,99,0,40.23,101.94,16.00,508.00,0.210555,0.217844,0.228977,0.216562,null,null,null
-2020-09-02T23:04:19Z,26.66,60.71,99,0,29.99,101.94,16.00,508.00,0.210211,0.216234,0.228586,0.215102,null,null,null
-2020-09-02T23:04:49Z,26.66,60.73,99,0,33.20,101.95,16.00,508.00,0.210531,0.216492,0.228547,0.215188,null,null,null
-2020-09-02T23:05:19Z,26.65,60.73,99,0,41.50,101.95,17.00,518.00,0.210250,0.217031,0.229258,0.215852,null,null,null
-2020-09-02T23:05:49Z,26.64,60.71,99,0,42.85,101.95,17.00,518.00,0.209133,0.215930,0.228938,0.215516,null,null,null
-2020-09-02T23:06:19Z,26.66,60.69,99,0,31.97,101.95,16.00,508.00,0.208898,0.216867,0.227437,0.215547,null,null,null
-2020-09-02T23:06:49Z,26.65,60.71,99,0,26.16,101.95,16.00,508.00,0.209586,0.216922,0.227719,0.214570,null,null,null
-2020-09-02T23:07:19Z,26.64,60.71,99,0,25.00,101.95,17.00,518.00,0.211070,0.217672,0.227914,0.215039,null,null,null
-2020-09-02T23:07:49Z,26.65,60.70,99,0,28.54,101.95,17.00,518.00,0.210078,0.216531,0.229375,0.215687,null,null,null
-2020-09-02T23:08:19Z,26.65,60.69,99,0,34.62,101.95,16.00,508.00,0.210070,0.217453,0.226203,0.214813,null,null,null
-2020-09-02T23:08:49Z,26.64,60.69,99,0,29.69,101.95,16.00,508.00,0.208875,0.216102,0.228375,0.215055,null,null,null
-2020-09-02T23:09:19Z,26.66,60.67,99,0,26.19,101.95,16.00,508.00,0.210602,0.217180,0.229391,0.215242,null,null,null
-2020-09-02T23:09:49Z,26.65,60.65,99,0,24.89,101.95,16.00,508.00,0.211227,0.218164,0.227539,0.215461,null,null,null
-2020-09-02T23:10:19Z,26.66,60.66,99,0,27.22,101.95,17.00,518.00,0.209930,0.217578,0.228797,0.215398,null,null,null
-2020-09-02T23:10:49Z,26.64,60.67,99,0,28.51,101.95,17.00,518.00,0.210133,0.217586,0.228047,0.215578,null,null,null
-2020-09-02T23:11:19Z,26.66,60.72,99,0,28.34,101.95,17.00,518.00,0.208922,0.216422,0.227742,0.215719,null,null,null
-2020-09-02T23:11:49Z,26.66,60.75,99,0,28.17,101.95,17.00,518.00,0.209977,0.217484,0.227984,0.215312,null,null,null
-2020-09-02T23:12:19Z,26.64,60.71,99,0,27.18,101.95,17.00,518.00,0.211688,0.217508,0.229445,0.215734,null,null,null
-2020-09-02T23:12:49Z,26.65,60.70,99,0,26.19,101.96,17.00,518.00,0.208805,0.216664,0.228781,0.215508,null,null,null
-2020-09-02T23:13:19Z,26.64,60.65,99,0,25.53,101.96,17.00,518.00,0.210109,0.216852,0.227719,0.215008,null,null,null
-2020-09-02T23:13:49Z,26.64,60.70,99,0,32.12,101.95,17.00,518.00,0.209461,0.217992,0.228383,0.215555,null,null,null
-2020-09-02T23:14:19Z,26.66,60.70,99,0,27.28,101.95,17.00,518.00,0.209383,0.217562,0.227648,0.215352,null,null,null
-2020-09-02T23:14:49Z,26.66,60.62,99,0,25.41,101.95,17.00,518.00,0.208109,0.217172,0.226594,0.214422,null,null,null
-2020-09-02T23:15:19Z,26.64,60.73,99,0,28.17,101.95,17.00,518.00,0.212023,0.217625,0.228188,0.215305,null,null,null
-2020-09-02T23:15:49Z,26.68,60.63,99,0,28.17,101.95,17.00,518.00,0.210641,0.217461,0.229102,0.215125,null,null,null
-2020-09-02T23:16:19Z,26.65,60.69,99,0,27.59,101.95,17.00,518.00,0.209898,0.215687,0.227711,0.215141,null,null,null
-2020-09-02T23:16:49Z,26.65,60.71,99,0,26.55,101.95,17.00,518.00,0.209891,0.218477,0.228219,0.215195,null,null,null
-2020-09-02T23:17:19Z,26.66,60.70,99,0,25.22,101.95,17.00,518.00,0.209266,0.216117,0.228641,0.214813,null,null,null
-2020-09-02T23:17:49Z,26.64,60.72,99,0,27.57,101.95,17.00,518.00,0.210367,0.217297,0.228727,0.215594,null,null,null
-2020-09-02T23:18:19Z,26.64,60.70,99,0,25.84,101.96,16.00,508.00,0.210313,0.217016,0.228109,0.214969,null,null,null
-2020-09-02T23:18:49Z,26.65,60.69,99,0,27.62,101.95,16.00,508.00,0.210570,0.217031,0.229016,0.215359,null,null,null
-2020-09-02T23:19:19Z,26.64,60.70,99,0,29.15,101.95,17.00,518.00,0.209328,0.217281,0.230070,0.215945,null,null,null
-2020-09-02T23:19:49Z,26.68,60.63,99,0,25.38,101.95,17.00,518.00,0.210750,0.216469,0.227570,0.214750,null,null,null
-2020-09-02T23:20:19Z,26.65,60.68,99,0,27.24,101.95,17.00,518.00,0.209328,0.217039,0.228055,0.215672,null,null,null
-2020-09-02T23:20:49Z,26.68,60.63,99,0,27.04,101.95,17.00,518.00,0.210719,0.217086,0.228383,0.214711,null,null,null
-2020-09-02T23:21:19Z,26.64,60.62,99,0,27.24,101.95,16.00,508.00,0.209297,0.216016,0.228141,0.216109,null,null,null
-2020-09-02T23:21:49Z,26.65,60.70,99,0,29.90,101.95,16.00,508.00,0.210648,0.217547,0.227055,0.215164,null,null,null
-2020-09-02T23:22:19Z,26.62,60.68,99,0,27.18,101.95,17.00,518.00,0.210641,0.217227,0.228836,0.215734,null,null,null
-2020-09-02T23:22:49Z,26.66,60.70,99,0,29.50,101.95,17.00,518.00,0.209867,0.217367,0.228516,0.216188,null,null,null
-2020-09-02T23:23:19Z,26.66,60.70,99,0,28.73,101.95,17.00,518.00,0.208508,0.218437,0.227914,0.216141,null,null,null
-2020-09-02T23:23:49Z,26.62,60.68,99,0,25.90,101.95,17.00,518.00,0.208813,0.218250,0.228625,0.215578,null,null,null
-2020-09-02T23:24:19Z,26.64,60.70,99,0,28.63,101.95,17.00,518.00,0.209242,0.216766,0.229219,0.216047,null,null,null
-2020-09-02T23:24:49Z,26.62,60.72,99,0,26.93,101.95,17.00,518.00,0.209758,0.216172,0.227914,0.214898,null,null,null
-2020-09-02T23:25:19Z,26.64,60.65,99,0,28.64,101.95,17.00,518.00,0.208180,0.216414,0.227852,0.215008,null,null,null
-2020-09-02T23:25:49Z,26.64,60.67,99,0,26.41,101.95,17.00,518.00,0.209719,0.217492,0.227477,0.214937,null,null,null
-2020-09-02T23:26:19Z,26.64,60.63,99,0,26.64,101.95,17.00,518.00,0.209594,0.217305,0.229977,0.215859,null,null,null
-2020-09-02T23:26:49Z,26.66,60.69,99,0,29.35,101.95,17.00,518.00,0.210430,0.216641,0.228461,0.215789,null,null,null
-2020-09-02T23:27:19Z,26.62,60.71,99,0,27.68,101.95,17.00,518.00,0.210594,0.216422,0.227828,0.215633,null,null,null
-2020-09-02T23:27:49Z,26.62,60.73,99,0,30.77,101.95,17.00,518.00,0.210703,0.217242,0.228898,0.215906,null,null,null
-2020-09-02T23:28:19Z,26.64,60.76,99,0,27.64,101.95,17.00,518.00,0.208492,0.217469,0.226938,0.215305,null,null,null
-2020-09-02T23:28:49Z,26.61,60.73,99,0,26.31,101.95,17.00,518.00,0.208422,0.216836,0.229813,0.215945,null,null,null
-2020-09-02T23:29:19Z,26.65,60.67,99,0,27.87,101.95,17.00,518.00,0.209984,0.217906,0.228141,0.214531,null,null,null
-2020-09-02T23:29:49Z,26.62,60.66,99,0,26.26,101.95,17.00,518.00,0.211125,0.217500,0.228906,0.215531,null,null,null
-2020-09-02T23:30:19Z,26.65,60.71,99,0,26.62,101.95,17.00,518.00,0.211016,0.218039,0.228305,0.214992,null,null,null
-2020-09-02T23:30:49Z,26.62,60.70,99,0,36.92,101.95,17.00,518.00,0.209523,0.217031,0.228000,0.215414,null,null,null
-2020-09-02T23:31:19Z,26.64,60.67,99,0,29.01,101.95,17.00,518.00,0.208750,0.217937,0.227680,0.215531,null,null,null
-2020-09-02T23:31:49Z,26.65,60.69,99,0,26.95,101.95,17.00,518.00,0.209883,0.218117,0.228883,0.215320,null,null,null
-2020-09-02T23:32:19Z,26.62,60.70,99,0,26.80,101.95,17.00,518.00,0.209109,0.215617,0.229422,0.215742,null,null,null
-2020-09-02T23:32:49Z,26.64,60.68,99,0,26.91,101.95,17.00,518.00,0.209813,0.215891,0.228023,0.214922,null,null,null
-2020-09-02T23:33:19Z,26.62,60.70,99,0,25.76,101.95,17.00,518.00,0.210953,0.217633,0.229055,0.215188,null,null,null
-2020-09-02T23:33:49Z,26.64,60.67,99,0,25.50,101.95,17.00,518.00,0.211219,0.217164,0.228344,0.214766,null,null,null
-2020-09-02T23:34:19Z,26.62,60.67,99,0,27.73,101.95,17.00,518.00,0.210352,0.217117,0.228117,0.215672,null,null,null
-2020-09-02T23:34:49Z,26.61,60.73,99,0,26.87,101.95,17.00,518.00,0.209383,0.216578,0.228563,0.215344,null,null,null
-2020-09-02T23:35:19Z,26.62,60.73,99,0,26.16,101.95,17.00,518.00,0.211531,0.217016,0.229977,0.215867,null,null,null
-2020-09-02T23:35:49Z,26.64,60.70,99,0,26.00,101.95,17.00,518.00,0.209867,0.216859,0.228773,0.215758,null,null,null
-2020-09-02T23:36:19Z,26.64,60.70,99,0,25.73,101.95,17.00,518.00,0.209750,0.217914,0.228758,0.214641,null,null,null
-2020-09-02T23:36:49Z,26.62,60.69,99,0,27.73,101.95,17.00,518.00,0.209883,0.217937,0.229078,0.215508,null,null,null
-2020-09-02T23:37:19Z,26.62,60.68,99,0,29.11,101.95,17.00,518.00,0.210453,0.217469,0.227656,0.215211,null,null,null
-2020-09-02T23:37:49Z,26.64,60.71,99,0,26.41,101.95,17.00,518.00,0.209359,0.217414,0.228836,0.215805,null,null,null
-2020-09-02T23:38:19Z,26.64,60.68,99,0,25.00,101.95,17.00,518.00,0.208641,0.216016,0.227117,0.215586,null,null,null
-2020-09-02T23:38:49Z,26.64,60.73,99,0,27.75,101.95,17.00,518.00,0.210008,0.217430,0.227953,0.215234,null,null,null
-2020-09-02T23:39:19Z,26.61,60.69,99,0,25.16,101.95,17.00,518.00,0.208500,0.217195,0.227945,0.215687,null,null,null
-2020-09-02T23:39:49Z,26.62,60.67,99,0,26.26,101.95,17.00,518.00,0.208773,0.217945,0.228359,0.215578,null,null,null
-2020-09-02T23:40:19Z,26.64,60.70,99,0,24.76,101.95,17.00,518.00,0.210000,0.217477,0.227078,0.215602,null,null,null
-2020-09-02T23:40:49Z,26.64,60.68,99,0,28.92,101.94,17.00,518.00,0.210836,0.218242,0.228633,0.215219,null,null,null
-2020-09-02T23:41:19Z,26.62,60.66,99,0,25.50,101.95,18.00,523.00,0.209594,0.216703,0.227875,0.216297,null,null,null
-2020-09-02T23:41:49Z,26.62,60.69,99,0,26.95,101.95,18.00,523.00,0.209477,0.217633,0.228961,0.215773,null,null,null
-2020-09-02T23:42:19Z,26.62,60.68,99,0,25.29,101.95,17.00,518.00,0.210609,0.217664,0.226383,0.215023,null,null,null
-2020-09-02T23:42:49Z,26.61,60.68,99,0,28.06,101.94,17.00,518.00,0.209680,0.216172,0.229320,0.215234,null,null,null
-2020-09-02T23:43:19Z,26.62,60.74,99,0,27.55,101.94,17.00,518.00,0.210406,0.216711,0.229266,0.215625,null,null,null
-2020-09-02T23:43:49Z,26.62,60.62,99,0,26.71,101.94,17.00,518.00,0.209602,0.217547,0.228141,0.215914,null,null,null
-2020-09-02T23:44:19Z,26.64,60.69,99,0,28.81,101.95,17.00,518.00,0.210320,0.216500,0.229000,0.215820,null,null,null
-2020-09-02T23:44:49Z,26.61,60.66,99,0,27.06,101.94,17.00,518.00,0.209914,0.217523,0.228125,0.215250,null,null,null
-2020-09-02T23:45:19Z,26.62,60.66,99,0,27.96,101.95,17.00,518.00,0.209148,0.216813,0.227984,0.215508,null,null,null
-2020-09-02T23:45:49Z,26.62,60.72,99,0,25.95,101.94,17.00,518.00,0.209031,0.217937,0.227875,0.215820,null,null,null
-2020-09-02T23:46:19Z,26.62,60.72,99,0,27.04,101.95,17.00,518.00,0.209578,0.216344,0.228625,0.215875,null,null,null
-2020-09-02T23:46:49Z,26.62,60.71,99,0,26.82,101.95,17.00,518.00,0.209930,0.217500,0.229445,0.215320,null,null,null
-2020-09-02T23:47:19Z,26.61,60.71,99,0,26.67,101.95,17.00,518.00,0.209922,0.217820,0.229492,0.215648,null,null,null
-2020-09-02T23:47:49Z,26.62,60.69,99,0,26.87,101.95,17.00,518.00,0.211539,0.217023,0.227758,0.214992,null,null,null
-2020-09-02T23:48:19Z,26.61,60.71,99,0,26.53,101.95,17.00,518.00,0.209562,0.217375,0.228898,0.215977,null,null,null
-2020-09-02T23:48:49Z,26.61,60.69,99,0,23.63,101.95,17.00,518.00,0.210094,0.216867,0.229297,0.215883,null,null,null
-2020-09-02T23:49:19Z,26.62,60.73,99,0,26.53,101.94,17.00,518.00,0.211531,0.217328,0.229086,0.215188,null,null,null
-2020-09-02T23:49:49Z,26.59,60.72,99,0,28.93,101.95,17.00,518.00,0.210328,0.217547,0.227781,0.215164,null,null,null
-2020-09-02T23:50:19Z,26.59,60.74,99,0,26.06,101.94,17.00,518.00,0.208914,0.217703,0.230750,0.215945,null,null,null
-2020-09-02T23:50:49Z,26.62,60.75,99,0,27.14,101.95,17.00,518.00,0.210195,0.218141,0.228008,0.215000,null,null,null
-2020-09-02T23:51:19Z,26.61,60.71,99,0,29.23,101.94,17.00,518.00,0.208758,0.217406,0.228602,0.215969,null,null,null
-2020-09-02T23:51:49Z,26.62,60.71,99,0,24.83,101.95,17.00,518.00,0.209789,0.217125,0.228516,0.215516,null,null,null
-2020-09-02T23:52:19Z,26.59,60.71,99,0,27.66,101.94,18.00,523.00,0.210656,0.217844,0.227742,0.215438,null,null,null
-2020-09-02T23:52:49Z,26.62,60.66,99,0,24.89,101.95,18.00,523.00,0.210453,0.216953,0.227023,0.215562,null,null,null
-2020-09-02T23:53:19Z,26.61,60.69,99,0,28.92,101.95,17.00,518.00,0.211492,0.217609,0.229641,0.215477,null,null,null
-2020-09-02T23:53:49Z,26.61,60.75,99,0,27.02,101.95,17.00,518.00,0.210852,0.218242,0.228742,0.215164,null,null,null
-2020-09-02T23:54:19Z,26.62,60.70,99,0,27.68,101.94,17.00,518.00,0.209047,0.217453,0.227766,0.214945,null,null,null
-2020-09-02T23:54:49Z,26.59,60.74,99,0,26.38,101.95,17.00,518.00,0.209438,0.217094,0.226609,0.215023,null,null,null
-2020-09-02T23:55:19Z,26.59,60.75,99,0,27.44,101.95,16.00,508.00,0.209914,0.218141,0.229297,0.215164,null,null,null
-2020-09-02T23:55:49Z,26.61,60.71,99,0,25.59,101.95,16.00,508.00,0.210859,0.217109,0.227492,0.214930,null,null,null
-2020-09-02T23:56:19Z,26.62,60.74,99,0,25.76,101.95,18.00,523.00,0.209609,0.217148,0.227437,0.215297,null,null,null
-2020-09-02T23:56:49Z,26.61,60.74,99,0,25.98,101.95,18.00,523.00,0.209727,0.216992,0.226844,0.214813,null,null,null
-2020-09-02T23:57:19Z,26.62,60.76,99,0,28.27,101.94,15.00,502.00,0.209648,0.217109,0.227859,0.215273,null,null,null
-2020-09-02T23:57:49Z,26.61,60.70,99,0,25.44,101.95,15.00,502.00,0.208805,0.217336,0.228945,0.215937,null,null,null
-2020-09-02T23:58:19Z,26.62,60.70,99,0,29.31,101.94,16.00,508.00,0.210859,0.217805,0.229844,0.215578,null,null,null
-2020-09-02T23:58:49Z,26.61,60.76,99,0,27.14,101.94,16.00,508.00,0.209742,0.216555,0.227008,0.214469,null,null,null
-2020-09-02T23:59:19Z,26.61,60.72,99,0,25.92,101.94,17.00,518.00,0.210141,0.216867,0.229797,0.216234,null,null,null
+TIME,TEMP,HUM,BATT,LIGHT,NOISE_A,PRESS,CCS811_VOCS,CCS811_ECO2,ADC_48_0,ADC_48_1,ADC_48_2,ADC_48_3,PM_1,PM_25,PM_10
+ISO 8601,C,%,%,Lux,dBA,kPa,ppb,ppm,V,V,V,V,ug/m3,ug/m3,ug/m3
+Time,Temperature,Humidity,Battery,Light,Noise dBA,Barometric pressure,VOC Gas CCS811,eCO2 Gas CCS811,ADS1x15 ADC 0x48 Ch0,ADS1x15 ADC 0x48 Ch1,ADS1x15 ADC 0x48 Ch2,ADS1x15 ADC 0x48 Ch3,PM 1.0,PM 2.5,PM 10.0
+,55,56,10,14,53,58,113,112,0,0,0,0,89,87,88
+2020-09-02T15:35:19Z,26.92,61.17,-1,5,43.34,101.53,null,null,0.204281,0.212750,0.218586,0.209000,null,null,null
+2020-09-02T15:35:49Z,26.90,61.18,100,8,46.94,101.55,null,null,0.202578,0.212055,0.219797,0.208891,null,null,null
+2020-09-02T15:36:19Z,26.92,61.17,100,7,47.10,101.54,null,null,0.204656,0.212156,0.221180,0.210086,null,null,null
+2020-09-02T15:36:49Z,27.00,61.17,100,7,40.23,101.54,null,null,0.202375,0.211820,0.217867,0.208695,null,null,null
+2020-09-02T15:37:19Z,27.02,61.19,99,6,50.44,101.53,null,null,0.204305,0.214047,0.220977,0.209359,null,null,null
+2020-09-02T15:37:49Z,27.06,60.90,99,8,55.43,101.53,null,null,0.204508,0.213484,0.220422,0.209727,null,null,null
+2020-09-02T15:38:19Z,27.13,60.77,99,7,61.21,101.53,null,null,0.204820,0.213289,0.219609,0.209453,null,null,null
+2020-09-02T15:38:49Z,27.10,60.56,99,8,43.58,101.53,null,null,0.204367,0.212547,0.221062,0.208687,null,null,null
+2020-09-02T15:39:19Z,27.07,60.51,99,6,42.34,101.53,null,null,0.205031,0.213109,0.220453,0.209469,null,null,null
+2020-09-02T15:39:49Z,27.05,60.52,99,6,37.82,101.54,null,null,0.205609,0.213156,0.219805,0.209508,null,null,null
+2020-09-02T15:40:19Z,27.06,60.58,99,7,32.72,101.54,0.00,400.00,0.205016,0.212984,0.220570,0.209367,null,null,null
+2020-09-02T15:40:49Z,27.06,60.53,99,7,34.22,101.54,0.00,400.00,0.204414,0.213031,0.222000,0.209312,null,null,null
+2020-09-02T15:41:19Z,27.03,60.60,99,7,32.29,101.54,0.00,400.00,0.205383,0.213047,0.220727,0.209586,null,null,null
+2020-09-02T15:41:49Z,27.03,60.59,99,7,34.32,101.54,0.00,400.00,0.203547,0.212711,0.220375,0.209641,null,null,null
+2020-09-02T15:42:19Z,26.99,60.62,99,7,40.97,101.54,0.00,400.00,0.205852,0.212242,0.221188,0.209469,null,null,null
+2020-09-02T15:42:49Z,27.02,60.63,99,7,46.62,101.54,0.00,400.00,0.205102,0.212969,0.222883,0.209883,null,null,null
+2020-09-02T15:43:19Z,26.99,60.69,99,7,42.23,101.54,0.00,400.00,0.205695,0.213742,0.221531,0.209570,null,null,null
+2020-09-02T15:43:49Z,27.00,60.64,99,7,41.76,101.54,0.00,400.00,0.205141,0.213445,0.220516,0.209219,null,null,null
+2020-09-02T15:44:19Z,26.99,60.59,99,7,41.79,101.54,0.00,400.00,0.204203,0.212109,0.220719,0.209148,null,null,null
+2020-09-02T15:44:49Z,26.97,60.61,99,7,40.08,101.54,0.00,400.00,0.205586,0.213641,0.222227,0.210219,null,null,null
+2020-09-02T15:45:19Z,26.97,60.65,99,6,43.69,101.54,0.00,400.00,0.204383,0.214031,0.221844,0.209500,null,null,null
+2020-09-02T15:45:49Z,26.95,60.66,99,7,32.34,101.55,0.00,400.00,0.205406,0.213484,0.221477,0.210125,null,null,null
+2020-09-02T15:46:19Z,26.97,60.66,99,7,34.11,101.55,0.00,400.00,0.204430,0.212977,0.221914,0.210531,null,null,null
+2020-09-02T15:46:49Z,26.99,60.56,99,7,43.35,101.54,0.00,400.00,0.205375,0.212883,0.221539,0.210187,null,null,null
+2020-09-02T15:47:19Z,26.97,60.57,99,7,33.25,101.54,0.00,400.00,0.205734,0.213000,0.220844,0.211203,null,null,null
+2020-09-02T15:47:49Z,26.99,60.58,99,7,32.76,101.54,0.00,400.00,0.205445,0.214086,0.220055,0.210250,null,null,null
+2020-09-02T15:48:19Z,27.00,60.54,99,7,37.54,101.54,0.00,400.00,0.204984,0.213172,0.220219,0.209500,null,null,null
+2020-09-02T15:48:49Z,27.00,60.48,99,7,35.26,101.54,0.00,400.00,0.206883,0.213398,0.222523,0.210008,null,null,null
+2020-09-02T15:49:19Z,27.00,60.50,99,7,36.43,101.54,0.00,400.00,0.205828,0.213250,0.221758,0.209422,null,null,null
+2020-09-02T15:49:49Z,26.96,60.57,99,7,32.70,101.55,0.00,400.00,0.205359,0.212797,0.220406,0.209586,null,null,null
+2020-09-02T15:50:19Z,27.00,60.57,99,7,35.76,101.54,0.00,400.00,0.204961,0.213039,0.221594,0.209375,null,null,null
+2020-09-02T15:50:49Z,26.95,60.57,99,8,42.94,101.55,0.00,400.00,0.206383,0.213766,0.221234,0.210000,null,null,null
+2020-09-02T15:51:19Z,26.96,60.59,99,7,38.18,101.55,0.00,400.00,0.204117,0.212852,0.221930,0.210906,null,null,null
+2020-09-02T15:51:49Z,26.95,60.61,99,6,38.26,101.55,0.00,400.00,0.207234,0.213297,0.222516,0.211008,null,null,null
+2020-09-02T15:52:19Z,26.95,60.61,99,5,32.14,101.55,0.00,400.00,0.205336,0.212898,0.221781,0.210836,null,null,null
+2020-09-02T15:52:49Z,26.97,60.57,99,8,30.17,101.55,0.00,400.00,0.204727,0.212508,0.222797,0.210336,null,null,null
+2020-09-02T15:53:19Z,26.97,60.55,99,8,37.34,101.55,0.00,400.00,0.206938,0.212891,0.222500,0.210984,null,null,null
+2020-09-02T15:53:49Z,26.99,60.53,99,7,32.21,101.55,0.00,400.00,0.205258,0.212023,0.221672,0.211008,null,null,null
+2020-09-02T15:54:19Z,26.99,60.64,99,7,32.19,101.55,0.00,400.00,0.206125,0.214664,0.222227,0.210727,null,null,null
+2020-09-02T15:54:49Z,26.99,60.60,99,8,43.76,101.55,0.00,400.00,0.204906,0.213086,0.222469,0.210547,null,null,null
+2020-09-02T15:55:19Z,26.96,60.58,99,8,34.39,101.55,0.00,400.00,0.204617,0.212484,0.222930,0.211391,null,null,null
+2020-09-02T15:55:49Z,26.99,60.58,99,8,36.21,101.54,0.00,400.00,0.205656,0.213414,0.222344,0.210797,null,null,null
+2020-09-02T15:56:19Z,27.02,60.52,99,8,48.76,101.54,0.00,400.00,0.205133,0.212633,0.222352,0.210305,null,null,null
+2020-09-02T15:56:49Z,26.97,60.53,99,8,36.52,101.54,0.00,400.00,0.205109,0.212516,0.221766,0.210484,null,null,null
+2020-09-02T15:57:19Z,26.99,60.60,99,7,37.21,101.54,0.00,400.00,0.206148,0.213695,0.221531,0.211094,null,null,null
+2020-09-02T15:57:49Z,26.99,60.55,99,8,31.64,101.54,0.00,400.00,0.206313,0.212711,0.223742,0.210859,null,null,null
+2020-09-02T15:58:19Z,27.00,60.56,99,8,34.39,101.55,0.00,400.00,0.204586,0.212961,0.222344,0.210281,null,null,null
+2020-09-02T15:58:49Z,27.00,60.59,99,8,41.08,101.54,0.00,400.00,0.207320,0.214797,0.222914,0.209898,null,null,null
+2020-09-02T15:59:19Z,26.97,60.59,99,8,34.42,101.55,0.00,400.00,0.205398,0.212945,0.222797,0.210688,null,null,null
+2020-09-02T15:59:49Z,27.03,60.56,99,7,32.98,101.54,0.00,400.00,0.205836,0.214078,0.223273,0.210930,null,null,null
+2020-09-02T16:00:19Z,27.02,60.47,99,7,45.93,101.55,0.00,400.00,0.206547,0.213687,0.221992,0.210367,null,null,null
+2020-09-02T16:00:49Z,27.03,60.56,99,7,45.68,101.55,0.00,400.00,0.206117,0.213086,0.223102,0.210484,null,null,null
+2020-09-02T16:01:19Z,27.03,60.51,99,7,36.86,101.55,0.00,400.00,0.206289,0.212992,0.222922,0.210445,null,null,null
+2020-09-02T16:01:49Z,27.03,60.46,99,8,40.82,101.55,0.00,400.00,0.206078,0.213062,0.223320,0.211375,null,null,null
+2020-09-02T16:02:19Z,27.02,60.50,99,7,39.18,101.54,0.00,400.00,0.205875,0.213367,0.223180,0.211406,null,null,null
+2020-09-02T16:02:49Z,27.00,60.52,99,7,45.35,101.54,0.00,400.00,0.206047,0.214047,0.222969,0.210422,null,null,null
+2020-09-02T16:03:19Z,27.00,60.51,99,7,34.89,101.55,0.00,400.00,0.206711,0.213508,0.223648,0.211547,null,null,null
+2020-09-02T16:03:49Z,27.03,60.47,99,7,32.08,101.54,0.00,400.00,0.204516,0.213039,0.222047,0.210570,null,null,null
+2020-09-02T16:04:19Z,27.06,60.48,99,7,31.69,101.55,0.00,400.00,0.205422,0.213477,0.223508,0.210727,null,null,null
+2020-09-02T16:04:49Z,27.07,60.41,99,7,36.52,101.54,0.00,400.00,0.205445,0.212398,0.223117,0.211187,null,null,null
+2020-09-02T16:05:19Z,27.05,60.43,99,7,35.50,101.54,0.00,400.00,0.206125,0.212609,0.221875,0.211305,null,null,null
+2020-09-02T16:05:49Z,27.07,60.42,99,8,32.35,101.54,0.00,400.00,0.207102,0.214508,0.223023,0.211469,null,null,null
+2020-09-02T16:06:19Z,27.05,60.49,99,7,36.51,101.55,0.00,400.00,0.206742,0.213922,0.223125,0.209969,null,null,null
+2020-09-02T16:06:49Z,27.02,60.53,99,7,36.01,101.54,0.00,400.00,0.207289,0.214484,0.224398,0.211156,null,null,null
+2020-09-02T16:07:19Z,26.99,60.60,99,7,35.25,101.54,0.00,400.00,0.205820,0.213930,0.223703,0.211555,null,null,null
+2020-09-02T16:07:49Z,26.97,60.65,99,7,34.31,101.55,0.00,400.00,0.206648,0.213461,0.223125,0.211383,null,null,null
+2020-09-02T16:08:19Z,26.96,60.73,99,7,38.52,101.56,0.00,400.00,0.204992,0.212555,0.221437,0.210734,null,null,null
+2020-09-02T16:08:49Z,26.97,60.74,99,7,35.89,101.55,0.00,400.00,0.205734,0.213273,0.223063,0.211195,null,null,null
+2020-09-02T16:09:19Z,26.93,60.78,99,7,33.21,101.55,0.00,400.00,0.207563,0.213555,0.223133,0.210875,null,null,null
+2020-09-02T16:09:49Z,26.93,60.80,99,7,36.80,101.55,0.00,400.00,0.205469,0.213523,0.222320,0.211680,null,null,null
+2020-09-02T16:10:19Z,26.87,60.95,99,7,36.63,101.55,0.00,400.00,0.206687,0.213414,0.222430,0.210742,null,null,null
+2020-09-02T16:10:49Z,26.87,61.00,99,8,46.74,101.55,0.00,400.00,0.207016,0.214195,0.223289,0.211391,null,null,null
+2020-09-02T16:11:19Z,26.86,61.04,99,7,35.17,101.55,0.00,400.00,0.207609,0.214445,0.224172,0.211297,null,null,null
+2020-09-02T16:11:49Z,26.85,61.08,99,7,42.57,101.55,0.00,400.00,0.205437,0.215094,0.223805,0.211781,null,null,null
+2020-09-02T16:12:19Z,26.83,61.16,99,7,44.69,101.54,0.00,400.00,0.207391,0.213977,0.223180,0.211430,null,null,null
+2020-09-02T16:12:49Z,26.82,61.16,99,7,47.68,101.55,0.00,400.00,0.207133,0.213227,0.223523,0.211562,null,null,null
+2020-09-02T16:13:19Z,26.83,61.16,99,7,32.53,101.55,0.00,400.00,0.205820,0.214117,0.223766,0.211578,null,null,null
+2020-09-02T16:13:49Z,26.79,61.20,99,7,31.89,101.55,0.00,400.00,0.205664,0.214711,0.222969,0.211195,null,null,null
+2020-09-02T16:14:19Z,26.80,61.15,99,7,37.32,101.55,0.00,400.00,0.206281,0.214453,0.222570,0.211367,null,null,null
+2020-09-02T16:14:49Z,26.82,61.18,99,7,32.34,101.55,0.00,400.00,0.206930,0.213391,0.224461,0.211672,null,null,null
+2020-09-02T16:15:19Z,26.83,61.12,99,7,45.62,101.55,0.00,400.00,0.207438,0.214492,0.224328,0.211078,null,null,null
+2020-09-02T16:15:49Z,26.80,61.18,99,7,41.62,101.55,0.00,400.00,0.206062,0.214328,0.222820,0.211266,null,null,null
+2020-09-02T16:16:19Z,26.82,61.16,99,7,34.80,101.55,0.00,400.00,0.205984,0.214695,0.223203,0.211453,null,null,null
+2020-09-02T16:16:49Z,26.79,61.14,99,6,35.80,101.54,0.00,400.00,0.208359,0.214234,0.223711,0.211437,null,null,null
+2020-09-02T16:17:19Z,26.80,61.27,99,6,36.20,101.55,0.00,400.00,0.206930,0.213594,0.224242,0.212016,null,null,null
+2020-09-02T16:17:49Z,26.78,61.22,99,7,33.81,101.55,0.00,400.00,0.205547,0.213945,0.223125,0.211508,null,null,null
+2020-09-02T16:18:19Z,26.80,61.23,99,6,38.43,101.55,0.00,400.00,0.207672,0.214211,0.223344,0.211891,null,null,null
+2020-09-02T16:18:49Z,26.79,61.27,99,1,45.28,101.55,0.00,400.00,0.206477,0.214055,0.224125,0.211414,null,null,null
+2020-09-02T16:19:19Z,26.76,61.28,99,0,43.63,101.54,0.00,400.00,0.206469,0.213453,0.223391,0.211852,null,null,null
+2020-09-02T16:19:49Z,26.75,61.32,99,0,41.21,101.55,0.00,400.00,0.205992,0.213898,0.224203,0.211570,null,null,null
+2020-09-02T16:20:19Z,26.75,61.33,99,1,44.33,101.55,0.00,400.00,0.205758,0.213734,0.222344,0.211898,null,null,null
+2020-09-02T16:20:49Z,26.75,61.36,99,4,40.12,101.55,0.00,400.00,0.206813,0.214000,0.222297,0.211492,null,null,null
+2020-09-02T16:21:19Z,26.75,61.37,99,6,40.87,101.55,0.00,400.00,0.205852,0.214367,0.223797,0.211672,null,null,null
+2020-09-02T16:21:49Z,26.75,61.41,99,7,32.16,101.55,0.00,400.00,0.205320,0.213961,0.221609,0.210898,null,null,null
+2020-09-02T16:22:19Z,26.75,61.40,99,6,39.42,101.55,0.00,400.00,0.207672,0.214813,0.221852,0.212117,null,null,null
+2020-09-02T16:22:49Z,26.76,61.41,99,6,36.05,101.55,0.00,400.00,0.206008,0.214141,0.224672,0.211570,null,null,null
+2020-09-02T16:23:19Z,26.76,61.31,99,6,32.24,101.55,0.00,400.00,0.205016,0.213344,0.223203,0.211680,null,null,null
+2020-09-02T16:23:49Z,26.76,61.31,99,7,39.06,101.55,0.00,400.00,0.207695,0.214789,0.223805,0.211625,null,null,null
+2020-09-02T16:24:19Z,26.78,61.33,99,7,35.99,101.54,0.00,400.00,0.207047,0.214836,0.224828,0.211477,null,null,null
+2020-09-02T16:24:49Z,26.75,61.37,99,8,40.18,101.55,0.00,400.00,0.205586,0.212586,0.223281,0.212070,null,null,null
+2020-09-02T16:25:19Z,26.75,61.36,99,7,40.32,101.54,0.00,400.00,0.206703,0.215062,0.224242,0.211539,null,null,null
+2020-09-02T16:25:49Z,26.76,61.35,99,7,39.47,101.54,0.00,400.00,0.207305,0.214164,0.224664,0.212141,null,null,null
+2020-09-02T16:26:19Z,26.78,61.34,99,2,59.45,101.55,0.00,400.00,0.206602,0.214422,0.224352,0.212078,null,null,null
+2020-09-02T16:26:49Z,26.80,61.31,99,6,46.54,101.55,0.00,400.00,0.207609,0.215031,0.224180,0.212102,null,null,null
+2020-09-02T16:27:19Z,26.79,61.22,99,7,46.24,101.55,0.00,400.00,0.206320,0.213844,0.224227,0.212094,null,null,null
+2020-09-02T16:27:49Z,26.76,61.28,99,7,43.74,101.55,0.00,400.00,0.209039,0.216055,0.224859,0.211500,null,null,null
+2020-09-02T16:28:19Z,26.78,61.31,99,6,46.79,101.55,0.00,402.00,0.207641,0.214789,0.223727,0.211203,null,null,null
+2020-09-02T16:28:49Z,26.80,61.30,99,6,43.63,101.55,0.00,402.00,0.206953,0.214203,0.224023,0.212062,null,null,null
+2020-09-02T16:29:19Z,26.76,61.28,99,5,35.82,101.55,0.00,400.00,0.206859,0.214570,0.222891,0.211195,null,null,null
+2020-09-02T16:29:49Z,26.79,61.31,99,5,41.48,101.55,0.00,400.00,0.206852,0.214547,0.224055,0.212008,null,null,null
+2020-09-02T16:30:19Z,26.75,61.35,99,7,44.71,101.55,0.00,400.00,0.205484,0.213828,0.225242,0.212727,null,null,null
+2020-09-02T16:30:49Z,26.78,61.35,99,5,45.54,101.55,0.00,400.00,0.205508,0.213180,0.224031,0.211352,null,null,null
+2020-09-02T16:31:19Z,26.79,61.35,99,7,45.54,101.55,0.00,400.00,0.207469,0.213523,0.223875,0.211805,null,null,null
+2020-09-02T16:31:49Z,26.78,61.41,99,6,56.88,101.55,0.00,400.00,0.207703,0.214992,0.222477,0.211820,null,null,null
+2020-09-02T16:32:19Z,26.76,61.36,99,6,43.66,101.54,0.00,400.00,0.206664,0.213047,0.223742,0.212445,null,null,null
+2020-09-02T16:32:49Z,26.78,61.38,99,6,56.30,101.55,0.00,400.00,0.206516,0.212938,0.223891,0.211516,null,null,null
+2020-09-02T16:33:19Z,26.78,61.41,99,5,53.03,101.54,0.00,400.00,0.206992,0.214039,0.223867,0.212344,null,null,null
+2020-09-02T16:33:49Z,26.79,61.42,99,5,52.41,101.55,0.00,400.00,0.207719,0.214008,0.224258,0.211375,null,null,null
+2020-09-02T16:34:19Z,26.76,61.41,99,5,43.36,101.55,0.00,400.00,0.206750,0.215180,0.224078,0.212000,null,null,null
+2020-09-02T16:34:49Z,26.78,61.41,99,5,51.47,101.54,0.00,400.00,0.207023,0.214602,0.222633,0.212039,null,null,null
+2020-09-02T16:35:19Z,26.76,61.42,99,5,53.53,101.55,0.00,400.00,0.205953,0.213906,0.225008,0.211875,null,null,null
+2020-09-02T16:35:49Z,26.80,61.42,99,5,46.54,101.55,0.00,400.00,0.206281,0.213094,0.226086,0.212117,null,null,null
+2020-09-02T16:36:19Z,26.78,61.43,99,6,34.88,101.55,0.00,400.00,0.206578,0.214500,0.224703,0.212031,null,null,null
+2020-09-02T16:36:49Z,26.75,61.36,99,5,65.30,101.55,0.00,400.00,0.207359,0.214445,0.223805,0.212047,null,null,null
+2020-09-02T16:37:19Z,26.82,61.37,99,5,46.50,101.55,0.00,400.00,0.206766,0.214336,0.224883,0.212305,null,null,null
+2020-09-02T16:37:49Z,26.79,61.35,99,4,34.38,101.55,0.00,400.00,0.208000,0.214156,0.223797,0.213313,null,null,null
+2020-09-02T16:38:19Z,26.78,61.39,99,5,48.38,101.55,0.00,400.00,0.205398,0.213492,0.224906,0.213117,null,null,null
+2020-09-02T16:38:49Z,26.75,61.42,99,6,34.31,101.55,0.00,400.00,0.207773,0.214586,0.223102,0.212688,null,null,null
+2020-09-02T16:39:19Z,26.75,61.43,99,5,50.82,101.55,0.00,400.00,0.208859,0.215453,0.225828,0.212836,null,null,null
+2020-09-02T16:39:49Z,26.78,61.45,99,7,47.49,101.55,0.00,400.00,0.207188,0.213484,0.224836,0.211977,null,null,null
+2020-09-02T16:40:19Z,26.76,61.45,99,6,46.84,101.55,0.00,400.00,0.206727,0.214508,0.223656,0.212164,null,null,null
+2020-09-02T16:40:49Z,26.79,61.45,99,5,48.08,101.55,0.00,400.00,0.208398,0.214859,0.224211,0.212328,null,null,null
+2020-09-02T16:41:19Z,26.78,61.47,99,5,48.27,101.55,0.00,400.00,0.205586,0.214328,0.224258,0.212211,null,null,null
+2020-09-02T16:41:49Z,26.80,61.43,99,5,35.00,101.55,0.00,400.00,0.206742,0.213648,0.224172,0.211906,null,null,null
+2020-09-02T16:42:19Z,26.78,61.45,99,6,51.34,101.55,0.00,400.00,0.207219,0.215109,0.223820,0.212094,null,null,null
+2020-09-02T16:42:49Z,26.79,61.43,99,7,59.59,101.55,0.00,400.00,0.206422,0.213898,0.223500,0.211391,null,null,null
+2020-09-02T16:43:19Z,26.79,61.38,99,6,53.25,101.55,0.00,400.00,0.206484,0.213695,0.223320,0.212234,null,null,null
+2020-09-02T16:43:49Z,26.76,61.39,99,5,51.15,101.55,0.00,400.00,0.207797,0.214617,0.224539,0.212711,null,null,null
+2020-09-02T16:44:19Z,26.78,61.44,99,6,61.55,101.55,0.00,400.00,0.207305,0.215000,0.225336,0.212219,null,null,null
+2020-09-02T16:44:49Z,26.78,61.46,99,7,55.02,101.55,0.00,400.00,0.207531,0.214461,0.223234,0.211562,null,null,null
+2020-09-02T16:45:19Z,26.79,61.46,99,6,54.41,101.55,0.00,400.00,0.206820,0.214336,0.224805,0.212578,null,null,null
+2020-09-02T16:45:49Z,26.78,61.38,99,5,44.06,101.55,0.00,400.00,0.207352,0.214844,0.225031,0.212148,null,null,null
+2020-09-02T16:46:19Z,26.76,61.41,99,5,45.74,101.55,1.00,408.00,0.206211,0.213234,0.224695,0.212711,null,null,null
+2020-09-02T16:46:49Z,26.78,61.40,99,5,43.05,101.55,1.00,408.00,0.206156,0.215219,0.224086,0.212523,null,null,null
+2020-09-02T16:47:19Z,26.78,61.36,99,7,46.29,101.55,0.00,403.00,0.208367,0.215367,0.223906,0.212164,null,null,null
+2020-09-02T16:47:49Z,26.76,61.37,99,6,38.83,101.55,0.00,403.00,0.207602,0.213984,0.226141,0.212297,null,null,null
+2020-09-02T16:48:19Z,26.80,61.46,99,6,49.41,101.56,1.00,408.00,0.208641,0.215797,0.224578,0.212383,null,null,null
+2020-09-02T16:48:49Z,26.76,61.42,99,7,54.37,101.56,1.00,408.00,0.207320,0.215383,0.225570,0.213031,null,null,null
+2020-09-02T16:49:19Z,26.78,61.42,99,7,38.22,101.56,0.00,400.00,0.207773,0.215164,0.224750,0.212375,null,null,null
+2020-09-02T16:49:49Z,26.78,61.40,99,5,48.10,101.55,0.00,400.00,0.207055,0.214469,0.225086,0.212930,null,null,null
+2020-09-02T16:50:19Z,26.80,61.41,99,6,47.12,101.56,0.00,400.00,0.206586,0.214000,0.226313,0.212727,null,null,null
+2020-09-02T16:50:49Z,26.78,61.43,99,6,39.72,101.56,0.00,400.00,0.208609,0.214609,0.223703,0.211812,null,null,null
+2020-09-02T16:51:19Z,26.80,61.43,99,5,32.02,101.56,0.00,400.00,0.208852,0.215758,0.223945,0.212617,null,null,null
+2020-09-02T16:51:49Z,26.82,61.39,99,7,50.12,101.56,0.00,400.00,0.207805,0.216219,0.225094,0.212555,null,null,null
+2020-09-02T16:52:19Z,26.82,61.37,99,7,40.76,101.56,0.00,400.00,0.207328,0.214469,0.224203,0.211898,null,null,null
+2020-09-02T16:52:49Z,26.80,61.40,99,5,32.03,101.56,0.00,400.00,0.206922,0.214133,0.226516,0.213156,null,null,null
+2020-09-02T16:53:19Z,26.79,61.39,99,5,47.70,101.56,0.00,400.00,0.205969,0.213117,0.224906,0.213055,null,null,null
+2020-09-02T16:53:49Z,26.82,61.39,99,6,34.54,101.56,0.00,400.00,0.207937,0.214273,0.224992,0.212563,null,null,null
+2020-09-02T16:54:19Z,26.78,61.41,99,11,44.06,101.56,0.00,400.00,0.209273,0.215672,0.224336,0.211969,null,null,null
+2020-09-02T16:54:49Z,26.79,61.40,99,5,46.32,101.56,0.00,400.00,0.207891,0.215250,0.223969,0.212836,null,null,null
+2020-09-02T16:55:19Z,26.79,61.41,99,5,43.35,101.56,0.00,400.00,0.206594,0.213719,0.225914,0.212344,null,null,null
+2020-09-02T16:55:49Z,26.79,61.41,99,6,42.66,101.55,0.00,400.00,0.208258,0.215445,0.225977,0.212969,null,null,null
+2020-09-02T16:56:19Z,26.79,61.39,99,7,34.32,101.56,0.00,400.00,0.207937,0.214820,0.225680,0.212367,null,null,null
+2020-09-02T16:56:49Z,26.80,61.39,99,6,34.39,101.56,0.00,400.00,0.206648,0.214336,0.224789,0.212453,null,null,null
+2020-09-02T16:57:19Z,26.82,61.39,99,5,39.51,101.56,0.00,400.00,0.207695,0.215461,0.224430,0.212563,null,null,null
+2020-09-02T16:57:49Z,26.80,61.37,99,6,30.78,101.56,0.00,400.00,0.206250,0.214492,0.224578,0.212461,null,null,null
+2020-09-02T16:58:19Z,26.80,61.38,99,5,34.31,101.56,0.00,400.00,0.207297,0.214250,0.223734,0.212477,null,null,null
+2020-09-02T16:58:49Z,26.80,61.34,99,5,33.83,101.56,0.00,400.00,0.206297,0.213625,0.226031,0.212625,null,null,null
+2020-09-02T16:59:19Z,26.80,61.37,99,6,34.66,101.56,0.00,400.00,0.207500,0.214289,0.226539,0.213430,null,null,null
+2020-09-02T16:59:49Z,26.80,61.33,99,6,35.41,101.56,0.00,400.00,0.206578,0.214547,0.225102,0.212742,null,null,null
+2020-09-02T17:00:19Z,26.78,61.37,99,5,28.19,101.56,0.00,400.00,0.207625,0.214445,0.223641,0.212352,null,null,null
+2020-09-02T17:00:49Z,26.79,61.37,99,5,33.32,101.56,0.00,400.00,0.207430,0.215664,0.224883,0.212625,null,null,null
+2020-09-02T17:01:19Z,26.79,61.32,99,5,30.39,101.56,0.00,400.00,0.206867,0.214656,0.224719,0.212437,null,null,null
+2020-09-02T17:01:49Z,26.79,61.32,99,3,36.65,101.56,0.00,400.00,0.207539,0.214023,0.225898,0.212711,null,null,null
+2020-09-02T17:02:19Z,26.80,61.28,99,3,39.84,101.56,0.00,400.00,0.207164,0.214500,0.224578,0.213398,null,null,null
+2020-09-02T17:02:49Z,26.82,61.33,99,5,36.84,101.56,0.00,400.00,0.208219,0.215352,0.224742,0.212859,null,null,null
+2020-09-02T17:03:19Z,26.79,61.33,99,2,39.69,101.56,0.00,400.00,0.206375,0.213859,0.224219,0.212672,null,null,null
+2020-09-02T17:03:49Z,26.80,61.29,99,2,38.25,101.56,0.00,400.00,0.206648,0.214117,0.226453,0.212969,null,null,null
+2020-09-02T17:04:19Z,26.82,61.32,99,1,32.85,101.56,0.00,400.00,0.207672,0.214719,0.225938,0.212609,null,null,null
+2020-09-02T17:04:49Z,26.80,61.29,99,1,33.37,101.56,0.00,400.00,0.206445,0.215312,0.224758,0.212484,null,null,null
+2020-09-02T17:05:19Z,26.85,61.30,99,0,28.27,101.56,0.00,400.00,0.206352,0.213633,0.224727,0.213109,null,null,null
+2020-09-02T17:05:49Z,26.82,61.33,99,0,34.98,101.57,0.00,400.00,0.206633,0.214422,0.224797,0.212570,null,null,null
+2020-09-02T17:06:19Z,26.82,61.34,99,0,35.85,101.56,0.00,400.00,0.207031,0.214281,0.226344,0.212852,null,null,null
+2020-09-02T17:06:49Z,26.82,61.33,99,0,38.67,101.56,0.00,400.00,0.207961,0.215492,0.226727,0.213148,null,null,null
+2020-09-02T17:07:19Z,26.80,61.31,99,0,37.07,101.56,0.00,400.00,0.207680,0.214039,0.224375,0.213039,null,null,null
+2020-09-02T17:07:49Z,26.80,61.34,99,0,30.61,101.56,0.00,400.00,0.207180,0.215070,0.225367,0.212367,null,null,null
+2020-09-02T17:08:19Z,26.82,61.29,99,0,38.02,101.56,0.00,400.00,0.206391,0.213844,0.225328,0.212437,null,null,null
+2020-09-02T17:08:49Z,26.79,61.31,99,0,31.37,101.56,0.00,400.00,0.207438,0.213516,0.226172,0.213125,null,null,null
+2020-09-02T17:09:19Z,26.80,61.37,99,0,29.62,101.57,0.00,402.00,0.207156,0.215523,0.224172,0.212820,null,null,null
+2020-09-02T17:09:49Z,26.80,61.38,99,0,31.27,101.56,0.00,402.00,0.209031,0.214883,0.223305,0.212711,null,null,null
+2020-09-02T17:10:19Z,26.80,61.36,99,0,29.51,101.56,0.00,400.00,0.207000,0.214344,0.226164,0.212883,null,null,null
+2020-09-02T17:10:49Z,26.83,61.31,99,0,29.40,101.57,0.00,400.00,0.206687,0.214961,0.226812,0.213250,null,null,null
+2020-09-02T17:11:19Z,26.82,61.30,99,0,36.35,101.57,0.00,400.00,0.208094,0.214586,0.224703,0.212531,null,null,null
+2020-09-02T17:11:49Z,26.85,61.26,99,0,32.61,101.57,0.00,400.00,0.206211,0.214477,0.225570,0.211906,null,null,null
+2020-09-02T17:12:19Z,26.82,61.24,99,0,33.21,101.57,0.00,400.00,0.206820,0.215023,0.225984,0.213922,null,null,null
+2020-09-02T17:12:49Z,26.82,61.21,99,0,29.61,101.57,0.00,400.00,0.208477,0.214820,0.225648,0.212555,null,null,null
+2020-09-02T17:13:19Z,26.83,61.26,99,0,42.91,101.57,0.00,400.00,0.208016,0.214961,0.226070,0.213828,null,null,null
+2020-09-02T17:13:49Z,26.80,61.28,99,0,41.18,101.57,0.00,400.00,0.208328,0.214945,0.226492,0.213047,null,null,null
+2020-09-02T17:14:19Z,26.78,61.31,99,0,43.03,101.57,0.00,400.00,0.207469,0.215141,0.226500,0.212641,null,null,null
+2020-09-02T17:14:49Z,26.83,61.28,99,0,43.33,101.57,0.00,400.00,0.205742,0.212578,0.224055,0.213188,null,null,null
+2020-09-02T17:15:19Z,26.80,61.20,99,0,41.11,101.57,0.00,400.00,0.208203,0.214227,0.224867,0.212961,null,null,null
+2020-09-02T17:15:49Z,26.79,61.27,99,0,30.39,101.57,0.00,400.00,0.207789,0.215219,0.225117,0.213117,null,null,null
+2020-09-02T17:16:19Z,26.79,61.27,99,0,36.02,101.57,0.00,401.00,0.207438,0.215047,0.225133,0.212414,null,null,null
+2020-09-02T17:16:49Z,26.80,61.27,99,0,29.92,101.57,0.00,401.00,0.209359,0.215578,0.226820,0.212984,null,null,null
+2020-09-02T17:17:19Z,26.80,61.24,99,0,36.32,101.57,0.00,401.00,0.206336,0.215016,0.225812,0.213211,null,null,null
+2020-09-02T17:17:49Z,26.80,61.22,99,0,35.67,101.57,0.00,401.00,0.207609,0.214648,0.225125,0.212867,null,null,null
+2020-09-02T17:18:19Z,26.80,61.21,99,0,32.17,101.57,0.00,400.00,0.207242,0.214820,0.224914,0.213305,null,null,null
+2020-09-02T17:18:49Z,26.82,61.21,99,0,31.75,101.57,0.00,400.00,0.206938,0.214094,0.224031,0.213023,null,null,null
+2020-09-02T17:19:19Z,26.78,61.18,99,0,40.38,101.57,0.00,405.00,0.207727,0.214953,0.225906,0.213195,null,null,null
+2020-09-02T17:19:49Z,26.80,61.18,99,0,31.25,101.57,0.00,405.00,0.207297,0.214617,0.226156,0.213406,null,null,null
+2020-09-02T17:20:19Z,26.78,61.15,99,0,38.03,101.57,0.00,405.00,0.208445,0.214695,0.225328,0.212898,null,null,null
+2020-09-02T17:20:49Z,26.80,61.21,99,0,32.58,101.57,0.00,405.00,0.206430,0.213727,0.225602,0.212633,null,null,null
+2020-09-02T17:21:19Z,26.79,61.15,99,0,41.62,101.57,0.00,402.00,0.207336,0.214969,0.226250,0.213156,null,null,null
+2020-09-02T17:21:49Z,26.82,61.15,99,0,29.18,101.57,0.00,402.00,0.205812,0.213859,0.226742,0.213500,null,null,null
+2020-09-02T17:22:19Z,26.79,61.14,99,0,31.99,101.57,0.00,400.00,0.208039,0.214164,0.224547,0.213305,null,null,null
+2020-09-02T17:22:49Z,26.79,61.15,99,0,44.61,101.57,0.00,400.00,0.207211,0.215258,0.226445,0.213117,null,null,null
+2020-09-02T17:23:19Z,26.82,61.18,99,0,29.50,101.57,0.00,400.00,0.208937,0.216547,0.225172,0.212922,null,null,null
+2020-09-02T17:23:49Z,26.80,61.15,99,0,33.33,101.57,0.00,400.00,0.206695,0.215125,0.224625,0.212555,null,null,null
+2020-09-02T17:24:19Z,26.79,61.11,99,0,36.83,101.57,0.00,400.00,0.207914,0.214547,0.225984,0.212883,null,null,null
+2020-09-02T17:24:49Z,26.79,61.13,99,0,30.81,101.57,0.00,400.00,0.207391,0.215375,0.225789,0.213109,null,null,null
+2020-09-02T17:25:19Z,26.80,61.12,99,0,29.84,101.57,0.00,400.00,0.207805,0.214430,0.224906,0.212852,null,null,null
+2020-09-02T17:25:49Z,26.79,61.17,99,0,37.42,101.57,0.00,400.00,0.208203,0.215703,0.225734,0.213227,null,null,null
+2020-09-02T17:26:19Z,26.82,61.20,99,0,31.45,101.57,0.00,400.00,0.206477,0.214359,0.226523,0.213570,null,null,null
+2020-09-02T17:26:49Z,26.80,61.15,99,0,30.40,101.57,0.00,400.00,0.206437,0.214586,0.227227,0.213367,null,null,null
+2020-09-02T17:27:19Z,26.82,61.08,99,0,35.69,101.57,0.00,400.00,0.207172,0.215352,0.225313,0.213094,null,null,null
+2020-09-02T17:27:49Z,26.82,61.10,99,0,31.87,101.57,0.00,400.00,0.208070,0.214516,0.227023,0.213719,null,null,null
+2020-09-02T17:28:19Z,26.83,61.08,99,0,32.04,101.57,0.00,400.00,0.207203,0.215719,0.225180,0.212648,null,null,null
+2020-09-02T17:28:49Z,26.82,61.15,99,0,33.93,101.57,0.00,400.00,0.206672,0.214234,0.224414,0.212617,null,null,null
+2020-09-02T17:29:19Z,26.85,61.15,99,0,43.52,101.57,0.00,400.00,0.208273,0.215297,0.224484,0.212656,null,null,null
+2020-09-02T17:29:49Z,26.83,61.09,99,0,37.06,101.57,0.00,400.00,0.208102,0.215359,0.225805,0.213477,null,null,null
+2020-09-02T17:30:19Z,26.79,61.14,99,0,40.34,101.57,0.00,400.00,0.208469,0.215320,0.227023,0.213234,null,null,null
+2020-09-02T17:30:49Z,26.82,61.13,99,0,42.09,101.57,0.00,400.00,0.207797,0.214680,0.224344,0.213211,null,null,null
+2020-09-02T17:31:19Z,26.79,61.12,99,0,29.60,101.57,0.00,400.00,0.207219,0.215008,0.227078,0.213750,null,null,null
+2020-09-02T17:31:49Z,26.82,61.13,99,0,34.32,101.57,0.00,400.00,0.206805,0.214695,0.226555,0.213117,null,null,null
+2020-09-02T17:32:19Z,26.80,60.99,99,0,42.81,101.57,0.00,400.00,0.207398,0.214031,0.226453,0.213094,null,null,null
+2020-09-02T17:32:49Z,26.85,60.99,99,0,34.25,101.58,0.00,400.00,0.208008,0.215836,0.226562,0.213969,null,null,null
+2020-09-02T17:33:19Z,26.82,61.00,99,0,34.73,101.57,0.00,400.00,0.207828,0.215539,0.224977,0.212836,null,null,null
+2020-09-02T17:33:49Z,26.85,61.05,99,0,36.24,101.58,0.00,400.00,0.209148,0.215375,0.224445,0.212453,null,null,null
+2020-09-02T17:34:19Z,26.85,61.08,99,0,34.10,101.58,0.00,400.00,0.206523,0.215633,0.224898,0.212664,null,null,null
+2020-09-02T17:34:49Z,26.83,61.04,99,0,32.62,101.58,0.00,400.00,0.207820,0.215023,0.226039,0.213086,null,null,null
+2020-09-02T17:35:19Z,26.82,61.07,99,0,32.95,101.58,0.00,400.00,0.208031,0.215641,0.223375,0.212648,null,null,null
+2020-09-02T17:35:49Z,26.85,61.09,99,0,33.98,101.58,0.00,400.00,0.208555,0.215687,0.225195,0.213344,null,null,null
+2020-09-02T17:36:19Z,26.85,61.07,99,0,30.12,101.58,0.00,400.00,0.207297,0.215039,0.224789,0.213172,null,null,null
+2020-09-02T17:36:49Z,26.82,61.12,99,0,28.95,101.58,0.00,400.00,0.206867,0.214625,0.224875,0.213484,null,null,null
+2020-09-02T17:37:19Z,26.83,61.07,99,0,32.12,101.58,0.00,400.00,0.207930,0.214156,0.226383,0.213789,null,null,null
+2020-09-02T17:37:49Z,26.83,61.05,99,0,35.35,101.58,0.00,400.00,0.207297,0.214711,0.225391,0.213367,null,null,null
+2020-09-02T17:38:19Z,26.83,61.06,99,0,33.84,101.58,0.00,400.00,0.208477,0.215180,0.226562,0.213336,null,null,null
+2020-09-02T17:38:49Z,26.85,60.99,99,0,37.91,101.59,0.00,400.00,0.207633,0.215625,0.226664,0.213656,null,null,null
+2020-09-02T17:39:19Z,26.85,61.07,99,0,43.89,101.58,0.00,400.00,0.207828,0.215562,0.224906,0.213344,null,null,null
+2020-09-02T17:39:49Z,26.83,61.06,99,0,42.91,101.58,0.00,400.00,0.207914,0.214680,0.227258,0.213211,null,null,null
+2020-09-02T17:40:19Z,26.83,61.10,99,0,33.79,101.58,0.00,400.00,0.208562,0.216000,0.227531,0.214320,null,null,null
+2020-09-02T17:40:49Z,26.86,61.05,99,0,31.88,101.59,0.00,400.00,0.208992,0.215375,0.225039,0.213617,null,null,null
+2020-09-02T17:41:19Z,26.85,61.02,99,0,34.28,101.59,0.00,400.00,0.207523,0.215930,0.226875,0.213266,null,null,null
+2020-09-02T17:41:49Z,26.86,61.01,99,0,33.50,101.59,0.00,400.00,0.208242,0.215047,0.227148,0.214398,null,null,null
+2020-09-02T17:42:19Z,26.83,61.06,99,0,29.00,101.59,0.00,400.00,0.207320,0.215672,0.225102,0.212563,null,null,null
+2020-09-02T17:42:49Z,26.83,61.07,99,0,30.12,101.59,0.00,400.00,0.207125,0.215648,0.226063,0.213820,null,null,null
+2020-09-02T17:43:19Z,26.83,61.03,99,0,29.49,101.59,0.00,400.00,0.207336,0.214719,0.227195,0.214188,null,null,null
+2020-09-02T17:43:49Z,26.85,61.04,99,0,44.31,101.59,0.00,400.00,0.206977,0.214227,0.225695,0.213695,null,null,null
+2020-09-02T17:44:19Z,26.83,61.02,99,0,31.26,101.60,0.00,400.00,0.208461,0.215945,0.226203,0.213570,null,null,null
+2020-09-02T17:44:49Z,26.82,61.08,99,0,33.97,101.59,0.00,400.00,0.207609,0.214680,0.226430,0.212859,null,null,null
+2020-09-02T17:45:19Z,26.83,61.11,99,0,39.32,101.60,0.00,400.00,0.207164,0.214086,0.223922,0.212602,null,null,null
+2020-09-02T17:45:49Z,26.82,61.10,99,0,28.84,101.60,0.00,400.00,0.208148,0.215562,0.226313,0.213766,null,null,null
+2020-09-02T17:46:19Z,26.83,61.13,99,0,31.38,101.59,0.00,400.00,0.209219,0.216477,0.225461,0.213250,null,null,null
+2020-09-02T17:46:49Z,26.83,61.16,99,0,32.88,101.60,0.00,400.00,0.207563,0.214914,0.225438,0.214102,null,null,null
+2020-09-02T17:47:19Z,26.83,61.13,99,0,31.17,101.60,0.00,400.00,0.208469,0.215414,0.225305,0.213469,null,null,null
+2020-09-02T17:47:49Z,26.82,61.15,99,0,32.94,101.60,0.00,400.00,0.208312,0.214789,0.226484,0.213141,null,null,null
+2020-09-02T17:48:19Z,26.83,61.14,99,0,31.19,101.60,0.00,400.00,0.207297,0.215547,0.226523,0.214016,null,null,null
+2020-09-02T17:48:49Z,26.83,61.19,99,0,54.83,101.60,0.00,400.00,0.207125,0.214742,0.225156,0.214203,null,null,null
+2020-09-02T17:49:19Z,26.82,61.14,99,0,30.29,101.61,0.00,400.00,0.208383,0.216188,0.225477,0.213758,null,null,null
+2020-09-02T17:49:49Z,26.82,61.16,99,0,31.22,101.61,0.00,400.00,0.208242,0.216039,0.225266,0.213188,null,null,null
+2020-09-02T17:50:19Z,26.80,61.16,99,0,42.41,101.61,0.00,400.00,0.206961,0.214297,0.227336,0.213930,null,null,null
+2020-09-02T17:50:49Z,26.83,61.20,99,0,41.23,101.61,0.00,400.00,0.208117,0.215891,0.227539,0.213500,null,null,null
+2020-09-02T17:51:19Z,26.80,61.16,99,0,34.44,101.61,0.00,400.00,0.206086,0.214273,0.224820,0.212812,null,null,null
+2020-09-02T17:51:49Z,26.82,61.20,99,0,29.99,101.61,0.00,400.00,0.206734,0.215133,0.225102,0.213625,null,null,null
+2020-09-02T17:52:19Z,26.80,61.20,99,0,31.04,101.61,0.00,400.00,0.207594,0.214844,0.226750,0.213242,null,null,null
+2020-09-02T17:52:49Z,26.80,61.18,99,0,31.11,101.61,0.00,400.00,0.209164,0.215289,0.225453,0.213305,null,null,null
+2020-09-02T17:53:19Z,26.80,61.20,99,0,33.92,101.61,0.00,400.00,0.208508,0.214977,0.226141,0.213523,null,null,null
+2020-09-02T17:53:49Z,26.82,61.20,99,0,31.50,101.61,0.00,400.00,0.209414,0.216289,0.226586,0.213383,null,null,null
+2020-09-02T17:54:19Z,26.78,61.19,99,0,34.70,101.61,0.00,400.00,0.208727,0.216258,0.225695,0.213508,null,null,null
+2020-09-02T17:54:49Z,26.79,61.21,99,0,38.10,101.61,0.00,400.00,0.208438,0.215266,0.226523,0.214234,null,null,null
+2020-09-02T17:55:19Z,26.79,61.27,99,0,31.31,101.61,0.00,400.00,0.207766,0.215102,0.227242,0.213273,null,null,null
+2020-09-02T17:55:49Z,26.80,61.23,99,0,28.57,101.61,0.00,400.00,0.207312,0.215086,0.226367,0.213734,null,null,null
+2020-09-02T17:56:19Z,26.80,61.27,99,0,38.48,101.61,0.00,400.00,0.206273,0.214898,0.225859,0.212992,null,null,null
+2020-09-02T17:56:49Z,26.82,61.23,99,0,28.91,101.61,0.00,400.00,0.207320,0.214898,0.225812,0.213867,null,null,null
+2020-09-02T17:57:19Z,26.79,61.24,99,0,31.91,101.61,0.00,400.00,0.208906,0.215352,0.225930,0.214086,null,null,null
+2020-09-02T17:57:49Z,26.79,61.24,99,0,29.27,101.61,0.00,400.00,0.209273,0.215547,0.226656,0.213781,null,null,null
+2020-09-02T17:58:19Z,26.80,61.22,99,0,30.29,101.61,0.00,400.00,0.207945,0.215062,0.226000,0.213766,null,null,null
+2020-09-02T17:58:49Z,26.80,61.22,99,0,29.99,101.62,0.00,400.00,0.208750,0.215805,0.226633,0.213461,null,null,null
+2020-09-02T17:59:19Z,26.78,61.20,99,0,30.26,101.61,0.00,400.00,0.207391,0.215125,0.226633,0.213820,null,null,null
+2020-09-02T17:59:49Z,26.79,61.25,99,0,34.72,101.61,0.00,400.00,0.208008,0.215148,0.226562,0.213680,null,null,null
+2020-09-02T18:00:19Z,26.79,61.28,99,0,31.31,101.61,0.00,400.00,0.205984,0.214539,0.227500,0.213695,null,null,null
+2020-09-02T18:00:49Z,26.78,61.29,99,0,27.02,101.62,0.00,400.00,0.205453,0.214266,0.225539,0.213867,null,null,null
+2020-09-02T18:01:19Z,26.80,61.27,99,0,29.32,101.62,0.00,400.00,0.209055,0.216070,0.226313,0.212906,null,null,null
+2020-09-02T18:01:49Z,26.78,61.26,99,0,35.63,101.62,0.00,400.00,0.209156,0.215953,0.226430,0.213547,null,null,null
+2020-09-02T18:02:19Z,26.78,61.26,99,0,38.88,101.62,0.00,400.00,0.208336,0.215242,0.225914,0.213461,null,null,null
+2020-09-02T18:02:49Z,26.79,61.28,99,0,39.33,101.62,0.00,400.00,0.209094,0.216242,0.226711,0.213844,null,null,null
+2020-09-02T18:03:19Z,26.79,61.25,99,0,31.27,101.62,0.00,400.00,0.209000,0.215570,0.224812,0.213062,null,null,null
+2020-09-02T18:03:49Z,26.78,61.24,99,0,34.29,101.62,0.00,400.00,0.207891,0.215133,0.227961,0.214086,null,null,null
+2020-09-02T18:04:19Z,26.78,61.24,99,0,46.69,101.62,0.00,400.00,0.207148,0.215133,0.226242,0.213227,null,null,null
+2020-09-02T18:04:49Z,26.79,61.23,99,0,40.83,101.62,0.00,400.00,0.209305,0.215648,0.226727,0.213383,null,null,null
+2020-09-02T18:05:19Z,26.78,61.26,99,0,37.27,101.62,0.00,400.00,0.208336,0.215516,0.226258,0.212992,null,null,null
+2020-09-02T18:05:49Z,26.76,61.28,99,0,31.74,101.62,0.00,400.00,0.208133,0.215266,0.226125,0.213766,null,null,null
+2020-09-02T18:06:19Z,26.79,61.21,99,0,32.77,101.63,0.00,400.00,0.206531,0.215484,0.225531,0.213570,null,null,null
+2020-09-02T18:06:49Z,26.78,61.27,99,0,29.96,101.63,0.00,400.00,0.208000,0.216195,0.225664,0.213602,null,null,null
+2020-09-02T18:07:19Z,26.79,61.22,99,0,29.92,101.63,0.00,400.00,0.208273,0.214320,0.226359,0.214008,null,null,null
+2020-09-02T18:07:49Z,26.79,61.25,99,0,42.11,101.63,0.00,400.00,0.206781,0.214570,0.226320,0.213273,null,null,null
+2020-09-02T18:08:19Z,26.76,61.27,99,0,32.64,101.63,0.00,400.00,0.206328,0.214781,0.226922,0.213500,null,null,null
+2020-09-02T18:08:49Z,26.78,61.21,99,0,37.51,101.63,0.00,400.00,0.207547,0.215531,0.224961,0.212906,null,null,null
+2020-09-02T18:09:19Z,26.79,61.26,99,0,47.01,101.63,0.00,400.00,0.208859,0.216266,0.227125,0.213547,null,null,null
+2020-09-02T18:09:49Z,26.79,61.26,99,0,40.44,101.63,0.00,400.00,0.209438,0.216672,0.227109,0.213492,null,null,null
+2020-09-02T18:10:19Z,26.76,61.24,99,0,33.06,101.63,0.00,400.00,0.208305,0.214883,0.226398,0.213570,null,null,null
+2020-09-02T18:10:49Z,26.76,61.30,99,0,36.35,101.63,0.00,400.00,0.207516,0.216461,0.227477,0.214453,null,null,null
+2020-09-02T18:11:19Z,26.79,61.27,99,0,29.37,101.63,0.00,405.00,0.207602,0.215523,0.226008,0.213500,null,null,null
+2020-09-02T18:11:49Z,26.76,61.24,99,0,32.70,101.64,0.00,405.00,0.210156,0.216102,0.225844,0.213703,null,null,null
+2020-09-02T18:12:19Z,26.78,61.22,99,0,47.85,101.63,0.00,400.00,0.207945,0.215914,0.228008,0.214234,null,null,null
+2020-09-02T18:12:49Z,26.78,61.25,99,0,28.51,101.63,0.00,400.00,0.208289,0.215875,0.225547,0.213523,null,null,null
+2020-09-02T18:13:19Z,26.82,61.26,99,0,29.62,101.63,0.00,405.00,0.207180,0.215836,0.224617,0.213211,null,null,null
+2020-09-02T18:13:49Z,26.75,61.27,99,0,35.93,101.63,0.00,405.00,0.207570,0.214719,0.226805,0.213992,null,null,null
+2020-09-02T18:14:19Z,26.79,61.22,99,0,33.99,101.64,0.00,400.00,0.207914,0.215258,0.226094,0.213336,null,null,null
+2020-09-02T18:14:49Z,26.75,61.31,99,0,27.99,101.63,0.00,400.00,0.208227,0.215547,0.226789,0.213125,null,null,null
+2020-09-02T18:15:19Z,26.75,61.25,99,0,27.64,101.64,0.00,400.00,0.206961,0.215555,0.226195,0.213352,null,null,null
+2020-09-02T18:15:49Z,26.75,61.29,99,0,33.47,101.64,0.00,400.00,0.208852,0.214234,0.226945,0.213898,null,null,null
+2020-09-02T18:16:19Z,26.78,61.27,99,0,32.46,101.64,0.00,400.00,0.207594,0.215039,0.226313,0.213531,null,null,null
+2020-09-02T18:16:49Z,26.78,61.26,99,0,29.94,101.64,0.00,400.00,0.208383,0.216273,0.224961,0.213820,null,null,null
+2020-09-02T18:17:19Z,26.78,61.29,99,0,42.46,101.64,0.00,400.00,0.207695,0.215734,0.227016,0.214023,null,null,null
+2020-09-02T18:17:49Z,26.78,61.26,99,0,27.38,101.64,0.00,400.00,0.207555,0.215578,0.228430,0.213961,null,null,null
+2020-09-02T18:18:19Z,26.78,61.27,99,0,29.92,101.64,0.00,405.00,0.206836,0.215930,0.226547,0.213516,null,null,null
+2020-09-02T18:18:49Z,26.78,61.28,99,0,37.84,101.64,0.00,405.00,0.208227,0.216953,0.226766,0.214031,null,null,null
+2020-09-02T18:19:19Z,26.79,61.27,99,0,41.44,101.64,0.00,400.00,0.206914,0.214219,0.226734,0.213859,null,null,null
+2020-09-02T18:19:49Z,26.78,61.29,99,0,33.56,101.64,0.00,400.00,0.207414,0.214789,0.225984,0.213211,null,null,null
+2020-09-02T18:20:19Z,26.78,61.33,99,0,36.98,101.64,0.00,400.00,0.207742,0.215391,0.226984,0.213609,null,null,null
+2020-09-02T18:20:49Z,26.76,61.26,99,0,26.48,101.64,0.00,400.00,0.207398,0.215438,0.225844,0.212789,null,null,null
+2020-09-02T18:21:19Z,26.75,61.32,99,0,29.26,101.64,0.00,400.00,0.208070,0.215531,0.227680,0.214367,null,null,null
+2020-09-02T18:21:49Z,26.76,61.37,99,0,30.91,101.65,0.00,400.00,0.208383,0.215148,0.224602,0.213570,null,null,null
+2020-09-02T18:22:19Z,26.76,61.31,99,0,36.29,101.64,0.00,400.00,0.208523,0.216562,0.226672,0.214070,null,null,null
+2020-09-02T18:22:49Z,26.76,61.27,99,0,37.99,101.65,0.00,400.00,0.207383,0.215617,0.227297,0.213555,null,null,null
+2020-09-02T18:23:19Z,26.78,61.29,99,0,33.18,101.65,0.00,400.00,0.207125,0.215805,0.226336,0.213523,null,null,null
+2020-09-02T18:23:49Z,26.78,61.29,99,0,30.20,101.65,0.00,400.00,0.208586,0.215055,0.226227,0.213391,null,null,null
+2020-09-02T18:24:19Z,26.78,61.27,99,0,30.31,101.65,0.00,400.00,0.208523,0.214687,0.227078,0.213961,null,null,null
+2020-09-02T18:24:49Z,26.76,61.26,99,0,27.77,101.65,0.00,400.00,0.208766,0.216109,0.226539,0.214453,null,null,null
+2020-09-02T18:25:19Z,26.76,61.26,99,0,33.83,101.65,0.00,400.00,0.208695,0.215516,0.226117,0.213570,null,null,null
+2020-09-02T18:25:49Z,26.78,61.34,99,0,29.15,101.66,0.00,400.00,0.208547,0.215914,0.226250,0.213828,null,null,null
+2020-09-02T18:26:19Z,26.79,61.27,99,0,28.52,101.65,0.00,400.00,0.208648,0.216148,0.226797,0.213336,null,null,null
+2020-09-02T18:26:49Z,26.76,61.27,99,0,47.22,101.65,0.00,400.00,0.208234,0.214750,0.224734,0.213680,null,null,null
+2020-09-02T18:27:19Z,26.76,61.27,99,0,29.17,101.66,0.00,400.00,0.208711,0.214930,0.226719,0.213422,null,null,null
+2020-09-02T18:27:49Z,26.76,61.25,99,0,30.46,101.66,0.00,400.00,0.209859,0.216984,0.226430,0.214062,null,null,null
+2020-09-02T18:28:19Z,26.78,61.27,99,0,45.85,101.66,0.00,400.00,0.207664,0.214719,0.225945,0.214094,null,null,null
+2020-09-02T18:28:49Z,26.76,61.29,99,0,26.93,101.66,0.00,400.00,0.208391,0.215578,0.226617,0.214039,null,null,null
+2020-09-02T18:29:19Z,26.76,61.29,99,0,32.36,101.66,0.00,400.00,0.209102,0.215094,0.227070,0.214461,null,null,null
+2020-09-02T18:29:49Z,26.75,61.26,99,0,29.56,101.66,0.00,400.00,0.207273,0.215445,0.224539,0.212883,null,null,null
+2020-09-02T18:30:19Z,26.78,61.28,99,0,33.74,101.66,0.00,400.00,0.208852,0.215359,0.226555,0.214344,null,null,null
+2020-09-02T18:30:49Z,26.75,61.25,99,0,30.80,101.66,0.00,400.00,0.207281,0.215141,0.227406,0.214633,null,null,null
+2020-09-02T18:31:19Z,26.75,61.29,99,0,29.90,101.66,0.00,400.00,0.208984,0.216766,0.227352,0.213742,null,null,null
+2020-09-02T18:31:49Z,26.76,61.26,99,0,29.49,101.67,0.00,400.00,0.209164,0.216781,0.227758,0.214719,null,null,null
+2020-09-02T18:32:19Z,26.76,61.24,99,0,29.27,101.67,0.00,400.00,0.208836,0.214898,0.226906,0.213727,null,null,null
+2020-09-02T18:32:49Z,26.76,61.25,99,0,29.91,101.67,0.00,400.00,0.209156,0.214914,0.227164,0.214172,null,null,null
+2020-09-02T18:33:19Z,26.75,61.28,99,0,32.42,101.67,0.00,400.00,0.207914,0.216281,0.226773,0.214305,null,null,null
+2020-09-02T18:33:49Z,26.78,61.26,99,0,31.13,101.67,0.00,400.00,0.209984,0.216039,0.227273,0.214016,null,null,null
+2020-09-02T18:34:19Z,26.73,61.27,99,0,31.28,101.67,0.00,400.00,0.208273,0.215367,0.225359,0.213055,null,null,null
+2020-09-02T18:34:49Z,26.76,61.26,99,0,40.61,101.67,0.00,400.00,0.208305,0.216266,0.227422,0.214148,null,null,null
+2020-09-02T18:35:19Z,26.75,61.28,99,0,28.73,101.67,0.00,400.00,0.208766,0.215195,0.228961,0.213695,null,null,null
+2020-09-02T18:35:49Z,26.73,61.29,99,0,27.68,101.68,0.00,400.00,0.209477,0.217234,0.226734,0.213352,null,null,null
+2020-09-02T18:36:19Z,26.78,61.27,99,0,28.02,101.68,0.00,400.00,0.208367,0.216430,0.227234,0.213820,null,null,null
+2020-09-02T18:36:49Z,26.73,61.26,99,0,30.34,101.68,0.00,400.00,0.209187,0.215570,0.225688,0.213070,null,null,null
+2020-09-02T18:37:19Z,26.72,61.28,99,0,37.77,101.68,0.00,400.00,0.208414,0.216391,0.227422,0.214031,null,null,null
+2020-09-02T18:37:49Z,26.75,61.28,99,0,26.21,101.68,0.00,400.00,0.208414,0.216891,0.226617,0.214930,null,null,null
+2020-09-02T18:38:19Z,26.79,61.27,99,0,38.24,101.68,0.00,400.00,0.208586,0.216391,0.225461,0.213406,null,null,null
+2020-09-02T18:38:49Z,26.75,61.29,99,0,29.46,101.68,0.00,400.00,0.207320,0.215211,0.227219,0.213734,null,null,null
+2020-09-02T18:39:19Z,26.76,61.30,99,0,37.09,101.68,0.00,400.00,0.206867,0.215633,0.226758,0.213602,null,null,null
+2020-09-02T18:39:49Z,26.75,61.26,99,0,30.16,101.69,0.00,400.00,0.210242,0.216117,0.226633,0.214711,null,null,null
+2020-09-02T18:40:19Z,26.73,61.27,99,0,27.77,101.69,0.00,400.00,0.208867,0.214953,0.227055,0.214586,null,null,null
+2020-09-02T18:40:49Z,26.75,61.25,99,0,27.22,101.69,0.00,400.00,0.209523,0.215617,0.227500,0.214414,null,null,null
+2020-09-02T18:41:19Z,26.75,61.25,99,0,29.97,101.68,0.00,405.00,0.209852,0.215898,0.224711,0.213484,null,null,null
+2020-09-02T18:41:49Z,26.75,61.26,99,0,27.99,101.69,0.00,405.00,0.207992,0.215234,0.226500,0.214250,null,null,null
+2020-09-02T18:42:19Z,26.75,61.27,99,0,30.08,101.69,0.00,400.00,0.208867,0.216133,0.226320,0.214195,null,null,null
+2020-09-02T18:42:49Z,26.72,61.25,99,0,33.02,101.69,0.00,400.00,0.207281,0.215211,0.227578,0.214430,null,null,null
+2020-09-02T18:43:19Z,26.73,61.25,99,0,31.84,101.69,0.00,400.00,0.209703,0.215805,0.227187,0.214305,null,null,null
+2020-09-02T18:43:49Z,26.75,61.25,99,0,28.54,101.69,0.00,400.00,0.208570,0.215844,0.225898,0.213648,null,null,null
+2020-09-02T18:44:19Z,26.75,61.20,99,0,38.93,101.69,0.00,400.00,0.208312,0.214719,0.226117,0.214219,null,null,null
+2020-09-02T18:44:49Z,26.76,61.25,99,0,27.77,101.70,0.00,400.00,0.208406,0.216195,0.226453,0.214148,null,null,null
+2020-09-02T18:45:19Z,26.73,61.23,99,0,34.12,101.69,0.00,405.00,0.208578,0.216422,0.227313,0.214695,null,null,null
+2020-09-02T18:45:49Z,26.75,61.25,99,0,29.40,101.70,0.00,405.00,0.207789,0.216102,0.226875,0.213625,null,null,null
+2020-09-02T18:46:19Z,26.75,61.26,99,0,30.90,101.69,0.00,400.00,0.209133,0.215531,0.227687,0.214227,null,null,null
+2020-09-02T18:46:49Z,26.75,61.22,99,0,27.44,101.70,0.00,400.00,0.206750,0.216047,0.226164,0.213781,null,null,null
+2020-09-02T18:47:19Z,26.75,61.25,99,0,38.95,101.70,0.00,400.00,0.207664,0.216188,0.228406,0.214914,null,null,null
+2020-09-02T18:47:49Z,26.73,61.25,99,0,33.23,101.70,0.00,400.00,0.209711,0.215750,0.226922,0.214820,null,null,null
+2020-09-02T18:48:19Z,26.73,61.25,99,0,32.01,101.70,0.00,405.00,0.207844,0.215961,0.228203,0.213945,null,null,null
+2020-09-02T18:48:49Z,26.73,61.27,99,0,27.87,101.70,0.00,405.00,0.208102,0.215062,0.227203,0.214445,null,null,null
+2020-09-02T18:49:19Z,26.73,61.26,99,0,32.92,101.70,0.00,405.00,0.208531,0.215820,0.228031,0.214180,null,null,null
+2020-09-02T18:49:49Z,26.73,61.26,99,0,32.59,101.71,0.00,405.00,0.207992,0.215906,0.226844,0.213859,null,null,null
+2020-09-02T18:50:19Z,26.75,61.26,99,0,40.72,101.70,0.00,400.00,0.207211,0.215242,0.226789,0.214375,null,null,null
+2020-09-02T18:50:49Z,26.75,61.24,99,0,40.23,101.70,0.00,400.00,0.207531,0.215547,0.226648,0.214227,null,null,null
+2020-09-02T18:51:19Z,26.73,61.27,99,0,30.17,101.71,0.00,400.00,0.207633,0.215539,0.227961,0.214891,null,null,null
+2020-09-02T18:51:49Z,26.73,61.21,99,0,30.91,101.71,0.00,400.00,0.208555,0.215312,0.227430,0.214430,null,null,null
+2020-09-02T18:52:19Z,26.73,61.21,99,0,30.26,101.71,0.00,401.00,0.208586,0.214648,0.227031,0.213469,null,null,null
+2020-09-02T18:52:49Z,26.75,61.22,99,0,28.14,101.71,0.00,401.00,0.208500,0.215797,0.225703,0.213398,null,null,null
+2020-09-02T18:53:19Z,26.73,61.24,99,0,30.46,101.71,0.00,401.00,0.208813,0.216625,0.226781,0.214289,null,null,null
+2020-09-02T18:53:49Z,26.73,61.20,99,0,27.59,101.71,0.00,401.00,0.208531,0.215703,0.228148,0.215211,null,null,null
+2020-09-02T18:54:19Z,26.73,61.20,99,0,37.89,101.71,0.00,401.00,0.209328,0.215859,0.227102,0.213992,null,null,null
+2020-09-02T18:54:49Z,26.75,61.23,99,0,40.86,101.71,0.00,401.00,0.208273,0.215250,0.226867,0.214109,null,null,null
+2020-09-02T18:55:19Z,26.76,61.19,99,0,35.40,101.71,0.00,400.00,0.208445,0.215703,0.227430,0.214023,null,null,null
+2020-09-02T18:55:49Z,26.76,61.19,99,0,36.41,101.72,0.00,400.00,0.208781,0.216008,0.228672,0.214703,null,null,null
+2020-09-02T18:56:19Z,26.73,61.20,99,0,27.30,101.71,0.00,400.00,0.209266,0.216594,0.227289,0.213922,null,null,null
+2020-09-02T18:56:49Z,26.75,61.23,99,0,41.40,101.72,0.00,400.00,0.208148,0.216844,0.227375,0.214312,null,null,null
+2020-09-02T18:57:19Z,26.76,61.23,99,0,29.22,101.72,0.00,402.00,0.208781,0.215844,0.228539,0.214969,null,null,null
+2020-09-02T18:57:49Z,26.73,61.22,99,0,35.73,101.72,0.00,402.00,0.207961,0.215141,0.226492,0.214250,null,null,null
+2020-09-02T18:58:19Z,26.72,61.22,99,0,33.97,101.72,0.00,400.00,0.207508,0.216484,0.227437,0.214305,null,null,null
+2020-09-02T18:58:49Z,26.72,61.22,99,0,41.50,101.72,0.00,400.00,0.207633,0.214781,0.226172,0.214133,null,null,null
+2020-09-02T18:59:19Z,26.72,61.21,99,0,31.43,101.72,0.00,403.00,0.208055,0.216680,0.226180,0.214281,null,null,null
+2020-09-02T18:59:49Z,26.72,61.20,99,0,28.45,101.72,0.00,403.00,0.209336,0.215477,0.226133,0.214273,null,null,null
+2020-09-02T19:00:19Z,26.75,61.20,99,0,43.51,101.72,0.00,400.00,0.209430,0.214883,0.226656,0.214344,null,null,null
+2020-09-02T19:00:49Z,26.76,61.19,99,0,38.56,101.72,0.00,400.00,0.209023,0.216289,0.227930,0.214211,null,null,null
+2020-09-02T19:01:19Z,26.72,61.20,99,0,35.51,101.73,0.00,400.00,0.208687,0.216219,0.228031,0.214578,null,null,null
+2020-09-02T19:01:49Z,26.73,61.16,99,0,26.41,101.72,0.00,400.00,0.208734,0.215594,0.226086,0.214523,null,null,null
+2020-09-02T19:02:19Z,26.73,61.18,99,0,28.89,101.73,0.00,402.00,0.206742,0.215289,0.228719,0.214961,null,null,null
+2020-09-02T19:02:49Z,26.73,61.18,99,0,30.12,101.73,0.00,402.00,0.208836,0.216117,0.227758,0.214422,null,null,null
+2020-09-02T19:03:19Z,26.75,61.20,99,0,29.28,101.73,0.00,402.00,0.208312,0.215180,0.225102,0.213750,null,null,null
+2020-09-02T19:03:49Z,26.75,61.21,99,0,27.66,101.73,0.00,402.00,0.207914,0.216258,0.226883,0.214719,null,null,null
+2020-09-02T19:04:19Z,26.75,61.18,99,0,38.16,101.73,0.00,400.00,0.209586,0.215836,0.226617,0.213625,null,null,null
+2020-09-02T19:04:49Z,26.72,61.19,99,0,29.47,101.73,0.00,400.00,0.208914,0.216391,0.225938,0.214047,null,null,null
+2020-09-02T19:05:19Z,26.73,61.20,99,0,31.08,101.73,0.00,400.00,0.210820,0.216688,0.228750,0.213953,null,null,null
+2020-09-02T19:05:49Z,26.72,61.18,99,0,35.06,101.74,0.00,400.00,0.208773,0.215727,0.227148,0.214141,null,null,null
+2020-09-02T19:06:19Z,26.73,61.18,99,0,28.42,101.74,0.00,400.00,0.208117,0.216281,0.227703,0.214352,null,null,null
+2020-09-02T19:06:49Z,26.75,61.15,99,0,27.49,101.74,0.00,400.00,0.207750,0.213992,0.227258,0.213805,null,null,null
+2020-09-02T19:07:19Z,26.73,61.17,99,0,36.86,101.74,0.00,400.00,0.208312,0.215906,0.228266,0.214836,null,null,null
+2020-09-02T19:07:49Z,26.73,61.20,99,0,28.06,101.74,0.00,400.00,0.209633,0.215805,0.226617,0.213766,null,null,null
+2020-09-02T19:08:19Z,26.73,61.15,99,0,42.98,101.74,0.00,400.00,0.210172,0.216727,0.228547,0.214898,null,null,null
+2020-09-02T19:08:49Z,26.73,61.17,99,0,30.73,101.74,0.00,400.00,0.207820,0.214781,0.226391,0.214711,null,null,null
+2020-09-02T19:09:19Z,26.73,61.18,99,0,35.31,101.74,0.00,400.00,0.207383,0.215742,0.226445,0.214203,null,null,null
+2020-09-02T19:09:49Z,26.76,61.15,99,0,34.41,101.74,0.00,400.00,0.209133,0.217023,0.228531,0.214789,null,null,null
+2020-09-02T19:10:19Z,26.75,61.13,99,0,36.97,101.74,0.00,400.00,0.207867,0.215758,0.227914,0.214320,null,null,null
+2020-09-02T19:10:49Z,26.73,61.15,99,0,32.75,101.74,0.00,400.00,0.207359,0.216828,0.225031,0.214047,null,null,null
+2020-09-02T19:11:19Z,26.73,61.15,99,0,31.48,101.75,0.00,400.00,0.211180,0.216969,0.226984,0.214141,null,null,null
+2020-09-02T19:11:49Z,26.72,61.15,99,0,30.40,101.74,0.00,400.00,0.207883,0.215539,0.225555,0.214570,null,null,null
+2020-09-02T19:12:19Z,26.72,61.13,99,0,31.59,101.75,0.00,400.00,0.208633,0.215477,0.227258,0.214594,null,null,null
+2020-09-02T19:12:49Z,26.72,61.15,99,0,32.65,101.75,0.00,400.00,0.208211,0.216227,0.226656,0.213992,null,null,null
+2020-09-02T19:13:19Z,26.75,61.15,99,0,28.17,101.75,0.00,400.00,0.208289,0.216242,0.224648,0.213953,null,null,null
+2020-09-02T19:13:49Z,26.73,61.17,99,0,36.33,101.75,0.00,400.00,0.207992,0.214500,0.227320,0.214906,null,null,null
+2020-09-02T19:14:19Z,26.72,61.15,99,0,44.19,101.75,0.00,400.00,0.208992,0.216086,0.227281,0.214273,null,null,null
+2020-09-02T19:14:49Z,26.75,61.17,99,0,36.57,101.75,0.00,400.00,0.209508,0.215539,0.228555,0.214687,null,null,null
+2020-09-02T19:15:19Z,26.73,61.18,99,0,36.84,101.76,0.00,400.00,0.208555,0.215594,0.227305,0.213594,null,null,null
+2020-09-02T19:15:49Z,26.75,61.17,99,0,28.63,101.75,0.00,400.00,0.209430,0.216312,0.226422,0.214844,null,null,null
+2020-09-02T19:16:19Z,26.72,61.16,99,0,28.77,101.75,0.00,400.00,0.207195,0.214891,0.226852,0.213633,null,null,null
+2020-09-02T19:16:49Z,26.73,61.18,99,0,29.79,101.76,0.00,400.00,0.209078,0.216320,0.227492,0.215070,null,null,null
+2020-09-02T19:17:19Z,26.73,61.15,99,0,28.77,101.76,0.00,402.00,0.209844,0.216219,0.227695,0.214211,null,null,null
+2020-09-02T19:17:49Z,26.72,61.18,99,0,37.14,101.75,0.00,402.00,0.209602,0.216633,0.226195,0.214195,null,null,null
+2020-09-02T19:18:19Z,26.72,61.12,99,0,31.29,101.76,0.00,400.00,0.208078,0.214867,0.226586,0.214156,null,null,null
+2020-09-02T19:18:49Z,26.72,61.13,99,0,30.90,101.76,0.00,400.00,0.210484,0.215547,0.226625,0.213875,null,null,null
+2020-09-02T19:19:19Z,26.71,61.18,99,0,27.06,101.76,0.00,400.00,0.209312,0.215961,0.227117,0.214852,null,null,null
+2020-09-02T19:19:49Z,26.75,61.15,99,0,35.30,101.76,0.00,400.00,0.208586,0.215047,0.227508,0.214859,null,null,null
+2020-09-02T19:20:19Z,26.72,61.16,99,0,29.25,101.76,0.00,400.00,0.208758,0.216391,0.227141,0.214039,null,null,null
+2020-09-02T19:20:49Z,26.72,61.15,99,0,33.06,101.76,0.00,400.00,0.210187,0.217539,0.227633,0.214508,null,null,null
+2020-09-02T19:21:19Z,26.72,61.16,99,0,27.36,101.77,1.00,407.00,0.209203,0.216867,0.228094,0.214367,null,null,null
+2020-09-02T19:21:49Z,26.73,61.12,99,0,28.17,101.76,1.00,407.00,0.207211,0.215719,0.226469,0.214008,null,null,null
+2020-09-02T19:22:19Z,26.72,61.14,99,0,31.75,101.76,0.00,401.00,0.208859,0.214992,0.227453,0.214547,null,null,null
+2020-09-02T19:22:49Z,26.73,61.13,99,0,44.82,101.77,0.00,401.00,0.209383,0.216555,0.225953,0.214094,null,null,null
+2020-09-02T19:23:19Z,26.72,61.15,99,0,30.23,101.77,0.00,400.00,0.208227,0.216797,0.224031,0.214469,null,null,null
+2020-09-02T19:23:49Z,26.73,61.08,99,0,29.87,101.77,0.00,400.00,0.210055,0.216406,0.228734,0.215203,null,null,null
+2020-09-02T19:24:19Z,26.72,61.14,99,0,31.47,101.77,0.00,400.00,0.208570,0.215250,0.226945,0.214836,null,null,null
+2020-09-02T19:24:49Z,26.72,61.13,99,0,26.08,101.77,0.00,400.00,0.209266,0.216805,0.226688,0.214211,null,null,null
+2020-09-02T19:25:19Z,26.73,61.12,99,0,27.26,101.77,0.00,403.00,0.210539,0.216656,0.228633,0.213938,null,null,null
+2020-09-02T19:25:49Z,26.72,61.15,99,0,29.54,101.77,0.00,403.00,0.208594,0.215609,0.228172,0.214258,null,null,null
+2020-09-02T19:26:19Z,26.73,61.13,99,0,41.14,101.77,0.00,402.00,0.209805,0.216180,0.226695,0.214781,null,null,null
+2020-09-02T19:26:49Z,26.72,61.11,99,0,30.75,101.77,0.00,402.00,0.208922,0.215813,0.227367,0.214984,null,null,null
+2020-09-02T19:27:19Z,26.72,61.12,99,0,27.42,101.77,0.00,402.00,0.209492,0.216594,0.226859,0.214328,null,null,null
+2020-09-02T19:27:49Z,26.72,61.12,99,0,31.28,101.78,0.00,402.00,0.208586,0.216078,0.228703,0.215109,null,null,null
+2020-09-02T19:28:19Z,26.72,61.12,99,0,29.96,101.77,0.00,403.00,0.210742,0.216578,0.227352,0.214328,null,null,null
+2020-09-02T19:28:49Z,26.72,61.11,99,0,28.04,101.77,0.00,403.00,0.209211,0.216742,0.227797,0.214094,null,null,null
+2020-09-02T19:29:19Z,26.72,61.08,99,0,32.06,101.77,0.00,403.00,0.208898,0.216133,0.227258,0.214687,null,null,null
+2020-09-02T19:29:49Z,26.73,61.10,99,0,30.08,101.77,0.00,403.00,0.208508,0.215664,0.226266,0.214383,null,null,null
+2020-09-02T19:30:19Z,26.73,61.11,99,0,33.14,101.77,0.00,402.00,0.209266,0.217000,0.226633,0.213750,null,null,null
+2020-09-02T19:30:49Z,26.73,61.05,99,0,35.19,101.77,0.00,402.00,0.208992,0.217000,0.228211,0.214492,null,null,null
+2020-09-02T19:31:19Z,26.73,61.09,99,0,31.43,101.77,0.00,400.00,0.206219,0.215203,0.226859,0.214414,null,null,null
+2020-09-02T19:31:49Z,26.73,61.11,99,0,31.24,101.77,0.00,400.00,0.209922,0.217273,0.228141,0.214930,null,null,null
+2020-09-02T19:32:19Z,26.71,61.09,99,0,35.33,101.78,0.00,400.00,0.209187,0.215852,0.226734,0.213547,null,null,null
+2020-09-02T19:32:49Z,26.75,61.11,99,0,43.97,101.78,0.00,400.00,0.209039,0.215898,0.227070,0.214805,null,null,null
+2020-09-02T19:33:19Z,26.73,61.09,99,0,29.88,101.78,0.00,400.00,0.208133,0.216219,0.226102,0.213961,null,null,null
+2020-09-02T19:33:49Z,26.71,61.10,99,0,37.48,101.78,0.00,400.00,0.209000,0.215672,0.228547,0.214820,null,null,null
+2020-09-02T19:34:19Z,26.72,61.06,99,0,28.64,101.78,0.00,400.00,0.208531,0.216672,0.226977,0.214070,null,null,null
+2020-09-02T19:34:49Z,26.72,61.06,99,0,30.42,101.78,0.00,400.00,0.210453,0.216281,0.227266,0.214234,null,null,null
+2020-09-02T19:35:19Z,26.72,61.07,99,0,25.29,101.78,0.00,400.00,0.208602,0.216523,0.226047,0.214016,null,null,null
+2020-09-02T19:35:49Z,26.72,61.06,99,0,30.02,101.78,0.00,400.00,0.207039,0.215164,0.228352,0.214531,null,null,null
+2020-09-02T19:36:19Z,26.72,61.09,99,0,28.19,101.78,0.00,401.00,0.208906,0.216453,0.226234,0.214039,null,null,null
+2020-09-02T19:36:49Z,26.72,61.07,99,0,34.66,101.78,0.00,401.00,0.210266,0.216648,0.228641,0.214914,null,null,null
+2020-09-02T19:37:19Z,26.73,61.07,99,0,29.86,101.78,0.00,400.00,0.209242,0.215672,0.227664,0.215188,null,null,null
+2020-09-02T19:37:49Z,26.72,61.05,99,0,27.82,101.78,0.00,400.00,0.209320,0.215430,0.227703,0.214813,null,null,null
+2020-09-02T19:38:19Z,26.73,61.05,99,0,26.21,101.78,0.00,400.00,0.207930,0.216156,0.228523,0.213687,null,null,null
+2020-09-02T19:38:49Z,26.73,61.06,99,0,34.64,101.79,0.00,400.00,0.207711,0.215438,0.227367,0.214633,null,null,null
+2020-09-02T19:39:19Z,26.73,61.05,99,0,32.47,101.78,0.00,401.00,0.208922,0.216617,0.226977,0.214766,null,null,null
+2020-09-02T19:39:49Z,26.73,61.07,99,0,28.92,101.79,0.00,401.00,0.208641,0.215219,0.225398,0.214609,null,null,null
+2020-09-02T19:40:19Z,26.72,61.05,99,0,31.59,101.79,0.00,400.00,0.209734,0.215773,0.226555,0.215227,null,null,null
+2020-09-02T19:40:49Z,26.71,61.07,99,0,32.36,101.78,0.00,400.00,0.208141,0.215984,0.227422,0.215039,null,null,null
+2020-09-02T19:41:19Z,26.73,61.02,99,0,33.23,101.78,0.00,401.00,0.208539,0.215383,0.225555,0.213961,null,null,null
+2020-09-02T19:41:49Z,26.75,61.02,99,0,30.48,101.78,0.00,401.00,0.208516,0.215727,0.229008,0.214937,null,null,null
+2020-09-02T19:42:19Z,26.72,60.99,99,0,31.95,101.78,0.00,400.00,0.208586,0.216219,0.227234,0.214102,null,null,null
+2020-09-02T19:42:49Z,26.72,61.02,99,0,33.64,101.78,0.00,400.00,0.208711,0.216086,0.227516,0.214656,null,null,null
+2020-09-02T19:43:19Z,26.72,61.04,99,0,32.90,101.78,0.00,402.00,0.209523,0.217117,0.228117,0.214523,null,null,null
+2020-09-02T19:43:49Z,26.73,61.04,99,0,38.04,101.79,0.00,402.00,0.209102,0.216203,0.225562,0.214602,null,null,null
+2020-09-02T19:44:19Z,26.73,61.02,99,0,33.80,101.79,0.00,400.00,0.209352,0.217016,0.227367,0.214781,null,null,null
+2020-09-02T19:44:49Z,26.73,61.05,99,0,28.67,101.79,0.00,400.00,0.209398,0.216508,0.227289,0.214539,null,null,null
+2020-09-02T19:45:19Z,26.72,61.02,99,0,29.05,101.79,0.00,402.00,0.208375,0.216047,0.227687,0.214789,null,null,null
+2020-09-02T19:45:49Z,26.72,61.04,99,0,30.29,101.78,0.00,402.00,0.208500,0.216844,0.226883,0.214180,null,null,null
+2020-09-02T19:46:19Z,26.72,60.94,99,0,28.88,101.79,0.00,400.00,0.210805,0.216906,0.227031,0.214188,null,null,null
+2020-09-02T19:46:49Z,26.72,61.02,99,0,39.67,101.79,0.00,400.00,0.208797,0.215414,0.227211,0.214461,null,null,null
+2020-09-02T19:47:19Z,26.73,60.99,99,0,27.24,101.79,0.00,400.00,0.209086,0.216398,0.228719,0.214836,null,null,null
+2020-09-02T19:47:49Z,26.72,61.00,99,0,36.90,101.79,0.00,400.00,0.207734,0.216430,0.226711,0.214648,null,null,null
+2020-09-02T19:48:19Z,26.73,61.02,99,0,42.65,101.79,0.00,400.00,0.208961,0.216078,0.226164,0.214445,null,null,null
+2020-09-02T19:48:49Z,26.72,60.99,99,0,28.71,101.79,0.00,400.00,0.210117,0.216656,0.226047,0.214586,null,null,null
+2020-09-02T19:49:19Z,26.73,61.00,99,0,26.67,101.79,0.00,400.00,0.209680,0.216477,0.228797,0.215273,null,null,null
+2020-09-02T19:49:49Z,26.73,60.99,99,0,26.26,101.79,0.00,400.00,0.208844,0.215125,0.227336,0.213883,null,null,null
+2020-09-02T19:50:19Z,26.73,61.02,99,0,30.18,101.79,0.00,400.00,0.208875,0.215711,0.229062,0.214758,null,null,null
+2020-09-02T19:50:49Z,26.73,60.98,99,0,32.47,101.79,0.00,400.00,0.210289,0.216914,0.228328,0.214437,null,null,null
+2020-09-02T19:51:19Z,26.73,60.99,99,0,29.72,101.80,0.00,400.00,0.210445,0.216781,0.226961,0.214133,null,null,null
+2020-09-02T19:51:49Z,26.72,60.98,99,0,26.24,101.79,0.00,400.00,0.209125,0.215875,0.228062,0.214906,null,null,null
+2020-09-02T19:52:19Z,26.69,61.02,99,0,28.40,101.80,0.00,400.00,0.209844,0.215930,0.228250,0.215586,null,null,null
+2020-09-02T19:52:49Z,26.73,60.99,99,0,30.34,101.80,0.00,400.00,0.210797,0.216227,0.228031,0.214625,null,null,null
+2020-09-02T19:53:19Z,26.73,60.96,99,0,41.29,101.80,0.00,400.00,0.208445,0.215883,0.228297,0.214914,null,null,null
+2020-09-02T19:53:49Z,26.72,60.98,99,0,32.49,101.80,0.00,400.00,0.209016,0.215977,0.227836,0.215023,null,null,null
+2020-09-02T19:54:19Z,26.72,61.00,99,0,28.91,101.81,0.00,400.00,0.208625,0.216523,0.227391,0.215000,null,null,null
+2020-09-02T19:54:49Z,26.72,60.96,99,0,36.37,101.80,0.00,400.00,0.208898,0.215711,0.226359,0.214102,null,null,null
+2020-09-02T19:55:19Z,26.75,60.99,99,0,27.78,101.80,0.00,400.00,0.207586,0.216156,0.227930,0.214445,null,null,null
+2020-09-02T19:55:49Z,26.75,60.94,99,0,44.31,101.81,0.00,400.00,0.209305,0.215813,0.227625,0.214344,null,null,null
+2020-09-02T19:56:19Z,26.75,60.97,99,0,27.36,101.81,0.00,403.00,0.209766,0.214867,0.228437,0.215383,null,null,null
+2020-09-02T19:56:49Z,26.72,60.95,99,0,28.84,101.81,0.00,403.00,0.208273,0.217391,0.228758,0.214922,null,null,null
+2020-09-02T19:57:19Z,26.71,60.97,99,0,27.47,101.81,0.00,406.00,0.207148,0.216805,0.225938,0.214055,null,null,null
+2020-09-02T19:57:49Z,26.73,60.96,99,0,27.28,101.80,0.00,406.00,0.209609,0.217586,0.226398,0.214344,null,null,null
+2020-09-02T19:58:19Z,26.71,60.94,99,0,44.64,101.81,0.00,403.00,0.208664,0.215680,0.227039,0.213852,null,null,null
+2020-09-02T19:58:49Z,26.73,60.98,99,0,27.30,101.81,0.00,403.00,0.207133,0.215258,0.228625,0.214625,null,null,null
+2020-09-02T19:59:19Z,26.72,60.94,99,0,29.94,101.81,0.00,400.00,0.206852,0.216414,0.227031,0.215234,null,null,null
+2020-09-02T19:59:49Z,26.73,60.95,99,0,33.01,101.81,0.00,400.00,0.210625,0.215703,0.228250,0.215406,null,null,null
+2020-09-02T20:00:19Z,26.72,60.92,99,0,26.53,101.81,0.00,400.00,0.208539,0.216047,0.227789,0.214516,null,null,null
+2020-09-02T20:00:49Z,26.72,60.97,99,0,27.06,101.82,0.00,400.00,0.209844,0.216258,0.227305,0.214672,null,null,null
+2020-09-02T20:01:19Z,26.71,60.91,99,0,27.60,101.81,0.00,400.00,0.209445,0.216047,0.229070,0.214672,null,null,null
+2020-09-02T20:01:49Z,26.73,60.93,99,0,26.31,101.81,0.00,400.00,0.210234,0.216734,0.228094,0.215344,null,null,null
+2020-09-02T20:02:19Z,26.75,60.97,99,0,28.51,101.81,0.00,400.00,0.209734,0.216594,0.228234,0.214008,null,null,null
+2020-09-02T20:02:49Z,26.75,60.99,99,0,45.60,101.82,0.00,400.00,0.207891,0.216836,0.227781,0.214742,null,null,null
+2020-09-02T20:03:19Z,26.75,60.98,99,0,29.01,101.82,0.00,400.00,0.208687,0.217141,0.228234,0.214742,null,null,null
+2020-09-02T20:03:49Z,26.72,60.98,99,0,30.45,101.81,0.00,400.00,0.209125,0.216953,0.226594,0.213859,null,null,null
+2020-09-02T20:04:19Z,26.73,60.92,99,0,33.90,101.82,0.00,400.00,0.208414,0.215578,0.228984,0.214078,null,null,null
+2020-09-02T20:04:49Z,26.72,60.94,99,0,27.08,101.82,0.00,400.00,0.209055,0.216078,0.227500,0.214578,null,null,null
+2020-09-02T20:05:19Z,26.72,60.93,99,0,28.19,101.82,0.00,401.00,0.209688,0.216609,0.227383,0.215016,null,null,null
+2020-09-02T20:05:49Z,26.72,60.91,99,0,41.74,101.81,0.00,401.00,0.207523,0.215937,0.227836,0.214648,null,null,null
+2020-09-02T20:06:19Z,26.71,60.96,99,0,27.77,101.81,0.00,401.00,0.209844,0.216797,0.228242,0.214437,null,null,null
+2020-09-02T20:06:49Z,26.72,60.89,99,0,27.14,101.82,0.00,401.00,0.210273,0.215914,0.227437,0.214023,null,null,null
+2020-09-02T20:07:19Z,26.72,60.97,99,0,25.87,101.82,0.00,400.00,0.209000,0.217609,0.228516,0.215273,null,null,null
+2020-09-02T20:07:49Z,26.71,60.95,99,0,25.90,101.82,0.00,400.00,0.207648,0.215945,0.227742,0.214883,null,null,null
+2020-09-02T20:08:19Z,26.73,60.93,99,0,38.44,101.82,0.00,400.00,0.208672,0.215625,0.227586,0.214445,null,null,null
+2020-09-02T20:08:49Z,26.72,60.93,99,0,35.06,101.82,0.00,400.00,0.209961,0.216820,0.226867,0.214305,null,null,null
+2020-09-02T20:09:19Z,26.72,60.92,99,0,30.11,101.82,0.00,406.00,0.208977,0.216375,0.226375,0.215188,null,null,null
+2020-09-02T20:09:49Z,26.72,60.91,99,0,30.43,101.82,0.00,406.00,0.208594,0.215836,0.228047,0.214531,null,null,null
+2020-09-02T20:10:19Z,26.71,60.92,99,0,28.47,101.82,0.00,400.00,0.209602,0.216273,0.227609,0.214352,null,null,null
+2020-09-02T20:10:49Z,26.75,60.89,99,0,40.78,101.82,0.00,400.00,0.207406,0.215320,0.227633,0.214664,null,null,null
+2020-09-02T20:11:19Z,26.72,60.92,99,0,30.17,101.82,0.00,401.00,0.208102,0.215625,0.228914,0.215398,null,null,null
+2020-09-02T20:11:49Z,26.72,60.91,99,0,27.28,101.83,0.00,401.00,0.208875,0.217078,0.227594,0.214922,null,null,null
+2020-09-02T20:12:19Z,26.72,60.91,99,0,33.95,101.82,0.00,400.00,0.209516,0.216602,0.225930,0.214094,null,null,null
+2020-09-02T20:12:49Z,26.72,60.90,99,0,28.70,101.82,0.00,400.00,0.209172,0.216602,0.227500,0.214734,null,null,null
+2020-09-02T20:13:19Z,26.73,60.88,99,0,32.72,101.82,0.00,400.00,0.210141,0.217063,0.227445,0.214437,null,null,null
+2020-09-02T20:13:49Z,26.72,60.90,99,0,29.81,101.82,0.00,400.00,0.208922,0.216328,0.226336,0.214813,null,null,null
+2020-09-02T20:14:19Z,26.71,60.93,99,0,39.12,101.82,0.00,401.00,0.207750,0.216102,0.228313,0.214945,null,null,null
+2020-09-02T20:14:49Z,26.69,60.90,99,0,27.64,101.83,0.00,401.00,0.209070,0.217688,0.228039,0.215008,null,null,null
+2020-09-02T20:15:19Z,26.71,60.93,99,0,29.67,101.83,0.00,400.00,0.207094,0.214750,0.227289,0.213914,null,null,null
+2020-09-02T20:15:49Z,26.72,60.90,99,0,40.85,101.83,0.00,400.00,0.210734,0.217531,0.228398,0.215156,null,null,null
+2020-09-02T20:16:19Z,26.73,60.91,99,0,27.77,101.82,0.00,401.00,0.209141,0.217055,0.227281,0.215172,null,null,null
+2020-09-02T20:16:49Z,26.71,60.87,99,0,23.86,101.82,0.00,401.00,0.209164,0.216312,0.229008,0.214773,null,null,null
+2020-09-02T20:17:19Z,26.71,60.86,99,0,30.70,101.82,0.00,400.00,0.209219,0.216211,0.228492,0.215328,null,null,null
+2020-09-02T20:17:49Z,26.73,60.89,99,0,29.73,101.83,0.00,400.00,0.208250,0.216148,0.226797,0.214250,null,null,null
+2020-09-02T20:18:19Z,26.72,60.90,99,0,28.14,101.82,0.00,400.00,0.207445,0.215258,0.228203,0.214586,null,null,null
+2020-09-02T20:18:49Z,26.72,60.89,99,0,27.64,101.83,0.00,400.00,0.209352,0.215477,0.226992,0.215195,null,null,null
+2020-09-02T20:19:19Z,26.72,60.89,99,0,28.87,101.83,0.00,400.00,0.210508,0.216562,0.228383,0.214594,null,null,null
+2020-09-02T20:19:49Z,26.72,60.90,99,0,25.70,101.83,0.00,400.00,0.210453,0.216445,0.229555,0.215039,null,null,null
+2020-09-02T20:20:19Z,26.72,60.91,99,0,32.08,101.83,0.00,400.00,0.208945,0.215383,0.227867,0.214406,null,null,null
+2020-09-02T20:20:49Z,26.71,60.91,99,0,29.68,101.83,0.00,400.00,0.210258,0.217352,0.228109,0.214687,null,null,null
+2020-09-02T20:21:19Z,26.73,60.94,99,0,33.66,101.83,0.00,402.00,0.209352,0.217094,0.226156,0.214367,null,null,null
+2020-09-02T20:21:49Z,26.75,60.89,99,0,27.08,101.83,0.00,402.00,0.208281,0.216930,0.227008,0.214867,null,null,null
+2020-09-02T20:22:19Z,26.72,60.90,99,0,29.51,101.83,0.00,400.00,0.207797,0.216586,0.226531,0.214414,null,null,null
+2020-09-02T20:22:49Z,26.72,60.91,99,0,30.89,101.83,0.00,400.00,0.208062,0.215070,0.228359,0.215055,null,null,null
+2020-09-02T20:23:19Z,26.71,60.89,99,0,34.23,101.83,0.00,400.00,0.209438,0.217312,0.227891,0.214852,null,null,null
+2020-09-02T20:23:49Z,26.73,60.84,99,0,30.14,101.83,0.00,400.00,0.207469,0.215680,0.225773,0.214289,null,null,null
+2020-09-02T20:24:19Z,26.72,60.90,99,0,29.21,101.83,0.00,400.00,0.207766,0.215969,0.227336,0.214758,null,null,null
+2020-09-02T20:24:49Z,26.72,60.85,99,0,33.50,101.83,0.00,400.00,0.209133,0.216391,0.227906,0.215250,null,null,null
+2020-09-02T20:25:19Z,26.71,60.84,99,0,29.21,101.83,0.00,400.00,0.207195,0.214781,0.228898,0.214914,null,null,null
+2020-09-02T20:25:49Z,26.72,60.82,99,0,35.26,101.83,0.00,400.00,0.209805,0.215680,0.227406,0.214180,null,null,null
+2020-09-02T20:26:19Z,26.73,60.87,99,0,31.19,101.83,0.00,400.00,0.208602,0.215266,0.227898,0.214398,null,null,null
+2020-09-02T20:26:49Z,26.71,60.89,99,0,30.56,101.83,0.00,400.00,0.208844,0.216164,0.228016,0.214516,null,null,null
+2020-09-02T20:27:19Z,26.68,60.86,99,0,26.03,101.83,0.00,400.00,0.209297,0.216789,0.229500,0.215094,null,null,null
+2020-09-02T20:27:49Z,26.71,60.92,99,0,25.19,101.83,0.00,400.00,0.209813,0.217055,0.228391,0.214469,null,null,null
+2020-09-02T20:28:19Z,26.71,60.90,99,0,45.17,101.83,0.00,400.00,0.208562,0.216398,0.229164,0.215367,null,null,null
+2020-09-02T20:28:49Z,26.71,60.87,99,0,29.61,101.83,0.00,400.00,0.208453,0.215805,0.227367,0.215555,null,null,null
+2020-09-02T20:29:19Z,26.72,60.87,99,0,27.42,101.83,0.00,400.00,0.209445,0.215852,0.228492,0.215266,null,null,null
+2020-09-02T20:29:49Z,26.72,60.86,99,0,27.22,101.83,0.00,400.00,0.209422,0.216438,0.227320,0.214648,null,null,null
+2020-09-02T20:30:19Z,26.71,60.84,99,0,30.30,101.83,0.00,400.00,0.209531,0.216945,0.227938,0.214484,null,null,null
+2020-09-02T20:30:49Z,26.69,60.84,99,0,27.30,101.83,0.00,400.00,0.208594,0.216195,0.227477,0.214703,null,null,null
+2020-09-02T20:31:19Z,26.72,60.91,99,0,26.62,101.83,0.00,400.00,0.208344,0.216523,0.227305,0.214563,null,null,null
+2020-09-02T20:31:49Z,26.72,60.90,99,0,33.72,101.83,0.00,400.00,0.210180,0.216438,0.226359,0.214687,null,null,null
+2020-09-02T20:32:19Z,26.69,60.87,99,0,28.06,101.84,0.00,400.00,0.209359,0.216172,0.226508,0.214648,null,null,null
+2020-09-02T20:32:49Z,26.71,60.90,99,0,29.05,101.83,0.00,400.00,0.208773,0.215508,0.227828,0.214375,null,null,null
+2020-09-02T20:33:19Z,26.71,60.86,99,0,32.30,101.84,0.00,400.00,0.208945,0.216680,0.227453,0.214312,null,null,null
+2020-09-02T20:33:49Z,26.69,60.86,99,0,28.70,101.84,0.00,400.00,0.209430,0.215680,0.227375,0.214883,null,null,null
+2020-09-02T20:34:19Z,26.72,60.89,99,0,27.28,101.84,0.00,400.00,0.209906,0.216570,0.226617,0.215273,null,null,null
+2020-09-02T20:34:49Z,26.71,60.89,99,0,27.06,101.84,0.00,400.00,0.209203,0.216609,0.226758,0.214398,null,null,null
+2020-09-02T20:35:19Z,26.72,60.87,99,0,29.41,101.84,0.00,402.00,0.209562,0.217453,0.230320,0.215547,null,null,null
+2020-09-02T20:35:49Z,26.72,60.86,99,0,27.84,101.84,0.00,402.00,0.209391,0.217219,0.228008,0.215422,null,null,null
+2020-09-02T20:36:19Z,26.72,60.86,99,0,50.97,101.84,0.00,402.00,0.206375,0.216906,0.227016,0.215305,null,null,null
+2020-09-02T20:36:49Z,26.73,60.85,99,0,29.50,101.84,0.00,402.00,0.209367,0.216805,0.226953,0.214859,null,null,null
+2020-09-02T20:37:19Z,26.72,60.86,99,0,26.46,101.84,0.00,400.00,0.211102,0.217266,0.228188,0.214352,null,null,null
+2020-09-02T20:37:49Z,26.71,60.83,99,0,33.62,101.84,0.00,400.00,0.208930,0.216508,0.227820,0.214750,null,null,null
+2020-09-02T20:38:19Z,26.73,60.83,99,0,26.99,101.84,0.00,400.00,0.208984,0.217039,0.227930,0.215289,null,null,null
+2020-09-02T20:38:49Z,26.69,60.89,99,0,28.27,101.84,0.00,400.00,0.210859,0.217164,0.227961,0.214766,null,null,null
+2020-09-02T20:39:19Z,26.71,60.90,99,0,36.91,101.84,0.00,400.00,0.209672,0.217797,0.226773,0.214539,null,null,null
+2020-09-02T20:39:49Z,26.71,60.82,99,0,28.17,101.85,0.00,400.00,0.210820,0.216688,0.228062,0.215234,null,null,null
+2020-09-02T20:40:19Z,26.72,60.82,99,0,28.68,101.84,0.00,400.00,0.208773,0.215687,0.228391,0.214852,null,null,null
+2020-09-02T20:40:49Z,26.72,60.84,99,0,24.65,101.84,0.00,400.00,0.209891,0.217719,0.228789,0.215484,null,null,null
+2020-09-02T20:41:19Z,26.73,60.87,99,0,27.28,101.84,0.00,400.00,0.209023,0.215859,0.228336,0.214813,null,null,null
+2020-09-02T20:41:49Z,26.72,60.86,99,0,26.16,101.84,0.00,400.00,0.210164,0.216266,0.229102,0.215047,null,null,null
+2020-09-02T20:42:19Z,26.71,60.85,99,0,25.73,101.84,0.00,400.00,0.208805,0.216625,0.226430,0.214305,null,null,null
+2020-09-02T20:42:49Z,26.72,60.80,99,0,32.94,101.85,0.00,400.00,0.209641,0.216531,0.227906,0.214727,null,null,null
+2020-09-02T20:43:19Z,26.71,60.84,99,0,28.50,101.85,0.00,403.00,0.209344,0.216477,0.227984,0.214648,null,null,null
+2020-09-02T20:43:49Z,26.73,60.83,99,0,27.49,101.84,0.00,403.00,0.210047,0.217344,0.227742,0.215656,null,null,null
+2020-09-02T20:44:19Z,26.73,60.86,99,0,32.37,101.85,0.00,403.00,0.208148,0.215344,0.225977,0.213734,null,null,null
+2020-09-02T20:44:49Z,26.72,60.85,99,0,38.05,101.85,0.00,403.00,0.207078,0.215781,0.227391,0.214719,null,null,null
+2020-09-02T20:45:19Z,26.72,60.82,99,0,39.45,101.85,0.00,403.00,0.209148,0.216172,0.227555,0.214422,null,null,null
+2020-09-02T20:45:49Z,26.73,60.81,99,0,41.65,101.85,0.00,403.00,0.210391,0.216945,0.228977,0.215148,null,null,null
+2020-09-02T20:46:19Z,26.69,60.82,99,0,26.26,101.85,0.00,403.00,0.208656,0.216180,0.227305,0.214805,null,null,null
+2020-09-02T20:46:49Z,26.72,60.81,99,0,27.16,101.85,0.00,403.00,0.210250,0.217086,0.227367,0.215172,null,null,null
+2020-09-02T20:47:19Z,26.72,60.82,99,0,27.60,101.85,4.00,428.00,0.208734,0.216484,0.225766,0.215125,null,null,null
+2020-09-02T20:47:49Z,26.73,60.83,99,0,26.46,101.85,4.00,428.00,0.209453,0.215844,0.227570,0.214766,null,null,null
+2020-09-02T20:48:19Z,26.73,60.83,99,0,31.35,101.85,3.00,424.00,0.209156,0.216312,0.226680,0.214906,null,null,null
+2020-09-02T20:48:49Z,26.72,60.85,99,0,29.84,101.85,3.00,424.00,0.211070,0.217180,0.228211,0.214602,null,null,null
+2020-09-02T20:49:19Z,26.72,60.85,99,0,27.62,101.85,4.00,428.00,0.208430,0.216359,0.228625,0.214648,null,null,null
+2020-09-02T20:49:49Z,26.73,60.82,99,0,26.55,101.85,4.00,428.00,0.209445,0.217406,0.226711,0.215219,null,null,null
+2020-09-02T20:50:19Z,26.71,60.83,99,0,26.60,101.85,3.00,424.00,0.207867,0.216000,0.229125,0.214992,null,null,null
+2020-09-02T20:50:49Z,26.72,60.83,99,0,37.48,101.85,3.00,424.00,0.208078,0.216781,0.227867,0.214664,null,null,null
+2020-09-02T20:51:19Z,26.71,60.82,99,0,28.60,101.85,4.00,428.00,0.209992,0.217281,0.228188,0.215469,null,null,null
+2020-09-02T20:51:49Z,26.72,60.83,99,0,27.08,101.85,4.00,428.00,0.208359,0.215680,0.227625,0.213656,null,null,null
+2020-09-02T20:52:19Z,26.72,60.83,99,0,36.21,101.85,3.00,424.00,0.210328,0.216695,0.229320,0.215328,null,null,null
+2020-09-02T20:52:49Z,26.72,60.83,99,0,27.42,101.85,3.00,424.00,0.207312,0.216500,0.226906,0.214336,null,null,null
+2020-09-02T20:53:19Z,26.72,60.81,99,0,27.66,101.85,3.00,424.00,0.209922,0.216953,0.227305,0.215297,null,null,null
+2020-09-02T20:53:49Z,26.71,60.77,99,0,33.46,101.85,3.00,424.00,0.208406,0.215875,0.226953,0.214578,null,null,null
+2020-09-02T20:54:19Z,26.71,60.80,99,0,25.03,101.85,3.00,424.00,0.209172,0.216344,0.227211,0.215562,null,null,null
+2020-09-02T20:54:49Z,26.72,60.85,99,0,25.19,101.86,3.00,424.00,0.208687,0.216734,0.228547,0.215453,null,null,null
+2020-09-02T20:55:19Z,26.72,60.81,99,0,27.40,101.85,4.00,428.00,0.208719,0.216984,0.228844,0.215438,null,null,null
+2020-09-02T20:55:49Z,26.71,60.82,99,0,29.01,101.85,4.00,428.00,0.209250,0.216391,0.227633,0.215578,null,null,null
+2020-09-02T20:56:19Z,26.71,60.86,99,0,33.32,101.85,4.00,428.00,0.209195,0.216422,0.227094,0.214477,null,null,null
+2020-09-02T20:56:49Z,26.72,60.79,99,0,37.93,101.85,4.00,428.00,0.208703,0.215625,0.227727,0.215156,null,null,null
+2020-09-02T20:57:19Z,26.71,60.81,99,0,39.76,101.85,3.00,422.00,0.209484,0.216797,0.229594,0.214586,null,null,null
+2020-09-02T20:57:49Z,26.72,60.81,99,0,30.31,101.85,3.00,422.00,0.210117,0.216461,0.226156,0.214461,null,null,null
+2020-09-02T20:58:19Z,26.71,60.79,99,0,29.90,101.85,5.00,434.00,0.210781,0.217242,0.226008,0.214352,null,null,null
+2020-09-02T20:58:49Z,26.71,60.80,99,0,41.31,101.85,5.00,434.00,0.208844,0.216859,0.227313,0.214781,null,null,null
+2020-09-02T20:59:19Z,26.72,60.85,99,0,26.55,101.85,3.00,424.00,0.210781,0.216820,0.227695,0.214539,null,null,null
+2020-09-02T20:59:49Z,26.72,60.82,99,0,27.42,101.85,3.00,424.00,0.208500,0.216930,0.227023,0.215062,null,null,null
+2020-09-02T21:00:19Z,26.69,60.80,99,0,33.66,101.85,5.00,434.00,0.210219,0.218047,0.229445,0.214852,null,null,null
+2020-09-02T21:00:49Z,26.71,60.80,99,0,32.42,101.85,5.00,434.00,0.208930,0.216469,0.228906,0.215227,null,null,null
+2020-09-02T21:01:19Z,26.73,60.81,99,0,28.51,101.85,3.00,424.00,0.210773,0.217406,0.228117,0.214570,null,null,null
+2020-09-02T21:01:49Z,26.69,60.78,99,0,31.35,101.85,3.00,424.00,0.208805,0.215969,0.227836,0.215000,null,null,null
+2020-09-02T21:02:19Z,26.72,60.80,99,0,42.70,101.85,3.00,424.00,0.209734,0.217578,0.228734,0.214953,null,null,null
+2020-09-02T21:02:49Z,26.72,60.83,99,0,32.68,101.85,3.00,424.00,0.208703,0.217203,0.227398,0.214547,null,null,null
+2020-09-02T21:03:19Z,26.71,60.80,99,0,27.80,101.85,3.00,424.00,0.210406,0.217266,0.227875,0.214367,null,null,null
+2020-09-02T21:03:49Z,26.71,60.81,99,0,27.62,101.85,3.00,424.00,0.210406,0.217273,0.227281,0.214945,null,null,null
+2020-09-02T21:04:19Z,26.71,60.82,99,0,26.71,101.85,5.00,434.00,0.209523,0.216102,0.227484,0.215016,null,null,null
+2020-09-02T21:04:49Z,26.73,60.80,99,0,27.26,101.85,5.00,434.00,0.210336,0.217250,0.230086,0.215625,null,null,null
+2020-09-02T21:05:19Z,26.71,60.79,99,0,28.28,101.86,5.00,434.00,0.208586,0.216070,0.228906,0.215023,null,null,null
+2020-09-02T21:05:49Z,26.69,60.80,99,0,27.94,101.85,5.00,434.00,0.210008,0.216484,0.228000,0.215547,null,null,null
+2020-09-02T21:06:19Z,26.69,60.75,99,0,31.34,101.86,4.00,428.00,0.208969,0.216523,0.228062,0.215742,null,null,null
+2020-09-02T21:06:49Z,26.71,60.83,99,0,27.42,101.85,4.00,428.00,0.208531,0.216906,0.229031,0.215687,null,null,null
+2020-09-02T21:07:19Z,26.73,60.77,99,0,27.77,101.85,4.00,428.00,0.209531,0.216289,0.226242,0.214336,null,null,null
+2020-09-02T21:07:49Z,26.73,60.81,99,0,27.71,101.85,4.00,428.00,0.209320,0.216523,0.228078,0.214781,null,null,null
+2020-09-02T21:08:19Z,26.72,60.80,99,0,30.29,101.85,4.00,428.00,0.209586,0.217227,0.228758,0.215984,null,null,null
+2020-09-02T21:08:49Z,26.71,60.83,99,0,27.89,101.85,4.00,428.00,0.208047,0.216711,0.226234,0.214109,null,null,null
+2020-09-02T21:09:19Z,26.72,60.81,99,0,30.78,101.86,3.00,424.00,0.208961,0.216227,0.227047,0.215047,null,null,null
+2020-09-02T21:09:49Z,26.69,60.79,99,0,28.17,101.86,3.00,424.00,0.209047,0.216422,0.228453,0.215461,null,null,null
+2020-09-02T21:10:19Z,26.71,60.80,99,0,28.78,101.86,3.00,424.00,0.211406,0.216227,0.228172,0.215148,null,null,null
+2020-09-02T21:10:49Z,26.71,60.81,99,0,29.04,101.86,3.00,424.00,0.208586,0.217023,0.226703,0.215445,null,null,null
+2020-09-02T21:11:19Z,26.71,60.81,99,0,31.60,101.86,3.00,424.00,0.209258,0.215844,0.229563,0.215312,null,null,null
+2020-09-02T21:11:49Z,26.72,60.79,99,0,30.42,101.86,3.00,424.00,0.208750,0.216406,0.230023,0.215008,null,null,null
+2020-09-02T21:12:19Z,26.71,60.78,99,0,27.96,101.86,3.00,424.00,0.208203,0.216570,0.227266,0.215141,null,null,null
+2020-09-02T21:12:49Z,26.72,60.76,99,0,24.03,101.86,3.00,424.00,0.208914,0.216508,0.229438,0.215852,null,null,null
+2020-09-02T21:13:19Z,26.68,60.81,99,0,27.38,101.87,5.00,434.00,0.209688,0.217211,0.225828,0.214367,null,null,null
+2020-09-02T21:13:49Z,26.72,60.81,99,0,29.13,101.86,5.00,434.00,0.210945,0.218211,0.226859,0.214703,null,null,null
+2020-09-02T21:14:19Z,26.71,60.79,99,0,26.55,101.87,5.00,434.00,0.208641,0.216477,0.228437,0.215047,null,null,null
+2020-09-02T21:14:49Z,26.69,60.76,99,0,25.95,101.87,5.00,434.00,0.209164,0.216117,0.229430,0.215953,null,null,null
+2020-09-02T21:15:19Z,26.69,60.82,99,0,27.08,101.87,4.00,428.00,0.208258,0.215453,0.228148,0.214977,null,null,null
+2020-09-02T21:15:49Z,26.69,60.79,99,0,27.14,101.87,4.00,428.00,0.209891,0.216805,0.227414,0.214406,null,null,null
+2020-09-02T21:16:19Z,26.71,60.78,99,0,27.99,101.87,4.00,428.00,0.209531,0.216609,0.228680,0.214914,null,null,null
+2020-09-02T21:16:49Z,26.71,60.83,99,0,27.90,101.87,4.00,428.00,0.210383,0.217398,0.228133,0.215492,null,null,null
+2020-09-02T21:17:19Z,26.73,60.80,99,0,28.23,101.87,4.00,428.00,0.209609,0.217461,0.228414,0.214711,null,null,null
+2020-09-02T21:17:49Z,26.71,60.74,99,0,30.60,101.87,4.00,428.00,0.209398,0.217570,0.228617,0.215484,null,null,null
+2020-09-02T21:18:19Z,26.72,60.76,99,0,25.09,101.87,4.00,428.00,0.210609,0.218133,0.228352,0.215406,null,null,null
+2020-09-02T21:18:49Z,26.71,60.79,99,0,29.28,101.87,4.00,428.00,0.210406,0.217242,0.227141,0.214617,null,null,null
+2020-09-02T21:19:19Z,26.72,60.77,99,0,28.66,101.87,4.00,428.00,0.208750,0.216516,0.228781,0.215258,null,null,null
+2020-09-02T21:19:49Z,26.71,60.77,99,0,27.32,101.87,4.00,428.00,0.210320,0.216891,0.225883,0.214766,null,null,null
+2020-09-02T21:20:19Z,26.69,60.79,99,0,26.00,101.87,4.00,428.00,0.210047,0.216914,0.226914,0.213961,null,null,null
+2020-09-02T21:20:49Z,26.69,60.76,99,0,30.44,101.87,4.00,428.00,0.210648,0.217586,0.228555,0.215055,null,null,null
+2020-09-02T21:21:19Z,26.72,60.84,99,0,28.15,101.87,3.00,424.00,0.209094,0.216937,0.230297,0.215656,null,null,null
+2020-09-02T21:21:49Z,26.69,60.84,99,0,33.63,101.87,3.00,424.00,0.209172,0.215789,0.229375,0.214828,null,null,null
+2020-09-02T21:22:19Z,26.69,60.81,99,0,28.55,101.87,4.00,428.00,0.209063,0.216359,0.229414,0.215477,null,null,null
+2020-09-02T21:22:49Z,26.71,60.81,99,0,31.48,101.87,4.00,428.00,0.209273,0.216805,0.229102,0.215672,null,null,null
+2020-09-02T21:23:19Z,26.71,60.80,99,0,27.85,101.87,5.00,434.00,0.207617,0.217320,0.228563,0.215086,null,null,null
+2020-09-02T21:23:49Z,26.72,60.83,99,0,32.42,101.87,5.00,434.00,0.210203,0.216320,0.229734,0.215492,null,null,null
+2020-09-02T21:24:19Z,26.71,60.80,99,0,26.95,101.88,4.00,428.00,0.208570,0.215867,0.227070,0.214961,null,null,null
+2020-09-02T21:24:49Z,26.73,60.77,99,0,29.68,101.88,4.00,428.00,0.210734,0.216664,0.227867,0.215297,null,null,null
+2020-09-02T21:25:19Z,26.69,60.80,99,0,37.26,101.88,3.00,424.00,0.210680,0.217359,0.228766,0.215531,null,null,null
+2020-09-02T21:25:49Z,26.73,60.77,99,0,26.60,101.88,3.00,424.00,0.209813,0.216750,0.226734,0.214414,null,null,null
+2020-09-02T21:26:19Z,26.72,60.76,99,0,26.82,101.88,5.00,434.00,0.210063,0.217367,0.226305,0.214922,null,null,null
+2020-09-02T21:26:49Z,26.72,60.75,99,0,32.89,101.88,5.00,434.00,0.209266,0.217148,0.228641,0.215547,null,null,null
+2020-09-02T21:27:19Z,26.71,60.77,99,0,29.72,101.88,5.00,434.00,0.208555,0.217250,0.228813,0.215453,null,null,null
+2020-09-02T21:27:49Z,26.69,60.76,99,0,30.57,101.88,5.00,434.00,0.208219,0.215531,0.228813,0.215570,null,null,null
+2020-09-02T21:28:19Z,26.72,60.71,99,0,28.25,101.88,4.00,428.00,0.209672,0.217891,0.226797,0.214680,null,null,null
+2020-09-02T21:28:49Z,26.71,60.78,99,0,28.89,101.88,4.00,428.00,0.209094,0.216102,0.228398,0.215273,null,null,null
+2020-09-02T21:29:19Z,26.69,60.75,99,0,31.28,101.88,4.00,428.00,0.208773,0.215445,0.230203,0.214898,null,null,null
+2020-09-02T21:29:49Z,26.69,60.76,99,0,26.57,101.88,4.00,428.00,0.210477,0.217000,0.228477,0.215234,null,null,null
+2020-09-02T21:30:19Z,26.71,60.77,99,0,25.92,101.88,5.00,434.00,0.211031,0.216781,0.229969,0.215898,null,null,null
+2020-09-02T21:30:49Z,26.68,60.76,99,0,39.18,101.88,5.00,434.00,0.209180,0.216648,0.227250,0.214297,null,null,null
+2020-09-02T21:31:19Z,26.71,60.77,99,0,26.38,101.88,5.00,435.00,0.209648,0.216930,0.226812,0.214437,null,null,null
+2020-09-02T21:31:49Z,26.71,60.79,99,0,27.62,101.88,5.00,435.00,0.208414,0.216141,0.228563,0.215961,null,null,null
+2020-09-02T21:32:19Z,26.71,60.74,99,0,31.86,101.88,4.00,428.00,0.209562,0.216703,0.228445,0.214828,null,null,null
+2020-09-02T21:32:49Z,26.71,60.77,99,0,29.30,101.88,4.00,428.00,0.211258,0.217500,0.227461,0.215195,null,null,null
+2020-09-02T21:33:19Z,26.69,60.76,99,0,27.99,101.88,5.00,434.00,0.209516,0.217305,0.227273,0.214992,null,null,null
+2020-09-02T21:33:49Z,26.71,60.80,99,0,40.89,101.88,5.00,434.00,0.210719,0.217477,0.228188,0.214844,null,null,null
+2020-09-02T21:34:19Z,26.71,60.76,99,0,26.57,101.88,5.00,435.00,0.209367,0.216680,0.228406,0.214836,null,null,null
+2020-09-02T21:34:49Z,26.71,60.76,99,0,28.20,101.88,5.00,435.00,0.210562,0.216984,0.228836,0.215117,null,null,null
+2020-09-02T21:35:19Z,26.71,60.78,99,0,36.26,101.88,5.00,435.00,0.208242,0.217219,0.228391,0.215328,null,null,null
+2020-09-02T21:35:49Z,26.66,60.77,99,0,29.00,101.88,5.00,435.00,0.210344,0.217023,0.229211,0.215664,null,null,null
+2020-09-02T21:36:19Z,26.71,60.78,99,0,27.10,101.88,5.00,434.00,0.208148,0.216906,0.227922,0.215195,null,null,null
+2020-09-02T21:36:49Z,26.71,60.76,99,0,31.85,101.88,5.00,434.00,0.209898,0.216844,0.228437,0.215352,null,null,null
+2020-09-02T21:37:19Z,26.71,60.75,99,0,40.83,101.88,5.00,434.00,0.208562,0.216023,0.228117,0.214656,null,null,null
+2020-09-02T21:37:49Z,26.71,60.77,99,0,27.73,101.88,5.00,434.00,0.210164,0.216195,0.225977,0.214102,null,null,null
+2020-09-02T21:38:19Z,26.69,60.71,99,0,29.49,101.88,5.00,434.00,0.209969,0.217586,0.226977,0.214469,null,null,null
+2020-09-02T21:38:49Z,26.71,60.73,99,0,28.91,101.88,5.00,434.00,0.210773,0.218117,0.229070,0.215805,null,null,null
+2020-09-02T21:39:19Z,26.73,60.77,99,0,27.49,101.88,5.00,439.00,0.209586,0.216328,0.228672,0.215430,null,null,null
+2020-09-02T21:39:49Z,26.68,60.72,99,0,30.47,101.88,5.00,439.00,0.207914,0.215719,0.229281,0.216125,null,null,null
+2020-09-02T21:40:19Z,26.68,60.79,99,0,33.80,101.88,5.00,439.00,0.210109,0.217117,0.227617,0.214148,null,null,null
+2020-09-02T21:40:49Z,26.68,60.80,99,0,27.84,101.88,5.00,439.00,0.210531,0.217484,0.227023,0.214617,null,null,null
+2020-09-02T21:41:19Z,26.69,60.74,99,0,39.36,101.88,5.00,434.00,0.210523,0.217430,0.227328,0.215312,null,null,null
+2020-09-02T21:41:49Z,26.69,60.79,99,0,29.36,101.88,5.00,434.00,0.210328,0.216242,0.226469,0.215148,null,null,null
+2020-09-02T21:42:19Z,26.72,60.75,99,0,28.01,101.88,6.00,441.00,0.208766,0.216797,0.228047,0.214281,null,null,null
+2020-09-02T21:42:49Z,26.69,60.80,99,0,27.30,101.89,6.00,441.00,0.211063,0.217719,0.227578,0.215039,null,null,null
+2020-09-02T21:43:19Z,26.68,60.80,99,0,27.08,101.88,6.00,445.00,0.210133,0.216781,0.228164,0.215367,null,null,null
+2020-09-02T21:43:49Z,26.71,60.76,99,0,28.71,101.88,6.00,445.00,0.207891,0.216984,0.228523,0.215570,null,null,null
+2020-09-02T21:44:19Z,26.71,60.81,99,0,27.02,101.88,5.00,434.00,0.210016,0.217023,0.227383,0.215094,null,null,null
+2020-09-02T21:44:49Z,26.69,60.77,99,0,26.73,101.88,5.00,434.00,0.209156,0.217047,0.228914,0.215078,null,null,null
+2020-09-02T21:45:19Z,26.72,60.74,99,0,26.43,101.88,6.00,445.00,0.207906,0.215086,0.228148,0.215148,null,null,null
+2020-09-02T21:45:49Z,26.72,60.79,99,0,27.77,101.88,6.00,445.00,0.209883,0.216758,0.228352,0.215086,null,null,null
+2020-09-02T21:46:19Z,26.69,60.75,99,0,28.61,101.88,6.00,445.00,0.209453,0.217055,0.228563,0.215453,null,null,null
+2020-09-02T21:46:49Z,26.68,60.70,99,0,28.84,101.88,6.00,445.00,0.207742,0.216172,0.228570,0.215867,null,null,null
+2020-09-02T21:47:19Z,26.72,60.73,99,0,26.89,101.89,7.00,450.00,0.209187,0.216078,0.229625,0.215641,null,null,null
+2020-09-02T21:47:49Z,26.71,60.73,99,0,26.31,101.88,7.00,450.00,0.210086,0.217344,0.228250,0.215266,null,null,null
+2020-09-02T21:48:19Z,26.72,60.77,99,0,34.83,101.89,7.00,450.00,0.209766,0.216289,0.226805,0.214516,null,null,null
+2020-09-02T21:48:49Z,26.69,60.76,99,0,26.34,101.89,7.00,450.00,0.208891,0.217172,0.228258,0.214602,null,null,null
+2020-09-02T21:49:19Z,26.71,60.75,99,0,27.22,101.89,7.00,448.00,0.210727,0.216117,0.228156,0.215086,null,null,null
+2020-09-02T21:49:49Z,26.71,60.74,99,0,37.59,101.89,7.00,448.00,0.210125,0.217508,0.227812,0.214953,null,null,null
+2020-09-02T21:50:19Z,26.72,60.77,99,0,26.41,101.89,7.00,448.00,0.210797,0.216391,0.227445,0.214813,null,null,null
+2020-09-02T21:50:49Z,26.69,60.74,99,0,24.93,101.89,7.00,448.00,0.211836,0.217844,0.229445,0.215453,null,null,null
+2020-09-02T21:51:19Z,26.69,60.70,99,0,26.43,101.89,7.00,448.00,0.208781,0.216539,0.229383,0.215305,null,null,null
+2020-09-02T21:51:49Z,26.69,60.73,99,0,28.51,101.89,7.00,448.00,0.209336,0.216750,0.229484,0.216102,null,null,null
+2020-09-02T21:52:19Z,26.71,60.71,99,0,25.59,101.88,8.00,454.00,0.208258,0.215625,0.227094,0.214195,null,null,null
+2020-09-02T21:52:49Z,26.72,60.75,99,0,26.97,101.89,8.00,454.00,0.209141,0.217258,0.228109,0.215203,null,null,null
+2020-09-02T21:53:19Z,26.72,60.77,99,0,26.82,101.89,8.00,459.00,0.208961,0.217633,0.229586,0.215766,null,null,null
+2020-09-02T21:53:49Z,26.69,60.72,99,0,27.51,101.89,8.00,459.00,0.208930,0.215953,0.228047,0.215453,null,null,null
+2020-09-02T21:54:19Z,26.71,60.73,99,0,32.14,101.89,7.00,448.00,0.209414,0.216836,0.227266,0.215023,null,null,null
+2020-09-02T21:54:49Z,26.69,60.75,99,0,36.11,101.89,7.00,448.00,0.210180,0.216734,0.228109,0.215180,null,null,null
+2020-09-02T21:55:19Z,26.69,60.76,99,0,26.87,101.89,8.00,459.00,0.209195,0.216609,0.227617,0.215219,null,null,null
+2020-09-02T21:55:49Z,26.71,60.75,99,0,28.76,101.89,8.00,459.00,0.209484,0.216695,0.228836,0.215562,null,null,null
+2020-09-02T21:56:19Z,26.69,60.73,99,0,26.57,101.89,8.00,454.00,0.209742,0.216594,0.228266,0.215320,null,null,null
+2020-09-02T21:56:49Z,26.71,60.74,99,0,26.82,101.89,8.00,454.00,0.209203,0.217055,0.229375,0.215414,null,null,null
+2020-09-02T21:57:19Z,26.71,60.73,99,0,30.16,101.89,8.00,459.00,0.209344,0.216367,0.228719,0.215633,null,null,null
+2020-09-02T21:57:49Z,26.69,60.72,99,0,27.45,101.89,8.00,459.00,0.208070,0.216656,0.226906,0.214633,null,null,null
+2020-09-02T21:58:19Z,26.68,60.82,99,0,26.93,101.89,8.00,459.00,0.211234,0.217672,0.227516,0.215062,null,null,null
+2020-09-02T21:58:49Z,26.68,60.79,99,0,26.57,101.89,8.00,459.00,0.208953,0.217063,0.225406,0.214070,null,null,null
+2020-09-02T21:59:19Z,26.71,60.75,99,0,29.04,101.89,8.00,459.00,0.209734,0.216711,0.226766,0.215727,null,null,null
+2020-09-02T21:59:49Z,26.68,60.69,99,0,26.14,101.89,8.00,459.00,0.208102,0.216297,0.227891,0.215172,null,null,null
+2020-09-02T22:00:19Z,26.69,60.70,99,0,28.06,101.89,8.00,454.00,0.208664,0.216945,0.228172,0.215539,null,null,null
+2020-09-02T22:00:49Z,26.69,60.76,99,0,28.47,101.90,8.00,454.00,0.209937,0.216781,0.227812,0.215352,null,null,null
+2020-09-02T22:01:19Z,26.71,60.71,99,0,25.76,101.90,8.00,459.00,0.209484,0.216273,0.227742,0.215133,null,null,null
+2020-09-02T22:01:49Z,26.69,60.71,99,0,26.31,101.90,8.00,459.00,0.210492,0.216813,0.228008,0.214398,null,null,null
+2020-09-02T22:02:19Z,26.69,60.70,99,0,25.59,101.90,10.00,470.00,0.209852,0.216961,0.228055,0.215398,null,null,null
+2020-09-02T22:02:49Z,26.66,60.69,99,0,39.59,101.90,10.00,470.00,0.208813,0.216156,0.227500,0.214398,null,null,null
+2020-09-02T22:03:19Z,26.69,60.69,99,0,28.34,101.90,10.00,470.00,0.209211,0.217102,0.228813,0.215023,null,null,null
+2020-09-02T22:03:49Z,26.71,60.67,99,0,28.39,101.90,10.00,470.00,0.208891,0.216898,0.227812,0.215258,null,null,null
+2020-09-02T22:04:19Z,26.69,60.74,99,0,28.25,101.90,10.00,470.00,0.209094,0.217211,0.229312,0.215641,null,null,null
+2020-09-02T22:04:49Z,26.69,60.70,99,0,27.55,101.90,10.00,470.00,0.208430,0.216609,0.227109,0.215406,null,null,null
+2020-09-02T22:05:19Z,26.69,60.70,99,0,29.03,101.90,8.00,459.00,0.209453,0.216734,0.227820,0.215172,null,null,null
+2020-09-02T22:05:49Z,26.69,60.71,99,0,29.16,101.90,8.00,459.00,0.209898,0.217867,0.229469,0.215367,null,null,null
+2020-09-02T22:06:19Z,26.71,60.77,99,0,27.85,101.90,10.00,470.00,0.209906,0.218539,0.227883,0.215125,null,null,null
+2020-09-02T22:06:49Z,26.69,60.77,99,0,28.61,101.90,10.00,470.00,0.208055,0.216484,0.229133,0.214883,null,null,null
+2020-09-02T22:07:19Z,26.69,60.67,99,0,27.92,101.90,10.00,470.00,0.209047,0.217141,0.228258,0.215680,null,null,null
+2020-09-02T22:07:49Z,26.68,60.72,99,0,27.30,101.90,10.00,470.00,0.208203,0.217414,0.227477,0.215016,null,null,null
+2020-09-02T22:08:19Z,26.69,60.71,99,0,31.69,101.90,10.00,470.00,0.209539,0.217055,0.228766,0.214312,null,null,null
+2020-09-02T22:08:49Z,26.65,60.68,99,0,26.24,101.90,10.00,470.00,0.208547,0.215984,0.227078,0.215297,null,null,null
+2020-09-02T22:09:19Z,26.68,60.70,99,0,30.99,101.91,10.00,470.00,0.209133,0.217523,0.226437,0.215289,null,null,null
+2020-09-02T22:09:49Z,26.68,60.75,99,0,26.53,101.91,10.00,470.00,0.208367,0.216242,0.229148,0.215422,null,null,null
+2020-09-02T22:10:19Z,26.71,60.75,99,0,26.21,101.91,10.00,470.00,0.210984,0.217852,0.228164,0.214383,null,null,null
+2020-09-02T22:10:49Z,26.69,60.73,99,0,27.89,101.90,10.00,470.00,0.209648,0.216813,0.228414,0.214883,null,null,null
+2020-09-02T22:11:19Z,26.71,60.70,99,0,25.87,101.91,10.00,470.00,0.208813,0.216109,0.227617,0.215547,null,null,null
+2020-09-02T22:11:49Z,26.72,60.71,99,0,25.73,101.91,10.00,470.00,0.210805,0.218906,0.227070,0.215500,null,null,null
+2020-09-02T22:12:19Z,26.69,60.68,99,0,29.58,101.91,12.00,480.00,0.211086,0.217594,0.228734,0.215109,null,null,null
+2020-09-02T22:12:49Z,26.65,60.70,99,0,26.11,101.91,12.00,480.00,0.208602,0.217836,0.227336,0.215188,null,null,null
+2020-09-02T22:13:19Z,26.68,60.66,99,0,26.55,101.91,12.00,480.00,0.210109,0.217336,0.226055,0.214492,null,null,null
+2020-09-02T22:13:49Z,26.69,60.71,99,0,27.34,101.91,12.00,480.00,0.209508,0.217734,0.229578,0.215469,null,null,null
+2020-09-02T22:14:19Z,26.69,60.68,99,0,26.11,101.91,12.00,480.00,0.210570,0.216562,0.229656,0.215148,null,null,null
+2020-09-02T22:14:49Z,26.68,60.73,99,0,26.95,101.91,12.00,480.00,0.210133,0.216711,0.228578,0.215344,null,null,null
+2020-09-02T22:15:19Z,26.66,60.68,99,0,27.75,101.91,11.00,476.00,0.209609,0.216727,0.226453,0.215625,null,null,null
+2020-09-02T22:15:49Z,26.71,60.66,99,0,26.87,101.91,11.00,476.00,0.209234,0.216836,0.228039,0.214906,null,null,null
+2020-09-02T22:16:19Z,26.71,60.70,99,0,31.86,101.91,12.00,480.00,0.208727,0.215531,0.226562,0.214953,null,null,null
+2020-09-02T22:16:49Z,26.71,60.68,99,0,28.17,101.91,12.00,480.00,0.208813,0.216977,0.228969,0.215359,null,null,null
+2020-09-02T22:17:19Z,26.71,60.69,99,0,28.37,101.91,12.00,480.00,0.209695,0.217492,0.227719,0.214977,null,null,null
+2020-09-02T22:17:49Z,26.69,60.71,99,0,29.62,101.91,12.00,480.00,0.210750,0.216617,0.227141,0.214695,null,null,null
+2020-09-02T22:18:19Z,26.66,60.72,99,0,29.31,101.91,11.00,476.00,0.209656,0.216758,0.228047,0.215227,null,null,null
+2020-09-02T22:18:49Z,26.71,60.67,99,0,25.65,101.91,11.00,476.00,0.209766,0.217383,0.228352,0.215414,null,null,null
+2020-09-02T22:19:19Z,26.69,60.70,99,0,28.12,101.91,13.00,486.00,0.209391,0.216391,0.227969,0.215023,null,null,null
+2020-09-02T22:19:49Z,26.68,60.68,99,0,27.73,101.92,13.00,486.00,0.210109,0.216555,0.229258,0.214828,null,null,null
+2020-09-02T22:20:19Z,26.71,60.68,99,0,27.28,101.92,13.00,486.00,0.208453,0.218070,0.228180,0.215484,null,null,null
+2020-09-02T22:20:49Z,26.68,60.72,99,0,26.99,101.92,13.00,486.00,0.209656,0.217625,0.230500,0.215047,null,null,null
+2020-09-02T22:21:19Z,26.68,60.70,99,0,28.15,101.92,13.00,486.00,0.209039,0.217766,0.227891,0.215172,null,null,null
+2020-09-02T22:21:49Z,26.68,60.74,99,0,26.91,101.92,13.00,486.00,0.209344,0.216258,0.228672,0.215406,null,null,null
+2020-09-02T22:22:19Z,26.71,60.76,99,0,28.15,101.92,14.00,492.00,0.208703,0.215820,0.226844,0.215273,null,null,null
+2020-09-02T22:22:49Z,26.69,60.73,99,0,25.59,101.92,14.00,492.00,0.209711,0.216805,0.229898,0.215891,null,null,null
+2020-09-02T22:23:19Z,26.68,60.74,99,0,24.83,101.92,13.00,486.00,0.209609,0.217336,0.227633,0.215391,null,null,null
+2020-09-02T22:23:49Z,26.68,60.74,99,0,29.32,101.92,13.00,486.00,0.209734,0.216461,0.227750,0.215273,null,null,null
+2020-09-02T22:24:19Z,26.68,60.67,99,0,27.64,101.92,12.00,480.00,0.209250,0.216992,0.228719,0.215828,null,null,null
+2020-09-02T22:24:49Z,26.68,60.71,99,0,27.16,101.93,12.00,480.00,0.210305,0.217852,0.226891,0.215211,null,null,null
+2020-09-02T22:25:19Z,26.66,60.72,99,0,27.32,101.92,14.00,492.00,0.211047,0.217781,0.227984,0.215258,null,null,null
+2020-09-02T22:25:49Z,26.69,60.71,99,0,27.78,101.92,14.00,492.00,0.210375,0.219086,0.227789,0.214805,null,null,null
+2020-09-02T22:26:19Z,26.65,60.71,99,0,29.27,101.92,14.00,492.00,0.209602,0.216922,0.228352,0.214898,null,null,null
+2020-09-02T22:26:49Z,26.68,60.72,99,0,33.66,101.92,14.00,492.00,0.209695,0.216055,0.228414,0.214547,null,null,null
+2020-09-02T22:27:19Z,26.66,60.71,99,0,25.82,101.93,14.00,492.00,0.209391,0.217125,0.227695,0.214758,null,null,null
+2020-09-02T22:27:49Z,26.69,60.71,99,0,29.82,101.93,14.00,492.00,0.208820,0.216820,0.228008,0.216102,null,null,null
+2020-09-02T22:28:19Z,26.68,60.75,99,0,37.01,101.93,13.00,486.00,0.211055,0.218023,0.229836,0.216578,null,null,null
+2020-09-02T22:28:49Z,26.66,60.73,99,0,26.87,101.93,13.00,486.00,0.211430,0.216727,0.226930,0.214273,null,null,null
+2020-09-02T22:29:19Z,26.66,60.72,99,0,27.36,101.93,13.00,486.00,0.209805,0.217195,0.227016,0.215227,null,null,null
+2020-09-02T22:29:49Z,26.69,60.73,99,0,27.20,101.92,13.00,486.00,0.210203,0.217375,0.227859,0.214742,null,null,null
+2020-09-02T22:30:19Z,26.66,60.73,99,0,28.63,101.93,14.00,492.00,0.208922,0.216977,0.227750,0.215195,null,null,null
+2020-09-02T22:30:49Z,26.69,60.73,99,0,27.40,101.93,14.00,492.00,0.207891,0.216906,0.228617,0.215039,null,null,null
+2020-09-02T22:31:19Z,26.69,60.75,99,0,27.32,101.93,13.00,486.00,0.210688,0.217711,0.228695,0.215273,null,null,null
+2020-09-02T22:31:49Z,26.66,60.70,99,0,29.89,101.93,13.00,486.00,0.209781,0.216703,0.228352,0.215297,null,null,null
+2020-09-02T22:32:19Z,26.69,60.73,99,0,26.84,101.93,14.00,496.00,0.211375,0.217141,0.227609,0.215000,null,null,null
+2020-09-02T22:32:49Z,26.69,60.73,99,0,30.55,101.93,14.00,496.00,0.210227,0.216609,0.227516,0.215695,null,null,null
+2020-09-02T22:33:19Z,26.68,60.69,99,0,24.93,101.93,14.00,496.00,0.210625,0.217258,0.229266,0.215594,null,null,null
+2020-09-02T22:33:49Z,26.68,60.70,99,0,27.12,101.93,14.00,496.00,0.210648,0.217648,0.229281,0.215609,null,null,null
+2020-09-02T22:34:19Z,26.69,60.75,99,0,29.17,101.93,14.00,492.00,0.210047,0.217117,0.227961,0.215359,null,null,null
+2020-09-02T22:34:49Z,26.68,60.71,99,0,29.26,101.93,14.00,492.00,0.206883,0.216078,0.227375,0.215195,null,null,null
+2020-09-02T22:35:19Z,26.66,60.72,99,0,27.96,101.93,14.00,496.00,0.211797,0.218156,0.227328,0.215547,null,null,null
+2020-09-02T22:35:49Z,26.66,60.77,99,0,28.22,101.93,14.00,496.00,0.209617,0.215672,0.228617,0.215500,null,null,null
+2020-09-02T22:36:19Z,26.66,60.73,99,0,26.71,101.93,14.00,492.00,0.209187,0.216680,0.227836,0.214687,null,null,null
+2020-09-02T22:36:49Z,26.68,60.74,99,0,28.34,101.93,14.00,492.00,0.210086,0.216102,0.228945,0.214281,null,null,null
+2020-09-02T22:37:19Z,26.69,60.72,99,0,26.06,101.93,14.00,496.00,0.209211,0.216445,0.227789,0.215953,null,null,null
+2020-09-02T22:37:49Z,26.69,60.72,99,0,26.78,101.93,14.00,496.00,0.209531,0.216750,0.228406,0.215258,null,null,null
+2020-09-02T22:38:19Z,26.65,60.72,99,0,26.53,101.93,14.00,492.00,0.210703,0.218203,0.227531,0.215117,null,null,null
+2020-09-02T22:38:49Z,26.68,60.69,99,0,27.12,101.93,14.00,492.00,0.209187,0.217438,0.228719,0.215523,null,null,null
+2020-09-02T22:39:19Z,26.68,60.72,99,0,27.75,101.93,14.00,496.00,0.210562,0.217141,0.229133,0.215273,null,null,null
+2020-09-02T22:39:49Z,26.69,60.75,99,0,25.84,101.93,14.00,496.00,0.209305,0.217078,0.226930,0.214914,null,null,null
+2020-09-02T22:40:19Z,26.68,60.69,99,0,24.58,101.93,14.00,492.00,0.210828,0.218484,0.227117,0.215141,null,null,null
+2020-09-02T22:40:49Z,26.68,60.69,99,0,27.59,101.93,14.00,492.00,0.210945,0.217406,0.228258,0.214961,null,null,null
+2020-09-02T22:41:19Z,26.66,60.70,99,0,28.02,101.93,15.00,501.00,0.209359,0.217391,0.228844,0.215344,null,null,null
+2020-09-02T22:41:49Z,26.68,60.69,99,0,28.52,101.93,15.00,501.00,0.208195,0.217023,0.227984,0.214734,null,null,null
+2020-09-02T22:42:19Z,26.68,60.71,99,0,26.67,101.94,15.00,501.00,0.208758,0.217242,0.228375,0.215602,null,null,null
+2020-09-02T22:42:49Z,26.66,60.71,99,0,29.03,101.93,15.00,501.00,0.209234,0.217672,0.228828,0.215406,null,null,null
+2020-09-02T22:43:19Z,26.68,60.75,99,0,26.41,101.94,15.00,501.00,0.210289,0.218187,0.227461,0.214867,null,null,null
+2020-09-02T22:43:49Z,26.66,60.69,99,0,28.06,101.94,15.00,501.00,0.208734,0.217023,0.228125,0.215633,null,null,null
+2020-09-02T22:44:19Z,26.68,60.66,99,0,28.14,101.94,15.00,501.00,0.209844,0.216773,0.229305,0.214813,null,null,null
+2020-09-02T22:44:49Z,26.66,60.69,99,0,25.67,101.94,15.00,501.00,0.211477,0.217195,0.227055,0.214414,null,null,null
+2020-09-02T22:45:19Z,26.66,60.73,99,0,25.79,101.94,15.00,501.00,0.209555,0.217297,0.229672,0.215469,null,null,null
+2020-09-02T22:45:49Z,26.68,60.72,99,0,30.96,101.94,15.00,501.00,0.208406,0.216109,0.228586,0.216133,null,null,null
+2020-09-02T22:46:19Z,26.68,60.69,99,0,26.95,101.94,15.00,501.00,0.209531,0.216266,0.227398,0.214500,null,null,null
+2020-09-02T22:46:49Z,26.66,60.71,99,0,25.38,101.94,15.00,501.00,0.208922,0.216742,0.230086,0.215562,null,null,null
+2020-09-02T22:47:19Z,26.66,60.71,99,0,28.09,101.94,15.00,501.00,0.209680,0.216422,0.228086,0.215406,null,null,null
+2020-09-02T22:47:49Z,26.69,60.75,99,0,26.48,101.94,15.00,501.00,0.208609,0.216891,0.228391,0.214594,null,null,null
+2020-09-02T22:48:19Z,26.66,60.70,99,0,27.45,101.94,16.00,508.00,0.208438,0.216617,0.227898,0.215672,null,null,null
+2020-09-02T22:48:49Z,26.68,60.72,99,0,30.01,101.94,16.00,508.00,0.209992,0.217289,0.227445,0.215070,null,null,null
+2020-09-02T22:49:19Z,26.66,60.67,99,0,26.57,101.94,16.00,508.00,0.210305,0.217266,0.229086,0.215625,null,null,null
+2020-09-02T22:49:49Z,26.66,60.74,99,0,24.65,101.94,16.00,508.00,0.210164,0.217187,0.227625,0.215156,null,null,null
+2020-09-02T22:50:19Z,26.68,60.73,99,0,27.32,101.94,16.00,508.00,0.208195,0.216258,0.228938,0.214891,null,null,null
+2020-09-02T22:50:49Z,26.68,60.72,99,0,26.78,101.94,16.00,508.00,0.209930,0.217453,0.227187,0.214195,null,null,null
+2020-09-02T22:51:19Z,26.66,60.68,99,0,26.14,101.94,15.00,502.00,0.210367,0.217727,0.228289,0.215031,null,null,null
+2020-09-02T22:51:49Z,26.65,60.71,99,0,28.07,101.94,15.00,502.00,0.210000,0.217234,0.227828,0.215469,null,null,null
+2020-09-02T22:52:19Z,26.68,60.77,99,0,27.73,101.94,16.00,508.00,0.210547,0.217492,0.228406,0.215641,null,null,null
+2020-09-02T22:52:49Z,26.66,60.70,99,0,26.82,101.94,16.00,508.00,0.208789,0.217195,0.231500,0.215281,null,null,null
+2020-09-02T22:53:19Z,26.68,60.74,99,0,26.11,101.94,16.00,508.00,0.210367,0.218484,0.229672,0.215453,null,null,null
+2020-09-02T22:53:49Z,26.66,60.70,99,0,26.97,101.94,16.00,508.00,0.209305,0.218273,0.227852,0.215813,null,null,null
+2020-09-02T22:54:19Z,26.66,60.70,99,0,26.26,101.94,16.00,508.00,0.210555,0.217609,0.229609,0.215406,null,null,null
+2020-09-02T22:54:49Z,26.68,60.69,99,0,27.30,101.94,16.00,508.00,0.209148,0.217391,0.228125,0.215164,null,null,null
+2020-09-02T22:55:19Z,26.68,60.72,99,0,25.38,101.94,16.00,508.00,0.209906,0.217391,0.228516,0.215172,null,null,null
+2020-09-02T22:55:49Z,26.65,60.70,99,0,25.82,101.95,16.00,508.00,0.210648,0.217328,0.230391,0.215906,null,null,null
+2020-09-02T22:56:19Z,26.66,60.67,99,0,26.73,101.95,16.00,508.00,0.210703,0.217344,0.228602,0.215297,null,null,null
+2020-09-02T22:56:49Z,26.68,60.67,99,0,29.61,101.95,16.00,508.00,0.210328,0.217945,0.228617,0.215023,null,null,null
+2020-09-02T22:57:19Z,26.68,60.67,99,0,24.72,101.95,17.00,518.00,0.210195,0.217063,0.228313,0.215242,null,null,null
+2020-09-02T22:57:49Z,26.65,60.71,99,0,29.16,101.94,17.00,518.00,0.209602,0.217836,0.227305,0.214625,null,null,null
+2020-09-02T22:58:19Z,26.66,60.67,99,0,25.98,101.94,16.00,508.00,0.209891,0.217609,0.229578,0.215359,null,null,null
+2020-09-02T22:58:49Z,26.68,60.69,99,0,41.57,101.94,16.00,508.00,0.209531,0.217445,0.228758,0.215219,null,null,null
+2020-09-02T22:59:19Z,26.66,60.70,99,0,26.84,101.94,16.00,508.00,0.208758,0.216633,0.227641,0.215328,null,null,null
+2020-09-02T22:59:49Z,26.65,60.67,99,0,27.68,101.95,16.00,508.00,0.209867,0.217133,0.227273,0.215766,null,null,null
+2020-09-02T23:00:19Z,26.65,60.71,99,0,31.87,101.94,16.00,508.00,0.209781,0.218070,0.228906,0.215234,null,null,null
+2020-09-02T23:00:49Z,26.68,60.68,99,0,27.59,101.94,16.00,508.00,0.210320,0.217328,0.227914,0.215641,null,null,null
+2020-09-02T23:01:19Z,26.68,60.74,99,0,26.64,101.95,16.00,508.00,0.210695,0.216930,0.229383,0.216133,null,null,null
+2020-09-02T23:01:49Z,26.66,60.74,99,0,31.88,101.94,16.00,508.00,0.209727,0.218219,0.226961,0.214930,null,null,null
+2020-09-02T23:02:19Z,26.66,60.69,99,0,26.00,101.94,16.00,508.00,0.211766,0.218242,0.229461,0.215141,null,null,null
+2020-09-02T23:02:49Z,26.66,60.76,99,0,27.47,101.94,16.00,508.00,0.209648,0.216602,0.227094,0.215367,null,null,null
+2020-09-02T23:03:19Z,26.68,60.70,99,0,32.38,101.95,16.00,508.00,0.209711,0.216875,0.229508,0.215312,null,null,null
+2020-09-02T23:03:49Z,26.66,60.69,99,0,40.23,101.94,16.00,508.00,0.210555,0.217844,0.228977,0.216562,null,null,null
+2020-09-02T23:04:19Z,26.66,60.71,99,0,29.99,101.94,16.00,508.00,0.210211,0.216234,0.228586,0.215102,null,null,null
+2020-09-02T23:04:49Z,26.66,60.73,99,0,33.20,101.95,16.00,508.00,0.210531,0.216492,0.228547,0.215188,null,null,null
+2020-09-02T23:05:19Z,26.65,60.73,99,0,41.50,101.95,17.00,518.00,0.210250,0.217031,0.229258,0.215852,null,null,null
+2020-09-02T23:05:49Z,26.64,60.71,99,0,42.85,101.95,17.00,518.00,0.209133,0.215930,0.228938,0.215516,null,null,null
+2020-09-02T23:06:19Z,26.66,60.69,99,0,31.97,101.95,16.00,508.00,0.208898,0.216867,0.227437,0.215547,null,null,null
+2020-09-02T23:06:49Z,26.65,60.71,99,0,26.16,101.95,16.00,508.00,0.209586,0.216922,0.227719,0.214570,null,null,null
+2020-09-02T23:07:19Z,26.64,60.71,99,0,25.00,101.95,17.00,518.00,0.211070,0.217672,0.227914,0.215039,null,null,null
+2020-09-02T23:07:49Z,26.65,60.70,99,0,28.54,101.95,17.00,518.00,0.210078,0.216531,0.229375,0.215687,null,null,null
+2020-09-02T23:08:19Z,26.65,60.69,99,0,34.62,101.95,16.00,508.00,0.210070,0.217453,0.226203,0.214813,null,null,null
+2020-09-02T23:08:49Z,26.64,60.69,99,0,29.69,101.95,16.00,508.00,0.208875,0.216102,0.228375,0.215055,null,null,null
+2020-09-02T23:09:19Z,26.66,60.67,99,0,26.19,101.95,16.00,508.00,0.210602,0.217180,0.229391,0.215242,null,null,null
+2020-09-02T23:09:49Z,26.65,60.65,99,0,24.89,101.95,16.00,508.00,0.211227,0.218164,0.227539,0.215461,null,null,null
+2020-09-02T23:10:19Z,26.66,60.66,99,0,27.22,101.95,17.00,518.00,0.209930,0.217578,0.228797,0.215398,null,null,null
+2020-09-02T23:10:49Z,26.64,60.67,99,0,28.51,101.95,17.00,518.00,0.210133,0.217586,0.228047,0.215578,null,null,null
+2020-09-02T23:11:19Z,26.66,60.72,99,0,28.34,101.95,17.00,518.00,0.208922,0.216422,0.227742,0.215719,null,null,null
+2020-09-02T23:11:49Z,26.66,60.75,99,0,28.17,101.95,17.00,518.00,0.209977,0.217484,0.227984,0.215312,null,null,null
+2020-09-02T23:12:19Z,26.64,60.71,99,0,27.18,101.95,17.00,518.00,0.211688,0.217508,0.229445,0.215734,null,null,null
+2020-09-02T23:12:49Z,26.65,60.70,99,0,26.19,101.96,17.00,518.00,0.208805,0.216664,0.228781,0.215508,null,null,null
+2020-09-02T23:13:19Z,26.64,60.65,99,0,25.53,101.96,17.00,518.00,0.210109,0.216852,0.227719,0.215008,null,null,null
+2020-09-02T23:13:49Z,26.64,60.70,99,0,32.12,101.95,17.00,518.00,0.209461,0.217992,0.228383,0.215555,null,null,null
+2020-09-02T23:14:19Z,26.66,60.70,99,0,27.28,101.95,17.00,518.00,0.209383,0.217562,0.227648,0.215352,null,null,null
+2020-09-02T23:14:49Z,26.66,60.62,99,0,25.41,101.95,17.00,518.00,0.208109,0.217172,0.226594,0.214422,null,null,null
+2020-09-02T23:15:19Z,26.64,60.73,99,0,28.17,101.95,17.00,518.00,0.212023,0.217625,0.228188,0.215305,null,null,null
+2020-09-02T23:15:49Z,26.68,60.63,99,0,28.17,101.95,17.00,518.00,0.210641,0.217461,0.229102,0.215125,null,null,null
+2020-09-02T23:16:19Z,26.65,60.69,99,0,27.59,101.95,17.00,518.00,0.209898,0.215687,0.227711,0.215141,null,null,null
+2020-09-02T23:16:49Z,26.65,60.71,99,0,26.55,101.95,17.00,518.00,0.209891,0.218477,0.228219,0.215195,null,null,null
+2020-09-02T23:17:19Z,26.66,60.70,99,0,25.22,101.95,17.00,518.00,0.209266,0.216117,0.228641,0.214813,null,null,null
+2020-09-02T23:17:49Z,26.64,60.72,99,0,27.57,101.95,17.00,518.00,0.210367,0.217297,0.228727,0.215594,null,null,null
+2020-09-02T23:18:19Z,26.64,60.70,99,0,25.84,101.96,16.00,508.00,0.210313,0.217016,0.228109,0.214969,null,null,null
+2020-09-02T23:18:49Z,26.65,60.69,99,0,27.62,101.95,16.00,508.00,0.210570,0.217031,0.229016,0.215359,null,null,null
+2020-09-02T23:19:19Z,26.64,60.70,99,0,29.15,101.95,17.00,518.00,0.209328,0.217281,0.230070,0.215945,null,null,null
+2020-09-02T23:19:49Z,26.68,60.63,99,0,25.38,101.95,17.00,518.00,0.210750,0.216469,0.227570,0.214750,null,null,null
+2020-09-02T23:20:19Z,26.65,60.68,99,0,27.24,101.95,17.00,518.00,0.209328,0.217039,0.228055,0.215672,null,null,null
+2020-09-02T23:20:49Z,26.68,60.63,99,0,27.04,101.95,17.00,518.00,0.210719,0.217086,0.228383,0.214711,null,null,null
+2020-09-02T23:21:19Z,26.64,60.62,99,0,27.24,101.95,16.00,508.00,0.209297,0.216016,0.228141,0.216109,null,null,null
+2020-09-02T23:21:49Z,26.65,60.70,99,0,29.90,101.95,16.00,508.00,0.210648,0.217547,0.227055,0.215164,null,null,null
+2020-09-02T23:22:19Z,26.62,60.68,99,0,27.18,101.95,17.00,518.00,0.210641,0.217227,0.228836,0.215734,null,null,null
+2020-09-02T23:22:49Z,26.66,60.70,99,0,29.50,101.95,17.00,518.00,0.209867,0.217367,0.228516,0.216188,null,null,null
+2020-09-02T23:23:19Z,26.66,60.70,99,0,28.73,101.95,17.00,518.00,0.208508,0.218437,0.227914,0.216141,null,null,null
+2020-09-02T23:23:49Z,26.62,60.68,99,0,25.90,101.95,17.00,518.00,0.208813,0.218250,0.228625,0.215578,null,null,null
+2020-09-02T23:24:19Z,26.64,60.70,99,0,28.63,101.95,17.00,518.00,0.209242,0.216766,0.229219,0.216047,null,null,null
+2020-09-02T23:24:49Z,26.62,60.72,99,0,26.93,101.95,17.00,518.00,0.209758,0.216172,0.227914,0.214898,null,null,null
+2020-09-02T23:25:19Z,26.64,60.65,99,0,28.64,101.95,17.00,518.00,0.208180,0.216414,0.227852,0.215008,null,null,null
+2020-09-02T23:25:49Z,26.64,60.67,99,0,26.41,101.95,17.00,518.00,0.209719,0.217492,0.227477,0.214937,null,null,null
+2020-09-02T23:26:19Z,26.64,60.63,99,0,26.64,101.95,17.00,518.00,0.209594,0.217305,0.229977,0.215859,null,null,null
+2020-09-02T23:26:49Z,26.66,60.69,99,0,29.35,101.95,17.00,518.00,0.210430,0.216641,0.228461,0.215789,null,null,null
+2020-09-02T23:27:19Z,26.62,60.71,99,0,27.68,101.95,17.00,518.00,0.210594,0.216422,0.227828,0.215633,null,null,null
+2020-09-02T23:27:49Z,26.62,60.73,99,0,30.77,101.95,17.00,518.00,0.210703,0.217242,0.228898,0.215906,null,null,null
+2020-09-02T23:28:19Z,26.64,60.76,99,0,27.64,101.95,17.00,518.00,0.208492,0.217469,0.226938,0.215305,null,null,null
+2020-09-02T23:28:49Z,26.61,60.73,99,0,26.31,101.95,17.00,518.00,0.208422,0.216836,0.229813,0.215945,null,null,null
+2020-09-02T23:29:19Z,26.65,60.67,99,0,27.87,101.95,17.00,518.00,0.209984,0.217906,0.228141,0.214531,null,null,null
+2020-09-02T23:29:49Z,26.62,60.66,99,0,26.26,101.95,17.00,518.00,0.211125,0.217500,0.228906,0.215531,null,null,null
+2020-09-02T23:30:19Z,26.65,60.71,99,0,26.62,101.95,17.00,518.00,0.211016,0.218039,0.228305,0.214992,null,null,null
+2020-09-02T23:30:49Z,26.62,60.70,99,0,36.92,101.95,17.00,518.00,0.209523,0.217031,0.228000,0.215414,null,null,null
+2020-09-02T23:31:19Z,26.64,60.67,99,0,29.01,101.95,17.00,518.00,0.208750,0.217937,0.227680,0.215531,null,null,null
+2020-09-02T23:31:49Z,26.65,60.69,99,0,26.95,101.95,17.00,518.00,0.209883,0.218117,0.228883,0.215320,null,null,null
+2020-09-02T23:32:19Z,26.62,60.70,99,0,26.80,101.95,17.00,518.00,0.209109,0.215617,0.229422,0.215742,null,null,null
+2020-09-02T23:32:49Z,26.64,60.68,99,0,26.91,101.95,17.00,518.00,0.209813,0.215891,0.228023,0.214922,null,null,null
+2020-09-02T23:33:19Z,26.62,60.70,99,0,25.76,101.95,17.00,518.00,0.210953,0.217633,0.229055,0.215188,null,null,null
+2020-09-02T23:33:49Z,26.64,60.67,99,0,25.50,101.95,17.00,518.00,0.211219,0.217164,0.228344,0.214766,null,null,null
+2020-09-02T23:34:19Z,26.62,60.67,99,0,27.73,101.95,17.00,518.00,0.210352,0.217117,0.228117,0.215672,null,null,null
+2020-09-02T23:34:49Z,26.61,60.73,99,0,26.87,101.95,17.00,518.00,0.209383,0.216578,0.228563,0.215344,null,null,null
+2020-09-02T23:35:19Z,26.62,60.73,99,0,26.16,101.95,17.00,518.00,0.211531,0.217016,0.229977,0.215867,null,null,null
+2020-09-02T23:35:49Z,26.64,60.70,99,0,26.00,101.95,17.00,518.00,0.209867,0.216859,0.228773,0.215758,null,null,null
+2020-09-02T23:36:19Z,26.64,60.70,99,0,25.73,101.95,17.00,518.00,0.209750,0.217914,0.228758,0.214641,null,null,null
+2020-09-02T23:36:49Z,26.62,60.69,99,0,27.73,101.95,17.00,518.00,0.209883,0.217937,0.229078,0.215508,null,null,null
+2020-09-02T23:37:19Z,26.62,60.68,99,0,29.11,101.95,17.00,518.00,0.210453,0.217469,0.227656,0.215211,null,null,null
+2020-09-02T23:37:49Z,26.64,60.71,99,0,26.41,101.95,17.00,518.00,0.209359,0.217414,0.228836,0.215805,null,null,null
+2020-09-02T23:38:19Z,26.64,60.68,99,0,25.00,101.95,17.00,518.00,0.208641,0.216016,0.227117,0.215586,null,null,null
+2020-09-02T23:38:49Z,26.64,60.73,99,0,27.75,101.95,17.00,518.00,0.210008,0.217430,0.227953,0.215234,null,null,null
+2020-09-02T23:39:19Z,26.61,60.69,99,0,25.16,101.95,17.00,518.00,0.208500,0.217195,0.227945,0.215687,null,null,null
+2020-09-02T23:39:49Z,26.62,60.67,99,0,26.26,101.95,17.00,518.00,0.208773,0.217945,0.228359,0.215578,null,null,null
+2020-09-02T23:40:19Z,26.64,60.70,99,0,24.76,101.95,17.00,518.00,0.210000,0.217477,0.227078,0.215602,null,null,null
+2020-09-02T23:40:49Z,26.64,60.68,99,0,28.92,101.94,17.00,518.00,0.210836,0.218242,0.228633,0.215219,null,null,null
+2020-09-02T23:41:19Z,26.62,60.66,99,0,25.50,101.95,18.00,523.00,0.209594,0.216703,0.227875,0.216297,null,null,null
+2020-09-02T23:41:49Z,26.62,60.69,99,0,26.95,101.95,18.00,523.00,0.209477,0.217633,0.228961,0.215773,null,null,null
+2020-09-02T23:42:19Z,26.62,60.68,99,0,25.29,101.95,17.00,518.00,0.210609,0.217664,0.226383,0.215023,null,null,null
+2020-09-02T23:42:49Z,26.61,60.68,99,0,28.06,101.94,17.00,518.00,0.209680,0.216172,0.229320,0.215234,null,null,null
+2020-09-02T23:43:19Z,26.62,60.74,99,0,27.55,101.94,17.00,518.00,0.210406,0.216711,0.229266,0.215625,null,null,null
+2020-09-02T23:43:49Z,26.62,60.62,99,0,26.71,101.94,17.00,518.00,0.209602,0.217547,0.228141,0.215914,null,null,null
+2020-09-02T23:44:19Z,26.64,60.69,99,0,28.81,101.95,17.00,518.00,0.210320,0.216500,0.229000,0.215820,null,null,null
+2020-09-02T23:44:49Z,26.61,60.66,99,0,27.06,101.94,17.00,518.00,0.209914,0.217523,0.228125,0.215250,null,null,null
+2020-09-02T23:45:19Z,26.62,60.66,99,0,27.96,101.95,17.00,518.00,0.209148,0.216813,0.227984,0.215508,null,null,null
+2020-09-02T23:45:49Z,26.62,60.72,99,0,25.95,101.94,17.00,518.00,0.209031,0.217937,0.227875,0.215820,null,null,null
+2020-09-02T23:46:19Z,26.62,60.72,99,0,27.04,101.95,17.00,518.00,0.209578,0.216344,0.228625,0.215875,null,null,null
+2020-09-02T23:46:49Z,26.62,60.71,99,0,26.82,101.95,17.00,518.00,0.209930,0.217500,0.229445,0.215320,null,null,null
+2020-09-02T23:47:19Z,26.61,60.71,99,0,26.67,101.95,17.00,518.00,0.209922,0.217820,0.229492,0.215648,null,null,null
+2020-09-02T23:47:49Z,26.62,60.69,99,0,26.87,101.95,17.00,518.00,0.211539,0.217023,0.227758,0.214992,null,null,null
+2020-09-02T23:48:19Z,26.61,60.71,99,0,26.53,101.95,17.00,518.00,0.209562,0.217375,0.228898,0.215977,null,null,null
+2020-09-02T23:48:49Z,26.61,60.69,99,0,23.63,101.95,17.00,518.00,0.210094,0.216867,0.229297,0.215883,null,null,null
+2020-09-02T23:49:19Z,26.62,60.73,99,0,26.53,101.94,17.00,518.00,0.211531,0.217328,0.229086,0.215188,null,null,null
+2020-09-02T23:49:49Z,26.59,60.72,99,0,28.93,101.95,17.00,518.00,0.210328,0.217547,0.227781,0.215164,null,null,null
+2020-09-02T23:50:19Z,26.59,60.74,99,0,26.06,101.94,17.00,518.00,0.208914,0.217703,0.230750,0.215945,null,null,null
+2020-09-02T23:50:49Z,26.62,60.75,99,0,27.14,101.95,17.00,518.00,0.210195,0.218141,0.228008,0.215000,null,null,null
+2020-09-02T23:51:19Z,26.61,60.71,99,0,29.23,101.94,17.00,518.00,0.208758,0.217406,0.228602,0.215969,null,null,null
+2020-09-02T23:51:49Z,26.62,60.71,99,0,24.83,101.95,17.00,518.00,0.209789,0.217125,0.228516,0.215516,null,null,null
+2020-09-02T23:52:19Z,26.59,60.71,99,0,27.66,101.94,18.00,523.00,0.210656,0.217844,0.227742,0.215438,null,null,null
+2020-09-02T23:52:49Z,26.62,60.66,99,0,24.89,101.95,18.00,523.00,0.210453,0.216953,0.227023,0.215562,null,null,null
+2020-09-02T23:53:19Z,26.61,60.69,99,0,28.92,101.95,17.00,518.00,0.211492,0.217609,0.229641,0.215477,null,null,null
+2020-09-02T23:53:49Z,26.61,60.75,99,0,27.02,101.95,17.00,518.00,0.210852,0.218242,0.228742,0.215164,null,null,null
+2020-09-02T23:54:19Z,26.62,60.70,99,0,27.68,101.94,17.00,518.00,0.209047,0.217453,0.227766,0.214945,null,null,null
+2020-09-02T23:54:49Z,26.59,60.74,99,0,26.38,101.95,17.00,518.00,0.209438,0.217094,0.226609,0.215023,null,null,null
+2020-09-02T23:55:19Z,26.59,60.75,99,0,27.44,101.95,16.00,508.00,0.209914,0.218141,0.229297,0.215164,null,null,null
+2020-09-02T23:55:49Z,26.61,60.71,99,0,25.59,101.95,16.00,508.00,0.210859,0.217109,0.227492,0.214930,null,null,null
+2020-09-02T23:56:19Z,26.62,60.74,99,0,25.76,101.95,18.00,523.00,0.209609,0.217148,0.227437,0.215297,null,null,null
+2020-09-02T23:56:49Z,26.61,60.74,99,0,25.98,101.95,18.00,523.00,0.209727,0.216992,0.226844,0.214813,null,null,null
+2020-09-02T23:57:19Z,26.62,60.76,99,0,28.27,101.94,15.00,502.00,0.209648,0.217109,0.227859,0.215273,null,null,null
+2020-09-02T23:57:49Z,26.61,60.70,99,0,25.44,101.95,15.00,502.00,0.208805,0.217336,0.228945,0.215937,null,null,null
+2020-09-02T23:58:19Z,26.62,60.70,99,0,29.31,101.94,16.00,508.00,0.210859,0.217805,0.229844,0.215578,null,null,null
+2020-09-02T23:58:49Z,26.61,60.76,99,0,27.14,101.94,16.00,508.00,0.209742,0.216555,0.227008,0.214469,null,null,null
+2020-09-02T23:59:19Z,26.61,60.72,99,0,25.92,101.94,17.00,518.00,0.210141,0.216867,0.229797,0.216234,null,null,null
```

### Comparing `scdata-0.9.1/scdata/utils/interim/geodata.csv` & `scdata-1.0.0/scdata/tools/interim/geodata.csv`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/lazy.py` & `scdata-1.0.0/scdata/tools/lazy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
-from .out import std_out
+from .custom_logger import logger
 
 class LazyCallable(object):
     '''
         Adapted from Alex Martelli's answer on this post on stackoverflow:
         https://stackoverflow.com/questions/3349157/python-passing-a-function-name-as-an-argument-in-a-function
     '''
     def __init__(self, name):
         self.n = name
         self.f = None
     def __call__(self, *a, **k):
         if self.f is None:
-            std_out(f"Loading {self.n.rsplit('.', 1)[1]} from {self.n.rsplit('.', 1)[0]}")
+            logger.info(f"Loading {self.n.rsplit('.', 1)[1]} from {self.n.rsplit('.', 1)[0]}")
             modn, funcn = self.n.rsplit('.', 1)
             if modn not in sys.modules:
                 __import__(modn)
             self.f = getattr(sys.modules[modn], funcn)
         return self.f(*a, **k)
```

### Comparing `scdata-0.9.1/scdata/utils/location.py` & `scdata-1.0.0/scdata/tools/location.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from requests import get
 from pandas import json_normalize
-from scdata.utils import std_out
+from scdata.tools.custom_logger import logger
 from scdata._config import config
 
 def get_elevation(_lat = None, _long = None):
     '''
         script for returning elevation from lat, long,
         based on open elevation data
         which in turn is based on SRTM - elevation in m
         From:
         https://stackoverflow.com/questions/19513212/can-i-get-the-altitude-with-geopy-in-python-with-longitude-latitude
     '''
     if _lat is None or _long is None: return None
-    
+
     query = ('https://api.open-elevation.com/api/v1/lookup'
              f'?locations={_lat},{_long}')
 
     # Request with a timeout for slow responses
     error = False
     try:
         r = get(query, timeout = config._timeout)
     except:
-        std_out(f'Cannot get altitude from {query}')
+        logger.info(f'Cannot get altitude from {query}')
         error = True
         pass
 
     if error: return None
 
     # Only get the json response in case of 200 or 201
     if r.status_code == 200 or r.status_code == 201:
```

### Comparing `scdata-0.9.1/scdata/utils/logs.py` & `scdata-1.0.0/scdata/test/tools/history.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from os import walk
 from os.path import join
 import yaml
 from scdata._config import config
 
-def get_tests_log(deep_description = False):
+def history(deep_description = False):
     '''
         Gets the tests in the given dir, looking for test_description.yaml
     '''
 
     # Get available tests in the data folder structure
     tests = dict()
 
     for root, dirs, files in walk(config.paths['processed']):
         for file in files:
-            if file.endswith(".yaml"):
+            # TODO Fix
+            if file.endswith(".yaml") or file.endswith(".json"):
                 test_name = root.split('/')[-1]
                 if test_name.startswith('.'): continue
-                
+
                 tests[test_name] = dict()
                 tests[test_name]['path'] = root
-                
+
                 if deep_description == True:
                     filePath = join(root, file)
                     with open(filePath, 'r') as stream:
                         yamlFile = yaml.load(stream, Loader = yaml.FullLoader)
                         for key in yamlFile.keys():
                             if key == 'devices': continue
                             tests[test_name][key] = yamlFile[key]
```

### Comparing `scdata-0.9.1/scdata/utils/report.py` & `scdata-1.0.0/scdata/tools/report.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/stats.py` & `scdata-1.0.0/scdata/tools/stats.py`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/uploads/example_upload_1.json` & `scdata-1.0.0/scdata/tools/uploads/example_upload_1.json`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/uploads/example_zenodo_upload.yaml` & `scdata-1.0.0/scdata/tools/uploads/example_zenodo_upload.yaml`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/uploads/report.pdf` & `scdata-1.0.0/scdata/tools/uploads/report.pdf`

 * *Files identical despite different names*

### Comparing `scdata-0.9.1/scdata/utils/zenodo.py` & `scdata-1.0.0/scdata/tools/zenodo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ''' Implementation of zenodo export '''
 
 from scdata._config import config
-from scdata.utils import std_out, get_tests_log
-from scdata.utils.report import include_footer
+from scdata.tools.custom_logger import logger
+from scdata.tools.report import include_footer
 from scdata import Test
 import json, yaml
 from os.path import join, dirname, getsize, exists
 from requests import post
 from os import environ
 
 def zenodo_upload(upload_descritor, sandbox = True, dry_run = True):
 	'''
 	This section uses the code inspired by this repo https://github.com/darvasd/upload-to-zenodo
 	Uploads a series of tests to zenodo.org using a template in /zenodo_templates and the descriptor
 	file in data/uploads. It will need a ZENODO_TOKEN environment variable to work
-	The submission needs an additional "Publish" step. 
-	This can also be done from a script, but to be on the safe side, it is not included. 
+	The submission needs an additional "Publish" step.
+	This can also be done from a script, but to be on the safe side, it is not included.
 	(The attached file cannot be changed after publication)
 	Parameters
 	----------
 		upload_descritor: string
 			The descriptor's filename (yaml) in the data/uploads. Check options in the example yaml
 			Option defaults:
 				include_processed_data: True (for tests)
@@ -33,15 +33,16 @@
 		dry_run:
 			True fakes uploads everything to check
 	Returns
 	----------
 		True if all data is uploaded, False otherwise
 
 	'''
-	
+	raise NotImplementedError
+
 	def fill_template(individual_descriptor, descriptor_file_name, upload_type = 'dataset'):
 		# Open base template with all keys
 
 		if upload_type == 'dataset': template_file_name = 'template_zenodo_dataset'
 		elif upload_type == 'publication': template_file_name = 'template_zenodo_publication'
 
 		with open (join(dirname(__file__), 'zenodo_templates', f'{template_file_name}.json'), 'r') as template_file:
@@ -55,216 +56,216 @@
 			value = individual_descriptor[key]
 
 			if key in filled_template['metadata'].keys():
 				filled_template['metadata'][key] = value
 
 		with open (join(config.paths['uploads'], descriptor_file_name), 'w') as descriptor_json:
 			json.dump(filled_template, descriptor_json, ensure_ascii=True)
-			std_out(f'Created descriptor file for {descriptor_file_name}', 'SUCCESS')
-		
+			logger.info(f'Created descriptor file for {descriptor_file_name}')
+
 		return json.dumps(filled_template)
 
 	def get_submission_id(metadata, base_url):
 		url = f"{base_url}/api/deposit/depositions"
 
 		headers = {"Content-Type": "application/json"}
 
 		response = post(url, params={'access_token': environ['ZENODO_TOKEN']}, data = metadata, headers = headers)
 		if response.status_code > 210:
-			std_out("Error happened during submission, status code: " + str(response.status_code), 'ERROR')
-			std_out(response.json()['message'], 'ERROR')
+			logger.error("Error happened during submission, status code: " + str(response.status_code))
+			logger.error(response.json()['message'])
 			return None
 
 		# Get the submission ID
 		submission_id = json.loads(response.text)["id"]
 
 		return submission_id
 
 	def upload_file(url, upload_metadata, files):
 		response = post(url, params={'access_token': environ['ZENODO_TOKEN']}, data = upload_metadata, files=files)
-		return response.status_code		
+		return response.status_code
+
+	logger.info(f'Uploading {upload_descritor} to zenodo')
 
-	std_out(f'Uploading {upload_descritor} to zenodo')
+	if dry_run: logger.warning(f'Dry run. Verify output before setting dry_run to False')
 
-	if dry_run: std_out(f'Dry run. Verify output before setting dry_run to False', 'WARNING')
-	
 	# Sandbox or not
-	if sandbox: 
-		std_out(f'Using sandbox. Verify output before setting sandbox to False', 'WARNING')
+	if sandbox:
+		logger.warning(f'Using sandbox. Verify output before setting sandbox to False')
 		base_url = config.zenodo_sandbox_base_url
 	else: base_url = config.zenodo_real_base_url
-	
+
 	if '.yaml' not in upload_descritor: upload_descritor = upload_descritor + '.yaml'
-	
+
 	with open (join(config.paths['uploads'], upload_descritor), 'r') as descriptor_file:
 		descriptor = yaml.load(descriptor_file, Loader = yaml.SafeLoader)
 
 	for key in descriptor:
 
 		# Set options for processed and raw uploads
 		stage_list = ['base']
-		
+
 		if 'options' in descriptor[key].keys(): options = descriptor[key]['options']
 		else: options = {'include_processed_data': False, 'include_footer_doi': True, 'include_td_html': False}
 
 		# Defaults
 		if 'include_processed_data' not in options: options['include_processed_data'] = False
 		if 'include_footer_doi' not in options: options['include_footer_doi'] = True
 		if 'include_td_html' not in options: options['include_td_html'] = False
-		
+
 		if options['include_processed_data']: stage_list.append('processed')
-		std_out(f'Options {options}')
+		logger.info(f'Options {options}')
 
 		# Fill template
 		if 'upload_type' in descriptor[key].keys(): upload_type = descriptor[key]['upload_type']
-		else: 
-			std_out(f'Upload type not set for key {key}. Skipping', 'ERROR')
+		else:
+			logger.error(f'Upload type not set for key {key}. Skipping')
 			continue
 
 		metadata = fill_template(descriptor[key], key, upload_type = upload_type)
-		
+
 		# Get submission ID
 		if not dry_run: submission_id = get_submission_id(metadata, base_url)
 		else: submission_id = 0
 
 		if submission_id is not None:
-			
+
 			# Dataset upload
 			if upload_type == 'dataset':
 				# Get the tests to upload
 				tests = descriptor[key]['tests']
-				
+
 				# Get url where to post the files
 				url = f"{base_url}/api/deposit/depositions/{submission_id}/files"
 
-				test_logs = get_tests_log()			
+				test_logs = get_tests_log()
 
 				for test_name in tests:
-					
+
 					# Get test path
-					std_out(f'Uploading data from test {test_name}')
-					
+					logger.info(f'Uploading data from test {test_name}')
+
 					test_path = test_logs[test_name]['path']
 
 					# Upload the test descriptor (yaml (and html) format)
 					td_upload = ['yaml']
-					with open (join(test_path, 'test_description.yaml'), 'r') as td: 
+					with open (join(test_path, 'test_description.yaml'), 'r') as td:
 						yaml_td = yaml.load(td, Loader = yaml.SafeLoader)
-					
+
 					if options['include_td_html']:
 						html_td = td_to_html(yaml_td, test_path)
 						if html_td: td_upload.append('html')
 
 					for td_format in td_upload:
 
 						upload_metadata = {'name': f'test_description_{test_name}.{td_format}'}
-					
+
 						files = {'file': open(join(test_path, f'test_description.{td_format}'), 'rb')}
 						file_size = getsize(join(test_path, f'test_description.{td_format}'))/(1024*1024.0*1024)
-					
-						if file_size > 50: std_out(f'File size for {test_name} is over 50Gb ({file_size})', 'WARNING')
-					
+
+						if file_size > 50: logger.warning(f'File size for {test_name} is over 50Gb ({file_size})')
+
 						if not dry_run: status_code = upload_file(url, upload_metadata, files)
 						else: status_code = 200
-					
-						if status_code > 210: 
-							std_out ("Error happened during file upload, status code: " + str(status_code), 'ERROR')
+
+						if status_code > 210:
+							logger.error ("Error happened during file upload, status code: " + str(status_code))
 							return
 						else:
-							std_out(f"{upload_metadata['name']} submitted with submission ID = \
-								 	{submission_id} (DOI: 10.5281/zenodo.{submission_id})" ,"SUCCESS")
-					
+							logger.info(f"{upload_metadata['name']} submitted with submission ID = \
+								 	{submission_id} (DOI: 10.5281/zenodo.{submission_id})")
+
 					# Load the api devices to have them up to date in the cache
-					if any(yaml_td['devices'][device]['source'] == 'api' for device in yaml_td['devices'].keys()): 
+					if any(yaml_td['devices'][device]['source'] == 'api' for device in yaml_td['devices'].keys()):
 						test = Test(test_name)
 						test.load(options = {'store_cached_api': True})
-					
+
 					for device in yaml_td['devices'].keys():
-						
-						std_out(f'Uploading data from device {device}')
-						
+
+						logger.info(f'Uploading data from device {device}')
+
 						# Upload basic and processed data
 						for file_stage in stage_list:
-							
+
 							file_path = ''
-							
+
 							try:
 
 								# Find device files
-								if file_stage == 'processed': 
+								if file_stage == 'processed':
 
 									file_name = f'{device}.csv'
 									file_path = join(test_path, 'processed', file_name)
 									upload_metadata = {'name': f'{device}_PROCESSED.csv'}
-								
+
 								elif file_stage == 'base':
 									if 'csv' in yaml_td['devices'][device]['source']:
 
 										file_name = yaml_td['devices'][device]['processed_data_file']
 										file_path = join(test_path, file_name)
-									
+
 									elif yaml_td['devices'][device]['source'] == 'api':
 										file_name = f'{device}.csv'
 										file_path = join(test_path, 'cached', file_name)
-									
+
 									upload_metadata = {'name': file_name}
 
 								if file_path != '':
 
 									files = {'file': open(file_path, 'rb')}
 									file_size = getsize(file_path)/(1024*1024.0*1024)
-									
-									if file_size > 50: std_out(f'File size for {file_name} over 50Gb ({file_size})', 'WARNING')
-									
+
+									if file_size > 50: logger.warning(f'File size for {file_name} over 50Gb')
+
 									if not dry_run: status_code = upload_file(url, upload_metadata, files)
 									else: status_code = 200
-									
-									if status_code > 210: 
-										std_out (f"Error happened during file upload, status code: {status_code}. Skipping", 'ERROR')
+
+									if status_code > 210:
+										logger.error (f"Error happened during file upload, status code: {status_code}. Skipping")
 										continue
 
-									std_out(f"{upload_metadata['name']} submitted with submission ID =\
-												{submission_id} (DOI: 10.5281/zenodo.{submission_id})" ,"SUCCESS")    
+									logger.info(f"{upload_metadata['name']} submitted with submission ID =\
+												{submission_id} (DOI: 10.5281/zenodo.{submission_id})")
 							except:
-								if not exists(file_path): std_out(f'File {file_name} does not exist (type = {file_stage}). Skipping', 'ERROR')
+								if not exists(file_path): logger.error(f'File {file_name} does not exist (type = {file_stage}). Skipping')
 								# print_exc()
 								pass
-				
+
 				# Check if we have a report in the keys
 				if 'report' in descriptor[key].keys():
 
 					for file_name in descriptor[key]['report']:
 
 						file_path = join(config.paths['uploads'], file_name)
-						
+
 						if options['include_footer_doi'] and file_name.endswith('.pdf'):
 
 							output_file_path = file_path[:file_path.index('.pdf')] + '_doi.pdf'
 							include_footer(file_path, output_file_path, link = f'https://doi.org/10.5281/zenodo.{submission_id}')
 							file_path = output_file_path
-						
+
 						upload_metadata = {'name': file_name}
 						files = {'file': open(file_path, 'rb')}
 						file_size = getsize(file_path)/(1024*1024.0*1024)
-						
-						if file_size > 50: std_out(f'File size for {file_name} is over 50Gb({file_size})', 'WARNING')
-						
+
+						if file_size > 50: logger.warning(f'File size for {file_name} is over 50Gb({file_size})')
+
 						if not dry_run: status_code = upload_file(url, upload_metadata, files)
 						else: status_code = 200
 
-						if status_code > 210: 
-							std_out (f"Error happened during file upload, status code: {status_code}. Skipping", 'ERROR')
+						if status_code > 210:
+							logger.error (f"Error happened during file upload, status code: {status_code}. Skipping")
 							continue
 
-						std_out(f"{upload_metadata['name']} submitted with submission ID = \
-								{submission_id} (DOI: 10.5281/zenodo.{submission_id})" ,"SUCCESS")
+						logger.info(f"{upload_metadata['name']} submitted with submission ID = \
+								{submission_id} (DOI: 10.5281/zenodo.{submission_id})")
 
 			if upload_type == 'publication':
-				std_out('Not implemented')
+				logger.info('Not implemented')
 				return False
-			
-			std_out(f'Submission completed - (DOI: 10.5281/zenodo.{submission_id})', 'SUCCESS')
-			std_out(f'------------------------------------------------------------')
+
+			logger.info(f'Submission completed - (DOI: 10.5281/zenodo.{submission_id})')
+			logger.info(f'------------------------------------------------------------')
 		else:
-			std_out(f'Submission ID error', 'ERROR')
+			logger.error(f'Submission ID error')
 			continue
 	return True
```

### Comparing `scdata-0.9.1/scdata.egg-info/PKG-INFO` & `scdata-1.0.0/scdata.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 Metadata-Version: 2.1
 Name: scdata
-Version: 0.9.1
+Version: 1.0.0
 Summary: Analysis of sensors and time series data
 Home-page: https://github.com/fablabbcn/smartcitizen-data
 Author: oscgonfer
 License: GNU-GPL3.0
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-data
 Keywords: air,sensors,Smart Citizen
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: branca~=0.4.0
+Requires-Dist: Flask~=2.2.2
+Requires-Dist: folium~=0.12.1
+Requires-Dist: geopy~=1.21.0
+Requires-Dist: Jinja2~=3.1.2
+Requires-Dist: matplotlib
+Requires-Dist: missingno~=0.5.2
+Requires-Dist: numpy~=1.25.2
+Requires-Dist: pandas~=2.2.2
+Requires-Dist: pydantic
+Requires-Dist: pytest
+Requires-Dist: PyYAML==5.3.1
+Requires-Dist: requests
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: seaborn
+Requires-Dist: smartcitizen-connector
+Requires-Dist: termcolor==1.1.0
+Requires-Dist: tqdm~=4.50.2
+Requires-Dist: timezonefinder~=6.1.9
+Requires-Dist: urllib3
 
 Smart Citizen Data
 =======
 
 [![DOI](https://zenodo.org/badge/97752018.svg)](https://zenodo.org/badge/latestdoi/97752018)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks)
 [![PyPI version](https://badge.fury.io/py/scdata.svg)](https://badge.fury.io/py/scdata)
+[![Python application](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml/badge.svg)](https://github.com/fablabbcn/smartcitizen-data/actions/workflows/python-app.yml)
 
 Welcome to **SmartCitizen Data**. This is a data analysis framework for working with sensor data in different ways:
 
 - Interacting with several sensors APIs
 - Clean data, export and calculate metrics
 - Model sensor data and calibrate sensors
 - Generate data visualisations - matplotlib, [plotly](https://plotly.com/) or [uplot](https://leeoniya.github.io/uPlot)
 - Generate analysis reports in html or pdf and upload them to [Zenodo](http://zenodo.org)
 
-A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/). 
+A full documentation of the framework is detailed in [the Smart Citizen Docs](https://docs.smartcitizen.me/Data/Data%20Analysis/).
 
 ## Installation
 
 You can check it out in the [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fablabbcn/smartcitizen-data-framework/master?filepath=%2Fexamples%2Fnotebooks) before installing if you want. Works with `Python 3.*` (tested until `python 3.9.5`).
 
 You can just run:
 
@@ -105,9 +126,7 @@
 ## Contribute
 
 Issues and PR more than welcome!
 
 ## Funding
 
 This work has received funding from the European Union's Horizon 2020 research and innovation program under the grant agreement [No. 689954](https://cordis.europa.eu/project/rcn/202639_en.html)
-
-
```

### Comparing `scdata-0.9.1/scdata.egg-info/SOURCES.txt` & `scdata-1.0.0/scdata.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 scdata/__init__.py
 scdata.egg-info/PKG-INFO
 scdata.egg-info/SOURCES.txt
 scdata.egg-info/dependency_links.txt
 scdata.egg-info/not-zip-safe
 scdata.egg-info/requires.txt
 scdata.egg-info/top_level.txt
 scdata/_config/__init__.py
 scdata/_config/config.py
+scdata/_config/custom_logger.py
 scdata/device/__init__.py
+scdata/device/device.py
 scdata/device/process/__init__.py
 scdata/device/process/alphasense.py
 scdata/device/process/baseline.py
 scdata/device/process/formulae.py
 scdata/device/process/geoseries.py
 scdata/device/process/params.py
 scdata/device/process/regression.py
 scdata/device/process/timeseries.py
 scdata/io/__init__.py
-scdata/io/csv.py
 scdata/io/device_api.py
-scdata/io/firmware.py
+scdata/io/device_file.py
 scdata/io/model.py
-scdata/io/user_api.py
+scdata/models/__init__.py
+scdata/models/models.py
 scdata/test/__init__.py
+scdata/test/test.py
+scdata/test/checks/__init__.py
+scdata/test/checks/checks.py
+scdata/test/dispersion/__init__.py
+scdata/test/dispersion/dispersion.py
 scdata/test/export/__init__.py
 scdata/test/export/to_file.py
 scdata/test/export/templates/sc_template.html
-scdata/test/load/__init__.py
-scdata/test/load/load.py
 scdata/test/plot/__init__.py
 scdata/test/plot/box_plot.py
 scdata/test/plot/heatmap_iplot.py
 scdata/test/plot/heatmap_plot.py
 scdata/test/plot/maps.py
 scdata/test/plot/plot_tools.py
 scdata/test/plot/scatter_dispersion_grid.py
@@ -47,46 +53,33 @@
 scdata/test/plot/ts_dispersion_grid.py
 scdata/test/plot/ts_dispersion_plot.py
 scdata/test/plot/ts_dispersion_uplot.py
 scdata/test/plot/ts_iplot.py
 scdata/test/plot/ts_plot.py
 scdata/test/plot/ts_scatter.py
 scdata/test/plot/ts_uplot.py
-scdata/test/utils/__init__.py
-scdata/test/utils/checks.py
-scdata/test/utils/combine.py
-scdata/test/utils/dispersion.py
-scdata/test/utils/prepare.py
-scdata/utils/__init__.py
-scdata/utils/cleaning.py
-scdata/utils/date.py
-scdata/utils/dictmerge.py
-scdata/utils/headers.py
-scdata/utils/lazy.py
-scdata/utils/location.py
-scdata/utils/logs.py
-scdata/utils/meta.py
-scdata/utils/out.py
-scdata/utils/report.py
-scdata/utils/stats.py
-scdata/utils/units.py
-scdata/utils/url_check.py
-scdata/utils/zenodo.py
-scdata/utils/interim/example.csv
-scdata/utils/interim/geodata.csv
-scdata/utils/uploads/example_upload_1.json
-scdata/utils/uploads/example_zenodo_upload.yaml
-scdata/utils/uploads/report.pdf
-scdata/utils/zenodo_templates/README.md
-scdata/utils/zenodo_templates/template_zenodo_dataset.json
-scdata/utils/zenodo_templates/template_zenodo_publication.json
-tools/__init__.py
-tools/asb-test.py
-tools/backup.py
-tools/esptool.py
-tools/options.py
-tools/register.py
-tools/sck.py
-tools/uf2conv.py
-tools/serialtools/__init__.py
-tools/serialtools/serialdevice.py
-tools/serialtools/serialworker.py
+scdata/test/tools/__init__.py
+scdata/test/tools/combine.py
+scdata/test/tools/history.py
+scdata/test/tools/prepare.py
+scdata/tools/__init__.py
+scdata/tools/cleaning.py
+scdata/tools/custom_logger.py
+scdata/tools/date.py
+scdata/tools/dictmerge.py
+scdata/tools/find.py
+scdata/tools/gets.py
+scdata/tools/lazy.py
+scdata/tools/location.py
+scdata/tools/report.py
+scdata/tools/stats.py
+scdata/tools/units.py
+scdata/tools/url_check.py
+scdata/tools/zenodo.py
+scdata/tools/interim/example.csv
+scdata/tools/interim/geodata.csv
+scdata/tools/uploads/example_upload_1.json
+scdata/tools/uploads/example_zenodo_upload.yaml
+scdata/tools/uploads/report.pdf
+scdata/tools/zenodo_templates/README.md
+scdata/tools/zenodo_templates/template_zenodo_dataset.json
+scdata/tools/zenodo_templates/template_zenodo_publication.json
```

