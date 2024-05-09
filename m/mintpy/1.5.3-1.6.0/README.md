# Comparing `tmp/mintpy-1.5.3.tar.gz` & `tmp/mintpy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintpy-1.5.3.tar", last modified: Thu Nov 23 12:47:22 2023, max compression
+gzip compressed data, was "mintpy-1.6.0.tar", last modified: Thu May  9 12:29:53 2024, max compression
```

## Comparing `mintpy-1.5.3.tar` & `mintpy-1.6.0.tar`

### file list

```diff
@@ -1,231 +1,351 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.350313 mintpy-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35900 2023-11-23 12:47:15.000000 mintpy-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-23 12:47:15.000000 mintpy-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2023-11-23 12:47:22.350313 mintpy-1.5.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.306311 mintpy-1.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2023-11-23 12:47:15.000000 mintpy-1.5.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-23 12:47:15.000000 mintpy-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 12:47:22.350313 mintpy-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2023-11-23 12:47:15.000000 mintpy-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.302310 mintpy-1.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.318311 mintpy-1.5.3/src/mintpy/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20506 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/add.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/asc_desc2horz_vert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.334312 mintpy-1.5.3/src/mintpy/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7484 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/asc_desc2horz_vert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5039 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/closure_phase_bias.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7651 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/dem_error.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2657 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/dem_gsi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3380 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9030 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/generate_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10837 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/geocode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12366 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/ifgram_inversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2743 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/image_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3243 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/image_stitch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3763 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6107 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/iono_tec.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4657 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/load_data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1929 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/load_gbis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/local_oscilator_drift.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/lookup_geo2radar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2994 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/mask.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11681 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/modify_network.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4465 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/multilook.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6726 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/plate_motion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5189 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/plot_coherence_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7382 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/plot_network.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8268 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/plot_transection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9818 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_aria.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1928 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_cosicorr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5056 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_fringe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5882 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_gamma.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_gmtsar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4305 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_hyp3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4997 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_isce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2687 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_nisar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2274 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_roipac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3891 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/prep_snap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/reference_date.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6752 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/reference_point.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2684 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/remove_hdf5_dset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5302 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/remove_ramp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5013 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/s1ab_range_bias.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_gbis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2511 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_gdal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2304 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_gmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4754 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_hdfeos5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3450 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_kite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7244 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_kmz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5379 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_kmz_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2756 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_qgis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4100 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/save_roipac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8348 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/smallbaselineApp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5530 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/solid_earth_tides.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2877 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/spatial_average.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3838 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/spatial_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5657 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4375 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/temporal_average.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1599 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/temporal_derivative.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2403 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/temporal_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10596 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/timeseries2velocity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3594 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/timeseries_rms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/tropo_gacos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3248 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/tropo_phase_elevation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7824 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/tropo_pyaps3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7953 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/tsview.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5914 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/unwrap_error_bridging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6719 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/unwrap_error_phase_closure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7902 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/cli/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    46305 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/closure_phase_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.334312 mintpy-1.5.3/src/mintpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.338312 mintpy-1.5.3/src/mintpy/data/colormaps/
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/BlueWhiteOrangeRed.cpt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/DEM_print.cpt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/GMT_haxby.cpt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/GMT_no_green.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/batlow.cpt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/differences.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/hawaii.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/oleron.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/roma.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/romanian.cpt
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/seminf-haxby.cpt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/temp-c.cpt
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/temperature.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10086 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/vik.cpt
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/vikO.cpt
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/wiki-2.0.cpt
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/wiki-schwarzwald-d050.cpt
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/colormaps/wiki-scotland.cpt
--rw-r--r--   0 runner    (1001) docker     (127)   220489 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/dygraph-combined.js
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/shaded_dot.png
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/data/star.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.338312 mintpy-1.5.3/src/mintpy/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/auto_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/job4stripmapStack.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/mintpy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/selectNetwork.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    23937 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/smallbaselineApp.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/smallbaselineApp_auto.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/defaults/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/dem_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/dem_gsi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/generate_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/geocode.py
--rw-r--r--   0 runner    (1001) docker     (127)    50423 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/ifgram_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/image_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/image_stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/iono_tec.py
--rw-r--r--   0 runner    (1001) docker     (127)    35235 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/load_gbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/local_oscilator_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/lookup_geo2radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/modify_network.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35675 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/multi_transect.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/multilook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.342313 mintpy-1.5.3/src/mintpy/objects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    16164 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/conncomp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22115 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/coord.py
--rw-r--r--   0 runner    (1001) docker     (127)    36124 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/euler_pole.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/giant.py
--rw-r--r--   0 runner    (1001) docker     (127)    25505 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13582 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/insar_vs_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/ionex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)    39102 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    62999 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    41835 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/objects/stackDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/plate_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/plot_coherence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/plot_transection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19482 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_aria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_cosicorr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14838 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_fringe.py
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_gmtsar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_hyp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_isce.py
--rw-r--r--   0 runner    (1001) docker     (127)    16065 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_nisar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/prep_roipac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/reference_date.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/reference_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/s1ab_range_bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_gbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_gdal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_gmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16450 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_hdfeos5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_kite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_kmz.py
--rw-r--r--   0 runner    (1001) docker     (127)    22100 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_kmz_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_qgis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/save_roipac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.342313 mintpy-1.5.3/src/mintpy/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/decorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/defo_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/fractal.py
--rw-r--r--   0 runner    (1001) docker     (127)    23699 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/iono.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/simulation/variance.py
--rw-r--r--   0 runner    (1001) docker     (127)    50622 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/smallbaselineApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/solid_earth_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/spatial_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18666 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27744 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/timeseries2velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/timeseries_rms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/tropo_gacos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/tropo_phase_elevation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25608 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/tropo_pyaps3.py
--rw-r--r--   0 runner    (1001) docker     (127)    38014 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/tsview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/unwrap_error_bridging.py
--rw-r--r--   0 runner    (1001) docker     (127)    17913 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/unwrap_error_phase_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.346313 mintpy-1.5.3/src/mintpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31402 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    45274 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/isce_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    36466 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    93646 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/plot_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    18186 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/ptime.py
--rw-r--r--   0 runner    (1001) docker     (127)    86920 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/readfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/s1_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.346313 mintpy-1.5.3/src/mintpy/utils/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/solvers/l1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5308 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/solvers/l1regls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/solvers/lstl1.py
--rw-r--r--   0 runner    (1001) docker     (127)    19547 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/time_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    20190 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46683 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/utils0.py
--rw-r--r--   0 runner    (1001) docker     (127)    37800 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/utils1.py
--rw-r--r--   0 runner    (1001) docker     (127)    30870 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/utils/writefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    64196 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.346313 mintpy-1.5.3/src/mintpy/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-23 12:47:15.000000 mintpy-1.5.3/src/mintpy/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 12:47:22.346313 mintpy-1.5.3/src/mintpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-23 12:47:22.000000 mintpy-1.5.3/src/mintpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.474532 mintpy-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.410531 mintpy-1.6.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-09 12:29:49.000000 mintpy-1.6.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.414532 mintpy-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.414532 mintpy-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.414532 mintpy-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/workflows/build-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-09 12:29:49.000000 mintpy-1.6.0/.github/workflows/build-n-publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-09 12:29:49.000000 mintpy-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-09 12:29:49.000000 mintpy-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 12:29:49.000000 mintpy-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-09 12:29:49.000000 mintpy-1.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35900 2024-05-09 12:29:49.000000 mintpy-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 12:29:49.000000 mintpy-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-09 12:29:53.474532 mintpy-1.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.418532 mintpy-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/FAQs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/QGIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.418532 mintpy-1.6.0/docs/_includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_includes/analytics.html
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_includes/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_includes/page-footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_includes/page-header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_includes/share.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.418532 mintpy-1.6.0/docs/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_layouts/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/_layouts/default_tactile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.418532 mintpy-1.6.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/attributes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/colormaps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/coord.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/data_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/doc_generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/latex.sty
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/api/module_hierarchy.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/dask.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/demo_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27183 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/dir_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/google_earth.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/hdfeos5.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/ports.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/references.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.422531 mintpy-1.6.0/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/FernandinaSenDT128.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/GalapagosAlosAT133.template
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/GalapagosEnvA2T061.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/GalapagosSenDT128.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/KirishimaAlos2DT23F2970.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/KujuAlosAT422F650.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/NCalAlos2DT169.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/RidgecrestSenDT71.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/SanFranSenDT42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/WCapeSenAT29.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-09 12:29:49.000000 mintpy-1.6.0/docs/templates/WellsEnvD2T399.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 12:29:49.000000 mintpy-1.6.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-09 12:29:49.000000 mintpy-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 12:29:49.000000 mintpy-1.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.422531 mintpy-1.6.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2226 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/compare_velocity_with_diff_tropo.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3710 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/fix_typos.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/jupyter_notebook_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/load_data_aoi.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4415 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/plot_smallbaselineApp.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5171 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/post_aoi.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10803 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/post_process_Alos.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      713 2024-05-09 12:29:49.000000 mintpy-1.6.0/scripts/run_stripmap_stack.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:29:53.474532 mintpy-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.406531 mintpy-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.434532 mintpy-1.6.0/src/mintpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20779 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/asc_desc2horz_vert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.446531 mintpy-1.6.0/src/mintpy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7484 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/asc_desc2horz_vert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5039 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/closure_phase_bias.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7643 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/dem_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2657 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/dem_gsi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3380 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9033 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/generate_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10837 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/geocode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12952 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/ifgram_inversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2743 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/image_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3243 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/image_stitch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3763 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6062 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/iono_split_spectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6107 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/iono_tec.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4657 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/load_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1929 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/load_gbis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2492 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/local_oscilator_drift.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/lookup_geo2radar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2994 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12232 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/modify_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4465 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/multilook.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6726 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/plate_motion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5189 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/plot_coherence_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7382 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/plot_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8252 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/plot_transection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9818 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_aria.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1928 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_cosicorr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5056 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_fringe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5882 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_gamma.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_gmtsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4305 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_hyp3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4997 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_isce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_nisar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2274 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_roipac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3891 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/prep_snap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/reference_date.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6752 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/reference_point.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2684 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/remove_hdf5_dset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5302 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/remove_ramp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5013 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/s1ab_range_bias.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_gbis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2511 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_gdal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2304 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_gmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4754 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_hdfeos5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3450 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_kite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7244 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_kmz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5379 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_kmz_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2756 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_qgis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4100 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/save_roipac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8367 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/smallbaselineApp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5530 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/solid_earth_tides.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2877 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/spatial_average.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3838 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/spatial_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5657 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4375 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/temporal_average.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1599 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/temporal_derivative.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2403 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/temporal_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11113 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/timeseries2velocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3594 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/timeseries_rms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/tropo_gacos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3248 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/tropo_phase_elevation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7824 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/tropo_pyaps3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7957 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/tsview.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5916 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/unwrap_error_bridging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6721 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/unwrap_error_phase_closure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8086 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46305 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/closure_phase_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.450531 mintpy-1.6.0/src/mintpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.450531 mintpy-1.6.0/src/mintpy/data/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/BlueWhiteOrangeRed.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/DEM_print.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/GMT_haxby.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/GMT_no_green.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/batlow.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/differences.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/hawaii.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/oleron.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/roma.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/romanian.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/seminf-haxby.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/temp-c.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/temperature.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/vik.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/vikO.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/wiki-2.0.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/wiki-schwarzwald-d050.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/colormaps/wiki-scotland.cpt
+-rw-r--r--   0 runner    (1001) docker     (127)   220489 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/dygraph-combined.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.450531 mintpy-1.6.0/src/mintpy/data/plate_boundary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.450531 mintpy-1.6.0/src/mintpy/data/plate_boundary/GSRM/
+-rw-r--r--   0 runner    (1001) docker     (127)   196747 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/plate_boundary/GSRM/plate_outlines.lola
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.450531 mintpy-1.6.0/src/mintpy/data/plate_boundary/MORVEL/
+-rw-r--r--   0 runner    (1001) docker     (127)   234267 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/plate_boundary/MORVEL/plate_outlines.lalo
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/plate_boundary/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/shaded_dot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/star.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/data/top_tec_perc_s1.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.454532 mintpy-1.6.0/src/mintpy/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/auto_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/job4stripmapStack.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/mintpy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/selectNetwork.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    24513 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/smallbaselineApp.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/smallbaselineApp_auto.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/defaults/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/dem_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/dem_gsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/generate_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50661 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/ifgram_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/image_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/image_stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/iono_split_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/iono_tec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.458531 mintpy-1.6.0/src/mintpy/legacy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3047 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/2to3_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3064 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/add_attribute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7144 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/baseline_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7441 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/baseline_trop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/correlation_with_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2965 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/ifgram_reconstruction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6016 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/ifgram_simulation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2427 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/incidence_angle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19474 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/insar_vs_gps_legacy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5022 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/load2hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/prep_giant.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1741 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/quality_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1897 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/range_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/save_ifg_list4giant.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5473 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/save_mat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23516 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/select_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34456 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/transect_legacy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18401 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/transect_legacy2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21969 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/tropo_pyaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35408 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/load_gbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/local_oscilator_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/lookup_geo2radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15326 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/modify_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35675 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/multi_transect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/multilook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.462531 mintpy-1.6.0/src/mintpy/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16164 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/conncomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23597 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36124 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/euler_pole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/giant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47838 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/gnss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/insar_vs_gnss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/ionex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39102 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23403 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62999 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41835 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/objects/stackDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/plate_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/plot_coherence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/plot_transection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19482 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_aria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_cosicorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_fringe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_gmtsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_isce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_nisar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/prep_roipac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/reference_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/reference_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/s1ab_range_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_gbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_gmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_hdfeos5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_kite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_kmz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22100 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_kmz_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/save_roipac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.462531 mintpy-1.6.0/src/mintpy/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/decorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/defo_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/fractal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23699 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/iono.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/simulation/variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52252 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/smallbaselineApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/solid_earth_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/spatial_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27744 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/timeseries2velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/timeseries_rms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/tropo_gacos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/tropo_phase_elevation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/tropo_pyaps3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38185 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/tsview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/unwrap_error_bridging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/unwrap_error_phase_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.466531 mintpy-1.6.0/src/mintpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33486 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46574 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/isce_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36466 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95430 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/plot_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/ptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87642 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/readfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/s1_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.466531 mintpy-1.6.0/src/mintpy/utils/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/solvers/l1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5308 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/solvers/l1regls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/solvers/lstl1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19547 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/time_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21555 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49105 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/utils0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37800 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/utils1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30870 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/utils/writefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65704 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.466531 mintpy-1.6.0/src/mintpy/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 12:29:49.000000 mintpy-1.6.0/src/mintpy/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.470531 mintpy-1.6.0/src/mintpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 12:29:53.000000 mintpy-1.6.0/src/mintpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.470531 mintpy-1.6.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4188 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/asc_desc2horz_vert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.470531 mintpy-1.6.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/FernandinaSenDT128.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/KujuAlosAT422F650.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/RidgecrestSenDT71.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/SanFranSenDT42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/WCapeSenAT29.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/WellsEnvD2T399.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/configs/unittestGalapagosSenDT128.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.470531 mintpy-1.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   859924 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/data/jplg3190.15i
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7314 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/dem_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.470531 mintpy-1.6.0/tests/objects/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2934 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/objects/euler_pole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2730 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/objects/ionex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8031 2024-05-09 12:29:49.000000 mintpy-1.6.0/tests/smallbaselineApp.py
```

### Comparing `mintpy-1.5.3/LICENSE` & `mintpy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/PKG-INFO` & `mintpy-1.6.0/docs/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,8 @@
-Metadata-Version: 2.1
-Name: mintpy
-Version: 1.5.3
-Summary: Miami INsar Time-series software in PYthon
-Home-page: https://github.com/insarlab/MintPy
-Download-URL: https://github.com/insarlab/MintPy/archive/v1.5.3.tar.gz
-Author: Zhang Yunjun, Heresh Fattahi
-Author-email: yunjunz@outlook.com
-License: GPL-3.0-or-later
-Project-URL: Bug Reports, https://github.com/insarlab/mintpy/issues
-Project-URL: Documentation, https://mintpy.readthedocs.io/
-Project-URL: Source, https://github.com/insarlab/mintpy
-Keywords: InSAR,deformation,time-series,volcano,earthquake,tectonics,geodesy,geophysics,remote-sensing
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argcomplete
-Requires-Dist: cartopy
-Requires-Dist: cvxopt
-Requires-Dist: dask>=1.0
-Requires-Dist: dask-jobqueue>=0.3
-Requires-Dist: h5py
-Requires-Dist: joblib
-Requires-Dist: lxml
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pre-commit
-Requires-Dist: pyaps3>=0.3
-Requires-Dist: pykml>=0.2
-Requires-Dist: pyproj
-Requires-Dist: pyresample
-Requires-Dist: pysolid
-Requires-Dist: rich
-Requires-Dist: setuptools
-Requires-Dist: scikit-image
-Requires-Dist: scipy
-Requires-Dist: shapely
-Requires-Dist: utm
-Provides-Extra: extra
-Requires-Dist: gdal; extra == "extra"
-Provides-Extra: fractal
-Requires-Dist: pyfftw; extra == "fractal"
-Provides-Extra: gbis
-Requires-Dist: geoid; extra == "gbis"
-Provides-Extra: isce
-Requires-Dist: isce; extra == "isce"
-Provides-Extra: kite
-Requires-Dist: kite; extra == "kite"
-Provides-Extra: all
-Requires-Dist: extra; extra == "all"
-Requires-Dist: fractal; extra == "all"
-Requires-Dist: gbis; extra == "all"
-Requires-Dist: isce; extra == "all"
-Requires-Dist: kite; extra == "all"
-
-[![Language](https://img.shields.io/badge/python-3.6%2B-blue.svg?style=flat-square)](https://www.python.org/)
+[![Language](https://img.shields.io/badge/python-3.8%2B-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs Status](https://readthedocs.org/projects/mintpy/badge/?version=latest&style=flat-square)](https://mintpy.readthedocs.io/?badge=latest)
 [![CircleCI](https://img.shields.io/circleci/build/github/insarlab/MintPy.svg?logo=circleci&label=tests&style=flat-square)](https://circleci.com/gh/insarlab/MintPy)
 [![Docker Status](https://img.shields.io/github/actions/workflow/status/insarlab/MintPy/build-docker.yml?label=docker&style=flat-square&logo=docker&logoColor=white)](https://github.com/insarlab/MintPy/pkgs/container/mintpy)
 [![Conda Download](https://img.shields.io/conda/dn/conda-forge/mintpy?color=green&style=flat-square&label=conda%20downloads)](https://anaconda.org/conda-forge/mintpy)
 [![Version](https://img.shields.io/github/v/release/insarlab/MintPy?color=yellow&label=version&style=flat-square)](https://github.com/insarlab/MintPy/releases)
 [![Forum](https://img.shields.io/badge/forum-Google%20Groups-orange.svg?style=flat-square)](https://groups.google.com/g/mintpy)
 [![License](https://img.shields.io/badge/license-GPLv3+-blue.svg?style=flat-square)](https://github.com/insarlab/MintPy/blob/main/LICENSE)
```

### Comparing `mintpy-1.5.3/src/mintpy/__main__.py` & `mintpy-1.6.0/src/mintpy/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,21 @@
 def get_info_parser(subparsers=None):
     from mintpy.cli import info
     parser = info.create_parser(subparsers)
     parser.set_defaults(func=info.main)
     return parser
 
 
+def get_iono_split_spectrum_parser(subparsers=None):
+    from mintpy.cli import iono_split_spectrum
+    parser = iono_split_spectrum.create_parser(subparsers)
+    parser.set_defaults(func=iono_split_spectrum.main)
+    return parser
+
+
 def get_iono_tec_parser(subparsers=None):
     from mintpy.cli import iono_tec
     parser = iono_tec.create_parser(subparsers)
     parser.set_defaults(func=iono_tec.main)
     return parser
 
 
@@ -603,14 +610,15 @@
     get_image_math_parser(sp)
     get_image_stitch_parser(sp)
     get_subset_parser(sp)
 
     # noise reduction / error correction
     get_closure_phase_bias_parser(sp)
     get_dem_error_parser(sp)
+    get_iono_split_spectrum_parser(sp)
     get_iono_tec_parser(sp)
     get_local_oscilator_drift_parser(sp)
     get_plate_motion_parser(sp)
     get_remove_ramp_parser(sp)
     get_s1ab_range_bias_parser(sp)
     get_solid_earth_tides_parser(sp)
     get_tropo_gacos_parser(sp)
```

### Comparing `mintpy-1.5.3/src/mintpy/add.py` & `mintpy-1.6.0/src/mintpy/add.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/asc_desc2horz_vert.py` & `mintpy-1.6.0/src/mintpy/asc_desc2horz_vert.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,15 @@
     else:
         los_inc_angle = np.zeros(num_file, dtype=np.float32)
         los_az_angle  = np.zeros(num_file, dtype=np.float32)
 
     for i, (atr, fname) in enumerate(zip(atr_list, inps.file)):
         # overlap SNWE --> box to read for each specific file
         coord = ut.coordinate(atr)
-        x0 = coord.lalo2yx(W, coord_type='lon')
-        y0 = coord.lalo2yx(N, coord_type='lat')
+        y0, x0 = coord.lalo2yx(N, W)
         box = (x0, y0, x0 + width, y0 + length)
 
         # read data
         dlos[i, :] = readfile.read(fname, box=box, datasetName=inps.ds_name)[0]
         msg = f'{inps.ds_name} ' if inps.ds_name else ''
         print(f'read {msg} from file: {fname}')
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/add.py` & `mintpy-1.6.0/src/mintpy/cli/add.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/asc_desc2horz_vert.py` & `mintpy-1.6.0/src/mintpy/cli/asc_desc2horz_vert.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/closure_phase_bias.py` & `mintpy-1.6.0/src/mintpy/cli/closure_phase_bias.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/dem_error.py` & `mintpy-1.6.0/src/mintpy/cli/dem_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     defo_model.add_argument('-t', '--template', dest='template_file',
                             help='template file with the options')
     defo_model.add_argument('--ex', '--exclude', dest='excludeDate', nargs='*', default=[],
                             help='Exclude date(s) for DEM error estimation.\n' +
                                  'All dates will be corrected for DEM residual phase still.')
     defo_model.add_argument('-p', '--poly-order', dest='polyOrder', type=int, default=2,
                             help='polynomial order number of temporal deformation model (default: %(default)s).')
-    defo_model.add_argument('-s', '--step-date', dest='stepFuncDate', nargs='*', default=[],
+    defo_model.add_argument('-s', '--step-date', dest='stepDate', nargs='*', default=[],
                             help='Date of step jump for temporal deformation model (default: %(default)s).'+
                                  ' i.e. date of earthquake/volcanic eruption')
     defo_model.add_argument('--periodic', '--period', '--peri', dest='periodic', type=float, nargs='+', default=[],
                             help='periodic functinos of temporal deformation model (default: %(default)s).')
 
     parser.add_argument('--phase-velocity', dest='phaseVelocity', action='store_true',
                         help='Use phase velocity instead of phase for inversion constrain.')
@@ -139,15 +139,15 @@
     for key in key_list:
         value = template[key_prefix+key]
         if key in ['phaseVelocity']:
             iDict[key] = value
         elif value:
             if key in ['polyOrder']:
                 iDict[key] = int(value)
-            elif key in ['excludeDate','stepFuncDate']:
+            elif key in ['excludeDate','stepDate']:
                 iDict[key] = ptime.yyyymmdd(value.split(','))
 
     # computing configurations
     dask_key_prefix = 'mintpy.compute.'
     key_list = [i for i in list(iDict.keys()) if dask_key_prefix+i in template.keys()]
     for key in key_list:
         value = template[dask_key_prefix+key]
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/dem_gsi.py` & `mintpy-1.6.0/src/mintpy/cli/dem_gsi.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/diff.py` & `mintpy-1.6.0/src/mintpy/cli/diff.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/generate_mask.py` & `mintpy-1.6.0/src/mintpy/cli/generate_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   generate_mask.py  temporalCoherence.h5 -m 0.7 -o maskTempCoh.h5 --base inputs/geometryRadar.h5 --base-dset shadow --base-value 1
   generate_mask.py  avgSpatialCoh.h5     -m 0.7 --base waterMask.h5 -o maskSpatialCoh.h5
 
   # exclude area by min/max value and/or subset in row/col direction
   generate_mask.py  081018_090118.unw -m 3 -M 8 -y 100 700 -x 200 800 -o mask_1.h5
 
   # exclude pixel cluster based on minimum number of pixels
-  generate_mask.py  maskTempCoh.h5 -p 10 mask_1.h5
+  generate_mask.py  maskTempCoh.h5 -p 10 -o mask_1.h5
 
   # exclude pixels with large velocity STD: |velocity| > cutoff (2 by default) * velocityStd
   generate_mask.py  velocity.h5 --vstd
   generate_mask.py  velocity.h5 --vstd --vstd-num 3
 
   # exclude / include an circular area
   generate_mask.py  maskTempCoh.h5 -m 0.5 --ex-circle 230 283 100 -o maskTempCoh_nonDef.h5
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/geocode.py` & `mintpy-1.6.0/src/mintpy/cli/geocode.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/ifgram_inversion.py` & `mintpy-1.6.0/src/mintpy/cli/ifgram_inversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,34 @@
 from mintpy.defaults.template import get_template_content
 from mintpy.utils import arg_utils
 
 ################################################################################################
 TEMPLATE = get_template_content('invert_network')
 
 REFERENCE = """references:
+  # SBAS
   Berardino, P., Fornaro, G., Lanari, R., & Sansosti, E. (2002). A new algorithm for surface
     deformation monitoring based on small baseline differential SAR interferograms. IEEE TGRS,
     40(11), 2375-2383. doi:10.1109/TGRS.2002.803792
-  Pepe, A., and Lanari, R. (2006), On the extension of the minimum cost flow algorithm for phase unwrapping
-    of multitemporal differential SAR interferograms, IEEE-TGRS, 44(9), 2374-2383.
+
+  # weighted SBAS: coh, fim, var
   Perissin, D., and Wang, T. (2012), Repeat-pass SAR interferometry with partially coherent targets, IEEE TGRS,
     50(1), 271-280, doi:10.1109/tgrs.2011.2160644.
   Samiei-Esfahany, S., Martins, J. E., Van Leijen, F., and Hanssen, R. F. (2016), Phase Estimation for Distributed
     Scatterers in InSAR Stacks Using Integer Least Squares Estimation, IEEE TGRS, 54(10), 5671-5687.
   Seymour, M. S., and Cumming, I. G. (1994), Maximum likelihood estimation for SAR interferometry, 1994.
     IGARSS '94., 8-12 Aug 1994.
   Yunjun, Z., Fattahi, H., and Amelung, F. (2019), Small baseline InSAR time series analysis: Unwrapping error
     correction and noise reduction, Computers & Geosciences, 133, 104331, doi:10.1016/j.cageo.2019.104331.
+
+  # temporal coherence
+  Pepe, A., and Lanari, R. (2006), On the extension of the minimum cost flow algorithm for phase unwrapping
+    of multitemporal differential SAR interferograms, IEEE-TGRS, 44(9), 2374-2383.
+
+  # time-series uncertainty
   Yunjun, Z., Fattahi, H., Brancato, V., Rosen, P., Simons, M. (2021), Oral: Tectonic displacement mapping from SAR
     offset time series: noise reduction and uncertainty quantification, ID 590, FRINGE 2021, 31 May – 4 Jun, 2021, Virtual.
 """
 
 EXAMPLE = """example:
   ifgram_inversion.py inputs/ifgramStack.h5 -t smallbaselineApp.cfg --update
   ifgram_inversion.py inputs/ifgramStack.h5 -w no  # turn off weight for fast processing
@@ -118,14 +125,19 @@
     parser = create_parser()
     inps = parser.parse_args(args=iargs)
 
     # import
     from mintpy.objects import cluster, ifgramStack
     from mintpy.utils import readfile
 
+    # save argv (to check the manually specified arguments)
+    # use iargs        for python call
+    # use sys.argv[1:] for command line call
+    inps.argv = iargs if iargs else sys.argv[1:]
+
     # check
     atr = readfile.read_attribute(inps.ifgramStackFile)
 
     # check: input file type
     if atr['FILE_TYPE'] not in ['ifgramStack']:
         raise ValueError('input is {} file, support ifgramStack file only.'.format(atr['FILE_TYPE']))
 
@@ -205,28 +217,33 @@
     from mintpy.ifgram_inversion import key_prefix
     from mintpy.utils import readfile, utils1 as ut
 
     iDict = vars(inps)
     template = readfile.read_template(template_file)
     template = ut.check_template_auto_value(template)
 
-    key_list = [i for i in list(iDict.keys()) if key_prefix+i in template.keys()]
+    key_list = [x for x in list(iDict.keys()) if key_prefix+x in template.keys()]
+    # ensure manually specified options in command line overwrite template options
+    # by ignoring the keys appeared in command line
+    dest_opt_str = arg_utils.get_dest_option_str_dict(create_parser())
+    key_list = [x for x in key_list if all(y not in inps.argv for y in dest_opt_str[x])]
+
     for key in key_list:
         value = template[key_prefix+key]
         if key in ['weightFunc', 'maskDataset', 'minNormVelocity']:
             iDict[key] = value
         elif value:
             if key in ['maskThreshold', 'minRedundancy']:
                 iDict[key] = float(value)
             elif key in ['residualNorm', 'waterMaskFile']:
                 iDict[key] = value
 
     # computing configurations
     dask_key_prefix = 'mintpy.compute.'
-    key_list = [i for i in list(iDict.keys()) if dask_key_prefix+i in template.keys()]
+    key_list = [x for x in list(iDict.keys()) if dask_key_prefix+x in template.keys()]
     for key in key_list:
         value = template[dask_key_prefix+key]
         if key in ['cluster', 'config']:
             iDict[key] = value
         elif value:
             if key in ['numWorker']:
                 iDict[key] = str(value)
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/image_math.py` & `mintpy-1.6.0/src/mintpy/cli/image_math.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/image_stitch.py` & `mintpy-1.6.0/src/mintpy/cli/image_stitch.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/info.py` & `mintpy-1.6.0/src/mintpy/cli/info.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/iono_tec.py` & `mintpy-1.6.0/src/mintpy/cli/iono_tec.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/load_data.py` & `mintpy-1.6.0/src/mintpy/cli/load_data.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/load_gbis.py` & `mintpy-1.6.0/src/mintpy/cli/load_gbis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/local_oscilator_drift.py` & `mintpy-1.6.0/src/mintpy/cli/local_oscilator_drift.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/lookup_geo2radar.py` & `mintpy-1.6.0/src/mintpy/cli/lookup_geo2radar.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/mask.py` & `mintpy-1.6.0/src/mintpy/cli/mask.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/modify_network.py` & `mintpy-1.6.0/src/mintpy/cli/modify_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     parser.add_argument('--max-conn-num', dest='connNumMax', type=int,
                         help='max number of connections/neighbors per acquisition')
     parser.add_argument('-r', '--reference', dest='referenceFile',
                         help='Reference hdf5 / list file with network information.\n'
                              'i.e. ifgramStack.h5, date12_list.txt')
     parser.add_argument('--exclude-ifg-index', dest='excludeIfgIndex', nargs='*',
                         help='index of interferograms to remove/drop.\n1 as the first')
-    parser.add_argument('--exclude-date', dest='excludeDate', nargs='*',
+    parser.add_argument('--exclude-ifg','--ex-ifg','--ex-date12', dest='excludeDate12', nargs='*',
+                        help='pair(s) to remove/drop in YYYYMMDD_YYYYMMDD format.')
+    parser.add_argument('--exclude-date','--ex-date', dest='excludeDate', nargs='*',
                         help='date(s) to remove/drop, all interferograms included date(s) will be removed')
     parser.add_argument('--start-date', '--min-date', dest='startDate',
                         help='remove/drop interferograms with date earlier than start-date in YYMMDD or YYYYMMDD format')
     parser.add_argument('--end-date', '--max-date', dest='endDate',
                         help='remove/drop interferograms with date later than end-date in YYMMDD or YYYYMMDD format')
 
     # 2. coherence-based network
@@ -105,32 +107,38 @@
 
 def cmd_line_parse(iargs=None):
     # parse
     parser = create_parser()
     inps = parser.parse_args(args=iargs)
 
     # import
-    from mintpy.utils import readfile, utils as ut
+    from mintpy.utils import ptime, readfile, utils as ut
 
     # check: --mask option
     if not os.path.isfile(inps.maskFile):
         inps.maskFile = None
 
     # check: --exclude-ifg-index option (convert input index to continuous index list)
     inps.excludeIfgIndex = read_input_index_list(inps.excludeIfgIndex, stackFile=inps.file)
 
+    # check: --ex-date(12) options
+    if inps.excludeDate:
+        inps.exlcudeDate = ptime.yyyymmdd(inps.excludeDate)
+    if inps.excludeDate12:
+        inps.excludeDate12 = ptime.yyyymmdd_date12(inps.excludeDate12)
+
     # check: -t / --template option
     if inps.template_file:
         inps = read_template2inps(inps.template_file, inps)
 
     # check: input arguments (required at least one)
     required_args = [
         inps.referenceFile, inps.tempBaseMax, inps.perpBaseMax, inps.connNumMax,
-        inps.excludeIfgIndex, inps.excludeDate, inps.coherenceBased, inps.areaRatioBased,
-        inps.startDate, inps.endDate, inps.reset, inps.manual,
+        inps.excludeIfgIndex, inps.excludeDate, inps.excludeDate12, inps.coherenceBased,
+        inps.areaRatioBased, inps.startDate, inps.endDate, inps.reset, inps.manual,
     ]
     if all(not i for i in required_args + [inps.template_file]):
         msg = 'No input option found to remove interferogram, exit.\n'
         msg += 'To manually modify network, please use --manual option '
         raise Exception(msg)
 
     # default: --lookup option
@@ -195,14 +203,16 @@
                 sub_lon = sorted(float(i.strip()) for i in tmp[1].split(':'))
                 inps.aoiLALO = (sub_lon[0], sub_lat[1], sub_lon[1], sub_lat[0])
 
             elif key in ['startDate', 'endDate']:
                 iDict[key] = ptime.yyyymmdd(value)
             elif key == 'excludeDate':
                 iDict[key] = ptime.yyyymmdd(value.split(','))
+            elif key == 'excludeDate12':
+                iDict[key] = ptime.yyyymmdd_date12(value.split(','))
             elif key == 'excludeIfgIndex':
                 iDict[key] += value.split(',')
                 iDict[key] = read_input_index_list(iDict[key], stackFile=inps.file)
 
     return inps
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/multilook.py` & `mintpy-1.6.0/src/mintpy/cli/multilook.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/plate_motion.py` & `mintpy-1.6.0/src/mintpy/cli/plate_motion.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/plot_coherence_matrix.py` & `mintpy-1.6.0/src/mintpy/cli/plot_coherence_matrix.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/plot_network.py` & `mintpy-1.6.0/src/mintpy/cli/plot_network.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/plot_transection.py` & `mintpy-1.6.0/src/mintpy/cli/plot_transection.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 
     # check: --line-file option (lola_file --> start/end_lalo)
     if inps.lola_file:
         inps.start_lalo, inps.end_lalo = read_lonlat_file(inps.lola_file)
 
     # check: --start/end-lalo (start/end_lalo --> start/end_yx)
     if inps.start_lalo and inps.end_lalo:
-        [y0, y1] = inps.coord.lalo2yx([inps.start_lalo[0], inps.end_lalo[0]], coord_type='lat')
-        [x0, x1] = inps.coord.lalo2yx([inps.start_lalo[1], inps.end_lalo[1]], coord_type='lon')
+        [y0, y1], [x0, x1] = inps.coord.lalo2yx([inps.start_lalo[0], inps.end_lalo[0]],
+                                                [inps.start_lalo[1], inps.end_lalo[1]])
         inps.start_yx = [y0, x0]
         inps.end_yx = [y1, x1]
 
     # default: --dset option
     if not inps.dset:
         inps.dset = readfile.get_slice_list(inps.file[0])[0]
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_aria.py` & `mintpy-1.6.0/src/mintpy/cli/prep_aria.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_cosicorr.py` & `mintpy-1.6.0/src/mintpy/cli/prep_cosicorr.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_fringe.py` & `mintpy-1.6.0/src/mintpy/cli/prep_fringe.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_gamma.py` & `mintpy-1.6.0/src/mintpy/cli/prep_gamma.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_gmtsar.py` & `mintpy-1.6.0/src/mintpy/cli/prep_gmtsar.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_hyp3.py` & `mintpy-1.6.0/src/mintpy/cli/prep_hyp3.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_isce.py` & `mintpy-1.6.0/src/mintpy/cli/prep_isce.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_nisar.py` & `mintpy-1.6.0/src/mintpy/cli/prep_nisar.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,28 @@
         dest="dem_file",
         type=str,
         default="./dem.tif",
         help="path to the DEM (default: %(default)s).",
     )
 
     parser.add_argument(
+        "-m",
+        "--mask",
+        dest="mask_file",
+        type=str,
+        default=None,
+        help="path to the mask (default: %(default)s).",
+    )
+
+    parser.add_argument(
         "-o",
         "--out-dir",
         dest="out_dir",
         type=str,
-        default="./mintpy",
+        default=".",
         help="output directory (default: %(default)s).",
     )
 
     parser.add_argument(
         '--force',
         dest='update_mode',
         action='store_false',
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_roipac.py` & `mintpy-1.6.0/src/mintpy/cli/prep_roipac.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/prep_snap.py` & `mintpy-1.6.0/src/mintpy/cli/prep_snap.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/reference_date.py` & `mintpy-1.6.0/src/mintpy/cli/reference_date.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/reference_point.py` & `mintpy-1.6.0/src/mintpy/cli/reference_point.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/remove_hdf5_dset.py` & `mintpy-1.6.0/src/mintpy/cli/remove_hdf5_dset.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/remove_ramp.py` & `mintpy-1.6.0/src/mintpy/cli/remove_ramp.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/s1ab_range_bias.py` & `mintpy-1.6.0/src/mintpy/cli/s1ab_range_bias.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_gbis.py` & `mintpy-1.6.0/src/mintpy/cli/save_gbis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_gdal.py` & `mintpy-1.6.0/src/mintpy/cli/save_gdal.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_gmt.py` & `mintpy-1.6.0/src/mintpy/cli/save_gmt.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_hdfeos5.py` & `mintpy-1.6.0/src/mintpy/cli/save_hdfeos5.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_kite.py` & `mintpy-1.6.0/src/mintpy/cli/save_kite.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_kmz.py` & `mintpy-1.6.0/src/mintpy/cli/save_kmz.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_kmz_timeseries.py` & `mintpy-1.6.0/src/mintpy/cli/save_kmz_timeseries.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_qgis.py` & `mintpy-1.6.0/src/mintpy/cli/save_qgis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/save_roipac.py` & `mintpy-1.6.0/src/mintpy/cli/save_roipac.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/smallbaselineApp.py` & `mintpy-1.6.0/src/mintpy/cli/smallbaselineApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 import sys
 
 import mintpy
 from mintpy.defaults.template import STEP_LIST
 from mintpy.utils.arg_utils import create_argument_parser
 
 ##########################################################################
-STEP_HELP = """Command line options for steps processing with names are chosen from the following list:
+STEP_HELP = """Command line options for steps processing with names chosen from the following list:
 
 {}
 {}
 {}
+{}
 
 In order to use either --start or --dostep, it is necessary that a
 previous run was done using one of the steps options to process at least
 through the step immediately preceding the starting step of the current run.
-""".format(STEP_LIST[0:5], STEP_LIST[5:11], STEP_LIST[11:])
+""".format(STEP_LIST[0:5], STEP_LIST[5:10], STEP_LIST[10:16], STEP_LIST[16:])
 
 REFERENCE = """reference:
-  Yunjun, Z., H. Fattahi, and F. Amelung (2019), Small baseline InSAR time series analysis:
+  Yunjun, Z., Fattahi, H., and Amelung, F. (2019), Small baseline InSAR time series analysis:
     Unwrapping error correction and noise reduction, Computers & Geosciences, 133, 104331,
     doi:10.1016/j.cageo.2019.104331.
 """
 
 EXAMPLE = """example:
   smallbaselineApp.py                         # run with default template 'smallbaselineApp.cfg'
   smallbaselineApp.py <custom_template>       # run with default and custom templates
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/solid_earth_tides.py` & `mintpy-1.6.0/src/mintpy/cli/solid_earth_tides.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/spatial_average.py` & `mintpy-1.6.0/src/mintpy/cli/spatial_average.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/spatial_filter.py` & `mintpy-1.6.0/src/mintpy/cli/spatial_filter.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/subset.py` & `mintpy-1.6.0/src/mintpy/cli/subset.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/temporal_average.py` & `mintpy-1.6.0/src/mintpy/cli/temporal_average.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/temporal_derivative.py` & `mintpy-1.6.0/src/mintpy/cli/temporal_derivative.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/temporal_filter.py` & `mintpy-1.6.0/src/mintpy/cli/temporal_filter.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/timeseries2velocity.py` & `mintpy-1.6.0/src/mintpy/cli/timeseries2velocity.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 from mintpy.defaults.template import get_template_content
 from mintpy.utils import arg_utils
 
 ############################################################################
 TEMPLATE = get_template_content('velocity')
 
 REFERENCE = """references:
-  Fattahi, H., and F. Amelung (2015), InSAR bias and uncertainty due to the systematic and stochastic
-    tropospheric delay, J. Geophy. Res. Solid Earth, 120(12), 8758-8773, doi:10.1002/2015JB012419.
   Efron, B., and R. Tibshirani (1986), Bootstrap methods for standard errors, confidence intervals,
     and other measures of statistical accuracy, Statistical Science, 54-75, doi:10.1214/ss/1177013815.
+  Fattahi, H., and F. Amelung (2015), InSAR bias and uncertainty due to the systematic and stochastic
+    tropospheric delay, J. Geophy. Res. Solid Earth, 120(12), 8758-8773, doi:10.1002/2015JB012419.
+  Hetland, E., Musé, P., Simons, M., Lin, Y., Agram, P., & DiCaprio, C. (2012). Multiscale InSAR time
+    series (MInTS) analysis of surface deformation. Journal of Geophysical Research: Solid Earth,
+    117(B2), doi:10.1029/2011JB008731
 """
 
 EXAMPLE = """example:
   timeseries2velocity.py timeseries_ERA5_demErr.h5
   timeseries2velocity.py timeseries_ERA5_demErr_ramp.h5 -t KyushuAlosDT73.txt
   timeseries2velocity.py timeseries.h5  --start-date 20080201  --end-date 20100508
   timeseries2velocity.py timeseries.h5  --ex exclude_date.txt
@@ -82,15 +85,18 @@
                            '--exclude 20040502 20060708 20090103\n' +
                            '--exclude exclude_date.txt\n'+DROP_DATE_TXT)
 
     # Uncertainty quantification
     uq = parser.add_argument_group('Uncertainty quantification (UQ)', 'Estimating the time function parameters STD')
     uq.add_argument('--uq', '--uncertainty', dest='uncertaintyQuantification', metavar='VAL',
                     default='residue', choices={'residue', 'covariance', 'bootstrap'},
-                    help='Uncertainty quantification method (default: %(default)s).')
+                    help='Uncertainty quantification method (default: %(default)s).\n'
+                         'residue    - STD from time series fitting residue (Fattahi & Amelung, 2015)\n'
+                         'covariance - STD from time series covariance\n'
+                         'bootstrap  - STD from bootstrap resampling (Efron & Tibshirani, 1986)')
     uq.add_argument('--ts-cov','--ts-cov-file', dest='timeSeriesCovFile',
                     help='4D time-series (co)variance file for time function STD calculation')
     uq.add_argument('--bc', '--bootstrap-count', dest='bootstrapCount', type=int, default=400,
                     help='number of iterations for bootstrapping (default: %(default)s).')
 
     # time functions
     parser = arg_utils.add_timefunc_argument(parser)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/timeseries_rms.py` & `mintpy-1.6.0/src/mintpy/cli/timeseries_rms.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/tropo_gacos.py` & `mintpy-1.6.0/src/mintpy/cli/tropo_gacos.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/tropo_phase_elevation.py` & `mintpy-1.6.0/src/mintpy/cli/tropo_phase_elevation.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/tropo_pyaps3.py` & `mintpy-1.6.0/src/mintpy/cli/tropo_pyaps3.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/cli/tsview.py` & `mintpy-1.6.0/src/mintpy/cli/tsview.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     pixel.add_argument('--ew', '--edgewidth', dest='edge_width', type=float, default=1.0,
                        help='Edge width for the error bar (default: %(default)s)')
 
     # other groups
     parser = arg_utils.add_data_disp_argument(parser)
     parser = arg_utils.add_dem_argument(parser)
     parser = arg_utils.add_figure_argument(parser, figsize_img=True)
-    parser = arg_utils.add_gps_argument(parser)
+    parser = arg_utils.add_gnss_argument(parser)
     parser = arg_utils.add_mask_argument(parser)
     parser = arg_utils.add_map_argument(parser)
     parser = arg_utils.add_memory_argument(parser)
     parser = arg_utils.add_reference_argument(parser)
     parser = arg_utils.add_save_argument(parser)
     parser = arg_utils.add_subset_argument(parser)
 
@@ -120,17 +120,17 @@
     inps = parser.parse_args(args=iargs)
 
     # save argv (to check the manually specified arguments)
     # use iargs        for python call
     # use sys.argv[1:] for command line call
     inps.argv = iargs if iargs else sys.argv[1:]
 
-    # check: --gps-comp option (not implemented for tsview yet)
-    if inps.gps_component:
-        msg = f'--gps-comp is not supported for {os.path.basename(__file__)}'
+    # check: --gnss-comp option (not implemented for tsview yet)
+    if inps.gnss_component:
+        msg = f'--gnss-comp is not supported for {os.path.basename(__file__)}'
         raise NotImplementedError(msg)
 
     # check: --label option (same number as input files)
     if inps.file_label:
         if len(inps.file_label) != len(inps.file):
             raise Exception('input number of labels != number of files.')
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/unwrap_error_bridging.py` & `mintpy-1.6.0/src/mintpy/cli/unwrap_error_bridging.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from mintpy.defaults.template import get_template_content
 from mintpy.utils.arg_utils import create_argument_parser
 
 ####################################################################################################
 TEMPLATE = get_template_content('correct_unwrap_error')
 
 REFERENCE = """reference:
-  Yunjun, Z., H. Fattahi, and F. Amelung (2019), Small baseline InSAR time series analysis:
+  Yunjun, Z., Fattahi, H., and Amelung, F. (2019), Small baseline InSAR time series analysis:
     Unwrapping error correction and noise reduction, Computers & Geosciences, 133, 104331,
     doi:10.1016/j.cageo.2019.104331.
 """
 
 EXAMPLE = """Example:
   unwrap_error_bridging.py  ./inputs/ifgramStack.h5  -t GalapagosSenDT128.template --update
   unwrap_error_bridging.py  ./inputs/ifgramStack.h5  --water-mask waterMask.h5
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/unwrap_error_phase_closure.py` & `mintpy-1.6.0/src/mintpy/cli/unwrap_error_phase_closure.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from mintpy.utils.arg_utils import create_argument_parser
 
 ##########################################################################################
 TEMPLATE1 = get_template_content('quick_overview')
 TEMPLATE2 = get_template_content('correct_unwrap_error')
 
 REFERENCE = """reference:
-  Yunjun, Z., H. Fattahi, and F. Amelung (2019), Small baseline InSAR time series analysis:
+  Yunjun, Z., Fattahi, H., and Amelung, F. (2019), Small baseline InSAR time series analysis:
     Unwrapping error correction and noise reduction, Computers & Geosciences, 133, 104331,
     doi:10.1016/j.cageo.2019.104331.
 """
 
 EXAMPLE = """example:
   # correct phase unwrapping error with phase closure
   unwrap_error_phase_closure.py  ./inputs/ifgramStack.h5  --cc-mask maskConnComp.h5  -t smallbaselineApp.cfg   --update
```

### Comparing `mintpy-1.5.3/src/mintpy/cli/view.py` & `mintpy-1.6.0/src/mintpy/cli/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,33 @@
 ##################################################################################################
 EXAMPLE = """example:
   view.py velocity.h5
   view.py velocity.h5 velocity --wrap --wrap-range -2 2 -c cmy --lalo-label
   view.py velocity.h5 --ref-yx  210 566                              #change reference pixel for display
   view.py velocity.h5 --sub-lat 31.05 31.10 --sub-lon 130.05 130.10  #subset in lalo / yx
   view.py velocity.h5 velocity --mask waterBody.h5 --mask-vmax 1
+  view.py velocity.h5 velocity --style scatter --scatter-size 12
 
   view.py timeseries.h5
   view.py timeseries.h5 --ref-date 20101120     #change reference date
   view.py timeseries.h5 --ex drop_date.txt      #exclude dates to plot
   view.py timeseries.h5 '*2017*' '*2018*'       #all acquisitions in 2017 and 2018
   view.py timeseries.h5 20200616_20200908       #reconstruct interferogram on the fly
 
   view.py ifgramStack.h5 coherence
   view.py ifgramStack.h5 unwrapPhase-           #unwrapPhase only in the presence of unwrapPhase_bridging
   view.py ifgramStack.h5 -n 6                   #the 6th slice
   view.py ifgramStack.h5 20171010_20171115      #all data      related with 20171010_20171115
   view.py ifgramStack.h5 'coherence*20171010*'  #all coherence related with 20171010
 
-  # GPS (for one subplot in geo-coordinates only)
-  view.py geo_velocity_msk.h5 velocity --show-gps --gps-label   #show locations of available GPS
-  view.py geo_velocity_msk.h5 velocity --show-gps --gps-comp enu2los --ref-gps GV01
-  view.py geo_timeseries_ERA5_ramp_demErr.h5 20180619 --ref-date 20141213 --show-gps --gps-comp enu2los --ref-gps GV01
+  # GNSS (for one subplot in geo-coordinates only)
+  view.py geo_velocity_msk.h5 velocity --show-gnss --gnss-label   #show locations of available GPS
+  view.py geo_velocity_msk.h5 velocity --show-gnss --gnss-comp enu2los --ref-gnss GV01
+  view.py geo_velocity_msk.h5 velocity --show-gnss --gnss-comp enu2los --ref-gnss GV01 --gnss-source ESESES
+  view.py geo_timeseries_ERA5_ramp_demErr.h5 20180619 --ref-date 20141213 --show-gnss --gnss-comp enu2los --ref-gnss GV01
 
   # Faults
   view.py filt_dense_offsets.bil range --faultline simple_fault_confident.lonlat
 
   # Save and Output
   view.py velocity.h5 --save
   view.py velocity.h5 --nodisplay
@@ -78,15 +80,15 @@
                              '  sqrt    = x^1/2\n'
                              '  reverse = x * -1\n'
                              '  inverse = 1 / x')
 
     parser = arg_utils.add_data_disp_argument(parser)
     parser = arg_utils.add_dem_argument(parser)
     parser = arg_utils.add_figure_argument(parser)
-    parser = arg_utils.add_gps_argument(parser)
+    parser = arg_utils.add_gnss_argument(parser)
     parser = arg_utils.add_mask_argument(parser)
     parser = arg_utils.add_map_argument(parser)
     parser = arg_utils.add_memory_argument(parser)
     parser = arg_utils.add_point_argument(parser)
     parser = arg_utils.add_reference_argument(parser)
     parser = arg_utils.add_save_argument(parser)
     parser = arg_utils.add_subset_argument(parser)
@@ -149,15 +151,15 @@
         if inps.dem_file is None:
             parser.error("--dem-blend requires -d/-dem.")
         # --cbar-ext option is ignored
         if '--cbar-ext' in inps.argv:
             print('WARNING: --cbar-ext is NOT compatible with --dem-blend, ignore --cbar-ext and continue.')
 
     # check: conflicted options (geo-only options if inpput file is in radar-coordinates)
-    geo_opt_names = ['--coord', '--show-gps', '--coastline', '--lalo-label', '--lalo-step', '--scalebar', '--faultline']
+    geo_opt_names = ['--coord', '--show-gnss', '--coastline', '--lalo-label', '--lalo-step', '--scalebar', '--faultline']
     geo_opt_names = list(set(geo_opt_names) & set(inps.argv))
     if geo_opt_names and 'Y_FIRST' not in readfile.read_attribute(inps.file).keys():
         for opt_name in geo_opt_names:
             print(f'WARNING: {opt_name} is NOT supported for files in radar-coordinate, ignore it and continue.')
 
     # check: --noverbose option
     # print view.py command line if --noverbose (used in smallbaselineApp.py)
```

### Comparing `mintpy-1.5.3/src/mintpy/closure_phase_bias.py` & `mintpy-1.6.0/src/mintpy/closure_phase_bias.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/constants.py` & `mintpy-1.6.0/src/mintpy/constants.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/BlueWhiteOrangeRed.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/BlueWhiteOrangeRed.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/GMT_haxby.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/GMT_haxby.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/GMT_no_green.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/GMT_no_green.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/batlow.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/batlow.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/hawaii.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/hawaii.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/oleron.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/oleron.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/roma.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/roma.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/romanian.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/romanian.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/seminf-haxby.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/seminf-haxby.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/temp-c.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/temp-c.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/temperature.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/temperature.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/vik.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/vik.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/vikO.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/vikO.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/wiki-2.0.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/wiki-2.0.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/wiki-schwarzwald-d050.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/wiki-schwarzwald-d050.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/colormaps/wiki-scotland.cpt` & `mintpy-1.6.0/src/mintpy/data/colormaps/wiki-scotland.cpt`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/dygraph-combined.js` & `mintpy-1.6.0/src/mintpy/data/dygraph-combined.js`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/shaded_dot.png` & `mintpy-1.6.0/src/mintpy/data/shaded_dot.png`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/data/star.png` & `mintpy-1.6.0/src/mintpy/data/star.png`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/defaults/auto_path.py` & `mintpy-1.6.0/src/mintpy/defaults/auto_path.py`

 * *Files 19% similar despite different names*

```diff
@@ -57,24 +57,28 @@
 mintpy.load.bperpFile       = None
 '''
 
 AUTO_PATH_ISCE_ALOS = '''##----------Default file path of ISCE/alosStack products
 mintpy.load.metaFile         = ../dates_res*/${ref_date}/${ref_date}.track.xml
 mintpy.load.baselineDir      = ../baseline
 
-mintpy.load.unwFile          = ../pairs/*-*/insar/filt_*-*_5rlks_28alks.unw
-mintpy.load.corFile          = ../pairs/*-*/insar/*-*_5rlks_28alks.cor
-mintpy.load.connCompFile     = ../pairs/*-*/insar/filt_*-*_5rlks_28alks.unw.conncomp
-
-mintpy.load.demFile          = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.hgt
-mintpy.load.lookupYFile      = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.lat
-mintpy.load.lookupXFile      = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.lon
-mintpy.load.incAngleFile     = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.los
-mintpy.load.azAngleFile      = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.los
-mintpy.load.waterMaskFile    = ../dates_res*/${ref_date}/insar/*_5rlks_28alks.wbd
+mintpy.load.unwFile          = ../pairs/*-*/insar/filt_*-*_${multilook}.unw
+mintpy.load.corFile          = ../pairs/*-*/insar/*-*_${multilook}.cor
+mintpy.load.connCompFile     = ../pairs/*-*/insar/filt_*-*_${multilook}.unw.conncomp
+
+mintpy.load.ionUnwFile       = ../pairs_ion/*-*/ion/ion_cal/filt_ion_*.ion
+mintpy.load.ionCorFile       = ../pairs_ion/*-*/ion/ion_cal/diff_*.cor
+mintpy.load.ionConnCompFile  = None
+
+mintpy.load.demFile          = ../dates_res*/${ref_date}/insar/*_${multilook}.hgt
+mintpy.load.lookupYFile      = ../dates_res*/${ref_date}/insar/*_${multilook}.lat
+mintpy.load.lookupXFile      = ../dates_res*/${ref_date}/insar/*_${multilook}.lon
+mintpy.load.incAngleFile     = ../dates_res*/${ref_date}/insar/*_${multilook}.los
+mintpy.load.azAngleFile      = ../dates_res*/${ref_date}/insar/*_${multilook}.los
+mintpy.load.waterMaskFile    = ../dates_res*/${ref_date}/insar/*_${multilook}.wbd
 '''
 
 AUTO_PATH_ROIPAC = '''##----------Default file path of ROI_PAC products
 mintpy.load.processor       = roipac
 mintpy.load.unwFile         = ../PROCESS/DONE/IFG*/filt*.unw
 mintpy.load.corFile         = ../PROCESS/DONE/IFG*/filt*.cor
 mintpy.load.connCompFile    = ../PROCESS/DONE/IFG*/filt*snap_connect.byt
@@ -200,34 +204,76 @@
 
     elif processor == 'isce_stripmap':
         date_str = os.listdir(os.path.join(proj_dir, 'merged/SLC'))[0]
         var_dict['${ref_shelve}'] = os.path.join(proj_dir, 'merged/SLC', date_str, 'referenceShelve')
 
     elif processor == 'isce_alos':
         var_dict['${ref_date}'] = get_reference_date(proj_dir)
+        var_dict['${multilook}'] = get_multilook_suffix(proj_dir)
 
     # update auto_path_dict
     for key, value in auto_path_dict.items():
         if value:
             for var1, var2 in var_dict.items():
                 value = value.replace(var1, var2)
             auto_path_dict[key] = value
 
     ## 3. update input template option with auto value
+    ## so that one could overwrite part of the auto path with custom template option inputs
     max_digit = max(len(key) for key in auto_path_dict.keys())
     for key, value in auto_path_dict.items():
         if value and template[key] == 'auto':
             template[key] = value
             print('    {k:<{d}} : auto --> {v}'.format(d=max_digit, k=key, v=value))
 
     return template
 
 
+def get_multilook_suffix(proj_dir):
+    """Get multilook suffix in the interferogram file name for isce2/alosStack from its pairs dir.
+    There could be two multilooked versions for most files, the larger one should be used.
+    """
+    insar_dir = glob.glob(os.path.join(proj_dir, 'pairs/*-*/insar'))[0]
+    int_file = sorted(glob.glob(os.path.join(insar_dir, 'filt_*-*.int')))[-1]
+    print(f'Grab multilook suffix from file: {int_file}')
+    rlks, alks = os.path.splitext(os.path.basename(int_file))[0].split('_')[-2:]
+    lks_suffix = f'{rlks}_{alks}'
+    print(f'multilook suffix of the interferogram stack: {lks_suffix}')
+    return lks_suffix
+
+
+def get_reference_date(proj_dir):
+    """Get reference date of the stack for isce2/alosStack from its XML config file."""
+    import xml.etree.ElementTree as ET
+
+    ref_date = None
+    ref_key = 'reference date of the stack'
+
+    xml_file = os.path.join(proj_dir, 'alosStack.xml')
+    print(f'Grab reference date from the config file: {xml_file}.')
+    if not os.path.exists(xml_file):
+        raise FileNotFoundError(f'Config file {xml_file} NOT found!')
+
+    # read the XML file
+    root = ET.parse(xml_file).getroot()
+    for child in root[0].findall('property'):
+        key = child.get('name').lower()
+        if key.replace(' ', '') == ref_key.replace(' ', ''):
+            ref_date = child.text
+            print('reference date of the stack:', ref_date)
+            break
+
+    if ref_date is None:
+        raise ValueError('NO element named: {ref_key} found in the config file!')
+
+    return ref_date
+
+
 def get_reference_date12(proj_dir, processor='roipac'):
-    """date12 of reference interferogram in YYMMDD-YYMMDD format"""
+    """date12 of reference interferogram in YYMMDD-YYMMDD format (for UMiami)."""
     import numpy as np
 
     ref_date12 = None
 
     # opt 1 - reference_ifgram.txt
     ref_ifg_file = os.path.join(proj_dir, 'PROCESS', 'reference_ifgram.txt')
     if os.path.isfile(ref_ifg_file):
@@ -248,43 +294,16 @@
             ref_date12 = os.walk(geom_dir).next()[1][0].split('sim_')[1]
         except:
             print("No reference interferogram found! Check the PROCESS/SIM/sim_* folder")
 
     return ref_date12
 
 
-def get_reference_date(proj_dir):
-    """Get reference date of the stack for isce2/alosStack from its XML config file."""
-    import xml.etree.ElementTree as ET
-
-    ref_date = None
-    ref_key = 'reference date of the stack'
-
-    xml_file = os.path.join(proj_dir, 'alosStack.xml')
-    print('Grab reference date from the config file: {xml_file}.')
-    if not os.path.exists(xml_file):
-        raise FileNotFoundError(f'Config file {xml_file} NOT found!')
-
-    # read the XML file
-    root = ET.parse(xml_file).getroot()
-    for child in root[0].findall('property'):
-        key = child.get('name').lower()
-        if key.replace(' ', '') == ref_key.replace(' ', ''):
-            ref_date = child.text
-            print('reference date of the stack:', ref_date)
-            break
-
-    if ref_date is None:
-        raise ValueError('NO element named: {ref_key} found in the config file!')
-
-    return ref_date
-
-
 def get_dem_file(proj_dir, ref_date12, processor):
-    """get DEM file in case both radar_2rlks.hgt and radar_8rlks.hgt exist"""
+    """get DEM file in case both radar_2rlks.hgt and radar_8rlks.hgt exist (for UMiami)"""
     dem_file = None
 
     if ref_date12 and processor == 'roipac':
         # get the number of looks used in lookup table file
         lookup_file = os.path.join(proj_dir, f'PROCESS/GEO/geo_{ref_date12}/geomap*.trans')
         lks = re.findall(r'_\d+rlks', glob.glob(lookup_file)[0])[0]
```

### Comparing `mintpy-1.5.3/src/mintpy/defaults/job4stripmapStack.cfg` & `mintpy-1.6.0/src/mintpy/defaults/job4stripmapStack.cfg`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/defaults/mintpy.yaml` & `mintpy-1.6.0/src/mintpy/defaults/mintpy.yaml`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/defaults/selectNetwork.cfg` & `mintpy-1.6.0/src/mintpy/defaults/selectNetwork.cfg`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/defaults/smallbaselineApp.cfg` & `mintpy-1.6.0/src/mintpy/defaults/smallbaselineApp.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 ## 1) Network modification based on temporal/perpendicular baselines, date, num of connections etc.
 mintpy.network.tempBaseMax     = auto  #[1-inf, no], auto for no, max temporal baseline in days
 mintpy.network.perpBaseMax     = auto  #[1-inf, no], auto for no, max perpendicular spatial baseline in meter
 mintpy.network.connNumMax      = auto  #[1-inf, no], auto for no, max number of neighbors for each acquisition
 mintpy.network.startDate       = auto  #[20090101 / no], auto for no
 mintpy.network.endDate         = auto  #[20110101 / no], auto for no
 mintpy.network.excludeDate     = auto  #[20080520,20090817 / no], auto for no
+mintpy.network.excludeDate12   = auto  #[20080520_20090817 / no], auto for no
 mintpy.network.excludeIfgIndex = auto  #[1:5,25 / no], auto for no, list of ifg index (start from 0)
 mintpy.network.referenceFile   = auto  #[date12_list.txt / ifgramStack.h5 / no], auto for no
 
 ## 2) Data-driven network modification
 ## a - Coherence-based network modification = (threshold + MST) by default
 ## reference: Yunjun et al. (2019, section 4.2 and 5.3.1); Chaussard et al. (2015, GRL)
 ## It calculates a average coherence for each interferogram using spatial coherence based on input mask (with AOI)
@@ -193,21 +194,29 @@
 ########## correct_LOD
 ## Local Oscillator Drift (LOD) correction (for Envisat only)
 ## reference: Marinkovic and Larsen (2013, Proc. LPS)
 ## automatically applied to Envisat data (identified via PLATFORM attribute)
 ## and skipped for all the other satellites.
 
 
-########## correct_SET
+########## 6. correct_SET
 ## Solid Earth tides (SET) correction [need to install insarlab/PySolid]
 ## reference: Milbert (2018); Yunjun et al. (2022, IEEE-TGRS)
 mintpy.solidEarthTides = auto #[yes / no], auto for no
 
 
-########## 6. correct_troposphere (optional but recommended)
+########## 7. correct_ionosphere (optional but recommended)
+## correct ionospheric delay [need split spectrum results from ISCE-2 stack processors]
+## reference: Fattahi et al. (2017, IEEE-TGRS); Liang et al. (2017 IEEE-TGRS; 2018 IEEE-TGRS)
+mintpy.ionosphericDelay.method        = auto  #[split_spectrum / no], auto for no
+mintpy.ionosphericDelay.excludeDate   = auto  #[20080520,20090817 / no], auto for no
+mintpy.ionosphericDelay.excludeDate12 = auto  #[20080520_20090817 / no], auto for no
+
+
+########## 8. correct_troposphere (optional but recommended)
 ## correct tropospheric delay using the following methods:
 ## a. height_correlation - correct stratified tropospheric delay (Doin et al., 2009, J Applied Geop)
 ## b. pyaps - use Global Atmospheric Models (GAMs) data (Jolivet et al., 2011; 2014)
 ##      ERA5  - ERA5    from ECMWF [need to install PyAPS from GitHub; recommended and turn ON by default]
 ##      MERRA - MERRA-2 from NASA  [need to install PyAPS from Caltech/EarthDef]
 ##      NARR  - NARR    from NOAA  [need to install PyAPS from Caltech/EarthDef; recommended for N America]
 ## c. gacos - use GACOS with the iterative tropospheric decomposition model (Yu et al., 2018, JGR)
@@ -234,57 +243,57 @@
 mintpy.troposphericDelay.minCorrelation = auto  #[0.0-1.0], auto for 0
 
 ## Notes for gacos:
 ## Set the path below to directory that contains the downloaded *.ztd* files
 mintpy.troposphericDelay.gacosDir = auto # [path2directory], auto for "./GACOS"
 
 
-########## 7. deramp (optional)
+########## 9. deramp (optional)
 ## Estimate and remove a phase ramp for each acquisition based on the reliable pixels.
 ## Recommended for localized deformation signals, i.e. volcanic deformation, landslide and land subsidence, etc.
 ## NOT recommended for long spatial wavelength deformation signals, i.e. co-, post- and inter-seimic deformation.
 mintpy.deramp          = auto  #[no / linear / quadratic], auto for no - no ramp will be removed
 mintpy.deramp.maskFile = auto  #[filename / no], auto for maskTempCoh.h5, mask file for ramp estimation
 
 
-########## 8. correct_topography (optional but recommended)
+########## 10. correct_topography (optional but recommended)
 ## Topographic residual (DEM error) correction
 ## reference: Fattahi and Amelung (2013, IEEE-TGRS)
-## stepFuncDate      - specify stepFuncDate option if you know there are sudden displacement jump in your area,
+## stepDate          - specify stepDate option if you know there are sudden displacement jump in your area,
 ##                     e.g. volcanic eruption, or earthquake
 ## excludeDate       - dates excluded for the error estimation
 ## pixelwiseGeometry - use pixel-wise geometry (incidence angle & slant range distance)
 ##                     yes - use pixel-wise geometry if they are available [slow; used by default]
 ##                     no  - use the mean   geometry [fast]
 mintpy.topographicResidual                   = auto  #[yes / no], auto for yes
 mintpy.topographicResidual.polyOrder         = auto  #[1-inf], auto for 2, poly order of temporal deformation model
 mintpy.topographicResidual.phaseVelocity     = auto  #[yes / no], auto for no - use phase velocity for minimization
-mintpy.topographicResidual.stepFuncDate      = auto  #[20080529,20190704T1733 / no], auto for no, date of step jump
+mintpy.topographicResidual.stepDate          = auto  #[20080529,20190704T1733 / no], auto for no, date of step jump
 mintpy.topographicResidual.excludeDate       = auto  #[20070321 / txtFile / no], auto for exclude_date.txt
 mintpy.topographicResidual.pixelwiseGeometry = auto  #[yes / no], auto for yes, use pixel-wise geometry info
 
 
-########## 9.1 residual_RMS (root mean squares for noise evaluation)
+########## 11.1 residual_RMS (root mean squares for noise evaluation)
 ## Calculate the Root Mean Square (RMS) of residual phase time-series for each acquisition
 ## reference: Yunjun et al. (2019, section 4.9 and 5.4)
 ## To get rid of long spatial wavelength component, a ramp is removed for each acquisition
 ## Set optimal reference date to date with min RMS
 ## Set exclude dates (outliers) to dates with RMS > cutoff * median RMS (Median Absolute Deviation)
 mintpy.residualRMS.maskFile = auto  #[file name / no], auto for maskTempCoh.h5, mask for ramp estimation
 mintpy.residualRMS.deramp   = auto  #[quadratic / linear / no], auto for quadratic
 mintpy.residualRMS.cutoff   = auto  #[0.0-inf], auto for 3
 
-########## 9.2 reference_date
+########## 11.2 reference_date
 ## Reference all time-series to one date in time
 ## reference: Yunjun et al. (2019, section 4.9)
 ## no     - do not change the default reference date (1st date)
 mintpy.reference.date = auto   #[reference_date.txt / 20090214 / no], auto for reference_date.txt
 
 
-########## 10. velocity
+########## 12. velocity
 ## Estimate a suite of time functions [linear velocity by default]
 ## from final displacement file (and from tropospheric delay file if exists)
 mintpy.timeFunc.startDate   = auto   #[20070101 / no], auto for no
 mintpy.timeFunc.endDate     = auto   #[20101230 / no], auto for no
 mintpy.timeFunc.excludeDate = auto   #[exclude_date.txt / 20080520,20090817 / no], auto for exclude_date.txt
 
 ## Fit a suite of time functions
@@ -307,32 +316,32 @@
 ## b. covariance - propagate from time series (co)variance matrix
 ## c. bootstrap  - bootstrapping (independently resampling with replacement; Efron & Tibshirani, 1986, Stat. Sci.)
 mintpy.timeFunc.uncertaintyQuantification = auto   #[residue, covariance, bootstrap], auto for residue
 mintpy.timeFunc.timeSeriesCovFile         = auto   #[filename / no], auto for no, time series covariance file
 mintpy.timeFunc.bootstrapCount            = auto   #[int>1], auto for 400, number of iterations for bootstrapping
 
 
-########## 11.1 geocode (post-processing)
+########## 13.1 geocode (post-processing)
 # for input dataset in radar coordinates only
 # commonly used resolution in meters and in degrees (on equator)
 # 100,         90,          60,          50,          40,          30,          20,          10
 # 0.000925926, 0.000833334, 0.000555556, 0.000462963, 0.000370370, 0.000277778, 0.000185185, 0.000092593
 mintpy.geocode              = auto  #[yes / no], auto for yes
 mintpy.geocode.SNWE         = auto  #[-1.2,0.5,-92,-91 / none ], auto for none, output extent in degree
 mintpy.geocode.laloStep     = auto  #[-0.000555556,0.000555556 / None], auto for None, output resolution in degree
 mintpy.geocode.interpMethod = auto  #[nearest], auto for nearest, interpolation method
 mintpy.geocode.fillValue    = auto  #[np.nan, 0, ...], auto for np.nan, fill value for outliers.
 
-########## 11.2 google_earth (post-processing)
+########## 13.2 google_earth (post-processing)
 mintpy.save.kmz             = auto   #[yes / no], auto for yes, save geocoded velocity to Google Earth KMZ file
 
-########## 11.3 hdfeos5 (post-processing)
+########## 13.3 hdfeos5 (post-processing)
 mintpy.save.hdfEos5         = auto   #[yes / no], auto for no, save time-series to HDF-EOS5 format
 mintpy.save.hdfEos5.update  = auto   #[yes / no], auto for no, put XXXXXXXX as endDate in output filename
 mintpy.save.hdfEos5.subset  = auto   #[yes / no], auto for no, put subset range info   in output filename
 
-########## 11.4 plot
+########## 13.4 plot
 # for high-resolution plotting, increase mintpy.plot.maxMemory
 # for fast plotting with more parallelization, decrease mintpy.plot.maxMemory
 mintpy.plot           = auto  #[yes / no], auto for yes, plot files generated by default processing to pic folder
 mintpy.plot.dpi       = auto  #[int], auto for 150, number of dots per inch (DPI)
 mintpy.plot.maxMemory = auto  #[float], auto for 4, max memory used by one call of view.py for plotting.
```

### Comparing `mintpy-1.5.3/src/mintpy/defaults/smallbaselineApp_auto.cfg` & `mintpy-1.6.0/src/mintpy/defaults/smallbaselineApp_auto.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ## temp/perp baseline, dates
 mintpy.network.tempBaseMax       = no
 mintpy.network.perpBaseMax       = no
 mintpy.network.connNumMax        = no
 mintpy.network.startDate         = no
 mintpy.network.endDate           = no
 mintpy.network.excludeDate       = no
+mintpy.network.excludeDate12     = no
 mintpy.network.excludeIfgIndex   = no
 mintpy.network.referenceFile     = no
 
 ## Coherence-based
 mintpy.network.coherenceBased    = no
 mintpy.network.minCoherence      = 0.7
 
@@ -81,14 +82,20 @@
 mintpy.networkInversion.shadowMask       = yes
 
 
 ########## correct_SET
 mintpy.solidEarthTides                   = no
 
 
+########## correct_ionosphere
+mintpy.ionosphericDelay.method           = no
+mintpy.ionosphericDelay.excludeDate      = no
+mintpy.ionosphericDelay.excludeDate12    = no
+
+
 ########## correct_troposphere
 mintpy.troposphericDelay.method          = pyaps
 
 ## pyaps
 mintpy.troposphericDelay.weatherModel    = ERA5
 mintpy.troposphericDelay.weatherDir      = ${WEATHER_DIR}
 
@@ -96,24 +103,25 @@
 mintpy.troposphericDelay.polyOrder       = 1
 mintpy.troposphericDelay.looks           = 8
 mintpy.troposphericDelay.minCorrelation  = 0
 
 ## gacos
 mintpy.troposphericDelay.gacosDir        = ./GACOS
 
+
 ########## deramp
 mintpy.deramp            = no
 mintpy.deramp.maskFile   = maskTempCoh.h5
 
 
 ########## correct_topography
 mintpy.topographicResidual                    = yes
 mintpy.topographicResidual.polyOrder          = 2
 mintpy.topographicResidual.phaseVelocity      = no
-mintpy.topographicResidual.stepFuncDate       = no
+mintpy.topographicResidual.stepDate           = no
 mintpy.topographicResidual.excludeDate        = exclude_date.txt
 mintpy.topographicResidual.pixelwiseGeometry  = yes
 
 
 ########## residual_RMS
 mintpy.residualRMS.maskFile  = maskTempCoh.h5
 mintpy.residualRMS.deramp    = quadratic
```

### Comparing `mintpy-1.5.3/src/mintpy/defaults/template.py` & `mintpy-1.6.0/src/mintpy/defaults/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     'modify_network',
     'reference_point',
     'quick_overview',
     'correct_unwrap_error',
     'invert_network',
     'correct_LOD',
     'correct_SET',
+    'correct_ionosphere',
     'correct_troposphere',
     'deramp',
     'correct_topography',
     'residual_RMS',
     'reference_date',
     'velocity',
     'geocode',
```

### Comparing `mintpy-1.5.3/src/mintpy/dem_error.py` & `mintpy-1.6.0/src/mintpy/dem_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mintpy.utils import ptime, readfile, time_func, utils as ut, writefile
 
 # key configuration parameter name
 key_prefix = 'mintpy.topographicResidual.'
 config_keys = [
     'polyOrder',
     'phaseVelocity',
-    'stepFuncDate',
+    'stepDate',
     'excludeDate',
 ]
 
 # debug mode
 debug_mode = False
 
 
@@ -92,15 +92,15 @@
     for key in keyList:
         value = template[key_prefix+key]
         if key in ['phaseVelocity']:
             iDict[key] = value
         elif value:
             if key in ['polyOrder']:
                 iDict[key] = int(value)
-            elif key in ['excludeDate','stepFuncDate']:
+            elif key in ['excludeDate','stepDate']:
                 iDict[key] = ptime.yyyymmdd(value.split(','))
 
     # computing configurations
     dask_key_prefix = 'mintpy.compute.'
     keyList = [i for i in list(iDict.keys()) if dask_key_prefix+i in template.keys()]
     for key in keyList:
         value = template[dask_key_prefix+key]
@@ -143,25 +143,25 @@
     # key msg
     msg = '-'*80
     msg += '\ncorrect topographic phase residual (DEM error) (Fattahi & Amelung, 2013, IEEE-TGRS)'
     msg += '\nordinal least squares (OLS) inversion with L2-norm minimization on: phase'
     if inps.phaseVelocity:
         msg += ' velocity'
     msg += f"\ntemporal deformation model: polynomial order = {inps.polyOrder}"
-    if inps.stepFuncDate:
-        msg += f"\ntemporal deformation model: step functions at {inps.stepFuncDate}"
+    if inps.stepDate:
+        msg += f"\ntemporal deformation model: step functions at {inps.stepDate}"
     if inps.periodic:
         msg += f"\ntemporal deformation model: periodic functions of {inps.periodic} yr"
     msg += '\n'+'-'*80
     print(msg)
 
     # prepare temporal deformation model
     model = dict()
     model['polynomial'] = inps.polyOrder
-    model['step'] = inps.stepFuncDate
+    model['stepDate'] = inps.stepDate
     model['periodic'] = inps.periodic
 
     # prepare SAR info
     ts_obj = timeseries(inps.ts_file)
     date_list = ts_obj.get_date_list()
     seconds = ts_obj.get_metadata().get('CENTER_LINE_UTC', 0)
 
@@ -440,15 +440,15 @@
 
     # 1.1 read date info
     ts_obj = timeseries(inps.ts_file)
     ts_obj.open()
     num_date = ts_obj.numDate
     length, width = ts_obj.length, ts_obj.width
 
-    num_step = len(inps.stepFuncDate)
+    num_step = len(inps.stepDate)
 
     # exclude dates
     date_flag = read_exclude_date(inps.excludeDate, ts_obj.dateList)[0]
     if inps.polyOrder > np.sum(date_flag):
         raise ValueError("input poly order {} > number of acquisition {}! Reduce it!".format(
             inps.polyOrder, np.sum(date_flag)))
```

### Comparing `mintpy-1.5.3/src/mintpy/dem_gsi.py` & `mintpy-1.6.0/src/mintpy/dem_gsi.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/diff.py` & `mintpy-1.6.0/src/mintpy/diff.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/generate_mask.py` & `mintpy-1.6.0/src/mintpy/generate_mask.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/geocode.py` & `mintpy-1.6.0/src/mintpy/geocode.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/ifgram_inversion.py` & `mintpy-1.6.0/src/mintpy/ifgram_inversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1056,14 +1056,19 @@
     meta.pop('REF_DATE')
     ds_name_dict = {meta['FILE_TYPE'] : [np.float32, (length, width)]}
     writefile.layout_hdf5(inps.invQualityFile, ds_name_dict, metadata=meta)
 
     # 2.4 instantiate number of inverted observations
     meta['FILE_TYPE'] = 'mask'
     meta['UNIT'] = '1'
+    # ignore NO_DATA_VALUE from ifgram stack file here as 1) it makes sense
+    # and 2) to avoid the weird error at https://github.com/insarlab/MintPy/issues/1185
+    if 'NO_DATA_VALUE' in meta.keys():
+        meta.pop('NO_DATA_VALUE')
+
     ds_name_dict = {"mask" : [np.float32, (length, width)]}
     writefile.layout_hdf5(inps.numInvFile, ds_name_dict, metadata=meta)
 
     ## 3. run the inversion / estimation and write to disk
 
     # 3.1 split ifgram_file into blocks to save memory
     box_list, num_box = stack_obj.split2boxes(max_memory=inps.maxMemory)
```

### Comparing `mintpy-1.5.3/src/mintpy/image_math.py` & `mintpy-1.6.0/src/mintpy/image_math.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/image_stitch.py` & `mintpy-1.6.0/src/mintpy/image_stitch.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 from skimage.transform import rescale
 
 from mintpy.multilook import multilook_data
-from mintpy.utils import plot as pp, readfile, writefile
+from mintpy.utils import plot as pp, readfile, utils as ut, writefile
 
 
 #############################################################################################
 def manual_offset_estimate(mat1, mat2):
     """Manually estimate offset between two data matrix.
     By manually selecting a line from each of them, and estimate the difference.
     It usually used when 2 input data matrix have no area in common.
@@ -174,14 +174,28 @@
     atr = dict()
     for key, value in atr1.items():
         atr[key] = value
     atr['WIDTH'] = width
     atr['LENGTH'] = length
     atr['X_FIRST'] = W
     atr['Y_FIRST'] = N
+    print(f'update LENGTH/WIDTH: {length}/{width}')
+    print(f'update Y/X_FIRST: {N}/{W}')
+
+    # update REF_Y/X
+    coord = ut.coordinate(atr)
+    ref_y, ref_x = coord.geo2radar(float(atr['REF_LAT']), float(atr['REF_LON']))[:2]
+    atr['REF_Y'], atr['REF_X'] = ref_y, ref_x
+    print(f'update REF_Y/X: {ref_y}/{ref_x}')
+
+    # delete SUBSET_Y/XMIN/MAX
+    for key in ['SUBSET_XMIN', 'SUBSET_XMAX', 'SUBSET_YMIN', 'SUBSET_YMAX']:
+        if key in atr.keys():
+            atr.pop(key)
+            print(f'remove {key}')
 
     return mat, atr, mat11, mat22, mat_diff
 
 
 def plot_stitch(mat11, mat22, mat, mat_diff, out_fig=None, disp_scale=1, disp_vlim=None, disp_cmap=None):
     """plot stitching result"""
```

### Comparing `mintpy-1.5.3/src/mintpy/info.py` & `mintpy-1.6.0/src/mintpy/info.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/iono_tec.py` & `mintpy-1.6.0/src/mintpy/iono_tec.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/load_data.py` & `mintpy-1.6.0/src/mintpy/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,17 +630,21 @@
                 ut.print_command_line(script_name, iargs)
                 # run
                 prep_module.main(iargs)
 
     elif processor == 'nisar':
         dem_file = iDict['mintpy.load.demFile']
         gunw_files = iDict['mintpy.load.unwFile']
+        water_mask = iDict['mintpy.load.waterMaskFile']
 
         # run prep_*.py
-        iargs = ['-i', gunw_files, '-d', dem_file, '-o', '../mintpy']
+        iargs = ['-i', gunw_files, '-d', dem_file]
+
+        if os.path.exists(water_mask):
+            iargs = iargs + ['--mask', water_mask]
 
         if iDict['mintpy.subset.yx']:
             warnings.warn('Subset in Y/X is not implemented for NISAR. \n'
                           'There might be shift in the coordinates of different products. \n'
                           'Use lat/lon instead.')
         if iDict['mintpy.subset.lalo']:
             lalo = iDict['mintpy.subset.lalo'].split(',')
@@ -664,14 +668,15 @@
         else:
             warnings.warn('No input metadata file found: {}'.format(iDict['mintpy.load.metaFile']))
             meta_file = 'auto'
 
         # --baseline-dir / --geometry-dir
         baseline_dir = iDict['mintpy.load.baselineDir']
         geom_dir = os.path.dirname(iDict['mintpy.load.demFile'])
+        geom_dir = os.path.abspath(geom_dir)
 
         # --dset-dir / --file-pattern
         obs_keys = [
             'mintpy.load.unwFile',
             'mintpy.load.ionUnwFile',
             'mintpy.load.rgOffFile',
             'mintpy.load.azOffFile',
```

### Comparing `mintpy-1.5.3/src/mintpy/load_gbis.py` & `mintpy-1.6.0/src/mintpy/load_gbis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/local_oscilator_drift.py` & `mintpy-1.6.0/src/mintpy/local_oscilator_drift.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/lookup_geo2radar.py` & `mintpy-1.6.0/src/mintpy/lookup_geo2radar.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/mask.py` & `mintpy-1.6.0/src/mintpy/mask.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/modify_network.py` & `mintpy-1.6.0/src/mintpy/modify_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,23 @@
         tempList = [date12ListAll[i] for i in inps.excludeIfgIndex]
         date12_to_drop += tempList
         print('--------------------------------------------------')
         print(f'Drop ifgrams with the following index number: {len(tempList)}')
         for ifg_idx, date12 in zip(inps.excludeIfgIndex, tempList):
             print(f'{ifg_idx} : {date12}')
 
+    # excludeDate12
+    if inps.excludeDate12:
+        tempList = [i for i in inps.excludeDate12 if i in date12ListAll]
+        date12_to_drop += tempList
+        print('--------------------------------------------------')
+        print(f'Drop ifgrams with the following date12: {len(tempList)}')
+        for date12 in tempList:
+            print(date12)
+
     # excludeDate
     if inps.excludeDate:
         tempList = [i for i in date12ListAll if any(j in inps.excludeDate for j in i.split('_'))]
         date12_to_drop += tempList
         print('-'*50+'\nDrop ifgrams including the following dates: ({})\n{}'.format(
             len(tempList), inps.excludeDate))
         print('-'*30+f'\n{tempList}')
```

### Comparing `mintpy-1.5.3/src/mintpy/multi_transect.py` & `mintpy-1.6.0/src/mintpy/multi_transect.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/multilook.py` & `mintpy-1.6.0/src/mintpy/multilook.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/cluster.py` & `mintpy-1.6.0/src/mintpy/objects/cluster.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/colors.py` & `mintpy-1.6.0/src/mintpy/objects/colors.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/conncomp.py` & `mintpy-1.6.0/src/mintpy/objects/conncomp.py`

 * *Files 4% similar despite different names*

```diff
@@ -351,27 +351,31 @@
             unw += ramp
         if print_msg:
             print(f'time used: {time.time()-start_time:.2f} secs.')
         return unw
 
 
     def plot_bridge(self, ax, cmap='jet', radius=50):
-        # label background
+        # background label
         ax.imshow(self.labelImg, cmap=cmap, interpolation='nearest')
-        # bridges
+
         for bridge in self.bridges:
+            # bridges
             ax.plot([bridge['x0'], bridge['x1']],
                     [bridge['y0'], bridge['y1']], 'w-', lw=1)
+
             # endpoint window
             if radius > 0:
                 aoi_mask0, aoi_mask1 = self.get_bridge_endpoint_aoi_mask(bridge, radius=radius)
                 label_mask0 = self.labelImg == bridge['label0']
                 label_mask1 = self.labelImg == bridge['label1']
-                mask0 = np.ma.masked_where(~(aoi_mask0*label_mask0), np.zeros(self.labelImg.shape))
-                mask1 = np.ma.masked_where(~(aoi_mask1*label_mask1), np.zeros(self.labelImg.shape))
-                ax.imshow(mask0, cmap='gray', alpha=0.3, vmin=0, vmax=1)
-                ax.imshow(mask1, cmap='gray', alpha=0.3, vmin=0, vmax=1)
+                # Note by Emre, Mar 2024: overlay bridge regions directly using plot() function,
+                # to save memory while calling this func in a loop by avoiding creating separate
+                # mask arrays (https://github.com/insarlab/MintPy/pull/1155)
+                ax.plot(np.nonzero(aoi_mask0*label_mask0)[1], np.nonzero(aoi_mask0*label_mask0)[0], 'gray', alpha=0.3)
+                ax.plot(np.nonzero(aoi_mask1*label_mask1)[1], np.nonzero(aoi_mask1*label_mask1)[0], 'gray', alpha=0.3)
+
         # reference pixel
         ax.plot(self.refX, self.refY, 'ks', ms=2)
         return ax
 
 ######################################## end of connectComponent class ####################################
```

### Comparing `mintpy-1.5.3/src/mintpy/objects/coord.py` & `mintpy-1.6.0/src/mintpy/objects/coord.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,104 +50,145 @@
             lookup_file = ut1.get_lookup_file(lookup_file, abspath=True, print_msg=False)
         if isinstance(lookup_file, str):
             lookup_file = [lookup_file, lookup_file]
         self.lookup_file = lookup_file
         self.lut_y = None
         self.lut_x = None
 
+
     def open(self):
         self.earth_radius = float(self.src_metadata.get('EARTH_RADIUS', EARTH_RADIUS))
 
         if 'Y_FIRST' in self.src_metadata.keys():
             self.geocoded = True
             self.lat0 = float(self.src_metadata['Y_FIRST'])
             self.lon0 = float(self.src_metadata['X_FIRST'])
             self.lat_step = float(self.src_metadata['Y_STEP'])
             self.lon_step = float(self.src_metadata['X_STEP'])
         else:
             self.geocoded = False
             if self.lookup_file:
                 self.lut_metadata = readfile.read_attribute(self.lookup_file[0])
 
-    def lalo2yx(self, coord_in, coord_type):
-        """convert geo coordinates into radar coordinates for Geocoded file only
-        Parameters: geoCoord   - list / tuple / 1D np.ndarray / float, coordinate(s) in latitude or longitude
-                    metadata   - dict, dictionary of file attributes
-                    coord_type - str, coordinate type: latitude or longitude
-        Example:    300 = coordinate.lalo2yx(32.104990,    metadata,'lat')
-                    [1000,1500] = coordinate.lalo2yx([130.5,131.4],metadata,'lon')
+        # remove empty attributes [to facilitate checking laterward]
+        key_list = ['UTM_ZONE']
+        for key in key_list:
+            if key in self.src_metadata and not self.src_metadata[key]:
+                self.src_metadata.pop(key)
+
+
+    def _clean_coord(self, coord1, coord2):
+        """Ensure input coordinate as list type and same size."""
+
+        def _to_list(x):
+            # convert numpy array to list or scalar
+            if isinstance(x, np.ndarray):
+                x = x.tolist()
+            # convert scalar / None to list
+            # Note: np.float128 is not supported on Windows OS,
+            #   use np.longdouble as a platform neutral syntax
+            float_types = (float, np.float16, np.float32, np.float64, np.longdouble)
+            int_types = (int, np.int16, np.int32, np.int64)
+            if isinstance(x, int_types + float_types):
+                x = [x]
+            elif x is None:
+                x = [None]
+            x = list(x)
+            return x
+
+        # convert to list type
+        coord1 = _to_list(coord1)
+        coord2 = _to_list(coord2)
+
+        # ensure the same size
+        if len(coord1) != len(coord2):
+            if len(coord1) == 1 and len(coord2) > 1:
+                coord1 *= len(coord2)
+            elif len(coord1) > 1 and len(coord2) == 1:
+                coord2 *= len(coord1)
+            else:
+                raise ValueError('Input two coordinates do NOT have the same size!')
+
+        return coord1, coord2
+
+
+    def lalo2yx(self, lat_in, lon_in):
+        """convert geo coordinates into radar coordinates for Geocoded file only.
+
+        Parameters: lat_in    - list / tuple / 1D np.ndarray / float, coordinate(s) in latitude / northing
+                    lon_in    - list / tuple / 1D np.ndarray / float, coordinate(s) in longitude / easting
+        Returns:    coord_out - tuple(list / float / 1D np.ndarray), coordinates(s) in (row, col) numbers
+        Example:    300, 1000 = coordinate.lalo2yx(32.1, 130.5)
+                    300 = coordinate.lalo2yx(32.1, None)[0]
+                    ([300, 301], [1000, 1001]) = coordinate.lalo2yx((32.1, 32.101), (130.5, 130.501))
         """
         self.open()
         if not self.geocoded:
-            raise ValueError('Input file is not geocoded.')
+            raise ValueError('Input file is NOT geocoded.')
+
+        lat_in, lon_in = self._clean_coord(lat_in, lon_in)
 
-        # input format
-        if isinstance(coord_in, np.ndarray):
-            coord_in = coord_in.tolist()
-        # note: np.float128 is not supported on Windows OS, use np.longdouble as a platform neutral syntax
-        if isinstance(coord_in, (float, np.float16, np.float32, np.float64, np.longdouble)):
-            coord_in = [coord_in]
-        coord_in = list(coord_in)
+        # attempts to convert lat/lon to utm coordinates if needed.
+        if (lat_in is not None and lon_in is not None
+                and 'UTM_ZONE' in self.src_metadata
+                and np.max(np.abs(lat_in)) <= 90
+                and np.max(np.abs(lon_in)) <= 360):
+            lat_in, lon_in = ut0.latlon2utm(self.src_metadata, np.array(lat_in), np.array(lon_in))
 
         # convert coordinates
-        coord_type = coord_type.lower()
-        coord_out = []
-        for coord_i in coord_in:
+        y_out = []
+        x_out = []
+        for lat_i, lon_i in zip(lat_in, lon_in):
             # plus 0.01 to be more robust in practice
-            if coord_type.startswith('lat'):
-                coord_o = int(np.floor((coord_i - self.lat0) / self.lat_step + 0.01))
-            elif coord_type.startswith('lon'):
-                coord_o = int(np.floor((coord_i - self.lon0) / self.lon_step + 0.01))
-            else:
-                raise ValueError('Unrecognized coordinate type: '+coord_type)
-            coord_out.append(coord_o)
+            y_i = None if lat_i is None else int(np.floor((lat_i - self.lat0) / self.lat_step + 0.01))
+            x_i = None if lon_i is None else int(np.floor((lon_i - self.lon0) / self.lon_step + 0.01))
+            y_out.append(y_i)
+            x_out.append(x_i)
 
         # output format
-        if len(coord_out) == 1:
-            coord_out = coord_out[0]
-        elif isinstance(coord_in, tuple):
-            coord_out = tuple(coord_out)
+        if len(y_out) == 1 and len(x_out) == 1:
+            coord_out = tuple([y_out[0], x_out[0]])
+        else:
+            coord_out = tuple([y_out, x_out])
+
         return coord_out
 
 
-    def yx2lalo(self, coord_in, coord_type):
+    def yx2lalo(self, y_in, x_in):
         """convert radar coordinates into geo coordinates (pixel center)
-            for Geocoded file only
-        Parameters: coord_in   _ list / tuple / 1D np.ndarray / int, coordinate(s) in row or col in int
-                    metadata   _ dict, dictionary of file attributes
-                    coord_type _ str, coordinate type: row / col / y / x
-        Example:    32.104990 = coord_yx2lalo(300, metadata, 'y')
-                    [130.5,131.4] = coord_yx2lalo([1000,1500], metadata, 'x')
+            for Geocoded file only.
+
+        Parameters: y_in      - list / tuple / 1D np.ndarray / int, coordinate(s) in row number
+                    x_in      - list / tuple / 1D np.ndarray / int, coordinate(s) in col number
+        Returns:    coord_out - tuple(list / 1D np.ndarray / int), coordinate(s) in (lat/northing, lon/easting)
+        Example:    32.1, 130.5 = coordinate.yx2lalo(300, 1000)
+                    32.1 = coordinate.yx2lalo(300, None)[0]
+                    ([32.1, 32.101], [130.5, 130.501]) = coordinate.lalo2yx([(300, 301), (1000, 1001)])
         """
         self.open()
         if not self.geocoded:
-            raise ValueError('Input file is not geocoded.')
+            raise ValueError('Input file is NOT geocoded.')
 
-        # Convert to List if input is String
-        if isinstance(coord_in, np.ndarray):
-            coord_in = coord_in.tolist()
-        if isinstance(coord_in, (int, np.int16, np.int32, np.int64)):
-            coord_in = [coord_in]
-        coord_in = list(coord_in)
-
-        coord_type = coord_type.lower()
-        coord_out = []
-        for i in range(len(coord_in)):
-            if coord_type.startswith(('row', 'y', 'az', 'azimuth')):
-                coord = (coord_in[i] + 0.5) * self.lat_step + self.lat0
-            elif coord_type.startswith(('col', 'x', 'rg', 'range')):
-                coord = (coord_in[i] + 0.5) * self.lon_step + self.lon0
-            else:
-                raise ValueError('Unrecognized coordinate type: '+coord_type)
-            coord_out.append(coord)
+        y_in, x_in = self._clean_coord(y_in, x_in)
+
+        # convert coordinates
+        lat_out = []
+        lon_out = []
+        for y_i, x_i in zip(y_in, x_in):
+            lat_i = None if y_i is None else (y_i + 0.5) * self.lat_step + self.lat0
+            lon_i = None if x_i is None else (x_i + 0.5) * self.lon_step + self.lon0
+            lat_out.append(lat_i)
+            lon_out.append(lon_i)
+
+        # output format
+        if len(lat_out) == 1 and len(lon_out) == 1:
+            coord_out = tuple([lat_out[0], lon_out[0]])
+        else:
+            coord_out = tuple([lat_out, lon_out])
 
-        if len(coord_out) == 1:
-            coord_out = coord_out[0]
-        elif isinstance(coord_in, tuple):
-            coord_out = tuple(coord_out)
         return coord_out
 
 
     def _get_lookup_row_col(self, y, x, y_factor=10, x_factor=10, geo_coord=False, debug_mode=False):
         """Get row/col number in y/x value matrix from input y/x
         Use overlap mean value between y and x buffer;
         To support point outside of value pool/matrix, could use np.polyfit to fit a line
@@ -193,14 +234,15 @@
     def read_lookup_table(self, print_msg=True):
         ds_name_x = 'rangeCoord' if 'Y_FIRST' in self.lut_metadata.keys() else 'longitude'
         ds_name_y = 'azimuthCoord' if 'Y_FIRST' in self.lut_metadata.keys() else 'latitude'
         self.lut_y = readfile.read(self.lookup_file[0], datasetName=ds_name_y, print_msg=print_msg)[0]
         self.lut_x = readfile.read(self.lookup_file[1], datasetName=ds_name_x, print_msg=print_msg)[0]
         return self.lut_y, self.lut_x
 
+
     def _read_geo_lut_metadata(self):
         """Read lat/lon0, lat/lon_step_deg, lat/lon_step into a Namespace - lut"""
         lut = Namespace()
         lut.lat0 = float(self.lut_metadata['Y_FIRST'])
         lut.lon0 = float(self.lut_metadata['X_FIRST'])
         lut.lat_step_deg = float(self.lut_metadata['Y_STEP'])
         lut.lon_step_deg = float(self.lut_metadata['X_STEP'])
@@ -208,22 +250,24 @@
         # Get lat/lon resolution/step in meter
         length = int(self.lut_metadata['LENGTH'])
         lat_c = lut.lat0 + lut.lat_step_deg * length / 2.
         lut.lat_step = lut.lat_step_deg * np.pi/180.0 * self.earth_radius
         lut.lon_step = lut.lon_step_deg * np.pi/180.0 * self.earth_radius * np.cos(lat_c * np.pi/180)
         return lut
 
+
     def geo2radar(self, lat, lon, print_msg=True, debug_mode=False):
         """Convert geo coordinates into radar coordinates.
+
         Parameters: lat/lon   - np.array / float, latitude/longitude
         Returns:    az/rg     - np.array / int, range/azimuth pixel number
                     az/rg_res - float, residul/uncertainty of coordinate conversion
         """
-        # ensure longitude convention to be consistent with src_metadata
-        if 'X_FIRST' in self.src_metadata.keys():
+        # check 1: ensure longitude convention to be consistent with src_metadata [for WGS84 coordinates]
+        if 'X_FIRST' in self.src_metadata.keys() and 'UTM_ZONE' not in self.src_metadata.keys():
             width = int(self.src_metadata['WIDTH'])
             lon_step = float(self.src_metadata['X_STEP'])
             min_lon = float(self.src_metadata['X_FIRST'])
             max_lon = min_lon + lon_step * width
 
             # skip if larger than (-180, 180)
             # e.g. IONEX file in (-182.25, 182.25)
@@ -240,18 +284,23 @@
             # ensure longitude within (-180, 180]
             else:
                 if np.isscalar(lon):
                     lon = lon - 360. if lon > 180. else lon
                 else:
                     lon[lon > 180.] -= 360
 
+        # check 2: attempts to convert lat/lon to utm coordinates if needed
+        if ('UTM_ZONE' in self.src_metadata
+                and np.max(np.abs(lat)) <= 90
+                and np.max(np.abs(lon)) <= 360):
+            lat, lon = ut0.latlon2utm(self.src_metadata, np.array(lat), np.array(lon))
+
         self.open()
         if self.geocoded:
-            az = self.lalo2yx(lat, coord_type='lat')
-            rg = self.lalo2yx(lon, coord_type='lon')
+            az, rg = self.lalo2yx(lat, lon)
             return az, rg, 0, 0
 
         if not isinstance(lat, np.ndarray):
             lat = np.array(lat)
             lon = np.array(lon)
 
         # read lookup table
@@ -332,16 +381,15 @@
         Parameters: rg/az      - np.array / int, range/azimuth pixel number
         Returns:    lon/lat    - np.array / float, longitude/latitude of input point (rg,az);
                                  nan if not found.
                     latlon_res - float, residul/uncertainty of coordinate conversion
         """
         self.open()
         if self.geocoded:
-            lat = self.yx2lalo(az, coord_type='az')
-            lon = self.yx2lalo(rg, coord_type='rg')
+            lat, lon = self.yx2lalo(az, rg)
             return lat, lon, 0, 0
 
         if not isinstance(az, np.ndarray):
             az = np.array(az)
             rg = np.array(rg)
 
         # read lookup table file
@@ -394,70 +442,73 @@
         else:
             lat = self.lut_y[az, rg]
             lon = self.lut_x[az, rg]
             lat_resid = 0.
             lon_resid = 0.
         return lat, lon, lat_resid, lon_resid
 
+
     def box_pixel2geo(self, pixel_box):
         """Convert pixel_box to geo_box in UL corner
         Parameters: pixel_box - list/tuple of 4 int   in (x0, y0, x1, y1)
         Returns:    geo_box   - tuple      of 4 float in (W, N, E, S)
         """
         try:
-            lat = self.yx2lalo([pixel_box[1], pixel_box[3]], coord_type='y')
-            lon = self.yx2lalo([pixel_box[0], pixel_box[2]], coord_type='x')
+            lat, lon = self.yx2lalo([pixel_box[1], pixel_box[3]], [pixel_box[0], pixel_box[2]])
             # shift lat from pixel center to the UL corner
             lat = [i - self.lat_step / 2.0 for i in lat]
             lon = [i - self.lon_step / 2.0 for i in lon]
             geo_box = (lon[0], lat[0], lon[1], lat[1])
         except:
             geo_box = None
         return geo_box
 
+
     def box_geo2pixel(self, geo_box):
         """Convert geo_box to pixel_box
         Parameters: geo_box   - tuple      of 4 float in (W, N, E, S)
         Returns:    pixel_box - list/tuple of 4 int   in (x0, y0, x1, y1)
         """
         try:
-            y = self.lalo2yx([geo_box[1], geo_box[3]], coord_type='latitude')
-            x = self.lalo2yx([geo_box[0], geo_box[2]], coord_type='longitude')
+            y, x = self.lalo2yx([geo_box[1], geo_box[3]], [geo_box[0], geo_box[2]])
             pixel_box = (x[0], y[0], x[1], y[1])
         except:
             pixel_box = None
         return pixel_box
 
+
     def bbox_radar2geo(self, pix_box, print_msg=False):
         """Calculate bounding box in lat/lon for file in geo coord, based on input radar/pixel box
         Parameters: pix_box - tuple of 4 int, in (x0, y0, x1, y1)
         Returns:    geo_box - tuple of 4 float, in (W, N, E, S)
         """
         x = np.array([pix_box[0], pix_box[2], pix_box[0], pix_box[2]])
         y = np.array([pix_box[1], pix_box[1], pix_box[3], pix_box[3]])
         lat, lon, lat_res, lon_res = self.radar2geo(y, x, print_msg=print_msg)
         buf = 2 * np.max(np.abs([lat_res, lon_res]))
         geo_box = (np.min(lon) - buf, np.max(lat) + buf,
                    np.max(lon) + buf, np.min(lat) - buf)
         return geo_box
 
+
     def bbox_geo2radar(self, geo_box, print_msg=False):
         """Calculate bounding box in x/y for file in radar coord, based on input geo box.
         Parameters: geo_box - tuple of 4 float, indicating the UL/LR lon/lat
         Returns:    pix_box - tuple of 4 int, indicating the UL/LR x/y of the bounding box in radar coord
                               for the corresponding lat/lon coverage.
         """
         lat = np.array([geo_box[3], geo_box[3], geo_box[1], geo_box[1]])
         lon = np.array([geo_box[0], geo_box[2], geo_box[0], geo_box[2]])
         y, x, y_res, x_res = self.geo2radar(lat, lon, print_msg=print_msg)
         buf = 2 * np.max(np.abs([x_res, y_res]))
         pix_box = (np.min(x) - buf, np.min(y) - buf,
                    np.max(x) + buf, np.max(y) + buf)
         return pix_box
 
+
     def check_box_within_data_coverage(self, pixel_box, print_msg=True):
         """Check the subset box's conflict with data coverage
         Parameters:  pixel_box - 4-tuple of int, indicating y/x coordinates of subset
         Returns:     out_box   - 4-tuple of int
         """
         self.open()
         length, width = int(self.src_metadata['LENGTH']), int(self.src_metadata['WIDTH'])
```

### Comparing `mintpy-1.5.3/src/mintpy/objects/euler_pole.py` & `mintpy-1.6.0/src/mintpy/objects/euler_pole.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/giant.py` & `mintpy-1.6.0/src/mintpy/objects/giant.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/gps.py` & `mintpy-1.6.0/src/mintpy/utils/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,594 +1,515 @@
-"""Class / utilities for GPS download / operations."""
+"""Miscellaneous utilities - dependent on utils0/1."""
 ############################################################
 # Program is part of MintPy                                #
 # Copyright (c) 2013, Zhang Yunjun, Heresh Fattahi         #
-# Author: Zhang Yunjun, Jul 2018                           #
+# Author: Zhang Yunjun, Heresh Fattahi, 2013               #
 ############################################################
 # Recommend import:
-#     from mintpy.objects.gps import GPS
+#   from mintpy.utils import utils as ut
 
 
-import csv
-import datetime as dt
-import glob
+import errno
 import os
-from urllib.request import urlretrieve
 
 import numpy as np
-from pyproj import Geod
+from scipy.ndimage import map_coordinates
 
+from mintpy.objects import (
+    GEOMETRY_DSET_NAMES,
+    geometry,
+    ifgramStack,
+    timeseries,
+)
 from mintpy.objects.coord import coordinate
-from mintpy.utils import ptime, readfile, time_func, utils1 as ut
+from mintpy.objects.resample import resample
+from mintpy.utils import attribute as attr, ptime, readfile
+from mintpy.utils.utils0 import *
+from mintpy.utils.utils1 import *
+
+
+#################################################################################
+def check_loaded_dataset(work_dir='./', print_msg=True, relpath=False):
+    """Check the loaded input files, following two rules:
+        1. file existence
+        2. file attribute readability
+
+    Parameters: work_dir    - str, MintPy working directory
+                print_msg   - bool, print out message
+    Returns:    stack_file  - str, path to the interferogram stack file
+                geom_file   - str, path to the geometry file
+                lookup_file - str, path to the look up table file, for radar-coord dataset only.
+                ion_file    - str, path to the ionosphere stack file
+    Example:    work_dir = os.path.expandvars('./FernandinaSenDT128/mintpy')
+                stack_file, geom_file, lookup_file = ut.check_loaded_dataset(work_dir)[:3]
+    """
+    if not work_dir:
+        work_dir = os.getcwd()
+    work_dir = os.path.abspath(work_dir)
+
+    # tips for prep_aria
+    template_file = os.path.join(work_dir, 'smallbaselineApp.cfg')
+    proc = readfile.read_template(template_file)['mintpy.load.processor']
+    if proc == 'aria':
+        msg_aria = '. Re-run "prep_aria.py" as printed out in "load_data" step for more information!'
+    else:
+        msg_aria = ''
 
-UNR_SITE_LIST_FILE = 'http://geodesy.unr.edu/NGLStationPages/DataHoldings.txt'
+    # 1. [required] interferograms stack file: unwrapPhase, coherence
+    stack_file = os.path.join(work_dir, 'inputs/ifgramStack.h5')
+    dnames = ['unwrapPhase', 'rangeOffset', 'azimuthOffset']
+
+    if is_file_exist(stack_file, abspath=True):
+        obj = ifgramStack(stack_file)
+        obj.open(print_msg=False)
+
+        if all(x not in obj.datasetNames for x in dnames):
+            msg = f'required dataset is missing in file {stack_file}:\n'
+            msg += ' OR '.join(dnames)
+            raise ValueError(msg)
+
+        # check coherence for phase stack
+        if 'unwrapPhase' in obj.datasetNames and 'coherence' not in obj.datasetNames:
+            print(f'WARNING: "coherence" is missing in file {stack_file}')
+    else:
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), stack_file + msg_aria)
 
+    # get coordinate type of the loaded dataset
+    atr = readfile.read_attribute(stack_file)
+    coord_type = 'GEO' if 'Y_FIRST' in atr.keys() else 'RADAR'
+    processor = atr['PROCESSOR']
+
+    # 2. [required] geom_file: height
+    geom_file = os.path.join(work_dir, 'inputs', f'geometry{coord_type.capitalize()}.h5')
+    dname = GEOMETRY_DSET_NAMES[0]
+
+    if is_file_exist(geom_file, abspath=True):
+        obj = geometry(geom_file)
+        obj.open(print_msg=False)
+        if dname not in obj.datasetNames:
+            raise ValueError(f'required dataset "{dname}" is missing in file {geom_file}')
+    else:
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), geom_file + msg_aria)
 
-def dload_site_list(out_file=None, url=UNR_SITE_LIST_FILE, print_msg=True):
-    """download DataHoldings.txt.
+    # 3. [required for radar-coord] lookup_file: latitude,longitude or rangeCoord,azimuthCoord
+    # could be different than geometry file in case of roipac and gamma
+    lookup_file = os.path.join(work_dir, 'inputs/geometry*.h5')
+    lookup_file = get_lookup_file(lookup_file, abspath=True, print_msg=print_msg)
+    if coord_type == 'RADAR':
+        if lookup_file is not None:
+            obj = geometry(lookup_file)
+            obj.open(print_msg=False)
+
+            # get the proper lookup table dataset names
+            if processor in ['isce', 'doris']:
+                dnames = GEOMETRY_DSET_NAMES[1:3]
+            elif processor in ['gamma', 'roipac']:
+                dnames = GEOMETRY_DSET_NAMES[3:5]
+            else:
+                msg = f'Unknown InSAR processor: {processor} to locate look up table!'
+                raise AttributeError(msg)
+
+            for dname in dnames:
+                if dname not in obj.datasetNames:
+                    raise Exception(f'required dataset "{dname}" is missing in file {lookup_file}')
+        else:
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), lookup_file)
+    else:
+        print("Input data seems to be geocoded. Lookup file not needed.")
 
-    Parameters: out_file - str, path to the local file.
-    Returns:    out_file - str, path to the local file.
-                           default: './GPS/DataHoldings.txt'
-    """
-    # output file path
-    if not out_file:
-        out_dir = os.path.abspath('./GPS')
-        out_file = os.path.join(out_dir, os.path.basename(url))
+    # 4. [optional] ionosphere stack file: unwrapPhase, coherence
+    ion_file = os.path.join(work_dir, 'inputs/ionStack.h5')
+    dname = 'unwrapPhase'
+
+    if is_file_exist(ion_file, abspath=True):
+        obj = ifgramStack(ion_file)
+        obj.open(print_msg=False)
+        if dname not in obj.datasetNames:
+            raise ValueError(f'required dataset "{dname}" is missing in file {ion_file}')
+
+        # check coherence for phase stack
+        if 'unwrapPhase' in obj.datasetNames and 'coherence' not in obj.datasetNames:
+            print(f'WARNING: "coherence" is missing in file {ion_file}')
     else:
-        out_dir = os.path.abspath(os.path.dirname(out_file))
+        ion_file = None
 
-    # output file directory
-    if not os.path.isdir(out_dir):
-        if print_msg:
-            print('create directory:', out_dir)
-        os.makedirs(out_dir)
+    if relpath:
+        stack_file  = os.path.relpath(stack_file)  if stack_file  else stack_file
+        geom_file   = os.path.relpath(geom_file)   if geom_file   else geom_file
+        lookup_file = os.path.relpath(lookup_file) if lookup_file else lookup_file
+        ion_file    = os.path.relpath(ion_file)    if ion_file    else ion_file
 
+    # print message
     if print_msg:
-        print(f'downloading site list from UNR Geod Lab: {url} to {out_file}')
-    urlretrieve(url, out_file)
-    return out_file
-
-
-def search_gps(SNWE, start_date=None, end_date=None, site_list_file=None, min_num_solution=50, print_msg=True):
-    """Search available GPS sites within the geo bounding box from UNR website.
-    Parameters: SNWE             - tuple of 4 float, indicating (South, North, West, East) in degrees
-                start_date       - str in YYYYMMDD format
-                end_date         - str in YYYYMMDD format
-                site_list_file   - str.
-                min_num_solution - int, minimum number of solutions available
-    Returns:    site_names       - 1D np.array of string for GPS station names
-                site_lats        - 1D np.array for lat
-                site_lons        - 1D np.array for lon
-    """
-    # download site list file if it's not found in current directory
-    if site_list_file is None:
-        site_list_file = os.path.basename(UNR_SITE_LIST_FILE)
-
-    if not os.path.isfile(site_list_file):
-        dload_site_list(site_list_file, print_msg=print_msg)
-
-    txt_data = np.loadtxt(site_list_file,
-                          dtype=bytes,
-                          skiprows=1,
-                          usecols=(0,1,2,3,4,5,6,7,8,9,10)).astype(str)
-    site_names = txt_data[:, 0]
-    site_lats, site_lons = txt_data[:, 1:3].astype(np.float32).T
-    site_lons -= np.round(site_lons / (360.)) * 360.
-    t0s = np.array([dt.datetime.strptime(i, "%Y-%m-%d") for i in txt_data[:, 7].astype(str)])
-    t1s = np.array([dt.datetime.strptime(i, "%Y-%m-%d") for i in txt_data[:, 8].astype(str)])
-    num_solution = txt_data[:, 10].astype(np.int16)
-
-    # limit in space
-    idx = ((site_lats >= SNWE[0]) * (site_lats <= SNWE[1]) *
-           (site_lons >= SNWE[2]) * (site_lons <= SNWE[3]))
-
-    # limit in time
-    t0 = ptime.date_list2vector([start_date])[0][0] if start_date else None
-    t1 = ptime.date_list2vector([end_date])[0][0] if end_date else None
-    if start_date:
-        idx *= t1s >= t0
-    if end_date:
-        idx *= t0s <= t1
-
-    # limit on number of solutions
-    if min_num_solution is not None:
-        idx *= num_solution >= min_num_solution
-
-    return site_names[idx], site_lats[idx], site_lons[idx]
-
-
-def get_baseline_change(dates1, pos_x1, pos_y1, pos_z1,
-                        dates2, pos_x2, pos_y2, pos_z2):
-    """Calculate the baseline change between two GPS displacement time-series.
-    Parameters: dates1/2     - 1D np.array of datetime.datetime object
-                pos_x/y/z1/2 - 1D np.ndarray of displacement in meters in np.float32
-    Returns:    dates        - 1D np.array of datetime.datetime object for the common dates
-                bases        - 1D np.ndarray of displacement in meters in np.float32 for the common dates
+        msg  = f'Loaded dataset are processed by InSAR software: {processor}'
+        msg += f'\nLoaded dataset are in {coord_type} coordinates'
+        msg += f'\nInterferogram Stack: {stack_file}'
+        msg += f'\nIonosphere    Stack: {ion_file}' if ion_file else ''
+        msg += f'\nGeometry      File : {geom_file}'
+        msg += f'\nLookup Table  File : {lookup_file}'
+        msg += '\n' + '-' * 50
+        print(msg)
+
+    return stack_file, geom_file, lookup_file, ion_file
+
+
+#################################################################################
+def read_timeseries_lalo(lat, lon, ts_file, lookup_file=None, ref_lat=None, ref_lon=None,
+                         zero_first=True, win_size=1, unit='m', method='mean', print_msg=True):
+    """ Read time-series of one pixel with input lat/lon
+    Parameters: lat/lon     - float, latitude/longitude
+                ts_file     - string, filename of time-series HDF5 file
+                lookup_file - string, filename of lookup table file
+                ref_lat/lon - float, latitude/longitude of reference pixel
+                zero_first  - bool, shift the time-series so that it starts from zero
+                win_size    - int, windows size centered at point of interest
+                unit        - str, output displacement unit
+                method      - str, method to calculate the output displacement and its dispersity
+    Returns:    dates       - 1D np.ndarray of datetime.datetime objects, i.e. datetime.datetime(2010, 10, 20, 0, 0)
+                dis         - 1D np.ndarray of float32, displacement
+                dis_std     - 1D np.ndarray of float32, displacement dispersity
     """
-    dates = np.array(sorted(list(set(dates1) & set(dates2))))
-    bases = np.zeros(dates.shape, dtype=np.float64)
-    for i, date_str in enumerate(dates):
-        idx1 = np.where(dates1 == date_str)[0][0]
-        idx2 = np.where(dates2 == date_str)[0][0]
-        basei = ((pos_x1[idx1] - pos_x2[idx2]) ** 2
-               + (pos_y1[idx1] - pos_y2[idx2]) ** 2
-               + (pos_z1[idx1] - pos_z2[idx2]) ** 2) ** 0.5
-        bases[i] = basei
-    bases -= bases[0]
-    bases = np.array(bases, dtype=np.float32)
-    return dates, bases
-
-
-def get_gps_los_obs(meta, obs_type, site_names, start_date, end_date, gps_comp='enu2los',
-                    horz_az_angle=-90., model=None, print_msg=True, redo=False):
-    """Get the GPS LOS observations given the query info.
-
-    Parameters: meta          - dict, dictionary of metadata of the InSAR file
-                obs_type      - str, GPS observation data type, displacement or velocity.
-                site_names    - list of str, GPS sites, output of search_gps()
-                start_date    - str, date in YYYYMMDD format
-                end_date      - str, date in YYYYMMDD format
-                gps_comp      - str, flag of projecting 2/3D GPS into LOS
-                                e.g. enu2los, hz2los, up2los
-                horz_az_angle - float, azimuth angle of the horizontal motion in degree
-                                measured from the north with anti-clockwise as positive
-                model         - dict, time function model, e.g. {'polynomial': 1, 'periodic': [1.0, 0.5]}
-                print_msg     - bool, print verbose info
-                redo          - bool, ignore existing CSV file and re-calculate
-    Returns:    site_obs      - 1D np.ndarray(), GPS LOS velocity or displacement in m or m/yr
-    Examples:   from mintpy.objects import gps
-                from mintpy.utils import readfile, utils as ut
-                meta = readfile.read_attribute('geo/geo_velocity.h5')
-                SNWE = ut.four_corners(meta)
-                site_names = gps.search_gps(SNWE, start_date='20150101', end_date='20190619')
-                vel = gps.get_gps_los_obs(meta, 'velocity',     site_names, start_date='20150101', end_date='20190619')
-                dis = gps.get_gps_los_obs(meta, 'displacement', site_names, start_date='20150101', end_date='20190619')
+    atr = readfile.read_attribute(ts_file)
+    coord = coordinate(atr, lookup_file=lookup_file)
+    y, x = coord.geo2radar(lat, lon)[0:2]
+    if print_msg:
+        print(f'input lat / lon: {lat} / {lon}')
+        print(f'corresponding y / x: {y} / {x}')
+
+    # reference pixel
+    ref_y, ref_x = None, None
+    if ref_lat is not None:
+        ref_y, ref_x = coord.geo2radar(ref_lat, ref_lon)[0:2]
+
+    # call read_timeseries_yx()
+    dates, dis, dis_std = read_timeseries_yx(y, x, ts_file,
+                                             ref_y=ref_y,
+                                             ref_x=ref_x,
+                                             zero_first=zero_first,
+                                             win_size=win_size,
+                                             unit=unit,
+                                             method=method,
+                                             print_msg=False)
+    return dates, dis, dis_std
+
+
+def read_timeseries_yx(y, x, ts_file, ref_y=None, ref_x=None, zero_first=True,
+                       win_size=1, unit='m', method='mean', print_msg=True):
+    """ Read time-series of one pixel with input y/x
+    Parameters: y/x        - int, row/column number of interest
+                ts_file    - string, filename of time-series HDF5 file
+                ref_y/x    - int, row/column number of reference pixel
+                zero_first - bool, shift the time-series so that it starts from zero
+                win_size   - int, windows size centered at point of interest
+                unit       - str, output displacement unit
+                method     - str, method to calculate the output displacement and its dispersity
+    Returns:    dates      - 1D np.ndarray of datetime.datetime objects, i.e. datetime.datetime(2010, 10, 20, 0, 0)
+                dis        - 1D np.ndarray of float32, displacement
+                dis_std    - 1D np.ndarray of float32, displacement dispersity
     """
-    vprint = print if print_msg else lambda *args, **kwargs: None
-    num_site = len(site_names)
+    # read date
+    obj = timeseries(ts_file)
+    obj.open(print_msg=False)
+    dates = ptime.date_list2vector(obj.dateList)[0]
+    dates = np.array(dates)
 
-    # obs_type --> obs_ind
-    obs_types = ['displacement', 'velocity']
-    if obs_type not in obs_types:
-        raise ValueError(f'un-supported obs_type: {obs_type}')
-    obs_ind = 3 if obs_type.lower() == 'displacement' else 4
-
-    # GPS CSV file info
-    file_dir = os.path.dirname(meta['FILE_PATH'])
-    csv_file = os.path.join(file_dir, f'gps_{gps_comp}')
-    csv_file += f'{horz_az_angle:.0f}' if gps_comp == 'horz' else ''
-    csv_file += '.csv'
-    col_names = ['Site', 'Lon', 'Lat', 'Displacement', 'Velocity']
-    col_types = ['U10'] + ['f8'] * (len(col_names) - 1)
-    vprint(f'default GPS observation file name: {csv_file}')
-
-    # skip re-calculate GPS if:
-    # 1. redo is False AND
-    # 2. csv_file exists (equivalent to num_row > 0) AND
-    # 3. num_row >= num_site
-    num_row = 0
-    if os.path.isfile(csv_file):
-        fc = np.genfromtxt(csv_file, dtype=col_types, delimiter=',', names=True)
-        num_row = fc.size
-
-    if not redo and os.path.isfile(csv_file) and num_row >= num_site:
-        # read from existing CSV file
-        vprint(f'read GPS observations from file: {csv_file}')
-        fc = np.genfromtxt(csv_file, dtype=col_types, delimiter=',', names=True)
-        site_obs = fc[col_names[obs_ind]]
-
-        # get obs for the input site names only
-        # in case the site_names are not consistent with the CSV file.
-        if num_row != num_site:
-            temp_names = fc[col_names[0]]
-            temp_obs = np.array(site_obs, dtype=np.float32)
-            site_obs = np.zeros(num_site, dtype=np.float32) * np.nan
-            for i, site_name in enumerate(site_names):
-                if site_name in temp_names:
-                    site_obs[i] = temp_obs[temp_names == site_name][0]
+    # read displacement
+    if print_msg:
+        print(f'input y / x: {y} / {x}')
+    box = (x, y, x+1, y+1)
+    dis = readfile.read(ts_file, box=box)[0]
+    dis_std = None
+
+    if win_size != 1:
+        buf = int(win_size / 2)
+        box_win = (x-buf, y-buf, x+buf+1, y+buf+1)
+        dis_win = readfile.read(ts_file, box=box_win)[0].reshape(obj.numDate, -1)
+
+        if method == 'mean':
+            dis = np.nanmean(dis_win, axis=1)
+            dis_std = np.nanstd(dis_win, axis=1)
+
+        elif method == 'median':
+            dis = np.nanmedian(dis_win, axis=1)
+            dis_std = median_abs_deviation(dis_win)
 
-    else:
-        # calculate and save to CSV file
-        data_list = []
-        vprint('calculating GPS observation ...')
-
-        # get geom_obj (meta / geom_file)
-        geom_file = ut.get_geometry_file(['incidenceAngle','azimuthAngle'], work_dir=file_dir, coord='geo')
-        if geom_file:
-            geom_obj = geom_file
-            vprint(f'use incidence / azimuth angle from file: {os.path.basename(geom_file)}')
         else:
-            geom_obj = meta
-            vprint('use incidence / azimuth angle from metadata')
-
-        # loop for calculation
-        prog_bar = ptime.progressBar(maxValue=num_site, print_msg=print_msg)
-        for i, site_name in enumerate(site_names):
-            prog_bar.update(i+1, suffix=f'{i+1}/{num_site} {site_name}')
-
-            # calculate gps data value
-            obj = GPS(site_name)
-            vel, dis_ts = obj.get_gps_los_velocity(
-                geom_obj,
-                start_date=start_date,
-                end_date=end_date,
-                gps_comp=gps_comp,
-                horz_az_angle=horz_az_angle,
-                model=model)
-
-            # ignore time-series if the estimated velocity is nan
-            dis = np.nan if np.isnan(vel) else dis_ts[-1] - dis_ts[0]
-
-            # save data to list
-            data_list.append([obj.site, obj.site_lon, obj.site_lat, dis, vel])
-        prog_bar.close()
-
-        # # discard invalid sites
-        # flag = np.isnan([x[-1] for x in data_list])
-        # vprint('discard extra {} stations due to limited overlap/observations in time:'.format(np.sum(flag)))
-        # vprint('  {}'.format(np.array(data_list)[flag][:,0].tolist()))
-        # data_list = [x for x in data_list if not np.isnan(x[-1])]
-
-        # write to CSV file
-        vprint(f'write GPS observations to file: {csv_file}')
-        with open(csv_file, 'w') as fc:
-            fcw = csv.writer(fc)
-            fcw.writerow(col_names)
-            fcw.writerows(data_list)
-
-        # prepare API output
-        site_obs = np.array([x[obs_ind] for x in data_list])
-
-    return site_obs
-
-
-
-
-#################################### Beginning of GPS-GSI utility functions ########################
-def read_pos_file(fname):
-    import codecs
-    fcp = codecs.open(fname, encoding = 'cp1252')
-    fc = np.loadtxt(fcp, skiprows=20, dtype=str, comments=('*','-DATA'))
-
-    ys = fc[:,0].astype(int)
-    ms = fc[:,1].astype(int)
-    ds = fc[:,2].astype(int)
-    dates = [dt.datetime(year=y, month=m, day=d) for y,m,d in zip(ys, ms, ds)]
-
-    X = fc[:,4].astype(np.float64).tolist()
-    Y = fc[:,5].astype(np.float64).tolist()
-    Z = fc[:,6].astype(np.float64).tolist()
-    return dates, X, Y, Z
-
-
-def get_pos_years(gps_dir, site):
-    fnames = glob.glob(os.path.join(gps_dir, f'{site}.*.pos'))
-    years = [os.path.basename(i).split('.')[1] for i in fnames]
-    years = ptime.yy2yyyy(years)
-    return years
-
-
-def read_GSI_F3(gps_dir, site, start_date=None, end_date=None):
-    year0 = int(start_date[0:4])
-    year1 = int(end_date[0:4])
-    num_year = year1 - year0 + 1
-
-    dates, X, Y, Z = [], [], [], []
-    for i in range(num_year):
-        yeari = str(year0 + i)
-        fname = os.path.join(gps_dir, f'{site}.{yeari[2:]}.pos')
-        datesi, Xi, Yi, Zi = read_pos_file(fname)
-        dates += datesi
-        X += Xi
-        Y += Yi
-        Z += Zi
-    dates = np.array(dates)
-    X = np.array(X)
-    Y = np.array(Y)
-    Z = np.array(Z)
-
-    date0 = dt.datetime.strptime(start_date, "%Y%m%d")
-    date1 = dt.datetime.strptime(end_date, "%Y%m%d")
-    flag = np.ones(X.shape, dtype=np.bool_)
-    flag[dates < date0] = False
-    flag[dates > date1] = False
-    return dates[flag], X[flag], Y[flag], Z[flag]
-
-#################################### End of GPS-GSI utility functions ##############################
+            raise ValueError(f'un-recognized method: {method}')
 
+    # reference pixel
+    if ref_y is not None:
+        ref_box = (ref_x, ref_y, ref_x+1, ref_y+1)
+        dis -= readfile.read(ts_file, box=ref_box)[0]
+
+    #start at zero
+    if zero_first:
+        dis -= dis[0]
+
+    # custom output unit
+    if unit == 'm':
+        pass
+    elif unit == 'cm':
+        dis *= 100.
+        dis_std = None if dis_std is None else dis_std * 100.
+    elif unit == 'mm':
+        dis *= 1000.
+        dis_std = None if dis_std is None else dis_std * 1000.
+    else:
+        raise ValueError(f'un-supported output unit: {unit}')
 
+    return dates, dis, dis_std
 
 
-#################################### Beginning of GPS-UNR class ####################################
-class GPS:
-    """GPS class for GPS time-series of daily solution
-
-    Example:
-      import matplotlib.pyplot as plt
-      from mintpy.objects.gps import GPS
-      from mintpy.utils import utils as ut
-      gps_obj = GPS(site='GV05', data_dir='~/insarlab/GPS')
-      gps_obj.open()
-      dis_los = ut.enu2los(gps_obj.dis_e,
-                           gps_obj.dis_n,
-                           gps_obj.dis_u)
-      dates = gps_obj.dates
-      plt.figure()
-      plt.scatter(dates, dis_los)
-      plt.show()
+#####################################################################
+def transect_yx(z, atr, start_yx, end_yx, interpolation='nearest'):
+    """Extract 2D matrix (z) value along the line [x0,y0;x1,y1]
+    Link: http://stackoverflow.com/questions/7878398/how-to-extract-an-arbitrary-line-of-values-from-a-numpy-array
+
+    Parameters: z        : (np.ndarray) 2D data matrix
+                atr      : (dict) attribute
+                start_yx : (list) y,x coordinate of start point
+                end_yx   : (list) y,x coordinate of end   point
+                interpolation : str, sampling/interpolation method, including:
+                    'nearest' - nearest neighbour
+                    'linear'  - linear  spline interpolation (order of 1)
+                    'cubic'   - cubic   spline interpolation (order of 3)
+                    'quintic' - quintic spline interpolation (order of 5)
+
+    Returns:    transect : (dict) containing 1D matrix:
+                    'X'        - 1D np.array for X/column coordinates in float32
+                    'Y'        - 1D np.array for Y/row    coordinates in float32
+                    'value'    - 1D np.array for z value in float32
+                    'distance' - 1D np.array for distance in float32
+
+    Example: from mintpy.utils import readfile, utils as ut
+             dem, atr = readfile.read('srtm1.dem.wgs84')
+             txn = transect_yx(dem, atr, [10,15], [100,115])
     """
+    interpolation = interpolation.lower()
+    [y0, x0] = start_yx
+    [y1, x1] = end_yx
+
+    # check
+    length, width = int(atr['LENGTH']), int(atr['WIDTH'])
+    if not all(0<= i < width and 0<= j < length for i,j in zip([x0,x1], [y0,y1])):
+        msg = 'input start/end point is out of data coverage'
+        msg += f'\nstart_yx: {start_yx}'
+        msg += f'\nend_yx:{end_yx}'
+        msg += f'\ndata size: ({length}, {width})'
+        raise ValueError(msg)
+
+    # Determine points coordinates along the line
+    num_pts = int(np.hypot(x1-x0, y1-y0))
+    ys = np.linspace(y0, y1, num_pts, dtype=np.float32)
+    xs = np.linspace(x0, x1, num_pts, dtype=np.float32)
+
+    # Extract z value along the line
+    # for nearest neighbor sampling, use indexing directly
+    # for other interpolation, use scipy.ndimage.map_coordinates
+    if interpolation == 'nearest':
+        z_line = z[np.rint(ys).astype(int), np.rint(xs).astype(int)]
 
-    def __init__(self, site, data_dir='./GPS', version='IGS14'):
-        self.site = site
-        self.data_dir = os.path.abspath(data_dir)
-        self.version = version
-        self.source = 'Nevada Geodetic Lab'
-
-        # time-series data from Nevada Geodetic Lab
-        # example link: http://geodesy.unr.edu/gps_timeseries/tenv3/IGS08/1LSU.IGS08.tenv3
-        #               http://geodesy.unr.edu/gps_timeseries/tenv3/IGS14/CASU.tenv3
-        if version == 'IGS08':
-            self.file = os.path.join(data_dir, f'{site}.{version}.tenv3')
-        elif version == 'IGS14':
-            self.file = os.path.join(data_dir, f'{site}.tenv3')
+    else:
+        # interpolation name to order
+        interpolate_name2order = {
+            'linear' : 1,
+            'cubic'  : 3,
+            'quintic': 5,
+        }
+        if interpolation not in interpolate_name2order.keys():
+            msg = f'un-supported interpolation method: {interpolation}'
+            msg += f'\navailable methods: {interpolate_name2order.keys()}'
+            raise ValueError(msg)
+        interp_order = interpolate_name2order[interpolation.lower()]
+        # run interpolation
+        z_line = map_coordinates(z, np.vstack((ys, xs)), order=interp_order)
+
+    # Calculate Distance along the line
+    earth_radius = 6.3781e6    # in meter
+    dist_unit = 'm'
+    if 'Y_FIRST' in atr.keys():
+        y_step = float(atr['Y_STEP'])
+        x_step = float(atr['X_STEP'])
+        if not atr.get('UTM_ZONE', None):   # WGS84 lat/lon
+            [lat0, lat1] = coordinate(atr).yx2lalo([y0, y1], [x0, x1])[0]
+            lat_c = (lat0 + lat1) / 2.
+            y_step *= np.pi/180.0 * earth_radius
+            x_step *= np.pi/180.0 * earth_radius * np.cos(lat_c * np.pi/180)
+    else:
+        try:
+            x_step = range_ground_resolution(atr)
+            y_step = azimuth_ground_resolution(atr)
+        except KeyError:
+            x_step = 1
+            y_step = 1
+            dist_unit = 'pixel'
+    dist_line = np.hypot((xs - x0) * x_step,
+                         (ys - y0) * y_step)
+
+    # remove points in masked out areas
+    mask = ~np.isnan(z_line)
+    mask *= z_line != 0.0
+
+    # prepare output
+    transect = {}
+    transect['Y'] = ys[mask]
+    transect['X'] = xs[mask]
+    transect['value'] = z_line[mask]
+    transect['distance'] = dist_line[mask]
+    transect['distance_unit'] = dist_unit
+
+    return transect
+
+
+def transect_lalo(z, atr, start_lalo, end_lalo, interpolation='nearest'):
+    """Extract 2D matrix (z) value along the line [start_lalo, end_lalo]
+
+    Parameters: z        : (np.ndarray) 2D data matrix
+                atr      : (dict) attribute
+                start_yx : (list) y,x coordinate of start point
+                end_yx   : (list) y,x coordinate of end   point
+                interpolation : str, sampling/interpolation method, including:
+                    'nearest' - nearest neighbour
+                    'linear'  - linear  spline interpolation (order of 1)
+                    'cubic'   - cubic   spline interpolation (order of 3)
+                    'quintic' - quintic spline interpolation (order of 5)
+
+    Returns:    transect : (dict) containing 1D matrix:
+                    'X'        - 1D np.array for X/column coordinates in float32
+                    'Y'        - 1D np.array for Y/row    coordinates in float32
+                    'value'    - 1D np.array for z value in float32
+                    'distance' - 1D np.array for distance in float32
+
+    Example: from mintpy.utils import readfile, utils as ut
+             vel, atr = readfile.read('geo_velocity_msk.h5')
+             txn = transect_yx(vel, atr, [30.0, 110.0], [30.2, 111.3])
+    """
+    coord = coordinate(atr)
+    [y0, y1], [x0, x1] = coord.lalo2yx([start_lalo[0], end_lalo[0]],
+                                       [start_lalo[1], end_lalo[1]])
+    transect = transect_yx(z, atr, [y0, x0], [y1, x1], interpolation)
+    return transect
+
+
+def transect_lines(z, atr, lines):
+    """Extract 2D matrix (z) value along multiple lines
+    Parameters: z     : 2D np.ndarray in size of (l,w)
+                atr   : dict, metadata of matrix z
+                lines : list of lines with each line is defined as:
+                    [[lat0, lon0], [lat1, lon1]] for geo coordinates
+                    [[y0, x0], [y1, x1]] for radar coordinates
+    Returns: transect : (dict) containing 1D matrix:
+                    'X' - 1D np.array for X/column coordinates in float32
+                    'Y' - 1D np.array for Y/row.   coordinates in float32
+                    'value' - 1D np.array for z value in float32
+                    'distance' - 1D np.array for distance in float32
+    """
+    transect = {}
+    start_distance = 0
+    transect['start_distance'] = []
+
+    for i, line in enumerate(lines):
+        # read segment data
+        start_lalo, end_lalo = line[0], line[1]
+        if 'Y_FIRST' in atr.keys():
+            seg = transect_lalo(z, atr, start_lalo, end_lalo)
         else:
-            raise ValueError(f'un-recognized GPS data version: {version}')
-
-        url_prefix = 'http://geodesy.unr.edu/gps_timeseries/tenv3'
-        self.file_url = os.path.join(url_prefix, version, os.path.basename(self.file))
-
-        # time-series plot from Nevada Geodetic Lab
-        # example link: http://geodesy.unr.edu/tsplots/IGS08/TimeSeries/CAMO.png
-        #               http://geodesy.unr.edu/tsplots/IGS14/IGS14/TimeSeries/CASU.png
-        self.plot_file = os.path.join(data_dir, f'pic/{site}.png')
-
-        url_prefix = 'http://geodesy.unr.edu/tsplots'
-        if version == 'IGS08':
-            url_prefix += f'/{version}'
-        elif version == 'IGS14':
-            url_prefix += '/{0}/{0}'.format(version)
-        self.plot_file_url = os.path.join(url_prefix, f'TimeSeries/{site}.png')
-
-        # list of stations from Nevada Geodetic Lab
-        self.site_list_file = os.path.join(data_dir, 'DataHoldings.txt')
-        if not os.path.isfile(self.site_list_file):
-            dload_site_list(self.site_list_file)
-        site_names = np.loadtxt(self.site_list_file, dtype=bytes, skiprows=1, usecols=(0)).astype(str)
-        if site not in site_names:
-            raise ValueError(f'Site {site} NOT found in file: {UNR_SITE_LIST_FILE}')
-
-        # directories for data files and plot files
-        for fdir in [data_dir, os.path.dirname(self.plot_file)]:
-            if not os.path.isdir(fdir):
-                os.makedirs(fdir)
-
-    def open(self, print_msg=True):
-        if not os.path.isfile(self.file):
-            self.dload_site()
-        self.get_stat_lat_lon(print_msg=print_msg)
-        self.read_displacement(print_msg=print_msg)
-
-    def dload_site(self, print_msg=True):
-        if print_msg:
-            print(f'downloading {self.site} from {self.file_url}')
-
-        urlretrieve(self.file_url, self.file)
-        urlretrieve(self.plot_file_url, self.plot_file)
-
-        return self.file
-
-    def get_stat_lat_lon(self, print_msg=True):
-        """Get station lat/lon"""
-        if print_msg:
-            print('calculating station lat/lon')
-        if not os.path.isfile(self.file):
-            self.dload_site(print_msg=print_msg)
-
-        data = np.loadtxt(self.file, dtype=bytes, skiprows=1).astype(str)
-        ref_lon, ref_lat = float(data[0, 6]), 0.
-        e0, e_off, n0, n_off = data[0, 7:11].astype(np.float32)
-        e0 += e_off
-        n0 += n_off
-
-        az = np.arctan2(e0, n0) / np.pi * 180.
-        dist = np.sqrt(e0**2 + n0**2)
-        g = Geod(ellps='WGS84')
-        self.site_lon, self.site_lat = g.fwd(ref_lon, ref_lat, az, dist)[0:2]
-        return self.site_lat, self.site_lon
-
-    def read_displacement(self, start_date=None, end_date=None, print_msg=True, display=False):
-        """ Read GPS displacement time-series (defined by start/end_date).
-        Parameters: start/end_date - str in YYYYMMDD format
-        Returns:    dates          - 1D np.ndarray of datetime.datetime object
-                    dis_e/n/u      - 1D np.ndarray of displacement in meters in np.float32
-                    std_e/n/u      - 1D np.ndarray of displacement STD in meters in np.float32
-        """
-        # download file if it's not exists.
-        if not os.path.isfile(self.file):
-            self.dload_site(print_msg=print_msg)
-
-        # read dates, dis_e, dis_n, dis_u
-        if print_msg:
-            print('reading time and displacement in east/north/vertical direction')
-        data = np.loadtxt(self.file, dtype=bytes, skiprows=1).astype(str)
-
-        self.dates = np.array([dt.datetime.strptime(i, "%y%b%d") for i in data[:, 1]])
-        #self.dates = np.array([ptime.decimal_year2datetime(i) for i in data[:, 2]])
-        self.date_list = [x.strftime('%Y%m%d') for x in self.dates]
-
-        (self.dis_e,
-         self.dis_n,
-         self.dis_u,
-         self.std_e,
-         self.std_n,
-         self.std_u) = data[:, (8,10,12,14,15,16)].astype(np.float32).T
-
-        # cut out the specified time range
-        t_flag = np.ones(len(self.dates), np.bool_)
-        if start_date:
-            t0 = ptime.date_list2vector([start_date])[0][0]
-            t_flag[self.dates < t0] = 0
-        if end_date:
-            t1 = ptime.date_list2vector([end_date])[0][0]
-            t_flag[self.dates > t1] = 0
-        self.dates = self.dates[t_flag]
-        self.dis_e = self.dis_e[t_flag]
-        self.dis_n = self.dis_n[t_flag]
-        self.dis_u = self.dis_u[t_flag]
-        self.std_e = self.std_e[t_flag]
-        self.std_n = self.std_n[t_flag]
-        self.std_u = self.std_u[t_flag]
-
-        if display:
-            import matplotlib.pyplot as plt
-            _, ax = plt.subplots(nrows=3, ncols=1, sharex=True)
-            ax[0].scatter(self.dates, self.dis_e, s=2**2, label='East')
-            ax[1].scatter(self.dates, self.dis_n, s=2**2, label='North')
-            ax[2].scatter(self.dates, self.dis_u, s=2**2, label='Up')
-            plt.show()
-
-        return (self.dates,
-                self.dis_e, self.dis_n, self.dis_u,
-                self.std_e, self.std_n, self.std_u)
-
-
-    #####################################  Utility Functions ###################################
-    def displacement_enu2los(self, inc_angle:float, az_angle:float, gps_comp='enu2los', horz_az_angle=-90.):
-        """Convert displacement in ENU to LOS direction.
-
-        Parameters: inc_angle     - float, LOS incidence angle in degree
-                    az_angle      - float, LOS aziuth angle in degree
-                                    from the north, defined as positive in clock-wise direction
-                    gps_comp      - str, GPS components used to convert to LOS direction
-                    horz_az_angle - float, fault azimuth angle used to convert horizontal to fault-parallel
-                                    measured from the north with anti-clockwise as positive
-        Returns:    dis_los       - 1D np.array for displacement in LOS direction
-                    std_los       - 1D np.array for displacement standard deviation in LOS direction
-        """
-        # get unit vector for the component of interest
-        unit_vec = ut.get_unit_vector4component_of_interest(
-            los_inc_angle=inc_angle,
-            los_az_angle=az_angle,
-            comp=gps_comp.lower(),
-            horz_az_angle=horz_az_angle,
-        )
-
-        # convert ENU to LOS direction
-        self.dis_los = (  self.dis_e * unit_vec[0]
-                        + self.dis_n * unit_vec[1]
-                        + self.dis_u * unit_vec[2])
-        # assuming ENU component are independent with each other
-        self.std_los = (   (self.std_e * unit_vec[0])**2
-                         + (self.std_n * unit_vec[1])**2
-                         + (self.std_u * unit_vec[2])**2 ) ** 0.5
-
-        return self.dis_los, self.std_los
-
-
-    def get_los_geometry(self, geom_obj, print_msg=False):
-        """Get the Line-of-Sight geometry info in incidence and azimuth angle in degrees."""
-        lat, lon = self.get_stat_lat_lon(print_msg=print_msg)
-
-        # get LOS geometry
-        if isinstance(geom_obj, str):
-            # geometry file
-            atr = readfile.read_attribute(geom_obj)
-            coord = coordinate(atr, lookup_file=geom_obj)
-            y, x = coord.geo2radar(lat, lon, print_msg=print_msg)[0:2]
-            # check against image boundary
-            y = max(0, y);  y = min(int(atr['LENGTH'])-1, y)
-            x = max(0, x);  x = min(int(atr['WIDTH'])-1, x)
-            box = (x, y, x+1, y+1)
-            inc_angle = readfile.read(geom_obj, datasetName='incidenceAngle', box=box, print_msg=print_msg)[0][0,0]
-            az_angle  = readfile.read(geom_obj, datasetName='azimuthAngle',   box=box, print_msg=print_msg)[0][0,0]
-
-        elif isinstance(geom_obj, dict):
-            # use mean inc/az_angle from metadata
-            inc_angle = ut.incidence_angle(geom_obj, dimension=0, print_msg=print_msg)
-            az_angle  = ut.heading2azimuth_angle(float(geom_obj['HEADING']))
+            seg = transect_yx(z, atr, start_lalo, end_lalo)
+        seg['distance'] += start_distance
 
+        # connect each segment
+        if i == 0:
+            # first segment
+            for key, value in seg.items():
+                transect[key] = np.array(value, dtype=np.float32)
         else:
-            raise ValueError(f'input geom_obj is neither str nor dict: {geom_obj}')
+            for key, value in seg.items():
+                transect[key] = np.concatenate((transect[key], value))
 
-        return inc_angle, az_angle
+        # update start_distance for the next segment
+        transect['start_distance'].append(start_distance)
+        start_distance = transect['distance'][-1]
+    transect['start_distance'] = np.array(transect['start_distance'], dtype=np.float32)
+    return transect
 
 
-    def read_gps_los_displacement(self, geom_obj, start_date=None, end_date=None, ref_site=None,
-                                  gps_comp='enu2los', horz_az_angle=-90., print_msg=False):
-        """Read GPS displacement in LOS direction.
-
-        Parameters: geom_obj      - dict / str, metadata of InSAR file, or geometry file path
-                    start_date    - str in YYYYMMDD format
-                    end_date      - str in YYYYMMDD format
-                    ref_site      - str, reference GPS site
-                    gps_comp      - str, GPS components used to convert to LOS direction
-                    horz_az_angle - float, fault azimuth angle used to convert horizontal to fault-parallel
-        Returns:    dates         - 1D np.array of datetime.datetime object
-                    dis/std       - 1D np.array of displacement / uncertainty in meters
-                    site_lalo     - tuple of 2 float, lat/lon of GPS site
-                    ref_site_lalo - tuple of 2 float, lat/lon of reference GPS site
-        """
-        # read GPS object
-        inc_angle, az_angle = self.get_los_geometry(geom_obj)
-        dates = self.read_displacement(start_date, end_date, print_msg=print_msg)[0]
-        dis, std = self.displacement_enu2los(inc_angle, az_angle, gps_comp=gps_comp, horz_az_angle=horz_az_angle)
-        site_lalo = self.get_stat_lat_lon(print_msg=print_msg)
-
-        # get LOS displacement relative to another GPS site
-        if ref_site:
-            ref_obj = GPS(site=ref_site, data_dir=self.data_dir)
-            ref_obj.read_displacement(start_date, end_date, print_msg=print_msg)
-            inc_angle, az_angle = ref_obj.get_los_geometry(geom_obj)
-            ref_obj.displacement_enu2los(inc_angle, az_angle, gps_comp=gps_comp, horz_az_angle=horz_az_angle)
-            ref_site_lalo = ref_obj.get_stat_lat_lon(print_msg=print_msg)
-
-            # get relative LOS displacement on common dates
-            dates = np.array(sorted(list(set(self.dates) & set(ref_obj.dates))))
-            dis = np.zeros(dates.shape, np.float32)
-            std = np.zeros(dates.shape, np.float32)
-            for i, date_i in enumerate(dates):
-                idx1 = np.where(self.dates == date_i)[0][0]
-                idx2 = np.where(ref_obj.dates == date_i)[0][0]
-                dis[i] = self.dis_los[idx1] - ref_obj.dis_los[idx2]
-                std[i] = (self.std_los[idx1]**2 + ref_obj.std_los[idx2]**2)**0.5
-        else:
-            ref_site_lalo = None
 
-        return dates, dis, std, site_lalo, ref_site_lalo
+#################################################################################
 
+def prepare_geo_los_geometry(geom_file, unit='rad'):
+    """Prepare LOS geometry data/info in geo-coordinates.
 
-    def get_gps_los_velocity(self, geom_obj, start_date=None, end_date=None, ref_site=None,
-                             gps_comp='enu2los', horz_az_angle=-90., model=None):
+    Parameters: geom_file - str, path of geometry file
+                unit      - str, rad or deg, output angle unit
+    Returns:    inc_angle - 2D np.ndarray, incidence angle in radians / degrees
+                            measured from the vertical
+                az_angle  - 2D np.ndarray, azimuth   angle in radians / degrees
+                            measured from the north with anti-clockwise direction as positive
+                atr       - dict, metadata in geo-coordinate
+    """
 
-        dates, dis = self.read_gps_los_displacement(
-            geom_obj,
-            start_date=start_date,
-            end_date=end_date,
-            ref_site=ref_site,
-            gps_comp=gps_comp,
-            horz_az_angle=horz_az_angle)[:2]
-
-        # displacement -> velocity
-        # if:
-        # 1. num of observations > 2 AND
-        # 2. time overlap > 1/4
-        dis2vel = True
-        if len(dates) <= 2:
-            dis2vel = False
-        elif start_date and end_date:
-            t0 = ptime.date_list2vector([start_date])[0][0]
-            t1 = ptime.date_list2vector([end_date])[0][0]
-            if dates[-1] - dates[0] <= (t1 - t0) / 4:
-                dis2vel = False
-
-        if dis2vel:
-            # specific time_func model
-            date_list = [dt.datetime.strftime(i, '%Y%m%d') for i in dates]
-            A = time_func.get_design_matrix4time_func(date_list, model=model)
-            self.velocity = np.dot(np.linalg.pinv(A), dis)[1]
-        else:
-            self.velocity = np.nan
+    print(f'prepare LOS geometry in geo-coordinates from file: {geom_file}')
+    atr = readfile.read_attribute(geom_file)
+
+    print(f'read incidenceAngle from file: {geom_file}')
+    inc_angle = readfile.read(geom_file, datasetName='incidenceAngle')[0]
 
-        return self.velocity, dis
+    if 'azimuthAngle' in readfile.get_dataset_list(geom_file):
+        print(f'read azimuthAngle   from file: {geom_file}')
+        az_angle  = readfile.read(geom_file, datasetName='azimuthAngle')[0]
+    else:
+        print('use the HEADING attribute as the mean heading angle')
+        print('convert heading angle to azimuth angle')
+        head_angle = np.ones(inc_angle.shape, dtype=np.float32) * float(atr['HEADING'])
+        az_angle = heading2azimuth_angle(head_angle)
+
+    # geocode inc/az angle data if in radar-coord
+    if 'Y_FIRST' not in atr.keys():
+        print('-'*50)
+        print('geocoding the incidence / heading angles ...')
+        res_obj = resample(lut_file=geom_file, src_file=geom_file)
+        res_obj.open()
+        res_obj.prepare()
+
+        # resample data
+        box = res_obj.src_box_list[0]
+        inc_angle = res_obj.run_resample(src_data=inc_angle[box[1]:box[3], box[0]:box[2]])
+        az_angle = res_obj.run_resample(src_data=az_angle[box[1]:box[3], box[0]:box[2]])
+
+        # update attribute
+        atr = attr.update_attribute4radar2geo(atr, res_obj=res_obj)
+
+    # for 'Y_FIRST' not in 'degree'
+    # e.g. meters for UTM projection from ASF HyP3
+    if not atr['Y_UNIT'].lower().startswith('deg'):
+        # get SNWE in meter
+        length, width = int(atr['LENGTH']), int(atr['WIDTH'])
+        N = float(atr['Y_FIRST'])
+        W = float(atr['X_FIRST'])
+        y_step = float(atr['Y_STEP'])
+        x_step = float(atr['X_STEP'])
+        S = N + y_step * length
+        E = W + x_step * width
+
+        # SNWE in meter --> degree
+        lat0, lon0 = utm2latlon(atr, W, N)
+        lat1, lon1 = utm2latlon(atr, E, S)
+        lat_step = (lat1 - lat0) / length
+        lon_step = (lon1 - lon0) / width
+
+        # update Y/X_FIRST/STEP/UNIT
+        atr['Y_FIRST'] = lat0
+        atr['X_FIRST'] = lon0
+        atr['Y_STEP'] = lat_step
+        atr['X_STEP'] = lon_step
+        atr['Y_UNIT'] = 'degrees'
+        atr['X_UNIT'] = 'degrees'
+
+    # set invalid values to nan
+    inc_angle[inc_angle == 0] = np.nan
+
+    # unit: degree to radian
+    if unit.startswith('rad'):
+        inc_angle *= np.pi / 180.
+        az_angle *= np.pi / 180.
 
-#################################### End of GPS-UNR class ####################################
+    return inc_angle, az_angle, atr
```

### Comparing `mintpy-1.5.3/src/mintpy/objects/insar_vs_gps.py` & `mintpy-1.6.0/src/mintpy/objects/insar_vs_gnss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,79 @@
-"""Class for comparing InSAR with GPS."""
+"""Class for comparing InSAR with GNSS."""
 ############################################################
 # Program is part of MintPy                                #
 # Copyright (c) 2013, Zhang Yunjun, Heresh Fattahi         #
 # Author: Zhang Yunjun, 2018                               #
 ############################################################
 # Recommend import:
-#   from mintpy.objects.insar_vs_gps import insar_vs_gps
+#   from mintpy.objects.insar_vs_gnss import insar_vs_gnss
 
 
 import datetime as dt
 import sys
 
 import numpy as np
 from scipy import stats
 from scipy.interpolate import griddata
 
 from mintpy.defaults.plot import *
-from mintpy.objects import giantTimeseries, timeseries
-from mintpy.objects.gps import GPS
+from mintpy.objects import giantTimeseries, gnss, timeseries
 from mintpy.utils import readfile, utils as ut
 
 
-############################## beginning of insar_vs_gps class ##############################
-class insar_vs_gps:
-    """ Comparing InSAR time-series with GPS time-series in LOS direction
-    Parameters: ts_file        : str, time-series HDF5 file
-                geom_file      : str, geometry HDF5 file
-                temp_coh_file  : str, temporal coherence HDF5 file
-                site_names     : list of str, GPS site names
-                gps_dir        : str, directory of the local GPS data files
-                ref_site       : str, common reference site in space for InSAR and GPS
-                start/end_date : str, date in YYYYMMDD format for the start/end date
-                min_ref_date   : str, date in YYYYMMDD format for the earliest common
-                    reference date between InSAR and GPS
-    Returns:    ds : dict, each element has the following components:
+############################## beginning of insar_vs_gnss class ##############################
+class insar_vs_gnss:
+    """ Comparing InSAR time-series with GNSS time-series in LOS direction
+    Parameters: ts_file        - str, time-series HDF5 file
+                geom_file      - str, geometry HDF5 file
+                temp_coh_file  - str, temporal coherence HDF5 file
+                site_names     - list of str, GNSS site names
+                gnss_source    - str, program or institution that processed the GNSS data
+                gnss_dir       - str, directory of the local GNSS data files
+                ref_site       - str, common reference site in space for InSAR and GNSS
+                start/end_date - str, date in YYYYMMDD format for the start/end date
+                min_ref_date   - str, date in YYYYMMDD format for the earliest common
+                                 reference date between InSAR and GNSS
+    Returns:    ds - dict, each element has the following components:
                     'GV03': {
-                      'name': 'GV03',
-                      'lat': -0.7977926892712729,
-                      'lon': -91.13294444114553,
-                      'gps_datetime': array([datetime.datetime(2014, 11, 1, 0, 0),
-                             datetime.datetime(2014, 11, 2, 0, 0),
-                             ...,
-                             datetime.datetime(2018, 6, 25, 0, 0)], dtype=object),
-                      'gps_dis': array([-2.63673663e-02, ..., 6.43612206e-01], dtype=float32),
-                      'gps_std': array([0.00496152, ..., 0.00477411], dtype=float32),
+                      'name'          : 'GV03',
+                      'lat'           : -0.7977926892712729,
+                      'lon'           : -91.13294444114553,
+                      'gnss_datetime' : array([datetime.datetime(2014, 11, 1, 0, 0),
+                                              datetime.datetime(2014, 11, 2, 0, 0),
+                                              ...,
+                                              datetime.datetime(2018, 6, 25, 0, 0),
+                                              ], dtype=object),
+                      'gnss_dis'      : array([-2.63673663e-02, ..., 6.43612206e-01], dtype=float32),
+                      'gnss_std'      : array([0.00496152, ..., 0.00477411], dtype=float32),
                       'reference_site': 'GV01',
                       'insar_datetime': array([datetime.datetime(2014, 12, 13, 0, 0),
-                             datetime.datetime(2014, 12, 25, 0, 0),
-                             ...,
-                             datetime.datetime(2018, 6, 19, 0, 0)], dtype=object),
+                                               datetime.datetime(2014, 12, 25, 0, 0),
+                                               ...,
+                                               datetime.datetime(2018, 6, 19, 0, 0),
+                                               ], dtype=object),
                       'insar_dis_linear': array([-0.01476493, ...,  0.62273948]),
-                      'temp_coh': 0.9961861392598478,
-                      'gps_std_mean': 0.004515478,
-                      'comm_dis_gps': array([-0.02635017, ..., 0.61315614], dtype=float32),
-                      'comm_dis_insar': array([-0.01476493, ..., 0.60640174], dtype=float32),
-                      'r_square': 0.9993494518609801,
-                      'dis_rmse': 0.008023425326946351
+                      'temp_coh'        : 0.9961861392598478,
+                      'gnss_std_mean'   : 0.004515478,
+                      'comm_dis_gnss'   : array([-0.02635017, ..., 0.61315614], dtype=float32),
+                      'comm_dis_insar'  : array([-0.01476493, ..., 0.60640174], dtype=float32),
+                      'r_square'        : 0.9993494518609801,
+                      'dis_rmse'        : 0.008023425326946351,
                     }
     """
 
-    def __init__(self, ts_file, geom_file, temp_coh_file,
-                 site_names, gps_dir='./GPS', ref_site='GV01',
-                 start_date=None, end_date=None, min_ref_date=None):
+    def __init__(self, ts_file, geom_file, temp_coh_file, site_names, gnss_source='UNR',
+                 gnss_dir='./GNSS', ref_site='GV01', start_date=None, end_date=None,
+                 min_ref_date=None):
         self.insar_file = ts_file
         self.geom_file = geom_file
         self.temp_coh_file = temp_coh_file
         self.site_names = site_names
-        self.gps_dir = gps_dir
+        self.gnss_source = gnss_source
+        self.gnss_dir = gnss_dir
         self.ref_site = ref_site
         self.num_site = len(site_names)
         self.ds = {}
         self.start_date = start_date
         self.end_date = end_date
         self.min_ref_date = min_ref_date
 
@@ -82,56 +85,60 @@
         elif k == 'giantTimeseries':
             ts_obj = giantTimeseries(self.insar_file)
         else:
             raise ValueError(f'Un-supported time-series file: {k}')
         ts_obj.open(print_msg=False)
         self.metadata = dict(ts_obj.metadata)
         self.num_date = ts_obj.numDate
-        # remove time info from insar_datetime to be consistent with gps_datetime
+        # remove time info from insar_datetime to be consistent with gnss_datetime
         self.insar_datetime = np.array([i.replace(hour=0, minute=0, second=0, microsecond=0)
                                         for i in ts_obj.times])
 
         # default start/end_date & min_ref_date
         dt_buffer = dt.timedelta(days=30)
         self.start_date = self.start_date if self.start_date else (ts_obj.times[0] - dt_buffer).strftime('%Y%m%d')
         self.end_date = self.end_date if self.end_date else (ts_obj.times[-1] + dt_buffer).strftime('%Y%m%d')
         self.min_ref_date = self.min_ref_date if self.min_ref_date else ts_obj.times[5].strftime('%Y%m%d')
         if self.min_ref_date not in ts_obj.dateList:
             msg = f'min_ref_date {self.min_ref_date} does NOT exist in InSAR file: {self.insar_file}'
             raise ValueError(msg)
 
-        self.read_gps()
+        self.read_gnss()
         self.read_insar()
         self.calculate_rmse()
         return
 
-    def read_gps(self):
+    def read_gnss(self):
+        # define GNSS station object based on processing source
+        GNSS = gnss.get_gnss_class(self.gnss_source)
+
+        # read data for each GNSS site
         for sname in self.site_names:
             site = {}
             site['name'] = sname
-            gps_obj = GPS(sname, data_dir=self.gps_dir)
-            gps_obj.open(print_msg=False)
-            site['lat'] = gps_obj.site_lat
-            site['lon'] = gps_obj.site_lon
+            gnss_obj = GNSS(sname, data_dir=self.gnss_dir)
+            gnss_obj.open(print_msg=False)
+            site['lat'] = gnss_obj.site_lat
+            site['lon'] = gnss_obj.site_lon
 
-            dates, dis, dis_std = gps_obj.read_gps_los_displacement(
+            dates, dis, dis_std = gnss_obj.get_los_displacement(
                 self.geom_file,
                 start_date=self.start_date,
                 end_date=self.end_date,
                 ref_site=self.ref_site,
-                gps_comp='enu2los',
+                gnss_comp='enu2los',
             )[0:3]
-            site['gps_datetime'] = dates
-            site['gps_dis'] = dis
-            site['gps_std'] = dis_std
+            site['gnss_datetime'] = dates
+            site['gnss_dis'] = dis
+            site['gnss_std'] = dis_std
 
             site['reference_site'] = self.ref_site
             self.ds[sname] = site
 
-            sys.stdout.write(f'\rreading GPS {sname}')
+            sys.stdout.write(f'\rreading GNSS {sname}')
             sys.stdout.flush()
         print()
         return
 
     def read_insar(self):
         # 2.1 prepare interpolation
         coord = ut.coordinate(self.metadata, lookup_file=self.geom_file)
@@ -172,81 +179,81 @@
         for i in range(self.num_site):
             site = self.ds[self.site_names[i]]
             site['insar_datetime'] = self.insar_datetime
             # reference insar to the precise location in space
             site[self.insar_dis_name] = insar_dis[i,:] - insar_dis_ref
             site['temp_coh'] = temp_coh[i]
 
-        # 2.4 reference insar and gps to a common date
-        print('reference insar and gps to a common date')
+        # 2.4 reference insar and gnss to a common date
+        print('reference insar and gnss to a common date')
         for i in range(self.num_site):
             site = self.ds[self.site_names[i]]
-            gps_date = site['gps_datetime']
+            gnss_date = site['gnss_datetime']
             insar_date = site['insar_datetime']
 
             # find common reference date
             ref_date = dt.datetime.strptime(self.min_ref_date, "%Y%m%d")
             ref_idx = insar_date.tolist().index(ref_date)
             while ref_idx < self.num_date:
-                if insar_date[ref_idx] not in gps_date:
+                if insar_date[ref_idx] not in gnss_date:
                     ref_idx += 1
                 else:
                     break
             if ref_idx == self.num_date:
-                msg = f"InSAR and GPS do not share ANY date for site: {site['name']}"
+                msg = f"InSAR and GNSS do not share ANY date for site: {site['name']}"
                 raise RuntimeError(msg)
             comm_date = insar_date[ref_idx]
 
             # reference insar in time
             site[self.insar_dis_name] -= site[self.insar_dis_name][ref_idx]
-            # reference gps dis/std in time
-            ref_idx_gps = np.where(gps_date == comm_date)[0][0]
-            site['gps_dis'] -= site['gps_dis'][ref_idx_gps]
-            site['gps_std'] = np.sqrt(site['gps_std']**2 + site['gps_std'][ref_idx_gps]**2)
-            site['gps_std_mean'] = np.mean(site['gps_std'])
+            # reference gnss dis/std in time
+            ref_idx_gnss = np.where(gnss_date == comm_date)[0][0]
+            site['gnss_dis'] -= site['gnss_dis'][ref_idx_gnss]
+            site['gnss_std'] = np.sqrt(site['gnss_std']**2 + site['gnss_std'][ref_idx_gnss]**2)
+            site['gnss_std_mean'] = np.mean(site['gnss_std'])
         return
 
 
     def calculate_rmse(self):
         ## 3. calculate RMSE
         for i in range(self.num_site):
             site = self.ds[self.site_names[i]]
-            gps_date = site['gps_datetime']
+            gnss_date = site['gnss_datetime']
             insar_date = site['insar_datetime']
-            comm_dates = np.array(sorted(list(set(gps_date) & set(insar_date))))
+            comm_dates = np.array(sorted(list(set(gnss_date) & set(insar_date))))
             num_comm_date = len(comm_dates)
 
             # get displacement at common dates
             comm_dis_insar = np.zeros(num_comm_date, np.float32)
-            comm_dis_gps   = np.zeros(num_comm_date, np.float32)
+            comm_dis_gnss   = np.zeros(num_comm_date, np.float32)
             for j in range(num_comm_date):
-                idx1 = np.where(gps_date   == comm_dates[j])[0][0]
+                idx1 = np.where(gnss_date   == comm_dates[j])[0][0]
                 idx2 = np.where(insar_date == comm_dates[j])[0][0]
-                comm_dis_gps[j]   = site['gps_dis'][idx1]
+                comm_dis_gnss[j]   = site['gnss_dis'][idx1]
                 comm_dis_insar[j] = site[self.insar_dis_name][idx2]
-            site['comm_dis_gps'] = comm_dis_gps
+            site['comm_dis_gnss'] = comm_dis_gnss
             site['comm_dis_insar'] = comm_dis_insar
-            site['r_square'] = stats.linregress(comm_dis_gps, comm_dis_insar)[2]
-            site['dis_rmse'] = np.sqrt(np.sum(np.square(comm_dis_gps - comm_dis_insar)) / (num_comm_date - 1))
+            site['r_square'] = stats.linregress(comm_dis_gnss, comm_dis_insar)[2]
+            site['dis_rmse'] = np.sqrt(np.sum(np.square(comm_dis_gnss - comm_dis_insar)) / (num_comm_date - 1))
             #print('site: {}, RMSE: {:.1f} cm'.format(self.site_names[i], dis_rmse*100.))
 
 
     def sort_by_velocity(ds):
         ## 4. calculate velocity to sort plotting order
         site_vel = {}
         site_names = sorted(list(ds.keys()))
         for sname in site_names:
             site = ds[sname]
             # design matrix
-            yr_diff = np.array([i.year + (i.timetuple().tm_yday - 1) / 365.25 for i in site['gps_datetime']])
+            yr_diff = np.array([i.year + (i.timetuple().tm_yday - 1) / 365.25 for i in site['gnss_datetime']])
             yr_diff -= yr_diff[0]
-            A = np.ones([len(site['gps_datetime']), 2], dtype=np.float32)
+            A = np.ones([len(site['gnss_datetime']), 2], dtype=np.float32)
             A[:, 0] = yr_diff
             # LS estimation
-            ts = np.array(site['gps_dis'])
+            ts = np.array(site['gnss_dis'])
             ts -= ts[0]
             X = np.dot(np.linalg.pinv(A), ts)[0]
             site_vel[sname] = X
 
         site_names2plot = [i[0] for i in sorted(site_vel.items(), key=lambda kv: kv[1], reverse=True)]
         site_names2plot = [i for i in site_names2plot if site_vel[i] != 0]
         return site_names2plot
@@ -260,22 +267,22 @@
                 site['dis_rmse']*100.,
                 site['r_square'],
                 site['temp_coh'],
             ))
         return
 
     def plot_one_site(ax, site, offset=0.):
-        # GPS
-        ax.errorbar(site['gps_datetime'],
-                    site['gps_dis']-offset,
-                    yerr=site['gps_std']*3.,
+        # GNSS
+        ax.errorbar(site['gnss_datetime'],
+                    site['gnss_dis']-offset,
+                    yerr=site['gnss_std']*3.,
                     ms=marker_size*0.2, lw=0, alpha=1., fmt='-o',
                     elinewidth=edge_width*0.5, ecolor='C0',
                     capsize=marker_size*0.25, markeredgewidth=edge_width*0.5,
-                    label='GPS', zorder=1)
+                    label='GNSS', zorder=1)
         # InSAR
         ecolor = 'gray' if site['temp_coh'] < 0.7 else 'C1'
         insar_dis_name = [i for i in site.keys() if i.startswith('insar_dis')][0]
         ax.scatter(site['insar_datetime'],
                    site[insar_dis_name]-offset,
                    s=5**2, label='InSAR',
                    facecolors='none', edgecolors=ecolor, linewidth=1., alpha=0.7, zorder=2)
@@ -286,8 +293,8 @@
                     color='k', fontsize=font_size)
         ax.annotate('{}'.format(site['name']),
                     xy=(0.05, site[insar_dis_name][0] - offset + 0.1),
                     xycoords=ax.get_yaxis_transform(),  # y in data untis, x in axes fraction
                     color='k', fontsize=font_size)
         return ax
 
-############################## end of insar_vs_gps class ####################################
+############################## end of insar_vs_gnss class ####################################
```

### Comparing `mintpy-1.5.3/src/mintpy/objects/ionex.py` & `mintpy-1.6.0/src/mintpy/objects/ionex.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/progress.py` & `mintpy-1.6.0/src/mintpy/objects/progress.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/ramp.py` & `mintpy-1.6.0/src/mintpy/objects/ramp.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/resample.py` & `mintpy-1.6.0/src/mintpy/objects/resample.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/sensor.py` & `mintpy-1.6.0/src/mintpy/objects/sensor.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 import os
 
 SENSOR_NAME_VARIATION = {
     'alos'  : ['alos', 'alos1', 'palsar', 'palsar1'],
     'alos2' : ['alos2', 'palsar2'],
+    'alos4' : ['alos4', 'palsar3'],
     'csk'   : ['csk', 'csk1', 'csk2', 'csk3', 'csk4', 'cos', 'cosmo', 'cosmoskymed'],
     'env'   : ['env', 'envisat', 'asar'],
     'ers'   : ['ers', 'ers1', 'ers2', 'ers12'],
     'gf3'   : ['gfen3', 'gaofen3', 'g3', 'gaofen'],
     'jers'  : ['jers', 'jers1'],
     'ksat5' : ['ksat5', 'kompsat5', 'kompsat', 'kmps5'],
     'lt1'   : ['lt1', 'lt', 'lutan', 'lutan1'],
@@ -193,133 +194,210 @@
 #     user-guides/sentinel-1-sar/acquisition-modes/interferometric-wide-swath
 # JERS       : SNR = 14 dB from https://directory.eoportal.org/web/eoportal/satellite-missions/j/jers-1
 
 
 ##--------------------  X-band  --------------------##
 # TerraSAR-X stripmap mode in single polarization
 # from Table 1 in Jung et al. (2014)
+# https://www.eoportal.org/satellite-missions/terrasar-x
 TSX = {
+    # orbit
+    'altitude'                   : 514.8e3,   # m, mean value, 505-533 km
+    'orbit_inclination'          : 97.44,     # deg
+    'repeat_cycle'               : 11,        # day
+    # sar / antenna
     'carrier_frequency'          : 9.65e9,    # Hz
-    'altitude'                   : 516e3,     # m, mean value
     'antenna_length'             : 4.8,       # m
+    'antenna_width'              : 0.8,       # m
     'doppler_bandwidth'          : 2770,      # Hz
     'pulse_repetition_frequency' : 3800,      # Hz
     'chirp_bandwidth'            : 100e6,     # Hz
     'sampling_frequency'         : 109.89e6,  # Hz
     'azimuth_pixel_size'         : 2.0,       # m
     'ground_range_pixel_size'    : 2.2,       # m
 }
 
 # COSMO-SkyMed stripmap HIMAGE mode
 # from Table 1 in Jung et al. (2014)
+# https://www.eoportal.org/satellite-missions/cosmo-skymed
 CSK = {
+    # orbit
+    'altitude'                   : 619.6e3,   # m, mean value
+    'orbit_inclination'          : 97.86,     # deg
+    'repeat_cycle'               : 16,        # day, single satellite
+    # sar / antenna
     'carrier_frequency'          : 9.6e9,     # Hz
-    'altitude'                   : 619e3,     # m, mean value
     'antenna_length'             : 5.7,       # m
+    'antenna_width'              : 1.4,       # m
     'doppler_bandwidth'          : 2670,      # Hz
     'pulse_repetition_frequency' : 3000,      # Hz
     'chirp_bandwidth'            : 117e6,     # Hz
     'sampling_frequency'         : 146.25e6,  # Hz
     'azimuth_pixel_size'         : 2.4,       # m
     'ground_range_pixel_size'    : 1.6,       # m
 }
 
-# Kompsat-5 stripmap mode
+# Kompsat-5 (Korea Multi-Purpose Satellite-5) stripmap mode
 # from Table 1 in Jung et al. (2014)
+# https://www.eoportal.org/satellite-missions/kompsat-5
 KSAT5 = {
-    'carrier_frequency'          : 9.66e9,    # Hz
+    # orbit
     'altitude'                   : 550e3,     # m, mean value
+    'orbit_inclination'          : 98.1,      # deg
+    'repeat_cycle'               : 28,        # day
+    # sar / antenna
+    'carrier_frequency'          : 9.66e9,    # Hz
     'antenna_length'             : 4.48,      # m
     'doppler_bandwidth'          : 3110,      # Hz
     'pulse_repetition_frequency' : 3530,      # Hz
     'chirp_bandwidth'            : 73.24e6,   # Hz
     'sampling_frequency'         : 88.125e6,  # Hz
     'azimuth_pixel_size'         : 2.1,       # m
     'ground_range_pixel_size'    : 2.7,       # m
 }
 
 # ICEYE SAR constellation
 # from Table 2.1 in ICEYE SAR Product Guide at:
 # https://earth.esa.int/eogateway/documents/20142/37627/ICEYE-SAR-Product-Guide-V4.pdf
+# https://www.eoportal.org/satellite-missions/iceye-constellation
 ICEYE = {
+    # orbit
+    'altitude'                   : 570e3,           # m, mean value, 560-580 km
+    'orbit_inclination'          : 97.7,            # deg
+    'repeat_cycle'               : 17,              # day, single satellite
+    # sar / antenna
     'carrier_frequency'          : 9.65e9,          # Hz
-    'altitude'                   : 570e3,           # m
     'antenna_length'             : 3.2,             # m
     'antenna_width'              : 0.4,             # m
     'pulse_repetition_frequency' : [2e3, 10e3],     # Hz
     'chirp_bandwidth'            : [37.6e6, 299e6], # Hz
 }
 
 
 ##--------------------  C-band  --------------------##
 
 # ERS-1/2
 # from Table 2 in Jung et al. (2014)
 # from Imaging Radar class by Howard Zebker, 2021.
+# https://www.esa.int/esapub/bulletin/bullet83/duc83.htm
+# https://www.eoportal.org/satellite-missions/ers-1
 ERS = {
-    'carrier_frequency'          : 5.300e9,     # Hz
-    'altitude'                   : 783e3,       # m, mean value
+    # orbit
+    'altitude'                   : 785e3,       # m, mean value, 782-785 km
+    'orbit_inclination'          : 98.52,       # deg
+    'repeat_cycle'               : 35,          # day
+    # sar / antenna
+    'carrier_frequency'          : 5.30e9,      # Hz
     'antenna_length'             : 10.0,        # m
+    'antenna_width'              : 1.0,         # m
     'doppler_bandwidth'          : 1500,        # Hz
     'pulse_repetition_frequency' : 1679.9,      # Hz
     'pulse_length'               : 37.12e-6,    # s
     'chirp_bandwidth'            : 15.55e6,     # Hz
     'chirp_slope'                : 4.189166e11, # Hz
     'sampling_frequency'         : 18.96e6,     # Hz
     'azimuth_pixel_size'         : 4.2,         # m
     'ground_range_pixel_size'    : 20.2,        # m
 }
 
 # Envisat
 # from Table 2 in Jung et al. (2014)
+# https://earth.esa.int/eogateway/missions/envisat/description
+# https://www.eoportal.org/satellite-missions/envisat#asar-advanced-sar
 ENV = {
+    # orbit
+    'altitude'                   : 799.8e3,   # m, mean value, 780-820 km
+    'orbit_inclination'          : 98.55,     # deg
+    'repeat_cycle'               : 35,        # day
+    # sar / antenna
     'carrier_frequency'          : 5.331e9,   # Hz
-    'altitude'                   : 800e3,     # m, mean value
     'antenna_length'             : 10.0,      # m
+    'antenna_width'              : 1.3,       # m
     'doppler_bandwidth'          : 1500,      # Hz
     'pulse_repetition_frequency' : 1650,      # Hz
     'chirp_bandwidth'            : 16.00e6,   # Hz
     'sampling_frequency'         : 18.00e6,   # Hz
     'azimuth_pixel_size'         : 4.3,       # m
     'ground_range_pixel_size'    : 21.3,      # m
 }
 
+# Radarsat-1
+# https://www.asc-csa.gc.ca/eng/satellites/radarsat/technical-features/radarsat-comparison.asp
+RSAT1 = {
+    # orbit
+    'altitude'                   : 807e3,     # m, mean value, 793-821 km
+    'orbit_inclination'          : 98.6,      # deg
+    'repeat_cycle'               : 14,        # day, 14.29 orbits per day (14 7/24)
+    # sar / antenna
+    'carrier_frequency'          : 5.3e9,     # Hz
+    'antenna_length'             : 15,        # m
+    'antenna_width'              : 1.5,       # m
+}
+
 # Radarsat-2 stripmap ultra-fine mode
 # from Table 2 in Jung et al. (2014)
 RSAT2 = {
+    # orbit
+    'altitude'                   : 798e3,     # m
+    'orbit_inclination'          : 98.6,      # deg
+    'repeat_cycle'               : 14,        # day, 14.29 orbits per day (14 7/24)
+    # sar / antenna
     'carrier_frequency'          : 5.405e9,   # Hz
-    'altitude'                   : 798e3,     # m, mean value
     'antenna_length'             : 6.55,      # m
     'doppler_bandwidth'          : 2308,      # Hz
     'pulse_repetition_frequency' : 3637,      # Hz
     'chirp_bandwidth'            : 78.16e6,   # Hz
     'sampling_frequency'         : 112.68e6,  # Hz
     'azimuth_pixel_size'         : 2.2,       # m
     'ground_range_pixel_size'    : 2.1,       # m
 }
 
+# Radarsat Constellation Mission
+# https://www.asc-csa.gc.ca/eng/satellites/radarsat/technical-features/radarsat-comparison.asp
+RCM = {
+    # orbit
+    'altitude'                   : 600.5e3,   # m, mean value, 586-615 km
+    'orbit_inclination'          : 97.74,     # deg
+    'repeat_cycle'               : 14,        # day, 14.92 orbits per day (14 11/12)
+    # sar / antenna
+    'carrier_frequency'          : 5.405e9,   # Hz
+    'antenna_length'             : 6.75,      # m
+    'antenna_width'              : 1.38,      # m
+}
+
 # GaoFen-3
 # Table 2 & 6 in https://directory.eoportal.org/web/eoportal/satellite-missions/g/gaofen-3
+# https://www.eoportal.org/satellite-missions/gaofen-3
+# Li et al. (2018, RS) at https://doi.org/10.3390/rs10121929
 GF3 = {
-    'carrier_frequency'          : 5.4e9,     # Hz
+    # orbit
     'altitude'                   : 755e3,     # m
+    'orbit_inclination'          : 98.41,     # deg
+    'repeat_cycle'               : 29,        # day
+    # sar / antenna
+    'carrier_frequency'          : 5.4e9,     # Hz
     'antenna_length'             : 15,        # m
+    'antenna_width'              : 1.5,       # m
     'sampling_frequency'         : 533.33e6,  # Hz
 }
 
 # Sentinel-1 Interferometric Wide (IW / TOPS) swath mode
 # Typical value:
 # azfact = azResolution / azPixelSize = 1.46
 # rgfact = rgResolution / rgPixelSize = 1.33
 # reference:
 #   1. Table 2 & Fig. 5d in Jung et al. (2014)
 #   2. Table 3-1 & 7-5 in https://sentinel.esa.int/documents/247904/1877131/Sentinel-1-Product-Definition
 SEN = {
-    'carrier_frequency'          : 5.405e9,   # Hz
+    # orbit
     'altitude'                   : 705e3,     # m, mean value
+    'orbit_inclination'          : 98.18,     # deg
+    'repeat_cycle'               : 12,        # day, single satellite
+    # sar / antenna
+    'carrier_frequency'          : 5.405e9,   # Hz
     'antenna_length'             : 12.3,      # m
     'antenna_width'              : 0.82,      # m
     'doppler_bandwidth'          : 380,       # Hz
     'pulse_repetition_frequency' : 1717.13,   # Hz, based on real data; 1000-3000 (programmable)
     'chirp_bandwidth'            : 56.50e6,   # Hz
     'sampling_frequency'         : 64.35e6,   # Hz
     'azimuth_pixel_size'         : 14.1,      # m, this is the ground azimuth pixel spacing, NOT on orbits!
@@ -331,42 +409,58 @@
 }
 
 
 ##--------------------  L-band  --------------------##
 
 # Seasat
 # from Table 6-1 in Kim and Jordan (2006)
+# https://www.eoportal.org/satellite-missions/seasat
 SEASAT = {
+    # orbit
+    'altitude'                   : 787e3,     # m, mean value, 775-799 km
+    'orbit_inclination'          : 108.0,     # deg
+    'repeat_cycle'               : 17,        # day
+    # sar / antenna
     'carrier_frequency'          : 1.275e9,   # Hz
-    'altitude'                   : 787e3,     # m, mean value
     'antenna_length'             : 10.74,     # m
     'antenna_width'              : 2.16,      # m
     'pulse_repetition_frequency' : 1555,      # Hz, 1463-1647
     'chirp_bandwidth'            : 19e6,      # Hz
 }
 
 # JERS-1
 # from Table 3 in Jung et al. (2014)
+# https://www.eoportal.org/satellite-missions/jers-1
 JERS = {
-    'carrier_frequency'          : 1.275e9,   # Hz
+    # orbit
     'altitude'                   : 568e3,     # m, mean value
+    'orbit_inclination'          : 97.7,      # deg
+    'repeat_cycle'               : 44,        # day
+    # sar / antenna
+    'carrier_frequency'          : 1.275e9,   # Hz
     'antenna_length'             : 11.92,     # m
+    'antenna_width'              : 2.2,       # m
     'doppler_bandwidth'          : 1157,      # Hz
     'pulse_repetition_frequency' : 1600,      # Hz, 1505-1606
     'chirp_bandwidth'            : 15.00e6,   # Hz
     'sampling_frequency'         : 17.10e6,   # Hz
     'azimuth_pixel_size'         : 4.3,       # m
     'ground_range_pixel_size'    : 13.9,      # m
 }
 
 # ALOS PALSAR FBS (fine beam single polarization) mode
 # from Table 3 in Jung et al. (2014)
+# https://www.eorc.jaxa.jp/ALOS/en/alos/a1_about_e.htm
 ALOS = {
-    'carrier_frequency'          : 1.270e9,   # Hz
+    # orbit
     'altitude'                   : 691.65e3,  # m, mean value
+    'orbit_inclination'          : 98.16,     # deg
+    'repeat_cycle'               : 46,        # day, sub cycle: 2 days
+    # sar / antenna
+    'carrier_frequency'          : 1.270e9,   # Hz
     'antenna_length'             : 8.9,       # m
     'doppler_bandwidth'          : 1700,      # Hz
     'pulse_repetition_frequency' : 2160,      # Hz
     'chirp_bandwidth'            : 28.00e6,   # Hz
     'sampling_frequency'         : 32.00e6,   # Hz
     'azimuth_pixel_size'         : 3.5,       # m
     'ground_range_pixel_size'    : 7.4,       # m
@@ -384,16 +478,20 @@
 #                                           sensitive
 #   Bandwidth (MHz)     84          84          42      28      14
 #   Ground reso (m)     3 x 1       3           6       10      100
 #   Swath (km)          25 x 25     50          50      70      350
 #                                            (FP:30)  (FP:30) (5 looks)
 # Notes: FP for full polarization
 ALOS2 = {
-    'carrier_frequency'          : 1.2575e9,  # Hz
+    # orbit
     'altitude'                   : 628e3,     # m, mean value
+    'orbit_inclination'          : 97.9,      # deg
+    'repeat_cycle'               : 14,        # day
+    # sar / antenna
+    'carrier_frequency'          : 1.2575e9,  # Hz
     'antenna_length'             : 9.9,       # m
     'antenna_width'              : 2.9,       # m
     'doppler_bandwidth'          : 1515,      # Hz
     'pulse_repetition_frequency' : 2000,      # Hz
     'chirp_bandwidth'            : 84.0e6,    # Hz
     'sampling_frequency'         : 100.0e6,   # Hz
     'azimuth_pixel_size'         : 3.8,       # m
@@ -401,46 +499,69 @@
     'range_pixel_size' : {
         'stripmap_ultrafine'     : 1.43,      # m
         'stripmap_highsensitive' : 2.86,      # m
         'scansar_normal'         : 8.58,      # m
     }
 }
 
+# ALOS-4 PALSAR-3
+# https://www.eorc.jaxa.jp/ALOS/en/alos-4/a4_about_e.htm
+ALOS4 = {
+    # orbit (same as ALOS-2)
+    'altitude'                   : 628e3,     # m, mean value
+    'orbit_inclination'          : 97.9,      # deg
+    'repeat_cycle'               : 14,        # day, (15-3/14 rev/day)
+}
+
 # SAOCOM-1A/B stripmap
 # from Giudici et al. (2017) and
 # https://directory.eoportal.org/web/eoportal/satellite-missions/s/saocom
+# https://www.eoportal.org/satellite-missions/saocom
 SAOCOM = {
-    'carrrier_frequency'         : 1.27414e9, # Hz
+    # orbit
     'altitude'                   : 619.6e3,   # m, mean value
+    'orbit_inclination'          : 97.86,     # deg
+    'repeat_cycle'               : 16,        # day, single satellite
+    # sar / antenna
+    'carrrier_frequency'         : 1.27414e9, # Hz
     'antenna_length'             : 10,        # m
     'pulse_repetition_frequency' : 4545,      # Hz
     'sampling_frequency'         : 50.0e6,    # Hz
 }
 
 # LuTan-1 (stripmap mode)
+# Table 1 from Liu et al. (2022, EUSAR) at https://ieeexplore.ieee.org/document/9944327
 # preliminary version: the azimuth bandwidth/frequency/pixelsize might change
 LT1 = {
-    'carrier_frequency'          : 1.26e9,    # Hz
+    # orbit
     'altitude'                   : 607e3,     # m, mean value
+    'orbit_inclination'          : 97.8,      # deg
+    'repeat_cycle'               : 8,         # day, single satellite
+    # sar / antenna
+    'carrier_frequency'          : 1.26e9,    # Hz
     'antenna_length'             : 9.8,       # m
     'antenna_width'              : 3.4,       # m
     'doppler_bandwidth'          : 2544,      # Hz
     'pulse_repetition_frequency' : 2934,      # Hz
     'chirp_bandwidth'            : 60.0e6,    # Hz
     'azimuth_pixel_size'         : 2.35,      # m
     'range_pixel_size'           : 1.67,      # m
     'azimuth_resolution'         : 7.15,      # m
     'range_resolution'           : 2.50,      # m
 }
 
 # NISAR
 # https://nisar.jpl.nasa.gov/system/documents/files/26_NISAR_FINAL_9-6-19.pdf
 NISAR_L = {
-    'carrier_frequency'          : 1.257e9,   # Hz
+    # orbit
     'altitude'                   : 747e3,     # m, mean value
+    'orbit_inclination'          : 98.4,      # deg
+    'repeat_cycle'               : 12,        # day
+    # sar / antenna
+    'carrier_frequency'          : 1.257e9,   # Hz
     'antenna_length'             : 12,        # m
     'pulse_repetition_frequency' : 1650,      # Hz
     'chirp_bandwidth'            : 80.0e6,    # Hz
     'range_pixel_size' : {
         '24MHz'                  : 6.25,      # m
         '44MHz'                  : 3.41,      # m
         '80MHz'                  : 1.87,      # m
@@ -454,15 +575,19 @@
     'csk'   : CSK,
     'ksat5' : KSAT5,
     'iceye' : ICEYE,
     # C-band
     'ers'   : ERS,
     'env'   : ENV,
     'sen'   : SEN,
+    'rsat1' : RSAT1,
     'rsat2' : RSAT2,
+    'rcm'   : RCM,
+    'gf3'   : GF3,
     # L-band
     'jers'  : JERS,
     'alos'  : ALOS,
     'alos2' : ALOS2,
+    'alos4' : ALOS4,
     'lt1'   : LT1,
     'ni'    : NISAR_L,
 }
```

### Comparing `mintpy-1.5.3/src/mintpy/objects/stack.py` & `mintpy-1.6.0/src/mintpy/objects/stack.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/objects/stackDict.py` & `mintpy-1.6.0/src/mintpy/objects/stackDict.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/plate_motion.py` & `mintpy-1.6.0/src/mintpy/plate_motion.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/plot_coherence_matrix.py` & `mintpy-1.6.0/src/mintpy/plot_coherence_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,13 +207,12 @@
         self.fig.canvas.draw_idle()
         self.fig.canvas.flush_events()
         return
 
     def update_coherence_matrix(self, event):
         if event.inaxes == self.ax_img:
             if self.fig_coord == 'geo':
-                yx = [self.coord.lalo2yx(event.ydata, coord_type='lat'),
-                      self.coord.lalo2yx(event.xdata, coord_type='lon')]
+                yx = self.coord.lalo2yx(event.ydata, event.xdata)
             else:
                 yx = [int(event.ydata+0.5),
                       int(event.xdata+0.5)]
             self.plot_coherence_matrix4pixel(yx)
```

### Comparing `mintpy-1.5.3/src/mintpy/plot_network.py` & `mintpy-1.6.0/src/mintpy/plot_network.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/plot_transection.py` & `mintpy-1.6.0/src/mintpy/plot_transection.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,15 @@
         """Draw the transect line in the map axes"""
         # erase existing line
         if self.line_ann is not None:
             self.line_ann.remove()
 
         # convert coordinates accordingly
         if 'Y_FIRST' in self.atr.keys():
-            ys = self.coord.yx2lalo([start_yx[0], end_yx[0]], coord_type='y')
-            xs = self.coord.yx2lalo([start_yx[1], end_yx[1]], coord_type='x')
+            ys, xs = self.coord.yx2lalo([start_yx[0], end_yx[0]], [start_yx[1], end_yx[1]])
         else:
             ys = [start_yx[0], end_yx[0]]
             xs = [start_yx[1], end_yx[1]]
 
         # plot
         line = self.ax_img.plot(xs, ys, 'k--', alpha=0)[0]
         self.line_ann = pp.add_arrow(line, position=xs[1])
```

### Comparing `mintpy-1.5.3/src/mintpy/prep_aria.py` & `mintpy-1.6.0/src/mintpy/prep_aria.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_cosicorr.py` & `mintpy-1.6.0/src/mintpy/prep_cosicorr.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_fringe.py` & `mintpy-1.6.0/src/mintpy/prep_fringe.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_gamma.py` & `mintpy-1.6.0/src/mintpy/prep_gamma.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_gmtsar.py` & `mintpy-1.6.0/src/mintpy/prep_gmtsar.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_hyp3.py` & `mintpy-1.6.0/src/mintpy/prep_hyp3.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,22 +33,28 @@
     meta_file = os.path.join(os.path.dirname(fname), f'{job_id}.txt')
     hyp3_meta = {}
     with open(meta_file) as f:
         for line in f:
             key, value = line.strip().replace(' ','').split(':')[:2]
             hyp3_meta[key] = value
 
-    # get date1/2 objects
+    # get product type and the correponding insar processor
     if job_id.split('_')[2].startswith('IW'):
         # burst-wide product using ISCE2
+        prod_type = 'isce2_burst'
+    else:
+        # scene-wide product using Gamma
+        prod_type = 'gamma_scene'
+
+    # get date1/2 objects
+    if prod_type == 'isce2_burst':
         date1_str, date2_str = job_id.split('_')[3:5]
         date1 = dt.datetime.strptime(f'{date1_str}','%Y%m%d')
         date2 = dt.datetime.strptime(f'{date2_str}','%Y%m%d')
     else:
-        # scene-wide product using Gamma
         date1_str, date2_str = job_id.split('_')[1:3]
         date1 = dt.datetime.strptime(date1_str,'%Y%m%dT%H%M%S')
         date2 = dt.datetime.strptime(date2_str,'%Y%m%dT%H%M%S')
 
     # add universal hyp3 metadata
     meta['PROCESSOR'] = 'hyp3'
     meta['CENTER_LINE_UTC'] = hyp3_meta['UTCtime']
@@ -63,18 +69,14 @@
     # add LAT/LON_REF1/2/3/4 based on whether satellite ascending or descending
     meta['ORBIT_DIRECTION'] = 'ASCENDING' if abs(meta['HEADING']) < 90 else 'DESCENDING'
     N = float(meta['Y_FIRST'])
     W = float(meta['X_FIRST'])
     S = N + float(meta['Y_STEP']) * int(meta['LENGTH'])
     E = W + float(meta['X_STEP']) * int(meta['WIDTH'])
 
-    # convert UTM to lat/lon
-    N, W = ut.utm2latlon(meta, W, N)
-    S, E = ut.utm2latlon(meta, E, S)
-
     if meta['ORBIT_DIRECTION'] == 'ASCENDING':
         meta['LAT_REF1'] = str(S)
         meta['LAT_REF2'] = str(S)
         meta['LAT_REF3'] = str(N)
         meta['LAT_REF4'] = str(N)
         meta['LON_REF1'] = str(W)
         meta['LON_REF2'] = str(E)
@@ -106,15 +108,45 @@
 
     # add metadata that is only relevant to interferogram files
     if is_ifg:
         meta['DATE12'] = f'{date1.strftime("%y%m%d")}-{date2.strftime("%y%m%d")}'
         meta['P_BASELINE_TOP_HDR'] = hyp3_meta['Baseline']
         meta['P_BASELINE_BOTTOM_HDR'] = hyp3_meta['Baseline']
 
-    return(meta)
+    # HDF-EOS5 metadata
+    ref_granule = hyp3_meta['ReferenceGranule']
+    if ref_granule.startswith('S1'):
+        # beam_mode
+        meta['beam_mode'] = 'IW'
+
+        # beam_swath
+        if prod_type == 'isce2_burst':
+            meta['beam_swath'] = job_id.split('_')[2][2:]
+        else:
+            meta['beam_swath'] = '123'
+
+        # relative_orbit
+        if ref_granule.startswith('S1A'):
+            meta['relative_orbit'] = ((int(hyp3_meta['ReferenceOrbitNumber']) - 73) % 175) + 1
+        elif ref_granule.startswith('S1B'):
+            meta['relative_orbit'] = ((int(hyp3_meta['ReferenceOrbitNumber']) - 202) % 175) + 1
+        else:
+            raise ValueError('Un-recognized Sentinel-1 satellite from {ref_granule}!')
+
+    # first/last_frame [from start/stopUTC]
+    # NOTE by Yunjun, Apr 2024: ascending node time is needed to calculate the first/last frame
+    # based on the start/end UTC time.
+    t0, t1 = ref_granule.split('_')[-5:-3]
+    meta['startUTC'] = dt.datetime.strptime(t0, '%Y%m%dT%H%M%S').strftime('%Y-%m-%d %H:%M:%S.%f')
+    meta['stopUTC']  = dt.datetime.strptime(t1, '%Y%m%dT%H%M%S').strftime('%Y-%m-%d %H:%M:%S.%f')
+
+    # unwrap_method
+    meta['unwrap_method'] = hyp3_meta['Unwrappingtype']
+
+    return meta
 
 
 #########################################################################
 def prep_hyp3(inps):
     """Prepare ASF HyP3 metadata files"""
 
     inps.file = ut.get_file_list(inps.file, abspath=True)
```

### Comparing `mintpy-1.5.3/src/mintpy/prep_isce.py` & `mintpy-1.6.0/src/mintpy/prep_isce.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/prep_nisar.py` & `mintpy-1.6.0/src/mintpy/prep_nisar.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from osgeo import gdal
 from pyproj.transformer import Transformer
 from scipy.interpolate import RegularGridInterpolator
 
 from mintpy.constants import EARTH_RADIUS, SPEED_OF_LIGHT
 from mintpy.utils import ptime, writefile
 
-DATASET_ROOT_UNW = '/science/LSAR/GUNW/grids/frequencyA/interferogram/unwrapped'
+DATASET_ROOT_UNW = '/science/LSAR/GUNW/grids/frequencyA/unwrappedInterferogram'
+PARAMETERS = '/science/LSAR/GUNW/metadata/processingInformation/parameters/unwrappedInterferogram/frequencyA'
 IDENTIFICATION = '/science/LSAR/identification'
 RADARGRID_ROOT = 'science/LSAR/GUNW/metadata/radarGrid'
 DATASETS = {
-    'xcoord'           : f"{DATASET_ROOT_UNW}/xCoordinates",
-    'ycoord'           : f"{DATASET_ROOT_UNW}/yCoordinates",
+    'xcoord'           : f"{DATASET_ROOT_UNW}/POL/xCoordinates",
+    'ycoord'           : f"{DATASET_ROOT_UNW}/POL/yCoordinates",
     'unw'              : f"{DATASET_ROOT_UNW}/POL/unwrappedPhase",
     'cor'              : f"{DATASET_ROOT_UNW}/POL/coherenceMagnitude",
     'connComp'         : f"{DATASET_ROOT_UNW}/POL/connectedComponents",
-    'layoverShadowMask': f"{DATASET_ROOT_UNW}/layoverShadowMask",
-    'waterMask'        : f"{DATASET_ROOT_UNW}/waterMask",
+    #'mask'             : f"{DATASET_ROOT_UNW}/mask",
     'epsg'             : f"{DATASET_ROOT_UNW}/projection",
     'xSpacing'         : f"{DATASET_ROOT_UNW}/xCoordinateSpacing",
     'ySpacing'         : f"{DATASET_ROOT_UNW}/yCoordinateSpacing",
-    'polarization'     : f"{DATASET_ROOT_UNW}/listOfPolarizations",
-    'range_look'       : f"{DATASET_ROOT_UNW}/numberOfRangeLooks",
-    'azimuth_look'     : f"{DATASET_ROOT_UNW}/numberOfAzimuthLooks",
+    'polarization'     : "/science/LSAR/GUNW/grids/frequencyA/listOfPolarizations",
+    'range_look'       : f"{PARAMETERS}/numberOfRangeLooks",
+    'azimuth_look'     : f"{PARAMETERS}/numberOfAzimuthLooks",
 }
 PROCESSINFO = {
     'centerFrequency': "/science/LSAR/GUNW/grids/frequencyA/centerFrequency",
     'orbit_direction': f"{IDENTIFICATION}/orbitPassDirection",
     'platform'       : f"{IDENTIFICATION}/missionId",
     'start_time'     : f"{IDENTIFICATION}/referenceZeroDopplerStartTime",
     'end_time'       : f"{IDENTIFICATION}/referenceZeroDopplerEndTime",
@@ -57,17 +57,17 @@
 
     print(f'update mode: {inps.update_mode}')
 
     input_files = sorted(glob.glob(inps.input_glob))
     print(f"Found {len(input_files)} unwrapped files")
 
     if inps.subset_lat:
-        bbox = (inps.subset_lat[0], inps.subset_lon[0], inps.subset_lat[1], inps.subset_lon[1])
+        bbox = (inps.subset_lon[0], inps.subset_lat[0], inps.subset_lon[1], inps.subset_lat[1])
     else:
-        bbox=None
+        bbox = None
 
     # extract metadata
     metadata, bounds = extract_metadata(input_files, bbox)
 
     # output filename
     stack_file = os.path.join(inps.out_dir, "inputs/ifgramStack.h5")
     geometry_file = os.path.join(inps.out_dir, "inputs/geometryGeo.h5")
@@ -76,15 +76,16 @@
     date12_list = _get_date_pairs(input_files)
 
     metadata = prepare_geometry(
         outfile=geometry_file,
         metaFile=input_files[0],
         bbox=bounds,
         metadata=metadata,
-        demFile=inps.dem_file
+        demFile=inps.dem_file,
+        maskFile=inps.mask_file
         )
 
     prepare_stack(
         outfile=stack_file,
         inp_files=input_files,
         metadata=metadata,
         bbox=bounds,
@@ -132,15 +133,23 @@
             t_mid - datetime.datetime(t_mid.year, t_mid.month, t_mid.day)
     ).total_seconds()
 
     meta["X_FIRST"] = x_origin - pixel_width//2
     meta["Y_FIRST"] = y_origin - pixel_height//2
     meta["X_STEP"] = pixel_width
     meta["Y_STEP"] = pixel_height
-    meta["X_UNIT"] = meta["Y_UNIT"] = "meters"
+
+    if meta["EPSG"] == 4326:
+        meta["X_UNIT"] = meta["Y_UNIT"] = 'degree'
+    else:
+        meta["X_UNIT"] = meta["Y_UNIT"] = "meters"
+        if str(meta["EPSG"]).startswith('326'):
+             meta["UTM_ZONE"] = str(meta["EPSG"])[3:] + 'N'
+        else:
+             meta["UTM_ZONE"] = str(meta["EPSG"])[3:] + 'S'
     meta["EARTH_RADIUS"] = EARTH_RADIUS
 
     # NISAR Altitude
     meta['HEIGHT'] = 747000
 
     # Range and Azimuth pixel size need revision, values are just to fill in
     meta["RANGE_PIXEL_SIZE"] = abs(pixel_width)
@@ -151,15 +160,14 @@
         # assuming bbox is in lat/lon coordinates
         epsg_src = 4326
         utm_bbox = bbox_to_utm(bbox, meta["EPSG"], epsg_src)
     else:
         utm_bbox = None
     bounds = common_raster_bound(input_files, utm_bbox)
     meta['bbox'] = ",".join([str(b) for b in bounds])
-
     col1, row1, col2, row2 = get_rows_cols(xcoord, ycoord, bounds)
     length = row2 - row1
     width = col2 - col1
     meta['LENGTH'] = length
     meta['WIDTH'] = width
 
     return meta, bounds
@@ -220,34 +228,33 @@
     dataset = {}
     with h5py.File(inp_file, 'r') as ds:
         xcoord = ds[DATASETS['xcoord']][:]
         ycoord = ds[DATASETS['ycoord']][:]
         col1, row1, col2, row2 = get_rows_cols(xcoord, ycoord, bbox)
 
         if geometry:
-            # Set all values to 1 temporarily because water mask is zero
-            dataset['water_mask'] = ds[DATASETS['waterMask']][row1:row2, col1:col2] * 0 + 1
-            dataset['layover_shadow_mask'] = ds[DATASETS['layoverShadowMask']][row1:row2, col1:col2]
+            # dataset['mask'] = ds[DATASETS['mask']][row1:row2, col1:col2]
             dataset['xybbox'] = (col1, row1, col2, row2)
         else:
             dataset['unw_data'] = ds[DATASETS['unw']][row1:row2, col1:col2]
             dataset['cor_data'] = ds[DATASETS['cor']][row1:row2, col1:col2]
             dataset['conn_comp'] = (ds[DATASETS['connComp']][row1:row2, col1:col2]).astype(np.float32)
             dataset['conn_comp'][dataset['conn_comp'] > 254] = np.nan
             dataset['pbase'] = np.nanmean(ds[PROCESSINFO['bperp']][()])
     return dataset
 
 
-def read_and_interpolate_geometry(gunw_file, dem_file, xybbox):
-    """Read the DEM, change projection and interpolate to data grid, interpolate slant range and incidence angle to data grid"""
-    dataset = gdal.Open(dem_file, gdal.GA_ReadOnly)
-    geotransform = dataset.GetGeoTransform()
-    proj = gdal.osr.SpatialReference(wkt=dataset.GetProjection())
-    src_epsg = int(proj.GetAttrValue('AUTHORITY', 1))
-    raster_array = dataset.ReadAsArray()
+def read_and_interpolate_geometry(gunw_file, dem_file, xybbox, mask_file=None):
+    """Read the DEM and mask, change projection and interpolate to data grid,
+       interpolate slant range and incidence angle to data grid"""
+    dem_dataset = gdal.Open(dem_file, gdal.GA_ReadOnly)
+    proj = gdal.osr.SpatialReference(wkt=dem_dataset.GetProjection())
+    dem_src_epsg = int(proj.GetAttrValue('AUTHORITY', 1))
+    del dem_dataset
+
     rdr_coords = {}
 
     with h5py.File(gunw_file, 'r') as ds:
         dst_epsg = ds[DATASETS['epsg']][()]
         xcoord = ds[DATASETS['xcoord']][xybbox[0]:xybbox[2]]
         ycoord = ds[DATASETS['ycoord']][xybbox[1]:xybbox[3]]
 
@@ -256,31 +263,58 @@
         rdr_coords['height_radar_grid'] = ds[PROCESSINFO['rdr_height']][()]
         rdr_coords['slant_range'] = ds[PROCESSINFO['rdr_slant_range']][()]
         rdr_coords['perp_baseline'] = ds[PROCESSINFO['bperp']][()]
         rdr_coords['incidence_angle'] = ds[PROCESSINFO['rdr_incidence']][()]
 
     subset_rows = len(ycoord)
     subset_cols = len(xcoord)
-    # dem_subset_array = np.zeros((subset_rows, subset_cols), dtype=raster_array.dtype)
+
     Y_2d, X_2d = np.meshgrid(ycoord, xcoord, indexing='ij')
+    bounds = (min(xcoord), min(ycoord), max(xcoord), max(ycoord))
+    output_projection = f"EPSG:{dst_epsg}"
 
-    if not src_epsg == dst_epsg:
-        coord_transform = Transformer.from_crs(dst_epsg, src_epsg, always_xy=True)
-        x_dem, y_dem = coord_transform.transform(X_2d.flatten(), Y_2d.flatten())
+    # Warp DEM to the interferograms grid
+    input_projection = f"EPSG:{dem_src_epsg}"
+    output_dem = os.path.join(os.path.dirname(dem_file), 'dem_transformed.tif' )
+    gdal.Warp(output_dem, dem_file, outputBounds=bounds, format='GTiff',
+              srcSRS=input_projection, dstSRS=output_projection, resampleAlg=gdal.GRA_Bilinear,
+              width=subset_cols, height=subset_rows,
+              options=['COMPRESS=DEFLATE'])
+
+    dem_subset_array =  gdal.Open(output_dem, gdal.GA_ReadOnly).ReadAsArray()
+
+    # Interpolate slant_range and incidence_angle
+    slant_range, incidence_angle = interpolate_geometry(X_2d, Y_2d, dem_subset_array, rdr_coords)
+
+    # Read and warp mask if necessary
+    if mask_file in ['auto', 'None', None]:
+        print('*** No mask was found ***')
+        mask_subset_array = np.ones(dem_subset_array.shape, dtype='byte')
     else:
-        x_dem, y_dem = X_2d.flatten(), Y_2d.flatten()
+        try:
+            mask_dataset = gdal.Open(mask_file, gdal.GA_ReadOnly)
+            proj = gdal.osr.SpatialReference(wkt=mask_dataset.GetProjection())
+            mask_src_epsg = int(proj.GetAttrValue('AUTHORITY', 1))
+            del mask_dataset
+
+            # Warp mask to the interferograms grid
+            input_projection = f"EPSG:{mask_src_epsg}"
+            output_mask = os.path.join(os.path.dirname(mask_file), 'mask_transformed.tif' )
+            gdal.Warp(output_mask, mask_file, outputBounds=bounds, format='GTiff',
+              srcSRS=input_projection, dstSRS=output_projection, resampleAlg=gdal.GRA_Byte,
+              width=subset_cols, height=subset_rows,
+              options=['COMPRESS=DEFLATE'])
 
-    cols = ((y_dem - geotransform[3]) / geotransform[5]).astype(int)
-    rows = ((x_dem - geotransform[0]) / geotransform[1]).astype(int)
+            mask_subset_array = gdal.Open(output_mask, gdal.GA_ReadOnly).ReadAsArray()
 
-    dem_subset_array = raster_array[cols.reshape(subset_rows, subset_cols), rows.reshape(subset_rows, subset_cols)]
+        except:
+            raise OSError('*** Mask is not gdal readable ***')
 
-    slant_range, incidence_angle = interpolate_geometry(X_2d, Y_2d, dem_subset_array, rdr_coords)
 
-    return dem_subset_array, slant_range, incidence_angle
+    return dem_subset_array, slant_range, incidence_angle, mask_subset_array
 
 
 def interpolate_geometry(X_2d, Y_2d, dem, rdr_coords):
     """Interpolate slant range and incidence angle"""
     pnts = np.stack((dem.flatten(), Y_2d.flatten(), X_2d.flatten()), axis=-1)
     length, width = Y_2d.shape
 
@@ -311,36 +345,40 @@
 
 
 def prepare_geometry(
         outfile,
         metaFile,
         metadata,
         bbox,
-        demFile
+        demFile,
+        maskFile
 ):
     """Prepare the geometry file."""
     print("-" * 50)
     print(f"preparing geometry file: {outfile}")
 
     # copy metadata to meta
     meta = {key: value for key, value in metadata.items()}
 
     # Read waterMask, LayoverShadowMask, xybbox:
     geo_ds = read_subset(metaFile, bbox, geometry=True)
-    dem_subset_array, slant_range, incidence_angle = read_and_interpolate_geometry(metaFile, demFile, geo_ds['xybbox'])
+    dem_subset_array, slant_range, incidence_angle, mask = read_and_interpolate_geometry(metaFile, demFile,
+                                                                                   geo_ds['xybbox'], mask_file=maskFile)
 
     length, width = dem_subset_array.shape
 
     ds_name_dict = {
         "height": [np.float32, (length, width), dem_subset_array],
         "incidenceAngle": [np.float32, (length, width), incidence_angle],
         "slantRangeDistance": [np.float32, (length, width), slant_range],
-        "shadowMask": [np.bool_, (length, width), geo_ds['layover_shadow_mask']],
-        "waterMask": [np.bool_, (length, width), geo_ds['water_mask']],
+        #"shadowMask": [np.bool_, (length, width), geo_ds['mask']],
+        #"waterMask": [np.bool_, (length, width), geo_ds['water_mask']],
     }
+    if maskFile:
+        ds_name_dict['waterMask'] = [np.bool_, (length, width), mask]
 
     # initiate HDF5 file
     meta["FILE_TYPE"] = "geometry"
     meta['STARTING_RANGE'] = np.nanmin(slant_range)
     writefile.layout_hdf5(outfile, ds_name_dict, metadata=meta)
 
     return meta
```

### Comparing `mintpy-1.5.3/src/mintpy/prep_roipac.py` & `mintpy-1.6.0/src/mintpy/prep_roipac.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/reference_date.py` & `mintpy-1.6.0/src/mintpy/reference_date.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/reference_point.py` & `mintpy-1.6.0/src/mintpy/reference_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,16 +167,15 @@
 
 def reference_point_attribute(atr, y, x):
     atrNew = dict()
     atrNew['REF_Y'] = str(y)
     atrNew['REF_X'] = str(x)
     coord = ut.coordinate(atr)
     if 'X_FIRST' in atr.keys():
-        atrNew['REF_LAT'] = str(coord.yx2lalo(y, coord_type='y'))
-        atrNew['REF_LON'] = str(coord.yx2lalo(x, coord_type='x'))
+        atrNew['REF_LAT'], atrNew['REF_LON'] = (str(val) for val in coord.yx2lalo(y, x))
     return atrNew
 
 
 ###############################################################
 def manual_select_reference_yx(data, inps, mask=None):
     """Manually select reference point in row/column number.
     Parameters: data : 2D np.ndarray, stack of input file
```

### Comparing `mintpy-1.5.3/src/mintpy/s1ab_range_bias.py` & `mintpy-1.6.0/src/mintpy/s1ab_range_bias.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_gbis.py` & `mintpy-1.6.0/src/mintpy/save_gbis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_gdal.py` & `mintpy-1.6.0/src/mintpy/save_gdal.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_gmt.py` & `mintpy-1.6.0/src/mintpy/save_gmt.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_hdfeos5.py` & `mintpy-1.6.0/src/mintpy/save_hdfeos5.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,28 +111,32 @@
 
     # Grabbed by script
     # date info
     unavco_meta['first_date'] = dt.datetime.strptime(dateList[0], '%Y%m%d').isoformat()[0:10]
     unavco_meta['last_date'] = dt.datetime.strptime(dateList[-1], '%Y%m%d').isoformat()[0:10]
 
     # footprint
-    lons = [meta['LON_REF1'],
-            meta['LON_REF3'],
-            meta['LON_REF4'],
-            meta['LON_REF2'],
-            meta['LON_REF1']]
-
-    lats = [meta['LAT_REF1'],
-            meta['LAT_REF3'],
-            meta['LAT_REF4'],
-            meta['LAT_REF2'],
-            meta['LAT_REF1']]
+    lons = [float(meta['LON_REF1']),
+            float(meta['LON_REF3']),
+            float(meta['LON_REF4']),
+            float(meta['LON_REF2']),
+            float(meta['LON_REF1'])]
+
+    lats = [float(meta['LAT_REF1']),
+            float(meta['LAT_REF3']),
+            float(meta['LAT_REF4']),
+            float(meta['LAT_REF2']),
+            float(meta['LAT_REF1'])]
+
+    # convert UTM to lat/lon
+    if not meta_in.get('Y_UNIT', 'degrees').lower().startswith('deg'):
+        lats, lons = ut.utm2latlon(meta_in, easting=lons, northing=lats)
 
     unavco_meta['scene_footprint'] = "POLYGON((" + ",".join(
-        [lon+' '+lat for lon, lat in zip(lons, lats)]) + "))"
+        [f'{lon} {lat}' for lon, lat in zip(lons, lats)]) + "))"
 
     unavco_meta['history'] = dt.datetime.utcnow().isoformat()[0:10]
 
     #################################
     # Recommended metadata
     #################################
     unavco_meta['first_frame'] = int(meta.get('first_frame', 0))
@@ -235,14 +239,18 @@
     if subset_mode:
         print('Subset mode is enabled, put subset range info in output filename.')
         lat1 = float(metadata['Y_FIRST'])
         lon0 = float(metadata['X_FIRST'])
         lat0 = lat1 + float(metadata['Y_STEP']) * int(metadata['LENGTH'])
         lon1 = lon0 + float(metadata['X_STEP']) * int(metadata['WIDTH'])
 
+        # convert UTM to lat/lon
+        if not metadata.get('Y_UNIT', 'degrees').lower().startswith('deg'):
+            [lat0, lat1], [lon0, lon1] = ut.utm2latlon(metadata, easting=[lon0, lon1], northing=[lat0, lat1])
+
         lat0Str = f'N{round(lat0*1e3):05d}'
         lat1Str = f'N{round(lat1*1e3):05d}'
         lon0Str = f'E{round(lon0*1e3):06d}'
         lon1Str = f'E{round(lon1*1e3):06d}'
         if lat0 < 0.0: lat0Str = f'S{round(abs(lat0)*1e3):05d}'
         if lat1 < 0.0: lat1Str = f'S{round(abs(lat1)*1e3):05d}'
         if lon0 < 0.0: lon0Str = f'W{round(abs(lon0)*1e3):06d}'
```

### Comparing `mintpy-1.5.3/src/mintpy/save_kite.py` & `mintpy-1.6.0/src/mintpy/save_kite.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_kmz.py` & `mintpy-1.6.0/src/mintpy/save_kmz.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
     width = int(meta['WIDTH'])
     length = int(meta['LENGTH'])
     ax.set_xlim([0, width])
     ax.set_ylim([length, 0])
 
     out_file_base = os.path.splitext(out_file)[0]
-    data_png_file = out_file_base + '.png'
+    data_png_file = out_file_base + '_data.png'
     print(f'writing {data_png_file} with dpi={inps.fig_dpi}')
     plt.savefig(data_png_file, pad_inches=0.0, transparent=True, dpi=inps.fig_dpi)
 
     # 2. Generate KML file
     kml_doc = KML.Document()
 
     # Add data png file
```

### Comparing `mintpy-1.5.3/src/mintpy/save_kmz_timeseries.py` & `mintpy-1.6.0/src/mintpy/save_kmz_timeseries.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_qgis.py` & `mintpy-1.6.0/src/mintpy/save_qgis.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/save_roipac.py` & `mintpy-1.6.0/src/mintpy/save_roipac.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/simulation/decorrelation.py` & `mintpy-1.6.0/src/mintpy/simulation/decorrelation.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/simulation/defo_model.py` & `mintpy-1.6.0/src/mintpy/simulation/defo_model.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/simulation/fractal.py` & `mintpy-1.6.0/src/mintpy/simulation/fractal.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/simulation/iono.py` & `mintpy-1.6.0/src/mintpy/simulation/iono.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     return inc_angle_iono
 
 
 def lalo_ground2iono(lat, lon, inc_angle, az_angle=None, head_angle=None, iono_height=450e3, method='spherical_distance'):
     """Calculate lat/lon of IPP with the given lat/lon on the ground and LOS geometry
 
-    Equation (12) in Yunjun et al. (2021, TGRS).
+    Equation (12) in Yunjun et al. (2022, TGRS).
 
     Parameters: lat/lon      - float, latitude/longitude of the point on the ground in degrees
                 inc_angle    - float/np.ndarray, incidence angle of the line-of-sight vector on the ground in degrees
                 az_angle     - float/np.ndarray, azimuth   angle of the line-of-sight vector
                 head_angle   - float, heading angle of the satellite orbit in degrees
                                from the north direction with positive in clockwise direction
                 iono_height  - float, height of the ionosphere thin-shell in meters
```

### Comparing `mintpy-1.5.3/src/mintpy/simulation/simulation.py` & `mintpy-1.6.0/src/mintpy/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/simulation/variance.py` & `mintpy-1.6.0/src/mintpy/simulation/variance.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/smallbaselineApp.py` & `mintpy-1.6.0/src/mintpy/smallbaselineApp.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,19 +456,22 @@
         Returns:    steps    : dict of dicts, input/output filenames for each step
         """
         work_dir = os.path.abspath(work_dir)
         fname0 = os.path.join(work_dir, 'timeseries.h5')
         fname1 = os.path.join(work_dir, 'timeseries.h5')
         atr = readfile.read_attribute(fname0)
 
-        phase_correction_steps = ['correct_LOD',
-                                  'correct_SET',
-                                  'correct_troposphere',
-                                  'deramp',
-                                  'correct_topography']
+        phase_correction_steps = [
+            'correct_LOD',
+            'correct_SET',
+            'correct_ionosphere',
+            'correct_troposphere',
+            'deramp',
+            'correct_topography',
+        ]
 
         # loop for all steps
         steps = dict()
         for sname in phase_correction_steps:
             # fname0 == fname1 if no valid correction method is set.
             fname0 = fname1
             if sname == 'correct_LOD':
@@ -476,14 +479,23 @@
                     fname1 = f'{os.path.splitext(fname0)[0]}_LOD.h5'
 
             elif sname == 'correct_SET':
                 method = template['mintpy.solidEarthTides']
                 if method:
                     fname1 = f'{os.path.splitext(fname0)[0]}_SET.h5'
 
+            elif sname == 'correct_ionosphere':
+                method = template['mintpy.ionosphericDelay.method']
+                if method:
+                    if method == 'split_spectrum':
+                        fname1 = f'{os.path.splitext(fname0)[0]}_ion.h5'
+                    else:
+                        msg = f'un-recognized ionospheric correction method: {method}'
+                        raise ValueError(msg)
+
             elif sname == 'correct_troposphere':
                 method = template['mintpy.troposphericDelay.method']
                 model  = template['mintpy.troposphericDelay.weatherModel']
                 if method:
                     if method == 'height_correlation':
                         fname1 = f'{os.path.splitext(fname0)[0]}_tropHgt.h5'
 
@@ -575,14 +587,36 @@
             if ut.run_or_skip(out_file=out_file, in_file=in_file) == 'run':
                 import mintpy.cli.solid_earth_tides
                 mintpy.cli.solid_earth_tides.main(iargs)
         else:
             print('No solid Earth tides correction.')
 
 
+    def run_ionospheric_delay_correction(self, step_name):
+        """Correct ionospheric delays."""
+        iono_stack_file = ut.check_loaded_dataset(self.workDir, print_msg=False)[3]
+
+        fnames = self.get_timeseries_filename(self.template, self.workDir)[step_name]
+        in_file = fnames['input']
+        out_file = fnames['output']
+        if in_file != out_file:
+            method = self.template['mintpy.ionosphericDelay.method']
+
+            # range split spectrum (Fattahi et al., 2017; Liang et al. 2018; 2019)
+            if method == 'split_spectrum':
+                print(f'ionospheric delay correction with {method} approach')
+                iargs = ['-t', self.templateFile, '-f', in_file, '-o', out_file,
+                         '--iono-stack-file', iono_stack_file]
+                print('\niono_split_spectrum.py', ' '.join(iargs))
+                import mintpy.cli.iono_split_spectrum
+                mintpy.cli.iono_split_spectrum.main(iargs)
+        else:
+            print('No ionospheric delay correction.')
+
+
     def run_tropospheric_delay_correction(self, step_name):
         """Correct tropospheric delays."""
         geom_file = ut.check_loaded_dataset(self.workDir, print_msg=False)[1]
         mask_file = os.path.join(self.workDir, 'maskTempCoh.h5')
 
         fnames = self.get_timeseries_filename(self.template, self.workDir)[step_name]
         in_file = fnames['input']
@@ -890,14 +924,17 @@
 
             elif sname == 'correct_LOD':
                 self.run_local_oscillator_drift_correction(sname)
 
             elif sname == 'correct_SET':
                 self.run_solid_earth_tides_correction(sname)
 
+            elif sname == 'correct_ionosphere':
+                self.run_ionospheric_delay_correction(sname)
+
             elif sname == 'correct_troposphere':
                 self.run_tropospheric_delay_correction(sname)
 
             elif sname == 'deramp':
                 self.run_phase_deramping(sname)
 
             elif sname == 'correct_topography':
@@ -992,14 +1029,15 @@
             # all the other files
             [f'velocity{tropo_model}.h5', '--mask', 'no'],
             ['numInvIfgram.h5',           '--mask', 'no'],
         ]
 
         if ion_file:
             iargs_list0 += [
+                [ion_file, 'unwrapPhase-', '--zero-mask', '--wrap', '-c', 'cmy'],
                 [ion_file, 'unwrapPhase-', '--zero-mask'],
                 [ion_file, 'coherence-',   '--mask', 'no', '-v', '0', '1'],
             ]
 
         # translate element list whose file path has *
         iargs_list = []
         for iargs in iargs_list0:
```

### Comparing `mintpy-1.5.3/src/mintpy/solid_earth_tides.py` & `mintpy-1.6.0/src/mintpy/solid_earth_tides.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/spatial_filter.py` & `mintpy-1.6.0/src/mintpy/spatial_filter.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/subset.py` & `mintpy-1.6.0/src/mintpy/subset.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,22 +180,22 @@
     # Data Coverage
     width = int(float(meta_dict['WIDTH']))
     length = int(float(meta_dict['LENGTH']))
 
     # Use subset_lat/lon input if existed,  priority: lat/lon > y/x > len/wid
     coord = ut.coordinate(meta_dict)
     if subset_dict.get('subset_lat', None):
-        sub_y = coord.lalo2yx(subset_dict['subset_lat'], coord_type='latitude')
+        sub_y = coord.lalo2yx(subset_dict['subset_lat'], None)[0]
     elif subset_dict['subset_y']:
         sub_y = subset_dict['subset_y']
     else:
         sub_y = [0, length]
 
     if subset_dict.get('subset_lon', None):
-        sub_x = coord.lalo2yx(subset_dict['subset_lon'], coord_type='longitude')
+        sub_x = coord.lalo2yx(None, subset_dict['subset_lon'])[1]
     elif subset_dict['subset_x']:
         sub_x = subset_dict['subset_x']
     else:
         sub_x = [0, width]
 
     # Get subset box in y/x
     sub_x = sorted(sub_x)
```

### Comparing `mintpy-1.5.3/src/mintpy/timeseries2velocity.py` & `mintpy-1.6.0/src/mintpy/timeseries2velocity.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/timeseries_rms.py` & `mintpy-1.6.0/src/mintpy/timeseries_rms.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/tropo_gacos.py` & `mintpy-1.6.0/src/mintpy/tropo_gacos.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/tropo_phase_elevation.py` & `mintpy-1.6.0/src/mintpy/tropo_phase_elevation.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/tropo_pyaps3.py` & `mintpy-1.6.0/src/mintpy/tropo_pyaps3.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ############################################################
 # Program is part of MintPy                                #
 # Copyright (c) 2013, Zhang Yunjun, Heresh Fattahi         #
 # Author: Zhang Yunjun, Heresh Fattahi, 2015               #
 ############################################################
 
 
+import glob
 import os
 import re
 from configparser import ConfigParser
 
 import h5py
 import numpy as np
 import pyaps3 as pa
@@ -83,14 +84,64 @@
 def get_grib_info(inps):
     """Read the following info from inps
         inps.grib_dir
         inps.atr
         inps.snwe
         inps.grib_files
     """
+    # utils sub-functions
+    def snwe_str2num(snwe_str):
+        snwe = snwe_str.split('_')
+        snwe = [x.replace('S','-').replace('N','').replace('W','-').replace('E','') for x in snwe]
+        snwe = [int(x) for x in snwe]
+        return snwe
+
+    def snwe1_contains_snwe2(snwe1, snwe2):
+        s1, n1, w1, e1 = snwe1
+        s2, n2, w2, e2 = snwe2
+        if s1 <= s2 and n1 >= n2 and w1 <= w2 and e1 >= e2:
+            return True
+        else:
+            return False
+
+    def get_larger_snwe_in_local_files(gfile):
+        # default output
+        larger_snwe = None
+
+        # 0. input grib file info
+        gdir = os.path.dirname(gfile)
+        gparts = os.path.basename(gfile).split('_')
+        # ignore grib files in global scale
+        if len(gparts) < 7:
+            return larger_snwe
+        snwe_str = '_'.join(gparts[1:5])
+        snwe = snwe_str2num(snwe_str)
+        suffix = os.path.basename(gfile).split(snwe_str)[1]
+
+        # 1. find candidate snwe in local files
+        cand_gfiles = glob.glob(os.path.join(gdir, f'*{suffix}'))
+        # ignore grib files in global scale
+        cand_gfiles = [x for x in cand_gfiles if len(os.path.basename(x).split('_')) >= 7]
+        if len(cand_gfiles) > 0:
+            cand_snwe_str_list = ['_'.join(os.path.basename(x).split('_')[1:5]) for x in cand_gfiles]
+            cand_snwe_list = [snwe_str2num(x) for x in cand_snwe_str_list]
+
+            # 2. find candidate snwe that contains the input snwe, i.e. larger_snwe
+            larger_snwe_list = []
+            for cand_snwe in cand_snwe_list:
+                if snwe1_contains_snwe2(cand_snwe, snwe):
+                    larger_snwe_list.append(cand_snwe)
+
+            # 3. locate the larger_snwe with the most existing files
+            if len(larger_snwe_list) > 0:
+                num_file_list = [len(glob.glob(os.path.join(gdir, f'*{x}*{suffix}'))) for x in larger_snwe_list]
+                larger_snwe = larger_snwe_list[np.argmax(num_file_list)]
+
+        return larger_snwe
+
     # grib data directory, under weather_dir
     inps.grib_dir = os.path.join(inps.weather_dir, inps.tropo_model)
     if not os.path.isdir(inps.grib_dir):
         os.makedirs(inps.grib_dir)
         print(f'make directory: {inps.grib_dir}')
 
     # read metadata
@@ -98,40 +149,68 @@
         inps.atr = readfile.read_attribute(inps.dis_file)
     elif inps.geom_file:
         inps.atr = readfile.read_attribute(inps.geom_file)
     else:
         inps.atr = dict()
 
     # area extent for ERA5 grib data download
-    if inps.atr:
-        inps.snwe = get_snwe(inps.atr, geom_file=inps.geom_file)
-    else:
-        inps.snwe = None
+    inps.snwe = get_snwe(inps.atr, geom_file=inps.geom_file) if inps.atr else None
 
     # grib file list
     inps.grib_files = get_grib_filenames(
         date_list=inps.date_list,
         hour=inps.hour,
         model=inps.tropo_model,
         grib_dir=inps.grib_dir,
         snwe=inps.snwe)
 
+    # check existing local files (with the same grib source and time) with larger area extent
+    larger_snwe = get_larger_snwe_in_local_files(inps.grib_files[0])
+    if larger_snwe is not None:
+        larger_grib_files = get_grib_filenames(
+            date_list=inps.date_list,
+            hour=inps.hour,
+            model=inps.tropo_model,
+            grib_dir=inps.grib_dir,
+            snwe=larger_snwe)
+
+        # use the larger grib file if more local files exist than the current snwe
+        #   to avoid re-downloading as much as possible
+        grib_files_exist = check_exist_grib_file(inps.grib_files, print_msg=False)
+        larger_grib_files_exist = check_exist_grib_file(larger_grib_files, print_msg=False)
+        if len(larger_grib_files_exist) > len(grib_files_exist):
+            print('Sweet! Find more local grib files with larger SNWE extent, use the larger SNWE instead.')
+            inps.snwe = larger_snwe
+            inps.grib_files = larger_grib_files
+
     return inps
 
 
 def get_grib_filenames(date_list, hour, model, grib_dir, snwe=None):
     """Get default grib file names based on input info.
     Parameters: date_list  - list of str, date in YYYYMMDD format
                 hour       - str, hour in 2-digit with zero padding
                 model      - str, global atmospheric model name
                 grib_dir   - str, local directory to save grib files
                 snwe       - tuple of 4 int, for ERA5 only.
     Returns:    grib_files - list of str, local grib file path
     """
     # area extent
+    def snwe2str(snwe):
+        """Get area extent in string"""
+        if not snwe:
+            return None
+        s, n, w, e = snwe
+        area = ''
+        area += f'_S{abs(s)}' if s < 0 else f'_N{abs(s)}'
+        area += f'_S{abs(n)}' if n < 0 else f'_N{abs(n)}'
+        area += f'_W{abs(w)}' if w < 0 else f'_E{abs(w)}'
+        area += f'_W{abs(e)}' if e < 0 else f'_E{abs(e)}'
+        return area
+
     area = snwe2str(snwe)
 
     grib_files = []
     for d in date_list:
         if model == 'ERA5':
             if area:
                 grib_file = f'ERA5{area}_{d}_{hour}.grb'
@@ -168,69 +247,66 @@
     grib_hr = f"{grib_hr:02d}"
     return grib_hr
 
 
 def safe2date_time(safe_file, tropo_model):
     """generate date_list and hour from safe_list"""
 
+    def define_date(string):
+        """extract date from *.SAFE"""
+        filename = string.split(str.encode('.'))[0].split(str.encode('/'))[-1]
+        date = filename.split(str.encode('_'))[5][0:8]
+        return date
+
+    def define_second(string):
+        """extract CENTER_LINE_UTC from *.SAFE"""
+        filename = string.split(str.encode('.'))[0].split(str.encode('/'))[-1]
+        time1 = filename.split(str.encode('_'))[5][9:15]
+        time2 = filename.split(str.encode('_'))[6][9:15]
+        time1_second = int(time1[0:2]) * 3600 + int(time1[2:4]) * 60 + int(time1[4:6])
+        time2_second = int(time2[0:2]) * 3600 + int(time2[2:4]) * 60 + int(time2[4:6])
+        utc_sec = (time1_second + time2_second) / 2
+        return utc_sec
+
     def seconds_UTC(seconds):
         """generate second list"""
         if isinstance(seconds, list):
             secondsOut = []
             for second in seconds:
                 secondsOut.append(second)
         else:
             print('\nUn-recognized CENTER_LINE_UTC input!')
             return None
-
         return secondsOut
 
     date_list = ptime.yyyymmdd(np.loadtxt(safe_file, dtype=bytes, converters={0:define_date}).astype(str).tolist())
     second_list = seconds_UTC(np.loadtxt(safe_file, dtype=bytes, converters={0:define_second}).astype(str).tolist())
 
     # change second into hour
     hour_list = [closest_weather_model_hour(float(second), tropo_model) for second in second_list]
     hour = ut.most_common(hour_list)
 
     return date_list, hour
 
 
-def define_date(string):
-    """extract date from *.SAFE"""
-    filename = string.split(str.encode('.'))[0].split(str.encode('/'))[-1]
-    date = filename.split(str.encode('_'))[5][0:8]
-    return date
-
-
-def define_second(string):
-    """extract CENTER_LINE_UTC from *.SAFE"""
-    filename = string.split(str.encode('.'))[0].split(str.encode('/'))[-1]
-    time1 = filename.split(str.encode('_'))[5][9:15]
-    time2 = filename.split(str.encode('_'))[6][9:15]
-    time1_second = int(time1[0:2]) * 3600 + int(time1[2:4]) * 60 + int(time1[4:6])
-    time2_second = int(time2[0:2]) * 3600 + int(time2[2:4]) * 60 + int(time2[4:6])
-    utc_sec = (time1_second + time2_second) / 2
-    return utc_sec
-
-
-def ceil2multiple(x, step=10):
-    """Given a number x, find the smallest number in multiple of step >= x."""
-    assert isinstance(x, INT_DATA_TYPES), f'input number is not int: {type(x)}'
-    if x % step == 0:
-        return x
-    return x + (step - x % step)
-
-
-def floor2multiple(x, step=10):
-    """Given a number x, find the largest number in multiple of step <= x."""
-    assert isinstance(x, INT_DATA_TYPES), f'input number is not int: {type(x)}'
-    return x - x % step
+def get_snwe(meta, geom_file=None, min_buffer=2, step=10):
+    # utils sub-functions
+    def ceil2multiple(x, step=10):
+        """Given a number x, find the smallest number in multiple of step >= x."""
+        assert isinstance(x, INT_DATA_TYPES), f'input number is not int: {type(x)}'
+        if x % step == 0:
+            return x
+        else:
+            return x + (step - x % step)
 
+    def floor2multiple(x, step=10):
+        """Given a number x, find the largest number in multiple of step <= x."""
+        assert isinstance(x, INT_DATA_TYPES), f'input number is not int: {type(x)}'
+        return x - x % step
 
-def get_snwe(meta, geom_file=None, min_buffer=2, step=10):
     # get bounding box
     lat0, lat1, lon0, lon1 = get_bounding_box(meta, geom_file=geom_file)
 
     # lat/lon0/1 --> SNWE
     S = np.floor(min(lat0, lat1) - min_buffer).astype(int)
     N = np.ceil( max(lat0, lat1) + min_buffer).astype(int)
     W = np.floor(min(lon0, lon1) - min_buffer).astype(int)
@@ -238,30 +314,16 @@
 
     # SNWE in multiple of 10
     if step > 1:
         S = floor2multiple(S, step=step)
         W = floor2multiple(W, step=step)
         N = ceil2multiple(N, step=step)
         E = ceil2multiple(E, step=step)
-    return (S, N, W, E)
-
 
-def snwe2str(snwe):
-    """Get area extent in string"""
-    if not snwe:
-        return None
-    s, n, w, e = snwe
-
-    area = ''
-    area += f'_S{abs(s)}' if s < 0 else f'_N{abs(s)}'
-    area += f'_S{abs(n)}' if n < 0 else f'_N{abs(n)}'
-    area += f'_W{abs(w)}' if w < 0 else f'_E{abs(w)}'
-    area += f'_W{abs(e)}' if e < 0 else f'_E{abs(e)}'
-
-    return area
+    return (S, N, W, E)
 
 
 def get_bounding_box(meta, geom_file=None):
     """Get lat/lon range (roughly), in the same order of data file
     lat0/lon0 - starting latitude/longitude (first row/column)
     lat1/lon1 - ending latitude/longitude (last row/column)
     """
@@ -271,18 +333,16 @@
         lat0 = float(meta['Y_FIRST'])
         lon0 = float(meta['X_FIRST'])
         lat_step = float(meta['Y_STEP'])
         lon_step = float(meta['X_STEP'])
         lat1 = lat0 + lat_step * (length - 1)
         lon1 = lon0 + lon_step * (width - 1)
 
-        # 'Y_FIRST' not in 'degree'
-        # e.g. meters for UTM projection from ASF HyP3
-        y_unit = meta.get('Y_UNIT', 'degrees').lower()
-        if not y_unit.startswith('deg'):
+        # for UTM projection, e.g. ASF HyP3
+        if not meta.get('Y_UNIT', 'degrees').lower().startswith('deg'):
             lat0, lon0 = ut.utm2latlon(meta, easting=lon0, northing=lat0)
             lat1, lon1 = ut.utm2latlon(meta, easting=lon1, northing=lat1)
 
     else:
         # radar coordinates
         if geom_file and os.path.isfile(geom_file):
             geom_dset_list = readfile.get_dataset_list(geom_file)
@@ -296,30 +356,34 @@
             lons[lons == 0] = np.nan
             lat0 = np.nanmin(lats)
             lat1 = np.nanmax(lats)
             lon0 = np.nanmin(lons)
             lon1 = np.nanmax(lons)
 
         else:
+            # use the rough (not accurate) lat/lon info of the four corners
             lats = [float(meta[f'LAT_REF{i}']) for i in [1,2,3,4]]
             lons = [float(meta[f'LON_REF{i}']) for i in [1,2,3,4]]
+            # for UTM projection, e.g. ASF HyP3
+            if not meta.get('Y_UNIT', 'degrees').lower().startswith('deg'):
+                lats, lons = ut.utm2latlon(meta, easting=lons, northing=lats)
             lat0 = np.mean(lats[0:2])
             lat1 = np.mean(lats[2:4])
             lon0 = np.mean(lons[0:3:2])
             lon1 = np.mean(lons[1:4:2])
 
     return lat0, lat1, lon0, lon1
 
 
 ###############################################################
 def check_exist_grib_file(gfile_list, print_msg=True):
     """Check input list of grib files, and return the existing ones with right size."""
     gfile_exist = ut.get_file_list(gfile_list)
     if gfile_exist:
-        file_sizes = [os.path.getsize(i) for i in gfile_exist] # if os.path.getsize(i) > 10e6]
+        file_sizes = [os.path.getsize(i) for i in gfile_exist]
         if file_sizes:
             comm_size = ut.most_common([i for i in file_sizes])
             if print_msg:
                 print(f'common file size: {comm_size} bytes')
                 print(f'number of grib files existed    : {len(gfile_exist)}')
 
             gfile_corrupt = []
@@ -415,15 +479,21 @@
     grib_files2dload = sorted(list(set(grib_files) - set(grib_files_exist)))
     date_list2dload = [str(re.findall(r'\d{8}', os.path.basename(i))[0]) for i in grib_files2dload]
     print('number of grib files to download: %d' % len(date_list2dload))
     print('-'*50)
 
     # Download grib file using PyAPS
     if len(date_list2dload) > 0:
-        hour = re.findall(r'\d{8}[-_]\d{2}', os.path.basename(grib_files2dload[0]))[0].replace('-', '_').split('_')[1]
+        # This was the default for a file pattern of "ERA5_N30_N50_W130_W110_20200403_14.grb"
+        pattern = re.findall(r'\d{8}[-_]\d{2}', os.path.basename(grib_files2dload[0]))
+        if len(pattern) == 0:
+            # This is an exception for when the file has a naming format like: "ERA5_N30_N40_W130_W110_20080125T000000_06.grb"
+            pattern = re.findall(r'\d{8}T\d{6}[-_]\d{2}', os.path.basename(grib_files2dload[0]))
+        hour = pattern[0].replace('-', '_').split('_')[1]
+        #hour = re.findall(r'\d{8}[-_]\d{2}', os.path.basename(grib_files2dload[0]))[0].replace('-', '_').split('_')[1]
         grib_dir = os.path.dirname(grib_files2dload[0])
 
         # Check for non-empty account info in PyAPS config file
         check_pyaps_account_config(tropo_model)
 
         # try 3 times to download, then use whatever downloaded to calculate delay
         i = 0
@@ -675,15 +745,15 @@
     ## 3. correct tropo delay from displacement time-series (using diff.py)
     if inps.dis_file:
         print('\n'+'-'*80)
         print('Applying tropospheric correction to displacement file...')
         if ut.run_or_skip(inps.cor_dis_file, [inps.dis_file, inps.tropo_file]) == 'run':
             # diff.py can handle different reference in space and time
             # e.g. the absolute delay and the double referenced time-series
-            print('correcting delay for using diff.py')
+            print('correcting delay via diff.py')
             iargs = [inps.dis_file, inps.tropo_file, '-o', inps.cor_dis_file, '--force']
             print('diff.py', ' '.join(iargs))
             mintpy.cli.diff.main(iargs)
 
         else:
             print(f'Skip re-applying and use existed corrected displacement file: {inps.cor_dis_file}.')
     else:
```

### Comparing `mintpy-1.5.3/src/mintpy/tsview.py` & `mintpy-1.6.0/src/mintpy/tsview.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,29 @@
         if not inps.ref_yx:
             inps.ref_yx = inps.coord.geo2radar(inps.ref_lalo[0], inps.ref_lalo[1], print_msg=False)[0:2]
 
     # use REF_Y/X if ref_yx not set in cmd
     if not inps.ref_yx and 'REF_Y' in atr.keys():
         inps.ref_yx = (int(atr['REF_Y']), int(atr['REF_X']))
 
-    # ref_yx --> ref_lalo if in geo-coord
-    # for plotting purpose only
-    if inps.ref_yx and 'Y_FIRST' in atr.keys():
-        inps.ref_lalo = inps.coord.radar2geo(inps.ref_yx[0], inps.ref_yx[1], print_msg=False)[0:2]
+    # print/plot ref_yx/lalo info
+    if inps.ref_yx:
+        vprint(f'reference point in y/x: {inps.ref_yx}')
+        # ref_yx --> ref_lalo if in geo-coord [for plotting purpose only]
+        if 'Y_FIRST' in atr.keys():
+            inps.ref_lalo = inps.coord.radar2geo(inps.ref_yx[0], inps.ref_yx[1], print_msg=False)[0:2]
+            vprint(f'reference point in lat/lon: {inps.ref_lalo}')
 
     # do not plot native reference point if it's out of the coverage due to subset
     if (inps.ref_yx and 'Y_FIRST' in atr.keys()
         and inps.ref_yx == (int(atr.get('REF_Y',-999)), int(atr.get('REF_X',-999)))
         and not (    inps.pix_box[0] <= inps.ref_yx[1] < inps.pix_box[2]
                  and inps.pix_box[1] <= inps.ref_yx[0] < inps.pix_box[3])):
         inps.disp_ref_pixel = False
-        print('the native REF_Y/X is out of subset box, thus do not display')
+        vprint('the native REF_Y/X is out of subset box, thus do not display')
 
     ## initial pixel coord
     if inps.lalo:
         inps.yx = inps.coord.geo2radar(inps.lalo[0], inps.lalo[1], print_msg=False)[0:2]
     if inps.yx:
         try:
             inps.lalo = inps.coord.radar2geo(inps.yx[0], inps.yx[1], print_msg=False)[0:2]
```

### Comparing `mintpy-1.5.3/src/mintpy/unwrap_error_bridging.py` & `mintpy-1.6.0/src/mintpy/unwrap_error_bridging.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/unwrap_error_phase_closure.py` & `mintpy-1.6.0/src/mintpy/unwrap_error_phase_closure.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/arg_utils.py` & `mintpy-1.6.0/src/mintpy/utils/arg_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,66 +34,104 @@
             name = __name__.split('.')[-1]
             parser = create_argument_parser(
                 name, synopsis=synopsis, description=synopsis+NOTE, epilog=epilog, subparsers=subparsers)
     """
     if subparsers:
         # for mintpy sub-command [used in linux with apt install]
         parser = subparsers.add_parser(
-            name, description=description, formatter_class=formatter_class, epilog=epilog, help=synopsis)
+            name,
+            description=description,
+            formatter_class=formatter_class,
+            epilog=epilog,
+            help=synopsis,
+        )
 
     else:
         # for regular command usage
         parser = argparse.ArgumentParser(
-            description=description, formatter_class=formatter_class, epilog=epilog)
+            description=description,
+            formatter_class=formatter_class,
+            epilog=epilog,
+        )
 
     return parser
 
 
+##################################  argument utils  ####################################
+def get_dest_option_str_dict(parser):
+    """Get the dict where key is the option dest and value is the option string.
+
+    Parameters: parser       - argparse.ArgumentParser object
+    Returns:    dest2opt_str - dict, dictionary for all options in the parser object, where
+                               key   is the option dest   in str,
+                               value is the option string in list of str.
+    Examples:   from mintpy.cli.ifgram_inversion import create_parser
+                parser = create_parser()
+                dest_opt_str = get_dest_option_str_dict(parser)
+    """
+    action_list = parser.__dict__['_actions']
+    dest_opt_str = {}
+    for action in action_list:
+        key = action.dest
+        val = action.option_strings
+        dest_opt_str[key] = val
+    return dest_opt_str
+
 
 ##################################  argument group  ####################################
 def add_data_disp_argument(parser):
     """Argument group parser for data display options"""
     data = parser.add_argument_group('Data Display Options', 'Options to adjust the dataset display')
     data.add_argument('-v','--vlim', dest='vlim', nargs=2, metavar=('VMIN', 'VMAX'), type=float,
                       help='Display limits for matrix plotting.')
     data.add_argument('-u', '--unit', dest='disp_unit', metavar='UNIT',
                       help='unit for display.  Its priority > wrap')
     data.add_argument('--nd','--no-data-val','--no-data-value', dest='no_data_value', type=float,
                       help='Specify the no-data-value to be ignored and masked.')
 
-    data.add_argument('--interp','--interpolation', dest='interpolation', default='nearest',
-                      help='matplotlib interpolation method for imshow, e.g.:\n'
-                           'none, antialiased, nearest, bilinear, bicubic, spline16, sinc, etc. Check more at:\n'
-                           'https://matplotlib.org/stable/gallery/images_contours_and_fields/'
-                           'interpolation_methods.html')
     data.add_argument('--wrap', action='store_true',
                       help='re-wrap data to display data in fringes.')
     data.add_argument('--wrap-range', dest='wrap_range', type=float, nargs=2,
                       default=[-1.*math.pi, math.pi], metavar=('MIN', 'MAX'),
                       help='range of one cycle after wrapping (default: %(default)s).')
 
+    data.add_argument('--interp','--interpolation', dest='interpolation', default='nearest',
+                      help='matplotlib interpolation method for imshow, e.g.:\n'
+                           'none, antialiased, nearest, bilinear, bicubic, spline16, sinc, etc. Check more at:\n'
+                           'https://matplotlib.org/stable/gallery/images_contours_and_fields/'
+                           'interpolation_methods.html')
+    data.add_argument('--alpha', dest='transparency', type=float,
+                      help='Data transparency. \n'
+                           '0.0 - fully transparent, 1.0 - no transparency.')
+
+    # flip X/Y-axis
     data.add_argument('--flip-lr', dest='flip_lr',
                       action='store_true', help='flip left-right')
     data.add_argument('--flip-ud', dest='flip_ud',
                       action='store_true', help='flip up-down')
     data.add_argument('--noflip', dest='auto_flip', action='store_false',
                       help='turn off auto flip for radar coordinate file')
 
+    # multilook / average for data reduction
     data.add_argument('--nmli','--num-multilook','--multilook-num', dest='multilook_num',
                       type=int, default=1, metavar='NUM',
                       help='multilook data in X and Y direction with a factor for display '
                            '(default: %(default)s).')
     data.add_argument('--nomultilook', '--no-multilook', dest='multilook', action='store_false',
                       help='do not multilook, for high quality display. \n'
                            'If multilook is True and multilook_num=1, '
                            'multilook_num will be estimated automatically.\n'
                            'Useful when displaying big datasets.')
-    data.add_argument('--alpha', dest='transparency', type=float,
-                      help='Data transparency. \n'
-                           '0.0 - fully transparent, 1.0 - no transparency.')
+
+    # plot data in different styles: image, scatter, contour etc.
+    parser.add_argument('--style', dest='style', choices={'image', 'scatter'}, default='image',
+                        help='Plot data as image or scatter (default: %(default)s).')
+    parser.add_argument('--scatter-size', dest='scatter_marker_size', type=float, metavar='SIZE', default=10,
+                        help='Scatter marker size in points**2 (default: %(default)s).')
+
     return parser
 
 
 def add_dem_argument(parser):
     """Argument group parser for DEM display options"""
     dem = parser.add_argument_group('DEM', 'display topography in the background')
     dem.add_argument('-d', '--dem', dest='dem_file', metavar='DEM_FILE',
@@ -230,45 +268,54 @@
                           '(for geocoded file only; default: %(default)s).')
     fig.add_argument('--animation', action='store_true',
                      help='enable animation mode')
 
     return parser
 
 
-def add_gps_argument(parser):
-    """Argument group parser for GPS options"""
-    gps = parser.add_argument_group('GPS', 'GPS data to display')
-    gps.add_argument('--show-gps', dest='disp_gps', action='store_true',
-                     help='Show UNR GPS location within the coverage.')
-    gps.add_argument('--mask-gps', dest='mask_gps', action='store_true',
-                     help='Mask out GPS stations not coincident with valid data pixels')
-    gps.add_argument('--gps-label', dest='disp_gps_label', action='store_true',
-                     help='Show GPS site name')
-    gps.add_argument('--gps-ms', dest='gps_marker_size', type=float, default=6,
-                     help='Plot GPS value as scatter in size of ms**2 (default: %(default)s).')
-    gps.add_argument('--gps-comp', dest='gps_component',
-                     choices={'enu2los', 'hz2los', 'up2los', 'horz', 'vert'},
-                     help='Plot GPS in color indicating deformation velocity direction')
-    gps.add_argument('--gps-redo', dest='gps_redo', action='store_true',
-                     help='Re-calculate GPS observations in LOS direction, '
-                          'instead of read from existing CSV file.')
-    gps.add_argument('--ref-gps', dest='ref_gps_site', type=str, help='Reference GPS site')
-    gps.add_argument('--ex-gps', dest='ex_gps_sites', type=str, nargs='*',
-                     help='Exclude GPS sites, require --gps-comp.')
-
-    gps.add_argument('--gps-start-date', dest='gps_start_date', type=str, metavar='YYYYMMDD',
-                     help='start date of GPS data, default is date of the 1st SAR acquisition')
-    gps.add_argument('--gps-end-date', dest='gps_end_date', type=str, metavar='YYYYMMDD',
-                     help='start date of GPS data, default is date of the last SAR acquisition')
-    gps.add_argument('--horz-az','--hz-az', dest='horz_az_angle', type=float, default=-90.,
-                     help='Azimuth angle (anti-clockwise from the north) of the horizontal movement in degrees\n'
-                          'E.g.: -90. for east  direction [default]\n'
-                          '       0.  for north direction\n'
-                          'Set to the azimuth angle of the strike-slip fault to '
-                          'show the fault-parallel displacement.')
+def add_gnss_argument(parser):
+    """Argument group parser for GNSS options"""
+    gnss = parser.add_argument_group('GNSS', 'GNSS data to display')
+    gnss.add_argument('--show-gnss','--show-gps', dest='disp_gnss', action='store_true',
+                      help='Show UNR GNSS location within the coverage.')
+    gnss.add_argument('--gnss-source','--gnss-src','--gps-source', dest='gnss_source', default='UNR',
+                      choices={'UNR', 'ESESES', 'JPL-SIDESHOW', 'GENERIC'},
+                      help='Source of the GNSS displacement solution (default: %(default)s).')
+
+    # compare GNSS with InSAR
+    gnss.add_argument('--gnss-comp','--gps-comp', dest='gnss_component',
+                      choices={'enu2los', 'hz2los', 'up2los', 'horz', 'vert'},
+                      help='Plot GNSS in color indicating deformation velocity in (default: %(default)s).')
+    gnss.add_argument('--ref-gnss','--ref-gps', dest='ref_gnss_site', type=str, metavar='SITE_NAME',
+                      help='Reference GNSS site')
+    gnss.add_argument('--ex-gnss','--ex-gps', dest='ex_gnss_sites', type=str, nargs='*', metavar='SITE_NAME',
+                      help='Exclude GNSS sites, require --gnss-comp.')
+
+    gnss.add_argument('--gnss-start-date','--gps-start-date', dest='gnss_start_date', type=str, metavar='YYYYMMDD',
+                      help='start date of GNSS data, default: the 1st SAR acquisition')
+    gnss.add_argument('--gnss-end-date','--gps-end-date', dest='gnss_end_date', type=str, metavar='YYYYMMDD',
+                      help='end   date of GNSS data, default: the last SAR acquisition')
+    gnss.add_argument('--horz-az','--hz-az', dest='horz_az_angle', type=float, default=-90., metavar='NUM',
+                      help='Azimuth angle (anti-clockwise from the north) of the horizontal movement in degrees\n'
+                           'E.g.: -90. for east  direction [default]\n'
+                           '       0.  for north direction\n'
+                           'Set to the azimuth angle of the strike-slip fault to '
+                           'show the fault-parallel displacement.')
+    gnss.add_argument('--gnss-redo','--gps-redo', dest='gnss_redo', action='store_true',
+                      help='Re-calculate GNSS observations in LOS direction, '
+                           'instead of read from existing CSV file.')
+
+    # plot style
+    gnss.add_argument('--gnss-label','--gps-label', dest='disp_gnss_label', action='store_true',
+                      help='Show GNSS site name')
+    gnss.add_argument('--mask-gnss','--mask-gps', dest='mask_gnss', action='store_true',
+                      help='Mask out GNSS stations not coincident with valid data pixels')
+    gnss.add_argument('--gnss-ms','--gps-ms', dest='gnss_marker_size', type=float, default=6, metavar='NUM',
+                      help='Plot GNSS value as scatter in size of ms**2 (default: %(default)s).')
+
     return parser
 
 
 def add_mask_argument(parser):
     """Argument group parser for mask options"""
     mask = parser.add_argument_group('Mask', 'Mask file/options')
     mask.add_argument('-m','--mask', dest='mask_file', metavar='FILE',
@@ -433,22 +480,22 @@
                            '\t2) output file is newer than input file.')
     return parser
 
 
 def add_subset_argument(parser, geo=True):
     """Argument group parser for subset options"""
     sub = parser.add_argument_group('Subset', 'Display dataset in subset range')
-    sub.add_argument('--sub-x','--subx','--subset-x', dest='subset_x', type=int, nargs=2,
+    sub.add_argument('--sub-x','--subset-x', dest='subset_x', type=int, nargs=2,
                      metavar=('XMIN', 'XMAX'), help='subset display in x/cross-track/range direction')
-    sub.add_argument('--sub-y','--suby','--subset-y', dest='subset_y', type=int, nargs=2,
+    sub.add_argument('--sub-y','--subset-y', dest='subset_y', type=int, nargs=2,
                      metavar=('YMIN', 'YMAX'), help='subset display in y/along-track/azimuth direction')
     if geo:
-        sub.add_argument('--sub-lat','--sublat','--subset-lat', dest='subset_lat', type=float, nargs=2,
+        sub.add_argument('--sub-lat','--subset-lat', dest='subset_lat', type=float, nargs=2,
                          metavar=('LATMIN', 'LATMAX'), help='subset display in latitude')
-        sub.add_argument('--sub-lon','--sublon','--subset-lon', dest='subset_lon', type=float, nargs=2,
+        sub.add_argument('--sub-lon','--subset-lon', dest='subset_lon', type=float, nargs=2,
                          metavar=('LONMIN', 'LONMAX'), help='subset display in longitude')
     return parser
 
 
 def add_timefunc_argument(parser):
     """Argument group parser for time functions"""
     model = parser.add_argument_group('Deformation Model', 'A suite of time functions')
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/attribute.py` & `mintpy-1.6.0/src/mintpy/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/isce_utils.py` & `mintpy-1.6.0/src/mintpy/utils/isce_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 
 def get_processor(meta_file):
     """
     Get the name of ISCE processor (imaging mode)
     """
-    meta_dir = os.path.dirname(meta_file)
+    meta_dir = os.path.dirname(os.path.abspath(meta_file))
     tops_meta_file = os.path.join(meta_dir, 'IW*.xml')
     alos_meta_file = os.path.join(meta_dir, '*.track.xml')
     stripmap_meta_files = [os.path.join(meta_dir, i) for i in ['data.db', 'data.dat', 'data']]
 
     processor = None
     if len(glob.glob(tops_meta_file)) > 0:
         # topsStack
@@ -362,37 +362,48 @@
     meta['NCORRLOOKS'] = meta['RLOOKS'] * meta['ALOOKS'] / (rgfact * azfact)
 
     # update pixel_size for multilooked data
     meta['rangePixelSize'] *= meta['RLOOKS']
     meta['azimuthPixelSize'] *= meta['ALOOKS']
 
     # LAT/LON_REF1/2/3/4
+    lat_files = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lat'))
+    if len(lat_files) > 0:
+        # geometry files from alosStack
+        lat_files = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lat'))
+        lon_files = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lon'))
+        los_files = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.los'))
+    else:
+        # geometry files from alos2App / dense offset, which are then multilooked by mintpy
+        lat_files = [os.path.join(geom_dir, 'lat.rdr.mli')]
+        lon_files = [os.path.join(geom_dir, 'lon.rdr.mli')]
+        los_files = [os.path.join(geom_dir, 'los.rdr.mli')]
+
     edge = 3
-    lat_file = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lat'))[0]
     img = isceobj.createImage()
-    img.load(lat_file+'.xml')
+    img.load(lat_files[0] + '.xml')
     width = img.width
     length = img.length
-    data = np.memmap(lat_file, dtype='float64', mode='r', shape=(length, width))
+
+    data = np.memmap(lat_files[0], dtype='float64', mode='r', shape=(length, width))
     meta['LAT_REF1'] = str(data[ 0+edge,  0+edge])
     meta['LAT_REF2'] = str(data[ 0+edge, -1-edge])
     meta['LAT_REF3'] = str(data[-1-edge,  0+edge])
     meta['LAT_REF4'] = str(data[-1-edge, -1-edge])
 
-    lon_file = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lon'))[0]
-    data = np.memmap(lon_file, dtype='float64', mode='r', shape=(length, width))
+    data = np.memmap(lon_files[0], dtype='float64', mode='r', shape=(length, width))
     meta['LON_REF1'] = str(data[ 0+edge,  0+edge])
     meta['LON_REF2'] = str(data[ 0+edge, -1-edge])
     meta['LON_REF3'] = str(data[-1-edge,  0+edge])
     meta['LON_REF4'] = str(data[-1-edge, -1-edge])
 
     # CENTER_INCIDENCE_ANGLE is optional
-    los_files = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.los'))
     if len(los_files) > 0:
-        data = np.memmap(los_files[0], dtype='float32', mode='r', shape=(length*2, width))[0:length*2:2, :]
+        # use readfile.read() instead of np.memmap() to better handle different interleaves
+        data = readfile.read(los_files[0], datasetName='incidenceAngle')[0]
         inc_angle = data[int(length/2), int(width/2)]
         meta['CENTER_INCIDENCE_ANGLE'] = str(inc_angle)
 
     pointingDirection = {'right': -1, 'left' :1}
     meta['ANTENNA_SIDE'] = str(pointingDirection[track.pointingDirection])
 
     return meta, track
@@ -410,28 +421,38 @@
     scansarWideModes = ['VBS', 'VBD']
     scansarModes = scansarNominalModes + scansarWideModes
 
     return (spotlightModes, stripmapModes, scansarNominalModes, scansarWideModes, scansarModes)
 
 
 def extract_image_size_alosStack(geom_dir):
-    import isce
-    import isceobj
 
     # grab the number of looks in azimuth / range direction
-    lats = glob.glob(os.path.join(geom_dir, '*_*rlks_*alks.lat'))
-    rlooks = max(int(os.path.splitext(os.path.basename(x))[0].split('_')[1].strip('rlks')) for x in lats)
-    alooks = max(int(os.path.splitext(os.path.basename(x))[0].split('_')[2].strip('alks')) for x in lats)
+    lat_files = glob.glob(os.path.join(geom_dir, '*_*rlks_*alks.lat'))
+    lat_xml_files = [os.path.join(geom_dir, f'lat.rdr{x}.xml') for x in ['', '.mli']]
+    lat_xml_files = [x for x in lat_xml_files if os.path.exists(x)]
+    if len(lat_files) > 0:
+        # alosStack for InSAR
+        rlooks = max(int(os.path.splitext(os.path.basename(x))[0].split('_')[1].strip('rlks')) for x in lat_files)
+        alooks = max(int(os.path.splitext(os.path.basename(x))[0].split('_')[2].strip('alks')) for x in lat_files)
+        lat_xml_file = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lat.xml'))[0]
+    elif len(lat_xml_files) == 2:
+        # alos2App for dense offset, which are multilooked by mintpy
+        meta_ori = readfile.read_isce_xml(lat_xml_files[0])
+        meta_mli = readfile.read_isce_xml(lat_xml_files[1])
+        rlooks = int(np.floor( int(meta_ori['WIDTH']) / int(meta_mli['WIDTH']) ))
+        alooks = int(np.floor( int(meta_ori['LENGTH']) / int(meta_mli['LENGTH']) ))
+        lat_xml_file = lat_xml_files[1]
+    else:
+        raise ValueError(f'Un-recognized lookup table files in directory: {geom_dir}!')
 
     # grab the number of rows / coluns
-    lat = glob.glob(os.path.join(geom_dir, f'*_{rlooks}rlks_{alooks}alks.lat'))[0]
-    img = isceobj.createImage()
-    img.load(lat+'.xml')
-    width = img.width
-    length = img.length
+    meta_mli = readfile.read_isce_xml(lat_xml_file)
+    width = int(meta_mli['WIDTH'])
+    length = int(meta_mli['LENGTH'])
 
     return (rlooks, alooks, width, length)
 
 
 def load_track(trackDir, dateStr):
     '''Load the track using Product Manager.
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/map.py` & `mintpy-1.6.0/src/mintpy/utils/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,19 @@
                 lalo_max_num   : int, rough major tick number along the longer axis
                 step_candidate : list of int, candidate list for the significant number of step
     Returns:    lats/lons : np.array of float, sequence of lat/lon auto calculated from input geo_box
                 lalo_step : float, lat/lon label step
     Example:    geo_box = (128.0, 37.0, 138.0, 30.0)
                 lats, lons, step = m.auto_lalo_sequence(geo_box)
     """
+    # check input arguments
+    if geo_box[1] <= geo_box[3] or geo_box[2] < geo_box[0]:
+        raise ValueError(f'Input geo_box {geo_box} has N <= S or E <= W! Check the order of (W, N, E, S).')
+    if lalo_step and lalo_step <= 0:
+        raise ValueError(f'Input lalo_step ({lalo_step}) must be positive!')
 
     max_lalo_dist = max([geo_box[1] - geo_box[3], geo_box[2] - geo_box[0]])
 
     if not lalo_step:
         # Initial tick step
         lalo_step = round_to_1(max_lalo_dist / lalo_max_num)
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/network.py` & `mintpy-1.6.0/src/mintpy/utils/network.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/plot.py` & `mintpy-1.6.0/src/mintpy/utils/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     '#9467bd',
     '#8c564b',
     '#e377c2',
     '#7f7f7f',
     '#bcbd22',
     '#17becf',
 ]
+# ensur UTM coordinate plot axes do not use scientific notation
+plt.rcParams["axes.formatter.limits"] = (-1e10, 1e10)
 
 
 ########################################### Parser utilities ##############################################
 def read_pts2inps(inps, coord_obj):
     """Read pts_* options"""
     ## 1. merge pts_file/lalo/yx into pts_yx
     # pts_file --> pts_lalo
@@ -409,16 +411,20 @@
 
             if print_msg:
                 msg = f'data has uniform and limited number ({unique_values.size} <= {max_discrete_num_step})'
                 msg += ' of unique values --> discretize colormap'
                 print(msg)
 
         else:
-            from mintpy.multilook import multilook_data
-            data_mli = multilook_data(data, num_multilook, num_multilook)
+            if min(data.shape[1:]) >= 100 and num_multilook > 1:
+                # multilook data (by 10X for 3D matrix by default) to ignore extreme values
+                from mintpy.multilook import multilook_data
+                data_mli = multilook_data(data, num_multilook, num_multilook)
+            else:
+                data_mli = np.array(data)
 
             cmap_lut = 256
             vlim = [np.nanmin(data_mli), np.nanmax(data_mli)]
             unique_values = None
 
             # convert near-pi value to pi
             vlim[0] = vlim[0] if abs(vlim[0] + np.pi) / np.pi >= 0.001 else np.pi * -1
@@ -540,24 +546,25 @@
     x_list = [i-bar_width/2 for i in dates]
 
     coh_mat = pnet.coherence_matrix(date12List, cohList)
 
     ax.bar(x_list, np.nanmax(coh_mat, axis=0), bar_width.days, label='Max {}'.format(p_dict['ds_name']))
     ax.bar(x_list, np.nanmin(coh_mat, axis=0), bar_width.days, label='Min {}'.format(p_dict['ds_name']))
 
+    # axis format
     if p_dict['disp_title']:
         ax.set_title('{} History: Min/Max of All Related Pairs'.format(p_dict['ds_name']))
-
     ax = auto_adjust_xaxis_date(ax, datevector, fontsize=p_dict['fontsize'],
                                 every_year=p_dict['every_year'])[0]
     ax.set_ylim([p_dict['vlim'][0], p_dict['vlim'][1]])
-
     #ax.set_xlabel('Time [years]', fontsize=p_dict['fontsize'])
-    ax.set_ylabel(p_dict['ds_name'], fontsize=p_dict['fontsize'])
+    ax.set_ylabel(p_dict['cbar_label'], fontsize=p_dict['fontsize'])
     ax.legend(loc='best')
+    ax.tick_params(which='both', direction='in', labelsize=p_dict['fontsize'],
+                   bottom=True, top=True, left=True, right=True)
 
     return ax
 
 
 def plot_network(ax, date12List, dateList, pbaseList, p_dict={}, date12List_drop=[], print_msg=True):
     """Plot Temporal-Perp baseline Network
     Parameters: ax         - matplotlib axes object
@@ -1099,112 +1106,143 @@
 
     return
 
 
 
 ###############################################  GNSS  ###############################################
 
-def plot_gps(ax, SNWE, inps, metadata=dict(), print_msg=True):
+def plot_gnss(ax, SNWE, inps, metadata=dict(), print_msg=True):
     """Plot GNSS as scatters on top of the input matplotlib.axes.
 
     Parameters: ax       - matplotlib.axes object
                 SNWE     - tuple of 4 float, for south, north, west and east
                 inps     - Namespace object, from view.py
                 metadata - dict, mintpy metadata
     Returns:    ax       - matplotlib.axes object
     """
+    from pyproj import Geod
 
-    from mintpy.objects import gps
+    from mintpy.objects import gnss
     vprint = print if print_msg else lambda *args, **kwargs: None
 
     vmin, vmax = inps.vlim
     cmap = ColormapExt(inps.colormap).colormap if isinstance(inps.colormap, str) else inps.colormap
 
     atr = dict(metadata)
     atr['UNIT'] = 'm'
     unit_fac = scale_data2disp_unit(metadata=atr, disp_unit=inps.disp_unit)[2]
 
-    start_date = inps.gps_start_date if inps.gps_start_date else metadata.get('START_DATE', None)
-    end_date = inps.gps_end_date if inps.gps_end_date else metadata.get('END_DATE', None)
+    start_date = inps.gnss_start_date if inps.gnss_start_date else metadata.get('START_DATE', None)
+    end_date = inps.gnss_end_date if inps.gnss_end_date else metadata.get('END_DATE', None)
+
+    # pre-query: convert UTM to lat/lon for query
+    if 'UTM_ZONE' in metadata.keys():
+        south, west = ut0.utm2latlon(atr, SNWE[2], SNWE[0])
+        north, east = ut0.utm2latlon(atr, SNWE[3], SNWE[1])
+        SNWE = (south, north, west, east)
 
     # query for GNSS stations
-    site_names, site_lats, site_lons = gps.search_gps(SNWE, start_date, end_date)
+    site_names, site_lats, site_lons = gnss.search_gnss(
+        SNWE,
+        start_date=start_date,
+        end_date=end_date,
+        source=inps.gnss_source,
+    )
     if site_names.size == 0:
         warnings.warn(f'No GNSS found within {SNWE} during {start_date} - {end_date}!')
         print('  continue without GNSS plots.')
         return ax
 
+    # print the nearest GNSS to the current reference point
+    # to facilitate the --ref-gnss option setup
+    if inps.ref_lalo:
+        site_dist = Geod(ellps='WGS84').inv(
+            np.tile(inps.ref_lalo[1], site_names.size),
+            np.tile(inps.ref_lalo[0], site_names.size),
+            site_lons,
+            site_lats,
+        )[2]
+        n_ind = np.argmin(site_dist)
+        msg = 'nearest GNSS site (potential --ref-gnss choice): '
+        msg += f'{site_names[n_ind]} at [{site_lats[n_ind]}, {site_lons[n_ind]}]'
+        print(msg)
+
+    # post-query: convert lat/lon to UTM for plotting
+    if 'UTM_ZONE' in metadata.keys():
+        site_lats, site_lons = ut0.latlon2utm(metadata, site_lats, site_lons)
+
     # mask out stations not coincident with InSAR data
-    if inps.mask_gps and inps.msk is not None:
+    if inps.mask_gnss and inps.msk is not None:
         msk = inps.msk if inps.msk.ndim == 2 else np.prod(inps.msk, axis=-1)
         coord = coordinate(metadata)
         site_ys, site_xs = coord.geo2radar(site_lats, site_lons)[0:2]
         flag = msk[site_ys, site_xs] != 0
         # update station list
         site_names = site_names[flag]
         site_lats = site_lats[flag]
         site_lons = site_lons[flag]
         # check
         if site_names.size == 0:
-            raise ValueError('No GNSS left after --mask-gps!')
+            raise ValueError('No GNSS left after --mask-gnss!')
 
-    if inps.ref_gps_site and inps.ref_gps_site not in site_names:
-        raise ValueError(f'input reference GPS site "{inps.ref_gps_site}" not available!')
+    if inps.ref_gnss_site and inps.ref_gnss_site not in site_names:
+        raise ValueError(f'input reference GNSS site "{inps.ref_gnss_site}" not available!')
 
     k = metadata['FILE_TYPE']
-    if inps.gps_component and k not in ['velocity', 'timeseries', 'displacement']:
-        inps.gps_component = None
-        vprint(f'WARNING: --gps-comp is not implemented for {k} file yet, set --gps-comp = None and continue')
-
-    plot_kwargs = dict(s=inps.gps_marker_size**2, edgecolors='k', lw=0.5, zorder=10)
-    if inps.gps_component:
-        # plot GPS velocity/displacement along LOS direction
+    if inps.gnss_component and k not in ['velocity', 'timeseries', 'displacement']:
+        inps.gnss_component = None
+        vprint(f'WARNING: --gnss-comp is not implemented for {k} file yet, set --gnss-comp = None and continue')
+
+    plot_kwargs = dict(s=inps.gnss_marker_size**2, edgecolors='k', lw=0.5, zorder=10)
+    if inps.gnss_component:
+        # plot GNSS velocity/displacement along LOS direction
         vprint('-'*30)
-        msg = 'plotting GPS '
+        msg = 'plotting GNSS '
         msg += 'velocity' if k == 'velocity' else 'displacement'
-        msg += f' in IGS14 reference frame in {inps.gps_component} direction'
-        msg += f' with respect to {inps.ref_gps_site} ...' if inps.ref_gps_site else ' ...'
+        msg += f' in IGS14 reference frame in {inps.gnss_component} direction'
+        msg += f' with respect to {inps.ref_gnss_site} ...' if inps.ref_gnss_site else ' ...'
         vprint(msg)
-        vprint(f'number of available GPS stations: {len(site_names)}')
+        vprint(f'number of available GNSS stations: {len(site_names)}')
         vprint(f'start date: {start_date}')
         vprint(f'end   date: {end_date}')
-        vprint(f'components projection: {inps.gps_component}')
+        vprint(f'components projection: {inps.gnss_component}')
 
-        # get GPS LOS observations
+        # get GNSS LOS observations
         # save absolute value to support both spatially relative and absolute comparison
         # without compromising the re-usability of the CSV file
         obs_type = 'velocity' if k == 'velocity' else 'displacement'
-        site_obs = gps.get_gps_los_obs(
+        site_obs = gnss.get_los_obs(
             meta=metadata,
             obs_type=obs_type,
             site_names=site_names,
             start_date=start_date,
             end_date=end_date,
-            gps_comp=inps.gps_component,
+            source=inps.gnss_source,
+            gnss_comp=inps.gnss_component,
             horz_az_angle=inps.horz_az_angle,
             print_msg=print_msg,
-            redo=inps.gps_redo,
+            redo=inps.gnss_redo,
         )
 
-        # reference GPS
-        if inps.ref_gps_site:
-            ref_ind = site_names.tolist().index(inps.ref_gps_site)
+        # reference GNSS
+        if inps.ref_gnss_site:
+            ref_ind = site_names.tolist().index(inps.ref_gnss_site)
             # plot label of the reference site
             #ax.annotate(site_names[ref_ind], xy=(site_lons[ref_ind], site_lats[ref_ind]), fontsize=inps.font_size)
             # update value
             ref_val = site_obs[ref_ind]
             if not np.isnan(ref_val):
                 site_obs -= ref_val
 
         # scale to the same unit as InSAR
         site_obs *= unit_fac
 
         # exclude sites
-        if inps.ex_gps_sites:
-            ex_flag = np.array([x in inps.ex_gps_sites for x in site_names], dtype=np.bool_)
+        if inps.ex_gnss_sites:
+            ex_flag = np.array([x in inps.ex_gnss_sites for x in site_names], dtype=np.bool_)
             if np.sum(ex_flag) > 0:
                 vprint(f'ignore the following specified stations:\n  {site_names[ex_flag]}')
                 site_names = site_names[~ex_flag]
                 site_lats = site_lats[~ex_flag]
                 site_lons = site_lons[~ex_flag]
                 site_obs = site_obs[~ex_flag]
 
@@ -1216,82 +1254,83 @@
         # plot
         for lat, lon, obs in zip(site_lats, site_lons, site_obs):
             if not np.isnan(obs):
                 color = cmap( (obs - vmin) / (vmax - vmin) )
                 ax.scatter(lon, lat, color=color, **plot_kwargs)
 
     else:
-        # plot GPS locations only
-        vprint('showing GPS locations')
+        # plot GNSS locations only
+        vprint('showing GNSS locations')
         ax.scatter(site_lons, site_lats, color='w', **plot_kwargs)
 
-    # plot GPS label
-    if inps.disp_gps_label:
+    # plot GNSS label
+    if inps.disp_gnss_label:
         for site_name, lat, lon in zip(site_names, site_lats, site_lons):
             ax.annotate(site_name, xy=(lon, lat), fontsize=inps.font_size)
 
     return ax
 
 
-def plot_insar_vs_gps_scatter(vel_file, csv_file='gps_enu2los.csv', msk_file=None, ref_gps_site=None, cutoff=5,
-                              fig_size=[4, 4], xname='InSAR', vlim=None, ex_gps_sites=[], display=True):
-    """Scatter plot to compare the velocities between SAR/InSAR and GPS.
-
-    Parameters: vel_file     - str, path of InSAR LOS velocity HDF5 file.
-                csv_file     - str, path of GNSS CSV file, generated after running view.py --gps-comp
-                msk_file     - str, path of InSAR mask file.
-                ref_gps_site - str, reference GNSS site name
-                cutoff       - float, threshold in terms of med abs dev (MAD) for outlier detection
-                xname        - str, xaxis label
-                vlim         - list of 2 float, display value range in the unit of cm/yr
-                               Default is None to grab from data
-                               If set, the range will be used to prune the SAR and GPS observations
-                ex_gps_sites - list of str, exclude GNSS sites for analysis and plotting.
-    Returns:    sites        - list of str, GNSS site names used for comparison
-                insar_obs    - 1D np.ndarray in float32, InSAR velocity in cm/yr
-                gps_obs      - 1D np.ndarray in float32, GNSS  velocity in cm/yr
+def plot_insar_vs_gnss_scatter(vel_file, csv_file='gnss_enu2los_UNR.csv', msk_file=None, ref_gnss_site=None,
+                               cutoff=5, fig_size=(4, 4), xname='InSAR', vlim=None, ex_gnss_sites=None,
+                               display=True):
+    """Scatter plot to compare the velocities between SAR/InSAR and GNSS.
+
+    Parameters: vel_file      - str, path of InSAR LOS velocity HDF5 file.
+                csv_file      - str, path of GNSS CSV file, generated after running view.py --gnss-comp
+                msk_file      - str, path of InSAR mask file.
+                ref_gnss_site - str, reference GNSS site name
+                cutoff        - float, threshold in terms of med abs dev (MAD) for outlier detection
+                xname         - str, xaxis label
+                vlim          - list of 2 float, display value range in the unit of cm/yr
+                                Default is None to grab from data
+                                If set, the range will be used to prune the SAR and GNSS observations
+                ex_gnss_sites - list of str, exclude GNSS sites for analysis and plotting.
+    Returns:    sites         - list of str, GNSS site names used for comparison
+                insar_obs     - 1D np.ndarray in float32, InSAR velocity in cm/yr
+                gnss_obs      - 1D np.ndarray in float32, GNSS  velocity in cm/yr
     Example:
         from mintpy.utils import plot as pp
-        csv_file = os.path.join(work_dir, 'geo/gps_enu2los.csv')
+        csv_file = os.path.join(work_dir, 'geo/gnss_enu2los_UNR.csv')
         vel_file = os.path.join(work_dir, 'geo/geo_velocity.h5')
         msk_file = os.path.join(work_dir, 'geo/geo_maskTempCoh.h5')
-        pp.plot_insar_vs_gps_scatter(
+        pp.plot_insar_vs_gnss_scatter(
             vel_file,
-            ref_gps_site='CACT',
+            ref_gnss_site='CACT',
             csv_file=csv_file,
             msk_file=msk_file,
             vlim=[-2.5, 2],
         )
     """
 
     disp_unit = 'cm/yr'
     unit_fac = 100.
 
-    # read GPS velocity from CSV file (generated by gps.get_gps_los_obs())
+    # read GNSS velocity from CSV file (generated by gnss.get_los_obs())
     col_names = ['Site', 'Lon', 'Lat', 'Displacement', 'Velocity']
     num_col = len(col_names)
     col_types = ['U10'] + ['f8'] * (num_col - 1)
 
-    print(f'read GPS velocity from file: {csv_file}')
+    print(f'read GNSS velocity from file: {csv_file:s}')
     fc = np.genfromtxt(csv_file, dtype=col_types, delimiter=',', names=True)
     sites = fc['Site']
     lats = fc['Lat']
     lons = fc['Lon']
-    gps_obs = fc[col_names[-1]] * unit_fac
+    gnss_obs = fc[col_names[-1]] * unit_fac
 
-    if ex_gps_sites:
-        ex_flag = np.array([x in ex_gps_sites for x in sites], dtype=np.bool_)
+    if ex_gnss_sites is not None:
+        ex_flag = np.array([site in ex_gnss_sites for site in sites], dtype=np.bool_)
         if np.sum(ex_flag) > 0:
             sites = sites[~ex_flag]
             lats = lats[~ex_flag]
             lons = lons[~ex_flag]
-            gps_obs = gps_obs[~ex_flag]
+            gnss_obs = gnss_obs[~ex_flag]
 
     # read InSAR velocity
-    print(f'read InSAR velocity from file: {vel_file}')
+    print(f'read InSAR velocity from file: {vel_file:s}')
     atr = readfile.read_attribute(vel_file)
     length, width = int(atr['LENGTH']), int(atr['WIDTH'])
     ys, xs = coordinate(atr).geo2radar(lats, lons)[:2]
 
     msk = readfile.read(msk_file)[0] if msk_file else np.ones((length, width), dtype=np.bool_)
 
     num_site = sites.size
@@ -1301,82 +1340,82 @@
         x, y = xs[i], ys[i]
         if (0 <= x < width) and (0 <= y < length) and msk[y, x]:
             box = (x, y, x+1, y+1)
             insar_obs[i] = readfile.read(vel_file, datasetName='velocity', box=box)[0] * unit_fac
         prog_bar.update(i+1, suffix=f'{i+1}/{num_site} {sites[i]}')
     prog_bar.close()
 
-    off_med = np.nanmedian(insar_obs - gps_obs)
-    print(f'median offset between InSAR and GPS [before common referencing]: {off_med:.2f} cm/year')
+    off_med = np.nanmedian(insar_obs - gnss_obs)
+    print(f'median offset between InSAR and GNSS [before common referencing]: {off_med:.2f} cm/year')
 
     # reference site
-    if ref_gps_site:
-        print(f'referencing both InSAR and GPS data to site: {ref_gps_site}')
-        ref_ind = sites.tolist().index(ref_gps_site)
-        gps_obs -= gps_obs[ref_ind]
+    if ref_gnss_site:
+        print(f'referencing both InSAR and GNSS data to site: {ref_gnss_site}')
+        ref_ind = sites.tolist().index(ref_gnss_site)
+        gnss_obs -= gnss_obs[ref_ind]
         insar_obs -= insar_obs[ref_ind]
 
     # remove NaN value
-    print(f'removing sites with NaN values in GPS or {xname}')
-    flag = np.multiply(~np.isnan(insar_obs), ~np.isnan(gps_obs))
+    print(f'removing sites with NaN values in GNSS or {xname}')
+    flag = np.multiply(~np.isnan(insar_obs), ~np.isnan(gnss_obs))
     if vlim is not None:
         print(f'pruning sites with value range: {vlim} {disp_unit}')
-        flag *= gps_obs >= vlim[0]
-        flag *= gps_obs <= vlim[1]
+        flag *= gnss_obs >= vlim[0]
+        flag *= gnss_obs <= vlim[1]
         flag *= insar_obs >= vlim[0]
         flag *= insar_obs <= vlim[1]
 
-    gps_obs = gps_obs[flag]
+    gnss_obs = gnss_obs[flag]
     insar_obs = insar_obs[flag]
     sites = sites[flag]
 
     # stats
-    print(f'GPS   min/max: {np.nanmin(gps_obs):.2f} / {np.nanmax(gps_obs):.2f}')
+    print(f'GNSS   min/max: {np.nanmin(gnss_obs):.2f} / {np.nanmax(gnss_obs):.2f}')
     print(f'InSAR min/max: {np.nanmin(insar_obs):.2f} / {np.nanmax(insar_obs):.2f}')
 
-    rmse = np.sqrt(np.sum((insar_obs - gps_obs)**2) / (gps_obs.size - 1))
-    r2 = stats.linregress(insar_obs, gps_obs)[2]
+    rmse = np.sqrt(np.sum((insar_obs - gnss_obs)**2) / (gnss_obs.size - 1))
+    r2 = stats.linregress(insar_obs, gnss_obs)[2]
     print(f'RMSE = {rmse:.2f} {disp_unit}')
     print(f'R^2 = {r2:.2f}')
 
     # preliminary outlier detection
-    diff_mad = ut0.median_abs_deviation(abs(insar_obs - gps_obs), center=0)
+    diff_mad = ut0.median_abs_deviation(abs(insar_obs - gnss_obs), center=0)
     print(f'Preliminary outliers detection: abs(InSAR - GNSS) > med abs dev ({diff_mad:.2f}) * {cutoff}')
     print('Site:  InSAR  GNSS')
-    for site_name, insar_val, gps_val in zip(sites, insar_obs, gps_obs):
-        if abs(insar_val - gps_val) > diff_mad * cutoff:
-            print(f'{site_name:s}: {insar_val:5.1f}, {gps_val:5.1f}  {disp_unit}')
+    for site_name, insar_val, gnss_val in zip(sites, insar_obs, gnss_obs):
+        if abs(insar_val - gnss_val) > diff_mad * cutoff:
+            print(f'{site_name:s}: {insar_val:5.1f}, {gnss_val:5.1f}  {disp_unit}')
 
     # plot
     if display:
         plt.rcParams.update({'font.size': 12})
         if vlim is None:
             vlim = [np.min(insar_obs), np.max(insar_obs)]
             vbuffer = (vlim[1] - vlim[0]) * 0.2
             vlim = [vlim[0] - vbuffer, vlim[1] + vbuffer]
 
         fig, ax = plt.subplots(figsize=fig_size)
         ax.plot((vlim[0], vlim[1]), (vlim[0], vlim[1]), 'k--')
-        ax.plot(insar_obs, gps_obs, '.', ms=15)
+        ax.plot(insar_obs, gnss_obs, '.', ms=15)
 
         # axis format
         ax.set_xlim(vlim)
         ax.set_ylim(vlim)
         ax.set_xlabel(f'{xname} [{disp_unit}]')
         ax.set_ylabel(f'GNSS [{disp_unit}]')
         ax.set_aspect('equal', 'box')
         fig.tight_layout()
 
         # output
-        out_fig = f'{xname.lower()}_vs_gps_scatter.pdf'
+        out_fig = f'{xname.lower()}_vs_gnss_scatter.pdf'
         plt.savefig(out_fig, bbox_inches='tight', transparent=True, dpi=300)
         print('save figure to file', out_fig)
         plt.show()
 
-    return sites, insar_obs, gps_obs
+    return sites, insar_obs, gnss_obs
 
 
 def plot_colorbar(inps, im, cax):
 
     # orientation
     if inps.cbar_loc in ['left', 'right']:
         orientation = 'vertical'
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/plot_ext.py` & `mintpy-1.6.0/src/mintpy/utils/plot_ext.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/ptime.py` & `mintpy-1.6.0/src/mintpy/utils/ptime.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
     elif len(re.findall(r'\d{4}-\d{2}-\d{2}T\d{2}', date_str)) > 0:
         date_str_format = '%Y-%m-%dT%H'
 
     elif len(re.findall(r'\d{4}-\d{2}-\d{2}', date_str)) > 0:
         date_str_format = '%Y-%m-%d'
 
+    elif len(re.findall(r'\d{8}:\d{6}', date_str)) > 0:
+        date_str_format = '%Y%m%d:%H%M%S'
+
     elif len(re.findall(r'\d{8}T\d{6}', date_str)) > 0:
         date_str_format = '%Y%m%dT%H%M%S'
 
     elif len(re.findall(r'\d{8}T\d{4}', date_str)) > 0:
         date_str_format = '%Y%m%dT%H%M'
 
     elif len(re.findall(r'\d{6}T\d{4}', date_str)) > 0:
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/readfile.py` & `mintpy-1.6.0/src/mintpy/utils/readfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -834,18 +834,25 @@
                 slice_list = ['magnitude', 'phase']
             else:
                 slice_list = ['complex']
 
         elif 'offset' in fbase and num_band == 2:
             # ampcor offset file, e.g. offset.bip, dense_offsets.bil
             slice_list = ['azimuthOffset', 'rangeOffset']
+            if fname.endswith('_denseoffset.off'):
+                # for alos2App dense offset, the file has the opposite band order
+                # e.g. 231206-240103_denseoffset.off
+                slice_list = ['rangeOffset', 'azimuthOffset']
 
-        elif 'offset' in fbase and '_cov' in fbase and num_band == 3:
+        elif 'offset' in fbase and 'cov' in fname and num_band == 3:
             # ampcor offset covariance file, e.g. offset_cov.bip, dense_offsets_cov.bil
             slice_list = ['azimuthOffsetVar', 'rangeOffsetVar', 'offsetCovar']
+            if fname.endswith('_denseoffset.cov'):
+                # for alos2App dense offset, e.g. 231206-240103_denseoffset.cov
+                slice_list = ['rangeOffsetVar', 'azimuthOffsetVar', 'offsetCovar']
 
         elif fext in ['.lkv']:
             slice_list = ['east', 'north', 'up']
 
         elif fext in ['.llh']:
             slice_list = ['latitude', 'longitude', 'height']
 
@@ -1360,16 +1367,24 @@
         processor = meta['PROCESSOR']
         fname = meta['FILE_PATH']
         fbase, fext = _get_file_base_and_ext(fname)
         num_band = int(meta.get('BANDS', 0))
 
         # known file types
         # isce2: dense offsets from topsApp.py
-        if processor == 'isce' and fname.endswith('dense_offsets.bil') and num_band == 2:
-            no_data_value = -10000.
+        if processor == 'isce' and num_band == 2:
+            # isce2 dense offset
+            if fname.endswith('dense_offsets.bil'):
+                # from topsApp.py
+                no_data_value = -10000.
+            elif fname.endswith('_denseoffset.off'):
+                # from alos2App.py
+                no_data_value = 0.
+            else:
+                no_data_value = None
 
         else:
             # default value for unknown file types
             no_data_value = None
 
     return str(no_data_value).lower()
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/s1_utils.py` & `mintpy-1.6.0/src/mintpy/utils/s1_utils.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/solvers/l1.py` & `mintpy-1.6.0/src/mintpy/utils/solvers/l1.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/solvers/l1regls.py` & `mintpy-1.6.0/src/mintpy/utils/solvers/l1regls.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/solvers/lstl1.py` & `mintpy-1.6.0/src/mintpy/utils/solvers/lstl1.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/time_func.py` & `mintpy-1.6.0/src/mintpy/utils/time_func.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/utils.py` & `mintpy-1.6.0/src/mintpy/legacy/tropo_pyaps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,489 +1,520 @@
-"""Miscellaneous utilities - dependent on utils0/1."""
+#!/usr/bin/env python
 ############################################################
 # Program is part of MintPy                                #
 # Copyright (c) 2013, Zhang Yunjun, Heresh Fattahi         #
-# Author: Zhang Yunjun, Heresh Fattahi, 2013               #
+# Author: Heresh Fattahi, Zhang Yunjun, 2015               #
 ############################################################
-# Recommend import:
-#   from mintpy.utils import utils as ut
 
 
-import errno
+import argparse
 import os
+import re
+import sys
 
 import numpy as np
-from scipy.ndimage import map_coordinates
 
-from mintpy.objects import (
-    GEOMETRY_DSET_NAMES,
-    geometry,
-    ifgramStack,
-    timeseries,
-)
-from mintpy.objects.coord import coordinate
-from mintpy.objects.resample import resample
-from mintpy.utils import attribute as attr, ptime, readfile
-from mintpy.utils.utils0 import *
-from mintpy.utils.utils1 import *
-
-
-#################################################################################
-def check_loaded_dataset(work_dir='./', print_msg=True, relpath=False):
-    """Check the loaded input files, following two rules:
-        1. file existence
-        2. file attribute readability
-
-    Parameters: work_dir    - str, MintPy working directory
-                print_msg   - bool, print out message
-    Returns:    stack_file  - str, path to the interferogram stack file
-                geom_file   - str, path to the geometry file
-                lookup_file - str, path to the look up table file, for radar-coord dataset only.
-                ion_file    - str, path to the ionosphere stack file
-    Example:    work_dir = os.path.expandvars('./FernandinaSenDT128/mintpy')
-                stack_file, geom_file, lookup_file = ut.check_loaded_dataset(work_dir)[:3]
-    """
-    if not work_dir:
-        work_dir = os.getcwd()
-    work_dir = os.path.abspath(work_dir)
-
-    # tips for prep_aria
-    template_file = os.path.join(work_dir, 'smallbaselineApp.cfg')
-    proc = readfile.read_template(template_file)['mintpy.load.processor']
-    if proc == 'aria':
-        msg_aria = '. Re-run "prep_aria.py" as printed out in "load_data" step for more information!'
-    else:
-        msg_aria = ''
+try:
+    import pyaps as pa
+except ImportError:
+    raise ImportError('Cannot import pyaps!')
+
+import mintpy.cli.diff
+from mintpy.objects import geometry, timeseries
+from mintpy.utils import ptime, readfile, utils as ut, writefile
+
+standardWeatherModelNames = {
+    'ERAI': 'ECMWF', 'ERAINT': 'ECMWF', 'ERAINTERIM': 'ECMWF',
+    'MERRA2': 'MERRA',
+}
+
+
+###############################################################
+EXAMPLE = """example:
+  # download reanalysys dataset, calculate tropospheric delays and correct time-series file.
+  tropo_pyaps.py -f timeseries.h5 -m ECMWF -g inputs/geometryRadar.h5 -w ${WEATHER_DIR}
+
+  # download reanalysys dataset, calculate tropospheric delays
+  tropo_pyaps.py -d date_list.txt     --hour 12 -m ECMWF -g inputs/geometryRadar.h5 --ref-yx 30 40
+  tropo_pyaps.py -d 20151002 20151003 --hour 12 -m MERRA -g inputs/geometryRadar.h5 --ref-yx 30 40
+
+  # download reanalysys dataset
+  tropo_pyaps.py -d date_list.txt     --hour 12 -m ECMWF
+"""
+
+REFERENCE = """reference:
+  Jolivet, R., R. Grandin, C. Lasserre, M.-P. Doin and G. Peltzer (2011), Systematic InSAR tropospheric
+  phase delay corrections from global meteorological reanalysis data, Geophys. Res. Lett., 38, L17311,
+  doi:10.1029/2011GL048757
+
+  Jolivet, R., P. S. Agram, N. Y. Lin, M. Simons, M. P. Doin, G. Peltzer, and Z. Li (2014), Improving
+  InSAR geodesy using global atmospheric models, Journal of Geophysical Research: Solid Earth, 119(3),
+  2324-2341.
+"""
+
+DATA_INFO = """
+  re-analysis_dataset        coverage   temporal_resolution    spatial_resolution      latency     analysis
+------------------------------------------------------------------------------------------------------------
+ERA-Interim (by ECMWF)        Global      00/06/12/18 UTC      0.75 deg (~83 km)       2-month      4D-var
+MERRA(2) (by NASA Goddard)    Global      00/06/12/18 UTC      0.5*0.625 (~50 km)     2-3 weeks     3D-var
+
+To download MERRA2, you need an Earthdata account, and pre-authorize the "NASA GESDISC DATA ARCHIVE" application
+    following https://disc.gsfc.nasa.gov/earthdata-login.
+"""
+
+WEATHER_DIR_DEMO = """--weather-dir ~/data/aux
+WEATHER/
+    /ECMWF
+        ERA-Int_20030329_06.grb
+        ERA-Int_20030503_06.grb
+    /MERRA
+        merra-20110126-06.nc4
+        merra-20110313-06.nc4
+"""
+
+
+def create_parser():
+    parser = argparse.ArgumentParser(description='Tropospheric correction using weather models\n' +
+                                     '  PyAPS is used to download and calculate the delay for each time-series epoch.',
+                                     formatter_class=argparse.RawTextHelpFormatter,
+                                     epilog=REFERENCE+'\n'+DATA_INFO+'\n'+EXAMPLE)
+    # For data download
+    parser.add_argument('-m', '--model', '-s', dest='trop_model', default='ECMWF',
+                        choices={'ECMWF', 'MERRA', 'NARR', 'ERA', 'MERRA1'},
+                        help='source of the atmospheric data.\nNARR is working for 1979-Jan to 2014-Oct.')
+    parser.add_argument('-d', '--date-list', dest='date_list', nargs='*',
+                        help='Read the first column of text file as list of date to download data\n' +
+                             'in YYYYMMDD or YYMMDD format')
+    parser.add_argument('--hour', help='time of data in HH, e.g. 12, 06')
+    parser.add_argument('-w', '--dir', '--weather-dir', dest='weather_dir', default='${WEATHER_DIR}',
+                        help='parent directory of downloaded weather data file. Default: ${WEATHER_DIR}\n' +
+                             'e.g.: '+WEATHER_DIR_DEMO)
+
+    # For delay calculation
+    parser.add_argument('-g','--geomtry', dest='geom_file', type=str,
+                        help='geometry file including height, incidenceAngle and/or latitude and longitude')
+    parser.add_argument('--ref-yx', dest='ref_yx', type=int,
+                        nargs=2, help='reference pixel in y/x')
+    parser.add_argument('--delay', dest='delay_type', default='comb', choices={'comb', 'dry', 'wet'},
+                        help='Delay type to calculate, comb contains both wet and dry delays')
+
+    # For delay correction
+    parser.add_argument('-f', '--file', dest='timeseries_file',
+                        help='timeseries HDF5 file, i.e. timeseries.h5')
+    parser.add_argument('-o', dest='outfile',
+                        help='Output file name for trospheric corrected timeseries.')
+    return parser
+
+
+def cmd_line_parse(iargs=None):
+    """Command line parser."""
+    parser = create_parser()
+    inps = parser.parse_args(args=iargs)
+
+    # check the input requirements
+    key_list = ['date_list', 'hour']
+    # with timeseries file
+    if inps.timeseries_file:
+        for key in key_list+['ref_yx']:
+            if vars(inps)[key]:
+                print(('input "{:<10}" is ignored because it will be extracted from '
+                       'timeseries file {}').format(key, inps.timeseries_file))
+
+    # without timeseries file
+    elif any(not vars(inps)[key] for key in key_list):
+        msg = f'No input timeseries file, all the following options are required: \n{key_list}'
+        msg += '\n\n'+EXAMPLE
+        raise ValueError(msg)
 
-    # 1. [required] interferograms stack file: unwrapPhase, coherence
-    stack_file = os.path.join(work_dir, 'inputs/ifgramStack.h5')
-    dnames = ['unwrapPhase', 'rangeOffset', 'azimuthOffset']
-
-    if is_file_exist(stack_file, abspath=True):
-        obj = ifgramStack(stack_file)
-        obj.open(print_msg=False)
-
-        if all(x not in obj.datasetNames for x in dnames):
-            msg = f'required dataset is missing in file {stack_file}:\n'
-            msg += ' OR '.join(dnames)
-            raise ValueError(msg)
-
-        # check coherence for phase stack
-        if 'unwrapPhase' in obj.datasetNames and 'coherence' not in obj.datasetNames:
-            print(f'WARNING: "coherence" is missing in file {stack_file}')
-    else:
-        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), stack_file + msg_aria)
 
-    # get coordinate type of the loaded dataset
-    atr = readfile.read_attribute(stack_file)
-    coord_type = 'GEO' if 'Y_FIRST' in atr.keys() else 'RADAR'
-    processor = atr['PROCESSOR']
-
-    # 2. [required] geom_file: height
-    geom_file = os.path.join(work_dir, 'inputs', f'geometry{coord_type.capitalize()}.h5')
-    dname = GEOMETRY_DSET_NAMES[0]
-
-    if is_file_exist(geom_file, abspath=True):
-        obj = geometry(geom_file)
-        obj.open(print_msg=False)
-        if dname not in obj.datasetNames:
-            raise ValueError(f'required dataset "{dname}" is missing in file {geom_file}')
+    ## default values
+    # Get Grib Source
+    inps.trop_model = standardize_trop_model(inps.trop_model, standardWeatherModelNames)
+    print('weather model: '+inps.trop_model)
+
+    # weather_dir
+    inps.weather_dir = os.path.expanduser(inps.weather_dir)
+    inps.weather_dir = os.path.expandvars(inps.weather_dir)
+    # Fallback value if WEATHER_DIR is not defined as environment variable
+    if inps.weather_dir == '${WEATHER_DIR}':
+        inps.weather_dir = './'
+    print('weather data directory: '+inps.weather_dir)
+
+    return inps
+
+
+###############################################################
+def check_inputs(inps):
+    parser = create_parser()
+
+    # output directories/files
+    atr = dict()
+    mintpy_dir = None
+    if inps.timeseries_file:
+        atr = readfile.read_attribute(inps.timeseries_file)
+        mintpy_dir = os.path.dirname(inps.timeseries_file)
+        if not inps.outfile:
+            fbase = os.path.splitext(inps.timeseries_file)[0]
+            inps.outfile = f'{fbase}_{inps.trop_model}.h5'
+    elif inps.geom_file:
+        atr = readfile.read_attribute(inps.geom_file)
+        mintpy_dir = os.path.join(os.path.dirname(inps.geom_file), '..')
     else:
-        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), geom_file + msg_aria)
+        mintpy_dir = os.path.abspath(os.getcwd())
 
-    # 3. [required for radar-coord] lookup_file: latitude,longitude or rangeCoord,azimuthCoord
-    # could be different than geometry file in case of roipac and gamma
-    lookup_file = os.path.join(work_dir, 'inputs/geometry*.h5')
-    lookup_file = get_lookup_file(lookup_file, abspath=True, print_msg=print_msg)
-    if coord_type == 'RADAR':
-        if lookup_file is not None:
-            obj = geometry(lookup_file)
-            obj.open(print_msg=False)
-
-            # get the proper lookup table dataset names
-            if processor in ['isce', 'doris']:
-                dnames = GEOMETRY_DSET_NAMES[1:3]
-            elif processor in ['gamma', 'roipac']:
-                dnames = GEOMETRY_DSET_NAMES[3:5]
-            else:
-                msg = f'Unknown InSAR processor: {processor} to locate look up table!'
-                raise AttributeError(msg)
-
-            for dname in dnames:
-                if dname not in obj.datasetNames:
-                    raise Exception(f'required dataset "{dname}" is missing in file {lookup_file}')
+    # trop_file
+    inps.trop_file = os.path.join(mintpy_dir, f'inputs/{inps.trop_model}.h5')
+    print(f'output tropospheric delay file: {inps.trop_file}')
+
+    # hour
+    if not inps.hour:
+        if 'CENTER_LINE_UTC' in atr.keys():
+            inps.hour = closest_weather_product_time(atr['CENTER_LINE_UTC'], inps.trop_model)
         else:
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), lookup_file)
-    else:
-        print("Input data seems to be geocoded. Lookup file not needed.")
+            parser.print_usage()
+            raise Exception('no input for hour')
+    print(f'time of cloest available product: {inps.hour}:00 UTC')
+
+    # date list
+    if inps.timeseries_file:
+        print(f'read date list from timeseries file: {inps.timeseries_file}')
+        ts_obj = timeseries(inps.timeseries_file)
+        ts_obj.open(print_msg=False)
+        inps.date_list = ts_obj.dateList
+    elif len(inps.date_list) == 1:
+        if os.path.isfile(inps.date_list[0]):
+            print(f'read date list from text file: {inps.date_list[0]}')
+            inps.date_list = ptime.yyyymmdd(np.loadtxt(inps.date_list[0],
+                                                       dtype=bytes,
+                                                       usecols=(0,)).astype(str).tolist())
+        else:
+            parser.print_usage()
+            raise Exception('ERROR: input date list < 2')
 
-    # 4. [optional] ionosphere stack file: unwrapPhase, coherence
-    ion_file = os.path.join(work_dir, 'inputs/ionStack.h5')
-    dname = 'unwrapPhase'
-
-    if is_file_exist(ion_file, abspath=True):
-        obj = ifgramStack(ion_file)
-        obj.open(print_msg=False)
-        if dname not in obj.datasetNames:
-            raise ValueError(f'required dataset "{dname}" is missing in file {ion_file}')
-
-        # check coherence for phase stack
-        if 'unwrapPhase' in obj.datasetNames and 'coherence' not in obj.datasetNames:
-            print(f'WARNING: "coherence" is missing in file {ion_file}')
-    else:
-        ion_file = None
+    # Grib data directory
+    inps.grib_dir = os.path.join(inps.weather_dir, inps.trop_model)
+    if not os.path.isdir(inps.grib_dir):
+        os.makedirs(inps.grib_dir)
+        print('making directory: '+inps.grib_dir)
+
+    # Date list to grib file list
+    inps.grib_file_list = date_list2grib_file(inps.date_list,
+                                              inps.hour,
+                                              inps.trop_model,
+                                              inps.grib_dir)
+
+    if 'REF_Y' in atr.keys():
+        inps.ref_yx = [int(atr['REF_Y']), int(atr['REF_X'])]
+        print(f'reference pixel: {inps.ref_yx}')
 
-    if relpath:
-        stack_file  = os.path.relpath(stack_file)  if stack_file  else stack_file
-        geom_file   = os.path.relpath(geom_file)   if geom_file   else geom_file
-        lookup_file = os.path.relpath(lookup_file) if lookup_file else lookup_file
-        ion_file    = os.path.relpath(ion_file)    if ion_file    else ion_file
-
-    # print message
-    if print_msg:
-        msg  = f'Loaded dataset are processed by InSAR software: {processor}'
-        msg += f'\nLoaded dataset are in {coord_type} coordinates'
-        msg += f'\nInterferogram Stack: {stack_file}'
-        msg += f'\nIonosphere    Stack: {ion_file}' if ion_file else ''
-        msg += f'\nGeometry      File : {geom_file}'
-        msg += f'\nLookup Table  File : {lookup_file}'
-        msg += '\n' + '-' * 50
-        print(msg)
-
-    return stack_file, geom_file, lookup_file, ion_file
-
-
-#################################################################################
-def read_timeseries_lalo(lat, lon, ts_file, lookup_file=None, ref_lat=None, ref_lon=None,
-                         zero_first=True, win_size=1, unit='m', method='mean', print_msg=True):
-    """ Read time-series of one pixel with input lat/lon
-    Parameters: lat/lon     - float, latitude/longitude
-                ts_file     - string, filename of time-series HDF5 file
-                lookup_file - string, filename of lookup table file
-                ref_lat/lon - float, latitude/longitude of reference pixel
-                zero_first  - bool, shift the time-series so that it starts from zero
-                win_size    - int, windows size centered at point of interest
-                unit        - str, output displacement unit
-                method      - str, method to calculate the output displacement and its dispersity
-    Returns:    dates       - 1D np.ndarray of datetime.datetime objects, i.e. datetime.datetime(2010, 10, 20, 0, 0)
-                dis         - 1D np.ndarray of float32, displacement
-                dis_std     - 1D np.ndarray of float32, displacement dispersity
-    """
-    atr = readfile.read_attribute(ts_file)
-    coord = coordinate(atr, lookup_file=lookup_file)
-    y, x = coord.geo2radar(lat, lon)[0:2]
-    if print_msg:
-        print(f'input lat / lon: {lat} / {lon}')
-        print(f'corresponding y / x: {y} / {x}')
-
-    # reference pixel
-    ref_y, ref_x = None, None
-    if ref_lat is not None:
-        ref_y, ref_x = coord.geo2radar(ref_lat, ref_lon)[0:2]
-
-    # call read_timeseries_yx()
-    dates, dis, dis_std = read_timeseries_yx(y, x, ts_file,
-                                             ref_y=ref_y,
-                                             ref_x=ref_x,
-                                             zero_first=zero_first,
-                                             win_size=win_size,
-                                             unit=unit,
-                                             method=method,
-                                             print_msg=False)
-    return dates, dis, dis_std
-
-
-def read_timeseries_yx(y, x, ts_file, ref_y=None, ref_x=None, zero_first=True,
-                       win_size=1, unit='m', method='mean', print_msg=True):
-    """ Read time-series of one pixel with input y/x
-    Parameters: y/x        - int, row/column number of interest
-                ts_file    - string, filename of time-series HDF5 file
-                ref_y/x    - int, row/column number of reference pixel
-                zero_first - bool, shift the time-series so that it starts from zero
-                win_size   - int, windows size centered at point of interest
-                unit       - str, output displacement unit
-                method     - str, method to calculate the output displacement and its dispersity
-    Returns:    dates      - 1D np.ndarray of datetime.datetime objects, i.e. datetime.datetime(2010, 10, 20, 0, 0)
-                dis        - 1D np.ndarray of float32, displacement
-                dis_std    - 1D np.ndarray of float32, displacement dispersity
-    """
-    # read date
-    obj = timeseries(ts_file)
-    obj.open(print_msg=False)
-    dates = ptime.date_list2vector(obj.dateList)[0]
-    dates = np.array(dates)
-
-    # read displacement
-    if print_msg:
-        print(f'input y / x: {y} / {x}')
-    box = (x, y, x+1, y+1)
-    dis = readfile.read(ts_file, box=box)[0]
-    dis_std = None
-
-    if win_size != 1:
-        buf = int(win_size / 2)
-        box_win = (x-buf, y-buf, x+buf+1, y+buf+1)
-        dis_win = readfile.read(ts_file, box=box_win)[0].reshape(obj.numDate, -1)
-
-        if method == 'mean':
-            dis = np.nanmean(dis_win, axis=1)
-            dis_std = np.nanstd(dis_win, axis=1)
-
-        elif method == 'median':
-            dis = np.nanmedian(dis_win, axis=1)
-            dis_std = median_abs_deviation(dis_win)
+    # Coordinate system: geocoded or not
+    inps.geocoded = False
+    if 'Y_FIRST' in atr.keys():
+        inps.geocoded = True
+    print(f'geocoded: {inps.geocoded}')
 
+    # Prepare DEM, inc_angle, lat/lon file for PyAPS to read
+    if inps.geom_file:
+        geom_obj = geometry(inps.geom_file)
+        geom_obj.open()
+
+        print('converting DEM/incAngle for PyAPS to read')
+        # DEM
+        dem = readfile.read(inps.geom_file, datasetName='height', print_msg=False)[0]
+        inps.dem_file = 'pyapsDem.hgt'
+        writefile.write(dem, inps.dem_file, metadata=atr)
+
+        # inc_angle
+        if 'incidenceAngle' in geom_obj.datasetNames:
+            inps.inc_angle = readfile.read(inps.geom_file, datasetName='incidenceAngle', print_msg=False)[0]
+        else:
+            atr = readfile.read_attribute(inps.timeseries_file)
+            inps.inc_angle = ut.incidence_angle(atr, dem=dem, dimension=0)
+            inps.inc_angle = np.ones(dem.shape, dtype=np.float32) * inps.inc_angle
+        inps.inc_angle_file = 'pyapsIncAngle.flt'
+        writefile.write(inps.inc_angle, inps.inc_angle_file, metadata=atr)
+
+        # latitude
+        if 'latitude' in geom_obj.datasetNames:
+            data = readfile.read(inps.geom_file, datasetName='latitude', print_msg=False)[0]
+            print('converting lat for PyAPS to read')
+            inps.lat_file = 'pyapsLat.flt'
+            writefile.write(data, inps.lat_file, metadata=atr)
         else:
-            raise ValueError(f'un-recognized method: {method}')
+            inps.lat_file = None
 
-    # reference pixel
-    if ref_y is not None:
-        ref_box = (ref_x, ref_y, ref_x+1, ref_y+1)
-        dis -= readfile.read(ts_file, box=ref_box)[0]
-
-    #start at zero
-    if zero_first:
-        dis -= dis[0]
-
-    # custom output unit
-    if unit == 'm':
-        pass
-    elif unit == 'cm':
-        dis *= 100.
-        dis_std = None if dis_std is None else dis_std * 100.
-    elif unit == 'mm':
-        dis *= 1000.
-        dis_std = None if dis_std is None else dis_std * 1000.
-    else:
-        raise ValueError(f'un-supported output unit: {unit}')
+        # longitude
+        if 'longitude' in geom_obj.datasetNames:
+            data = readfile.read(inps.geom_file, datasetName='longitude', print_msg=False)[0]
+            print('converting lon for PyAPS to read')
+            inps.lon_file = 'pyapsLon.flt'
+            writefile.write(data, inps.lon_file, metadata=atr)
+        else:
+            inps.lon_file = None
+    return inps, atr
 
-    return dates, dis, dis_std
 
+###############################################################
+def closest_weather_product_time(sar_acquisition_time, grib_source='ECMWF'):
+    """Find closest available time of weather product from SAR acquisition time
+    Inputs:
+        sar_acquisition_time - string, SAR data acquisition time in seconds
+        grib_source - string, Grib Source of weather reanalysis product
+    Output:
+        grib_hr - string, time of closest available weather product
+    Example:
+        '06' = closest_weather_product_time(atr['CENTER_LINE_UTC'])
+        '12' = closest_weather_product_time(atr['CENTER_LINE_UTC'], 'NARR')
+    """
+    # Get hour/min of SAR acquisition time
+    sar_time = float(sar_acquisition_time)
 
-#####################################################################
-def transect_yx(z, atr, start_yx, end_yx, interpolation='nearest'):
-    """Extract 2D matrix (z) value along the line [x0,y0;x1,y1]
-    Link: http://stackoverflow.com/questions/7878398/how-to-extract-an-arbitrary-line-of-values-from-a-numpy-array
-
-    Parameters: z : (np.array) 2D data matrix
-                atr : (dict) attribute
-                start_yx : (list) y,x coordinate of start point
-                end_yx : (list) y,x coordinate of end   point
-                interpolation : str, sampling/interpolation method, including:
-                    'nearest' - nearest neighbour
-                    'linear'  - linear  spline interpolation (order of 1)
-                    'cubic'   - cubic   spline interpolation (order of 3)
-                    'quintic' - quintic spline interpolation (order of 5)
-
-    Returns:    transect: (dict) containing 1D matrix:
-                    'X' - 1D np.array for X/column coordinates in float32
-                    'Y' - 1D np.array for Y/row.   coordinates in float32
-                    'value' - 1D np.array for z value in float32
-                    'distance' - 1D np.array for distance in float32
+    # Find closest time in available weather products
+    grib_hr_list = [0, 6, 12, 18]
+    grib_hr = int(min(grib_hr_list, key=lambda x: abs(x-sar_time/3600.)))
+
+    # Adjust time output format
+    grib_hr = "%02d" % grib_hr
+    return grib_hr
+
+
+def standardize_trop_model(tropModel, standardWeatherModelNames):
+    tropModel = tropModel.replace('-', '').upper()
+    if tropModel in standardWeatherModelNames.keys():
+        tropModel = standardWeatherModelNames[tropModel]
+    return tropModel
+
+
+def date_list2grib_file(date_list, hour, trop_model, grib_dir):
+    grib_file_list = []
+    for d in date_list:
+        grib_file = grib_dir+'/'
+        if   trop_model == 'ECMWF' :  grib_file += f'ERA-Int_{d}_{hour}.grb'
+        elif trop_model == 'MERRA' :  grib_file += f'merra-{d}-{hour}.nc4'
+        elif trop_model == 'NARR'  :  grib_file += f'narr-a_221_{d}_{hour}00_000.grb'
+        elif trop_model == 'ERA'   :  grib_file += f'ERA_{d}_{hour}.grb'
+        elif trop_model == 'MERRA1':  grib_file += f'merra-{d}-{hour}.hdf'
+        grib_file_list.append(grib_file)
+    return grib_file_list
+
+
+def grib_file_name2trop_model_name(grib_file):
+    grib_file = os.path.basename(grib_file)
+    if grib_file.startswith('ERA-Int'):  trop_model = 'ECMWF'
+    elif grib_file.startswith('merra'):  trop_model = 'MERRA'
+    elif grib_file.startswith('narr'):   trop_model = 'NARR'
+    elif grib_file.startswith('ERA_'):   trop_model = 'ERA'
+    return trop_model
+
+
+def check_exist_grib_file(gfile_list, print_msg=True):
+    """Check input list of grib files, and return the existing ones with right size."""
+    gfile_exist = ut.get_file_list(gfile_list)
+    if gfile_exist:
+        file_sizes = [os.path.getsize(i) for i in gfile_exist
+                      if os.path.getsize(i) > 10e6]
+        if file_sizes:
+            comm_size = ut.most_common([i for i in file_sizes])
+            if print_msg:
+                print(f'common file size: {comm_size} bytes')
+                print(f'number of grib files existed    : {len(gfile_exist)}')
+
+            gfile_corrupt = []
+            for gfile in gfile_exist:
+                if os.path.getsize(gfile) < comm_size * 0.9:
+                    gfile_corrupt.append(gfile)
+        else:
+            gfile_corrupt = gfile_exist
 
-    Example: transect = transect_yx(dem, demRsc, [10,15], [100,115])
+        if gfile_corrupt:
+            if print_msg:
+                print('------------------------------------------------------------------------------')
+                print('corrupted grib files detected! Delete them and re-download...')
+                print(f'number of grib files corrupted  : {len(gfile_corrupt)}')
+
+            for gfile in gfile_corrupt:
+                os.remove(gfile)
+                gfile_exist.remove(gfile)
+
+            if print_msg:
+                print('------------------------------------------------------------------------------')
+    return gfile_exist
+
+
+def dload_grib_pyaps(grib_file_list):
+    """Download weather re-analysis grib files using PyAPS
+    Parameters: grib_file_list : list of string of grib files
+    Returns:    grib_file_list : list of string
     """
-    interpolation = interpolation.lower()
-    [y0, x0] = start_yx
-    [y1, x1] = end_yx
-
-    # check
-    length, width = int(atr['LENGTH']), int(atr['WIDTH'])
-    if not all(0<= i < width and 0<= j < length for i,j in zip([x0,x1], [y0,y1])):
-        msg = 'input start/end point is out of data coverage'
-        msg += f'\nstart_yx: {start_yx}'
-        msg += f'\nend_yx:{end_yx}'
-        msg += f'\ndata size: ({length}, {width})'
-        raise ValueError(msg)
-
-    # Determine points coordinates along the line
-    num_pts = int(np.hypot(x1-x0, y1-y0))
-    ys = np.linspace(y0, y1, num_pts, dtype=np.float32)
-    xs = np.linspace(x0, x1, num_pts, dtype=np.float32)
-
-    # Extract z value along the line
-    # for nearest neighbor sampling, use indexing directly
-    # for other interpolation, use scipy.ndimage.map_coordinates
-    if interpolation == 'nearest':
-        z_line = z[np.rint(ys).astype(int), np.rint(xs).astype(int)]
+    print('\n------------------------------------------------------------------------------')
+    print('downloading weather model data using PyAPS ...')
 
+    # Get date list to download (skip already downloaded files)
+    grib_file_exist = check_exist_grib_file(grib_file_list, print_msg=True)
+    grib_file2dload = sorted(list(set(grib_file_list) - set(grib_file_exist)))
+    date_list2dload = [str(re.findall(r'\d{8}', i)[0]) for i in grib_file2dload]
+    print('number of grib files to download: %d' % len(date_list2dload))
+    print('------------------------------------------------------------------------------\n')
+
+    # Download grib file using PyAPS
+    if len(date_list2dload) > 0:
+        hour = re.findall(r'\d{8}[-_]\d{2}', grib_file2dload[0])[0].replace('-', '_').split('_')[1]
+        grib_dir = os.path.dirname(grib_file2dload[0])
+
+        # try 3 times to download, then use whatever downloaded to calculate delay
+        trop_model = grib_file_name2trop_model_name(grib_file2dload[0])
+        i = 0
+        while i < 3:
+            i += 1
+            try:
+                if   trop_model == 'ECMWF' :  pa.ECMWFdload( date_list2dload, hour, grib_dir)
+                elif trop_model == 'MERRA' :  pa.MERRAdload( date_list2dload, hour, grib_dir)
+                elif trop_model == 'NARR'  :  pa.NARRdload(  date_list2dload, hour, grib_dir)
+                elif trop_model == 'ERA'   :  pa.ERAdload(   date_list2dload, hour, grib_dir)
+                elif trop_model == 'MERRA1':  pa.MERRA1dload(date_list2dload, hour, grib_dir)
+            except:
+                pass
+
+    grib_file_list = check_exist_grib_file(grib_file_list, print_msg=False)
+    return grib_file_list
+
+
+def get_delay(grib_file, inps):
+    """Get delay matrix using PyAPS for one acquisition
+    Inputs:
+        grib_file - string, grib file path
+        atr       - dict, including the following attributes:
+                    dem_file    - string, DEM file path
+                    trop_model - string, Weather re-analysis data source
+                    delay_type  - string, comb/dry/wet
+                    ref_y/x     - string, reference pixel row/col number
+                    inc_angle   - np.array, 0/1/2 D
+    Output:
+        phs - 2D np.array, absolute tropospheric phase delay relative to ref_y/x
+    """
+    # initiate pyaps object
+    if inps.geocoded:
+        aps = pa.PyAPS_geo(grib_file, inps.dem_file, grib=inps.trop_model,
+                           demtype=np.float32, demfmt='RMG',
+                           verb=False, Del=inps.delay_type)
     else:
-        # interpolation name to order
-        interpolate_name2order = {
-            'linear' : 1,
-            'cubic'  : 3,
-            'quintic': 5,
-        }
-        if interpolation not in interpolate_name2order.keys():
-            msg = f'un-supported interpolation method: {interpolation}'
-            msg += f'\navailable methods: {interpolate_name2order.keys()}'
-            raise ValueError(msg)
-        interp_order = interpolate_name2order[interpolation.lower()]
-        # run interpolation
-        z_line = map_coordinates(z, np.vstack((ys, xs)), order=interp_order)
-
-    # Calculate Distance along the line
-    earth_radius = 6.3781e6    # in meter
-    dist_unit = 'm'
-    if 'Y_FIRST' in atr.keys():
-        [lat0, lat1] = coordinate(atr).yx2lalo([y0, y1], coord_type='y')
-        lat_c = (lat0 + lat1) / 2.
-        x_step = float(atr['X_STEP']) * np.pi/180.0 * earth_radius * np.cos(lat_c * np.pi/180)
-        y_step = float(atr['Y_STEP']) * np.pi/180.0 * earth_radius
+        aps = pa.PyAPS_rdr(grib_file, inps.dem_file, grib=inps.trop_model,
+                           demtype=np.float32, demfmt='RMG',
+                           verb=False, Del=inps.delay_type)
+
+    # estimate delay
+    phs = np.zeros((aps.ny, aps.nx), dtype=np.float32)
+    if not inps.geocoded and inps.lat_file is not None:
+        aps.getgeodelay(phs,
+                        lat=inps.lat_file,
+                        lon=inps.lon_file,
+                        inc=inps.inc_angle_file)
     else:
-        try:
-            x_step = range_ground_resolution(atr)
-            y_step = azimuth_ground_resolution(atr)
-        except KeyError:
-            x_step = 1
-            y_step = 1
-            dist_unit = 'pixel'
-    dist_line = np.hypot((xs - x0) * x_step,
-                         (ys - y0) * y_step)
-
-    # remove points in masked out areas
-    mask = ~np.isnan(z_line)
-    mask *= z_line != 0.0
-
-    # prepare output
-    transect = {}
-    transect['Y'] = ys[mask]
-    transect['X'] = xs[mask]
-    transect['value'] = z_line[mask]
-    transect['distance'] = dist_line[mask]
-    transect['distance_unit'] = dist_unit
-
-    return transect
-
-
-def transect_lalo(z, atr, start_lalo, end_lalo, interpolation='nearest'):
-    """Extract 2D matrix (z) value along the line [start_lalo, end_lalo]"""
-    coord = coordinate(atr)
-    [y0, y1] = coord.lalo2yx([start_lalo[0], end_lalo[0]], coord_type='lat')
-    [x0, x1] = coord.lalo2yx([start_lalo[1], end_lalo[1]], coord_type='lon')
-    transect = transect_yx(z, atr, [y0, x0], [y1, x1], interpolation)
-    return transect
-
-
-def transect_lines(z, atr, lines):
-    """Extract 2D matrix (z) value along multiple lines
-    Parameters: z     : 2D np.ndarray in size of (l,w)
-                atr   : dict, metadata of matrix z
-                lines : list of lines with each line is defined as:
-                    [[lat0, lon0], [lat1, lon1]] for geo coordinates
-                    [[y0, x0], [y1, x1]] for radar coordinates
-    Returns: transect : (dict) containing 1D matrix:
-                    'X' - 1D np.array for X/column coordinates in float32
-                    'Y' - 1D np.array for Y/row.   coordinates in float32
-                    'value' - 1D np.array for z value in float32
-                    'distance' - 1D np.array for distance in float32
-    """
-    transect = {}
-    start_distance = 0
-    transect['start_distance'] = []
-
-    for i, line in enumerate(lines):
-        # read segment data
-        start_lalo, end_lalo = line[0], line[1]
-        if 'Y_FIRST' in atr.keys():
-            seg = transect_lalo(z, atr, start_lalo, end_lalo)
-        else:
-            seg = transect_yx(z, atr, start_lalo, end_lalo)
-        seg['distance'] += start_distance
-
-        # connect each segment
-        if i == 0:
-            # first segment
-            for key, value in seg.items():
-                transect[key] = np.array(value, dtype=np.float32)
-        else:
-            for key, value in seg.items():
-                transect[key] = np.concatenate((transect[key], value))
-
-        # update start_distance for the next segment
-        transect['start_distance'].append(start_distance)
-        start_distance = transect['distance'][-1]
-    transect['start_distance'] = np.array(transect['start_distance'], dtype=np.float32)
-    return transect
-
+        aps.getdelay(phs, inc=0.)
+        phs /= np.cos(inps.inc_angle*np.pi/180.)
 
+    # Get relative phase delay in space
+    phs -= phs[inps.ref_yx[0], inps.ref_yx[1]]
+    phs *= -1    # reverse the sign for consistency between different phase correction steps/methods
+    return phs
 
-#################################################################################
 
-def prepare_geo_los_geometry(geom_file, unit='rad'):
-    """Prepare LOS geometry data/info in geo-coordinates.
-
-    Parameters: geom_file - str, path of geometry file
-                unit      - str, rad or deg, output angle unit
-    Returns:    inc_angle - 2D np.ndarray, incidence angle in radians / degrees
-                            measured from the vertical
-                az_angle  - 2D np.ndarray, azimuth   angle in radians / degrees
-                            measured from the north with anti-clockwise direction as positive
-                atr       - dict, metadata in geo-coordinate
+def get_delay_timeseries(inps, atr):
+    """Calculate delay time-series and write it to HDF5 file.
+    Parameters: inps : namespace, all input parameters
+                atr  : dict, metadata to be saved in trop_file
+    Returns:    trop_file : str, file name of ECMWF.h5
     """
+    def get_dataset_size(fname):
+        atr = readfile.read_attribute(fname)
+        return (atr['LENGTH'], atr['WIDTH'])
+
+    if (ut.run_or_skip(out_file=inps.trop_file, in_file=inps.grib_file_list, print_msg=False) == 'skip'
+            and get_dataset_size(inps.trop_file) == get_dataset_size(inps.geom_file)):
+        print(f'{inps.trop_file} file exists and is newer than all GRIB files, skip updating.')
+    else:
+        if any(i is None for i in [inps.geom_file, inps.ref_yx]):
+            print('No DEM / incidenceAngle / ref_yx found, skip calculating tropospheric delays.')
+            if not os.path.isfile(inps.trop_file):
+                inps.trop_file = None
+            return
 
-    print(f'prepare LOS geometry in geo-coordinates from file: {geom_file}')
-    atr = readfile.read_attribute(geom_file)
+        # calculate phase delay
+        length, width = int(atr['LENGTH']), int(atr['WIDTH'])
+        num_date = len(inps.grib_file_list)
+        date_list = [str(re.findall(r'\d{8}', i)[0]) for i in inps.grib_file_list]
+        trop_data = np.zeros((num_date, length, width), np.float32)
+
+        print('calculating delay for each date using PyAPS (Jolivet et al., 2011; 2014) ...')
+        print(f'number of grib files used: {num_date}')
+        prog_bar = ptime.progressBar(maxValue=num_date)
+        for i in range(num_date):
+            grib_file = inps.grib_file_list[i]
+            trop_data[i] = get_delay(grib_file, inps)
+            prog_bar.update(i+1, suffix=os.path.basename(grib_file))
+        prog_bar.close()
 
-    print(f'read incidenceAngle from file: {geom_file}')
-    inc_angle = readfile.read(geom_file, datasetName='incidenceAngle')[0]
+        # Convert relative phase delay on reference date
+        try:
+            inps.ref_date = atr['REF_DATE']
+        except:
+            inps.ref_date = date_list[0]
+        print('convert to relative phase delay with reference date: '+inps.ref_date)
+        inps.ref_idx = date_list.index(inps.ref_date)
+        trop_data -= np.tile(trop_data[inps.ref_idx, :, :], (num_date, 1, 1))
+
+        # Write tropospheric delay to HDF5
+        atr['REF_Y'] = inps.ref_yx[0]
+        atr['REF_X'] = inps.ref_yx[1]
+        ts_obj = timeseries(inps.trop_file)
+        ts_obj.write2hdf5(data=trop_data,
+                          dates=date_list,
+                          metadata=atr,
+                          refFile=inps.timeseries_file)
+
+    # Delete temporary DEM file in ROI_PAC format
+    if inps.geom_file:
+        temp_files =[fname for fname in [inps.dem_file,
+                                         inps.inc_angle_file,
+                                         inps.lat_file,
+                                         inps.lon_file]
+                     if (fname is not None and 'pyaps' in fname)]
+        if temp_files:
+            print(f'delete temporary geometry files: {temp_files}')
+            for temp_file in temp_files:
+                os.remove(temp_file)
+                os.remove(temp_file+'.rsc')
+    return
+
+
+###############################################################
+def main(iargs=None):
+    inps = cmd_line_parse(iargs)
+    inps, atr = check_inputs(inps)
+
+    inps.grib_file_list = dload_grib_pyaps(inps.grib_file_list)
+
+    if inps.trop_file:
+        get_delay_timeseries(inps, atr)
+
+    if inps.dis_file:
+        print('\n'+'-'*80)
+        print('Applying tropospheric correction to displacement file...')
+        if ut.run_or_skip(inps.cor_dis_file, [inps.dis_file, inps.tropo_file]) == 'run':
+            # diff.py can handle different reference in space and time
+            # e.g. the absolute delay and the double referenced time-series
+            print('correcting delay for using diff.py')
+            iargs = [inps.timeseries_file, inps.tropo_file, '-o', inps.outfile, '--force']
+            print('diff.py', ' '.join(iargs))
+            mintpy.cli.diff.main(iargs)
 
-    if 'azimuthAngle' in readfile.get_dataset_list(geom_file):
-        print(f'read azimuthAngle   from file: {geom_file}')
-        az_angle  = readfile.read(geom_file, datasetName='azimuthAngle')[0]
+        else:
+            print(f'Skip re-applying and use existed corrected displacement file: {inps.cor_dis_file}.')
     else:
-        print('use the HEADING attribute as the mean heading angle')
-        print('convert heading angle to azimuth angle')
-        head_angle = np.ones(inc_angle.shape, dtype=np.float32) * float(atr['HEADING'])
-        az_angle = heading2azimuth_angle(head_angle)
-
-    # geocode inc/az angle data if in radar-coord
-    if 'Y_FIRST' not in atr.keys():
-        print('-'*50)
-        print('geocoding the incidence / heading angles ...')
-        res_obj = resample(lut_file=geom_file, src_file=geom_file)
-        res_obj.open()
-        res_obj.prepare()
-
-        # resample data
-        box = res_obj.src_box_list[0]
-        inc_angle = res_obj.run_resample(src_data=inc_angle[box[1]:box[3], box[0]:box[2]])
-        az_angle = res_obj.run_resample(src_data=az_angle[box[1]:box[3], box[0]:box[2]])
-
-        # update attribute
-        atr = attr.update_attribute4radar2geo(atr, res_obj=res_obj)
-
-    # for 'Y_FIRST' not in 'degree'
-    # e.g. meters for UTM projection from ASF HyP3
-    if not atr['Y_UNIT'].lower().startswith('deg'):
-        # get SNWE in meter
-        length, width = int(atr['LENGTH']), int(atr['WIDTH'])
-        N = float(atr['Y_FIRST'])
-        W = float(atr['X_FIRST'])
-        y_step = float(atr['Y_STEP'])
-        x_step = float(atr['X_STEP'])
-        S = N + y_step * length
-        E = W + x_step * width
-
-        # SNWE in meter --> degree
-        lat0, lon0 = utm2latlon(atr, W, N)
-        lat1, lon1 = utm2latlon(atr, E, S)
-        lat_step = (lat1 - lat0) / length
-        lon_step = (lon1 - lon0) / width
-
-        # update Y/X_FIRST/STEP/UNIT
-        atr['Y_FIRST'] = lat0
-        atr['X_FIRST'] = lon0
-        atr['Y_STEP'] = lat_step
-        atr['X_STEP'] = lon_step
-        atr['Y_UNIT'] = 'degrees'
-        atr['X_UNIT'] = 'degrees'
-
-    # set invalid values to nan
-    inc_angle[inc_angle == 0] = np.nan
-
-    # unit: degree to radian
-    if unit.startswith('rad'):
-        inc_angle *= np.pi / 180.
-        az_angle *= np.pi / 180.
+        print('No input displacement file, skip correcting tropospheric delays.')
+
+    return inps.outfile
+
 
-    return inc_angle, az_angle, atr
+###############################################################
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/utils0.py` & `mintpy-1.6.0/src/mintpy/utils/utils0.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,48 +100,58 @@
     """Calculate 2D matrix of incidence angle from ROI_PAC attributes, very accurate.
     Parameters: atr : dict - ROI_PAC attributes including the following items:
                      STARTING_RANGE
                      RANGE_PIXEL_SIZE
                      EARTH_RADIUS
                      HEIGHT
                      WIDTH
-                     LENGTH     #for dimension=2
+                     LENGTH                  #for dimension=2
+                     CENTER_INCIDENCE_ANGLE  #for dimension=0
                 dem : 2D array for height to calculate local incidence angle
                 dimension : int,
                             2 for 2d matrix
                             1 for 1d array
                             0 for one center value
                 print_msg : bool
     Returns:    inc_angle : 2D np.array, incidence angle in degree for each pixel
     Example:    dem = readfile.read('hgt.rdr')[0]
                 atr = readfile.read_attribute('filt_fine.unw')
                 inc_angle = ut.incidence_angle(atr, dem=dem)
     """
+    vprint = print if print_msg else lambda *args, **kwargs: None
+
     # Return center value for geocoded input file
     if 'Y_FIRST' in atr.keys() and dimension > 0:
         dimension = 0
-        if print_msg:
-            print('input file is geocoded, return center incident angle only')
+        vprint('input file is geocoded, return center incident angle only')
+
+    # Check if the center inc angle already exist in the metadata
+    # Notes on Mar 2024 by Alex Handwerger & Talib Oliver-Cabrera:
+    # Proposing these changes after encountering a range_n value smaller than the platform height
+    # for UAVSAR dataset swatch_00540, thus, the calc equation w/o considering topography won't work.
+    if dimension == 0 and 'CENTER_INCIDENCE_ANGLE' in atr.keys():
+        inc_angle = float(atr['CENTER_INCIDENCE_ANGLE'])
+        vprint(f'center incidence angle : {inc_angle:.4f} degree (grabbed from metadata directly)')
+        return inc_angle
 
     # Read Attributes
     range_n = float(atr['STARTING_RANGE'])
     dR = float(atr['RANGE_PIXEL_SIZE'])
     r = float(atr.get('EARTH_RADIUS', EARTH_RADIUS))
     H = float(atr['HEIGHT'])
     width = int(atr['WIDTH'])
 
     # Calculation
-    range_f = range_n+dR*width
+    range_f = range_n + dR * width
     inc_angle_n = (np.pi - np.arccos((r**2 + range_n**2 - (r+H)**2)/(2*r*range_n))) * 180.0/np.pi
     inc_angle_f = (np.pi - np.arccos((r**2 + range_f**2 - (r+H)**2)/(2*r*range_f))) * 180.0/np.pi
     inc_angle_c = (inc_angle_n + inc_angle_f) / 2.0
-    if print_msg:
-        print(f'near   incidence angle : {inc_angle_n:.4f} degree')
-        print(f'center incidence angle : {inc_angle_c:.4f} degree')
-        print(f'far    incidence angle : {inc_angle_f:.4f} degree')
+    vprint(f'near   incidence angle : {inc_angle_n:.4f} degree')
+    vprint(f'center incidence angle : {inc_angle_c:.4f} degree')
+    vprint(f'far    incidence angle : {inc_angle_f:.4f} degree')
 
     if dimension == 0:
         inc_angle = inc_angle_c
 
     elif dimension == 1:
         inc_angle = np.linspace(inc_angle_n, inc_angle_f, num=width,
                                 endpoint='FALSE', dtype=np.float32)
@@ -256,14 +266,18 @@
 
 
 
 ################################## Coordinate ##########################################
 def utm_zone2epsg_code(utm_zone):
     """Convert UTM Zone string to EPSG code.
 
+    Reference:
+        https://docs.up42.com/data/reference/utm#utm-wgs84
+        https://pyproj4.github.io/pyproj/stable/examples.html#initializing-crs
+
     Parameters: utm_zone  - str, atr['UTM_ZONE'], comprises a zone number
                             and a hemisphere, e.g. 11N, 36S, etc.
     Returns:    epsg_code - str, EPSG code
     Examples:   epsg_code = utm_zone2epsg_code('11N')
     """
     from pyproj import CRS
     crs = CRS.from_dict({
@@ -271,14 +285,35 @@
         'zone': int(utm_zone[:-1]),
         'south': utm_zone[-1].upper() == 'S',
     })
     epsg_code = crs.to_authority()[1]
     return epsg_code
 
 
+def epsg_code2utm_zone(epsg_code):
+    """Convert EPSG code to UTM Zone string.
+
+    Reference:
+        https://docs.up42.com/data/reference/utm#utm-wgs84
+        https://pyproj4.github.io/pyproj/stable/examples.html#initializing-crs
+
+    Parameters: epsg_code - str / int, EPSG code
+    Returns:    utm_zone  - str, atr['UTM_ZONE'], comprises a zone number
+                            and a hemisphere, e.g. 11N, 36S, etc. None for
+                            a EPSG code not in a UTM coordnate system
+    Examples:   utm_zone = epsg_code2utm_zone('32736')
+    """
+    from pyproj import CRS
+    crs = CRS.from_epsg(epsg_code)
+    utm_zone = crs.utm_zone
+    if not utm_zone:
+        print(f'WARNING: input EPSG code ({epsg_code}) is NOT a UTM zone, return None and continue.')
+    return utm_zone
+
+
 def to_latlon(infile, x, y):
     """Convert x, y in the projection coordinates of the file to lat/lon in degree.
 
     Similar functionality also exists in utm.to_latlon() at:
         https://github.com/Turbo87/utm#utm-to-latitudelongitude
 
     Parameters: infile - str, GDAL supported file path
@@ -306,40 +341,60 @@
 
 
 def utm2latlon(meta, easting, northing):
     """Convert UTM easting/northing in meters to lat/lon in degrees.
 
     Parameters: meta     - dict, mintpy attributes that includes:
                            UTM_ZONE
-                easting  - scalar or 1/2D np.ndarray, UTM    coordinates in x direction
-                northing - scalar or 1/2D np.ndarray, UTM    coordinates in y direction
-    Returns:    lat      - scalar or 1/2D np.ndarray, WGS 84 coordinates in y direction
-                lon      - scalar or 1/2D np.ndarray, WGS 84 coordinates in x direction
+                easting  - scalar/list/tuple/1-2D np.ndarray, UTM    coordinates in x direction
+                northing - scalar/list/tuple/1-2D np.ndarray, UTM    coordinates in y direction
+    Returns:    lat      - scalar/list/tuple/1-2D np.ndarray, WGS 84 coordinates in y direction
+                lon      - scalar/list/tuple/1-2D np.ndarray, WGS 84 coordinates in x direction
     """
     import utm
     zone_num = int(meta['UTM_ZONE'][:-1])
     northern = meta['UTM_ZONE'][-1].upper() == 'N'
     # set 'strict=False' to allow coordinates outside the range of a typical single UTM zone,
     # which can be common for large area analysis, e.g. the Norwegian mapping authority
     # publishes a height data in UTM zone 33 coordinates for the whole country, even though
     # most of it is technically outside zone 33.
-    lat, lon = utm.to_latlon(easting, northing, zone_num, northern=northern, strict=False)
+    lat, lon = utm.to_latlon(np.array(easting), np.array(northing), zone_num,
+                             northern=northern, strict=False)
+
+    # output format
+    if any(isinstance(x, (list, tuple)) for x in [easting, northing]):
+        lat = lat.tolist()
+        lon = lon.tolist()
+
     return lat, lon
 
 
-def latlon2utm(lat, lon):
+def latlon2utm(meta, lat, lon):
     """Convert latitude/longitude in degrees to UTM easting/northing in meters.
 
-    Parameters: lat      - scalar or 1/2D np.ndarray, WGS 84 coordinates in y direction
-                lon      - scalar or 1/2D np.ndarray, WGS 84 coordinates in x direction
-    Returns:    easting  - scalar or 1/2D np.ndarray, UTM    coordinates in x direction
-                northing - scalar or 1/2D np.ndarray, UTM    coordinates in y direction
+    Parameters: meta     - dict, mintpy attributes that includes:
+                           UTM_ZONE
+                lat      - scalar/list/tuple/1-2D np.ndarray, WGS 84 coordinates in y direction
+                lon      - scalar/list/tuple/1-2D np.ndarray, WGS 84 coordinates in x direction
+    Returns:    easting  - scalar/list/tuple/1-2D np.ndarray, UTM    coordinates in x direction
+                northing - scalar/list/tuple/1-2D np.ndarray, UTM    coordinates in y direction
     """
     import utm
-    return utm.from_latlon(lat, lon)[:2]
+
+    # invoke zone_num to ensure all coordinates are converted into the same single UTM zone,
+    # even if they cross a UTM boundary.
+    zone_num = int(meta['UTM_ZONE'][:-1])
+    easting, northing = utm.from_latlon(np.array(lat), np.array(lon), force_zone_number=zone_num)[:2]
+
+    # output format
+    if any(isinstance(x, (list, tuple)) for x in [lat, lon]):
+        easting = easting.tolist()
+        northing = northing.tolist()
+
+    return northing, easting
 
 
 def snwe_to_wkt_polygon(snwe):
     """Convert the input bounding box in SNWE into WKT format POLYGON.
 
     Parameters: snwe    - list of 4 float, south, north, west and east in degrees/meters
     Returns:    polygon - str, WKT format POLYGON
```

### Comparing `mintpy-1.5.3/src/mintpy/utils/utils1.py` & `mintpy-1.6.0/src/mintpy/utils/utils1.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/utils/writefile.py` & `mintpy-1.6.0/src/mintpy/utils/writefile.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy/version.py` & `mintpy-1.6.0/src/mintpy/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import collections
 import os
 import subprocess
 
 ###########################################################################
 Tag = collections.namedtuple('Tag', 'version date')
 release_history = (
+    Tag('1.6.0', '2024-05-09'),
     Tag('1.5.3', '2023-11-23'),
     Tag('1.5.2', '2023-08-09'),
     Tag('1.5.1', '2023-01-03'),
     Tag('1.5.0', '2022-11-18'),
     Tag('1.4.1', '2022-08-15'),
     Tag('1.4.0', '2022-08-04'),
     Tag('1.3.3', '2022-04-14'),
@@ -90,11 +91,7 @@
  |__/     |__/|__/|__/  |__/   \___/  |__/       \____  ##
                                                  /##  | ##
                                                 |  ######/
    Miami InSAR Time-series software in Python    \______/
           MintPy {v}, {d}
 ___________________________________________________________
 """.format(v=version, d=version_date)
-
-website = 'https://github.com/insarlab/MintPy'
-
-description = 'Miami INsar Time-series software in PYthon'
```

### Comparing `mintpy-1.5.3/src/mintpy/view.py` & `mintpy-1.6.0/src/mintpy/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from mintpy import subset, version
 from mintpy.multilook import multilook_data
-from mintpy.objects import TIMESERIES_KEY_NAMES, giantIfgramStack, ifgramStack
-from mintpy.objects.gps import GPS
+from mintpy.objects import (
+    TIMESERIES_KEY_NAMES,
+    giantIfgramStack,
+    gnss,
+    ifgramStack,
+)
 from mintpy.utils import plot as pp, ptime, readfile, utils as ut
 
 
 ##################################################################################################
 def run_or_skip(inps):
     vprint('update mode: ON')
     flag = 'skip'
@@ -462,24 +466,36 @@
 
 ##################################################################################################
 def plot_slice(ax, data, metadata, inps):
     """Plot one slice of matrix
     Parameters: ax       : matplot.pyplot axes object
                 data     : 2D np.ndarray,
                 metadata : dictionary, attributes of data
-                inps     : Namespace, optional, input options for display
+                inps     : Namespace, input options for display
     Returns:    ax       : matplot.pyplot axes object
                 inps     : Namespace for input options
                 im       : matplotlib.image.AxesImage object
                 cbar     : matplotlib.colorbar.Colorbar object
     Example: See prep_slice() above for example usage.
     """
     global vprint
     vprint = print if inps.print_msg else lambda *args, **kwargs: None
 
+    def extent2meshgrid(extent: tuple, ds_shape: list):
+        """Get mesh grid coordinates for a given extent and shape.
+        Parameters: extent - tuple of float for (left, right, bottom, top) in data coordinates
+                    shape  - list of int for [length, width] of the data
+        Returns:    xx/yy  - 1D np.ndarray of the data coordinates
+        """
+        height, width = ds_shape
+        x = np.linspace(extent[0], extent[1], width)
+        y = np.linspace(extent[2], extent[3], height)[::-1]  # reverse the Y-axis
+        xx, yy = np.meshgrid(x, y)
+        return xx.flatten(), yy.flatten()
+
     # colormap: str -> object
     if isinstance(inps.colormap, str):
         inps.colormap = pp.ColormapExt(
             inps.colormap,
             cmap_lut=inps.cmap_lut,
             vlist=inps.cmap_vlist,
         ).colormap
@@ -493,14 +509,17 @@
             print_msg=inps.print_msg,
         )
 
     vprint('display data in transparency: '+str(inps.transparency))
     num_row, num_col = data.shape
     lalo_digit = ut.get_lalo_digit4display(metadata, coord_unit=inps.coord_unit)
 
+    # common options for data visualization
+    kwargs = dict(cmap=inps.colormap, vmin=inps.vlim[0], vmax=inps.vlim[1], alpha=inps.transparency, zorder=1)
+
     #----------------------- Plot in Geo-coordinate --------------------------------------------#
     if (inps.geo_box
             and inps.coord_unit.startswith(('deg', 'meter'))
             and inps.fig_coord == 'geo'):
         vprint('plot in geo-coordinate')
 
         # extent info for matplotlib.imshow and other functions
@@ -521,33 +540,43 @@
                 dem=dem,
                 inps=inps,
                 print_msg=inps.print_msg,
             )
 
         # Reference (InSAR) data to a GNSS site
         coord = ut.coordinate(metadata)
-        if inps.disp_gps and inps.gps_component and inps.ref_gps_site:
-            ref_site_lalo = GPS(site=inps.ref_gps_site).get_stat_lat_lon(print_msg=False)
+        if inps.disp_gnss and inps.gnss_component and inps.ref_gnss_site:
+            gnss_obj = gnss.get_gnss_class(inps.gnss_source)(site=inps.ref_gnss_site)
+            ref_site_lalo = gnss_obj.get_site_lat_lon()
             y, x = coord.geo2radar(ref_site_lalo[0], ref_site_lalo[1])[0:2]
             ref_data = data[y - inps.pix_box[1], x - inps.pix_box[0]]
             data -= ref_data
             vprint('referencing InSAR data to the pixel nearest to GNSS station: '
-                   f'{inps.ref_gps_site} at [{ref_site_lalo[0]:.6f}, {ref_site_lalo[1]:.6f}] '
+                   f'{inps.ref_gnss_site} at [{ref_site_lalo[0]:.6f}, {ref_site_lalo[1]:.6f}] '
                    f'by substrating {ref_data:.3f} {inps.disp_unit}')
             # do not show the original InSAR reference point
             inps.disp_ref_pixel = False
 
         # Plot data
         if inps.disp_dem_blend:
             im = pp.plot_blend_image(ax, data, dem, inps, print_msg=inps.print_msg)
+
+        elif inps.style == 'image':
+            vprint(f'plotting data as {inps.style} via matplotlib.pyplot.imshow ...')
+            im = ax.imshow(data, extent=inps.extent, origin='upper', interpolation=inps.interpolation,
+                           animated=inps.animation, **kwargs)
+
+        elif inps.style == 'scatter':
+            vprint(f'plotting data as {inps.style} via matplotlib.pyplot.scatter (can take some time) ...')
+            xx, yy = extent2meshgrid(inps.extent, data.shape)
+            im = ax.scatter(xx, yy, c=data.flatten(), marker='o', s=inps.scatter_marker_size, **kwargs)
+            ax.axis('equal')
+
         else:
-            vprint('plotting data ...')
-            im = ax.imshow(data, cmap=inps.colormap, vmin=inps.vlim[0], vmax=inps.vlim[1],
-                           extent=inps.extent, origin='upper', interpolation=inps.interpolation,
-                           alpha=inps.transparency, animated=inps.animation, zorder=1)
+            raise ValueError(f'Un-recognized plotting style: {inps.style}!')
 
         # Draw faultline using GMT lonlat file
         if inps.faultline_file:
             pp.plot_faultline(
                 ax=ax,
                 faultline_file=inps.faultline_file,
                 SNWE=SNWE,
@@ -598,36 +627,38 @@
         # Plot points of interest
         if inps.pts_lalo is not None:
             ax.plot(inps.pts_lalo[:, 1], inps.pts_lalo[:, 0],
                     inps.pts_marker, ms=inps.pts_marker_size,
                     mec='k', mew=1.)
             vprint('plot points of interest')
 
-        # Show UNR GPS stations
-        if inps.disp_gps:
-            ax = pp.plot_gps(ax, SNWE, inps, metadata, print_msg=inps.print_msg)
+        # Show UNR GNSS stations
+        if inps.disp_gnss:
+            ax = pp.plot_gnss(ax, SNWE, inps, metadata, print_msg=inps.print_msg)
 
         # Status bar
         if inps.dem_file:
             coord_dem = ut.coordinate(dem_metadata)
             dem_len, dem_wid = dem.shape
 
         def format_coord(x, y):
             # lat/lon
             msg = f'E={x:.{lalo_digit}f}, N={y:.{lalo_digit}f}'
             # value
-            col = coord.lalo2yx(x, coord_type='lon') - inps.pix_box[0]
-            row = coord.lalo2yx(y, coord_type='lat') - inps.pix_box[1]
+            row, col = coord.lalo2yx(y, x)
+            row -= inps.pix_box[1]
+            col -= inps.pix_box[0]
             if 0 <= col < num_col and 0 <= row < num_row:
                 v = data[row, col]
                 msg += ', v=[]' if np.isnan(v) or np.ma.is_masked(v) else f', v={v:.3f}'
                 # DEM
                 if inps.dem_file:
-                    dem_col = coord_dem.lalo2yx(x, coord_type='lon') - dem_pix_box[0]
-                    dem_row = coord_dem.lalo2yx(y, coord_type='lat') - dem_pix_box[1]
+                    dem_row, dem_col = coord_dem.lalo2yx(y, x)
+                    dem_row -= dem_pix_box[1]
+                    dem_col -= dem_pix_box[0]
                     if 0 <= dem_col < dem_wid and 0 <= dem_row < dem_len:
                         h = dem[dem_row, dem_col]
                         msg += ', h=[]' if np.isnan(h) else f', h={h:.1f}'
                 # x/y
                 msg += f', x={col+inps.pix_box[0]:.0f}'
                 msg += f', y={row+inps.pix_box[1]:.0f}'
             return msg
@@ -653,19 +684,27 @@
         # extent = (left, right, bottom, top) in data coordinates
         inps.extent = (inps.pix_box[0]-0.5, inps.pix_box[2]-0.5,
                        inps.pix_box[3]-0.5, inps.pix_box[1]-0.5)
 
         # Plot Data
         if inps.disp_dem_blend:
             im = pp.plot_blend_image(ax, data, dem, inps, print_msg=inps.print_msg)
+
+        elif inps.style == 'image':
+            vprint('plotting data via matplotlib.pyplot.imshow ...')
+            im = ax.imshow(data, extent=inps.extent, interpolation=inps.interpolation, **kwargs)
+
+        elif inps.style == 'scatter':
+            vprint('plotting data via matplotlib.pyplot.scatter (can take some time) ...')
+            xx, yy = extent2meshgrid(inps.extent, data.shape)
+            im = ax.scatter(xx, yy, c=data.flatten(), marker='o', s=inps.scatter_marker_size, **kwargs)
+            ax.axis('equal')
+
         else:
-            vprint('plotting data ...')
-            im = ax.imshow(data, cmap=inps.colormap, vmin=inps.vlim[0], vmax=inps.vlim[1],
-                           extent=inps.extent, interpolation=inps.interpolation,
-                           alpha=inps.transparency, zorder=1)
+            raise ValueError(f'Un-recognized plotting style: {inps.style}!')
         ax.tick_params(labelsize=inps.font_size)
 
         # Plot Seed Point
         if inps.disp_ref_pixel:
             ref_y, ref_x = None, None
             if inps.ref_yx:
                 ref_y, ref_x = inps.ref_yx[0], inps.ref_yx[1]
@@ -779,19 +818,19 @@
         # turn off tick labels
         ax.get_xaxis().set_ticks([])
         ax.get_yaxis().set_ticks([])
 
     # rotate Y-axis tick labels
     # link: https://stackoverflow.com/questions/10998621
     if inps.ylabel_rot:
-        kwargs = dict(rotation=inps.ylabel_rot)
+        tick_kwargs = dict(rotation=inps.ylabel_rot)
         # center the vertical alignment for vertical tick labels
         if inps.ylabel_rot % 90 == 0:
-            kwargs['va'] = 'center'
-        plt.setp(ax.get_yticklabels(), **kwargs)
+            tick_kwargs['va'] = 'center'
+        plt.setp(ax.get_yticklabels(), **tick_kwargs)
         vprint(f'rotate Y-axis tick labels by {inps.ylabel_rot} deg')
 
     return ax, inps, im, cbar
 
 
 ##################################################################################################
 def read_input_file_info(inps):
@@ -1646,15 +1685,15 @@
                     fig.savefig(self.outfile[0], transparent=True, dpi=self.fig_dpi, bbox_inches='tight')
                 if not self.disp_fig:
                     fig.clf()
 
         # Multiple Subplots
         else:
             # warn single-subplot options
-            opt_names = ['--show-gps', '--coastline', '--lalo-label', '--lalo-step', '--scalebar',
+            opt_names = ['--show-gnss', '--coastline', '--lalo-label', '--lalo-step', '--scalebar',
                          '--pts-yx', '--pts-lalo', '--pts-file']
             opt_names = list(set(opt_names) & set(self.argv))
             for opt_name in opt_names:
                 print(f'WARNING: {opt_name} is NOT supported for multi-subplots, ignore it and continue.')
 
             # prepare
             self = prepare4multi_subplots(self, metadata=self.atr)
```

### Comparing `mintpy-1.5.3/src/mintpy/workflow/__init__.py` & `mintpy-1.6.0/src/mintpy/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mintpy-1.5.3/src/mintpy.egg-info/entry_points.txt` & `mintpy-1.6.0/src/mintpy.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 diff.py = mintpy.cli.diff:main
 generate_mask.py = mintpy.cli.generate_mask:main
 geocode.py = mintpy.cli.geocode:main
 ifgram_inversion.py = mintpy.cli.ifgram_inversion:main
 image_math.py = mintpy.cli.image_math:main
 image_stitch.py = mintpy.cli.image_stitch:main
 info.py = mintpy.cli.info:main
+iono_split_spectrum.py = mintpy.cli.iono_split_spectrum:main
 iono_tec.py = mintpy.cli.iono_tec:main
 load_data.py = mintpy.cli.load_data:main
 load_gbis.py = mintpy.cli.load_gbis:main
 local_oscilator_drift.py = mintpy.cli.local_oscilator_drift:main
 lookup_geo2radar.py = mintpy.cli.lookup_geo2radar:main
 mask.py = mintpy.cli.mask:main
 mintpy = mintpy.__main__:main
```

