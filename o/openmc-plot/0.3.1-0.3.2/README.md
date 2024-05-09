# Comparing `tmp/openmc_plot-0.3.1.tar.gz` & `tmp/openmc_plot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_plot-0.3.1.tar", last modified: Thu May 18 13:23:57 2023, max compression
+gzip compressed data, was "openmc_plot-0.3.2.tar", last modified: Thu May  9 10:14:43 2024, max compression
```

## Comparing `openmc_plot-0.3.1.tar` & `openmc_plot-0.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.631119 openmc_plot-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.619118 openmc_plot-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.619118 openmc_plot-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.619118 openmc_plot-0.3.1/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-18 13:23:57.631119 openmc_plot-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.619118 openmc_plot-0.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/dagmc_geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/dagmc_geometry/create_geometry_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/default_source/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/default_source/settings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/pincell/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/pincell/geometry.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/regularmesh_plot/
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/ring_source/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/ring_source/make_ring_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/ring_source/make_two_ring_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/ring_source/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/ring_source/settings_multiple_sources.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/tokamak/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/create_geometry_xml_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/geometry_no_materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/geometry_some_materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/geometry_unordered_mat_ids.xml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/settings_multiple_sources.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/tokamak/summary.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.623118 openmc_plot-0.3.1/examples/weightwindows/
--rw-r--r--   0 runner    (1001) docker     (123)  1411929 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/examples/weightwindows/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:23:57.631119 openmc_plot-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.619118 openmc_plot-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.627119 openmc_plot-0.3.1/src/openmc_plot/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/cross_sections.xml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.627119 openmc_plot-0.3.1/src/openmc_plot/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/1_🖼_Geometry_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/3_✴️_Source_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/4_🪟_Weight_window_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/6_☢_Depletion_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/7_🛢️_Cylindrical_mesh_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)  4077544 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/pages/dagmc.h5m
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-18 13:23:40.000000 openmc_plot-0.3.1/src/openmc_plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:23:57.627119 openmc_plot-0.3.1/src/openmc_plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 13:23:57.000000 openmc_plot-0.3.1/src/openmc_plot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.567006 openmc_plot-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.547006 openmc_plot-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-09 10:14:43.563006 openmc_plot-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/dagmc_geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/dagmc_geometry/create_geometry_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/default_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/default_source/settings.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/pincell/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/pincell/geometry.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/regularmesh_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/examples/ring_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/ring_source/make_ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/ring_source/make_two_ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/ring_source/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/ring_source/settings_multiple_sources.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.555006 openmc_plot-0.3.2/examples/tokamak/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/create_geometry_xml_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/geometry_no_materials.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/geometry_some_materials.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/geometry_unordered_mat_ids.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/materials.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/settings_multiple_sources.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/tokamak/summary.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.555006 openmc_plot-0.3.2/examples/weightwindows/
+-rw-r--r--   0 runner    (1001) docker     (127)  1411929 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/examples/weightwindows/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:14:43.567006 openmc_plot-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.551005 openmc_plot-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.555006 openmc_plot-0.3.2/src/openmc_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/cross_sections.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.559006 openmc_plot-0.3.2/src/openmc_plot/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/1_🖼_Geometry_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/3_✴️_Source_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/4_🪟_Weight_window_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/6_☢_Depletion_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/7_🛢️_Cylindrical_mesh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4077544 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/pages/dagmc.h5m
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 10:14:32.000000 openmc_plot-0.3.2/src/openmc_plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:14:43.563006 openmc_plot-0.3.2/src/openmc_plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 10:14:43.000000 openmc_plot-0.3.2/src/openmc_plot.egg-info/top_level.txt
```

### Comparing `openmc_plot-0.3.1/.github/workflows/python-publish.yml` & `openmc_plot-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/.gitignore` & `openmc_plot-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/Dockerfile` & `openmc_plot-0.3.2/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 
 # maintained at https://github.com/fusion_energy/openmc_plot.com/
 
 FROM continuumio/miniconda3:4.12.0
 
 RUN conda install -c conda-forge openmc==0.13.3
 
-RUN pip install streamlit
 # Could be used to make matplotlib in streamlit interactive
 # see https://blog.streamlit.io/make-your-st-pyplot-interactive/
 # RUN pip install mpld3
-RUN pip install openmc_source_plotter>=0.6.2
-RUN pip install dagmc_geometry_slice_plotter>=0.3.1
-RUN pip install openmc_geometry_plot>=0.3.5
-RUN pip install regular_mesh_plotter>=0.5.3
-RUN pip install openmc_depletion_plotter>=0.3.1
-RUN pip install openmc_cylindrical_mesh_plotter>=0.1.2
+RUN pip install "openmc_source_plotter>=0.6.2"
+RUN pip install "dagmc_geometry_slice_plotter>=0.3.1"
+RUN pip install "openmc_geometry_plot>=0.3.5"
+RUN pip install "regular_mesh_plotter>=0.5.3"
+RUN pip install "openmc_depletion_plotter>=0.3.1"
+RUN pip install "openmc_cylindrical_mesh_plotter>=0.1.2"
 
 
 COPY src/* /
 # optional copy
 # COPY .streamlit/config.toml .streamlit/config.toml
 
 ENV PORT 8501
```

### Comparing `openmc_plot-0.3.1/LICENSE` & `openmc_plot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/PKG-INFO` & `openmc_plot-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_plot
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package containing a collection of scripts for producing and downloading data for OpenMC
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,25 @@
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_plot/issues
 Keywords: openmc,plot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: streamlit
+Requires-Dist: openmc_source_plotter>=0.6.2
+Requires-Dist: dagmc_geometry_slice_plotter>=0.3.1
+Requires-Dist: openmc_geometry_plot>=0.4.3
+Requires-Dist: regular_mesh_plotter>=0.5.3
+Requires-Dist: openmc_depletion_plotter>=0.3.1
+Requires-Dist: openmc_cylindrical_mesh_plotter>=0.1.2
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: requests; extra == "tests"
 
 A Python app for plotting OpenMC.
 
 This repository contains the source code for the OpenMC plot.
 
 Try the web app at [http://openmc-plot.xsplot.com](http://openmc-plot.xsplot.com)
```

### Comparing `openmc_plot-0.3.1/README.md` & `openmc_plot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/pincell/geometry.xml` & `openmc_plot-0.3.2/examples/pincell/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py` & `openmc_plot-0.3.2/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/ring_source/make_ring_source.py` & `openmc_plot-0.3.2/examples/ring_source/make_ring_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/ring_source/make_two_ring_source.py` & `openmc_plot-0.3.2/examples/ring_source/make_two_ring_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/ring_source/settings.xml` & `openmc_plot-0.3.2/examples/ring_source/settings.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/ring_source/settings_multiple_sources.xml` & `openmc_plot-0.3.2/examples/ring_source/settings_multiple_sources.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/create_geometry_xml_files.py` & `openmc_plot-0.3.2/examples/tokamak/create_geometry_xml_files.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/geometry.xml` & `openmc_plot-0.3.2/examples/tokamak/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/geometry_no_materials.xml` & `openmc_plot-0.3.2/examples/tokamak/geometry_no_materials.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/geometry_some_materials.xml` & `openmc_plot-0.3.2/examples/tokamak/geometry_some_materials.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/geometry_unordered_mat_ids.xml` & `openmc_plot-0.3.2/examples/tokamak/geometry_unordered_mat_ids.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/settings_multiple_sources.xml` & `openmc_plot-0.3.2/examples/tokamak/settings_multiple_sources.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/tokamak/summary.h5` & `openmc_plot-0.3.2/examples/tokamak/summary.h5`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/examples/weightwindows/settings.xml` & `openmc_plot-0.3.2/examples/weightwindows/settings.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/pyproject.toml` & `openmc_plot-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "streamlit",
     "openmc_source_plotter>=0.6.2",
     "dagmc_geometry_slice_plotter>=0.3.1",
-    "openmc_geometry_plot>=0.3.5",
+    "openmc_geometry_plot>=0.4.3",
     "regular_mesh_plotter>=0.5.3",
     "openmc_depletion_plotter>=0.3.1",
     "openmc_cylindrical_mesh_plotter>=0.1.2",
 ]
 dynamic = ["version"]
```

### Comparing `openmc_plot-0.3.1/src/openmc_plot/app.py` & `openmc_plot-0.3.2/src/openmc_plot/app.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/1_🖼_Geometry_plot.py` & `openmc_plot-0.3.2/src/openmc_plot/pages/1_🖼_Geometry_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py` & `openmc_plot-0.3.2/src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/3_✴️_Source_plot.py` & `openmc_plot-0.3.2/src/openmc_plot/pages/3_✴️_Source_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/4_🪟_Weight_window_plot.py` & `openmc_plot-0.3.2/src/openmc_plot/pages/4_🪟_Weight_window_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py` & `openmc_plot-0.3.2/src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/pages/dagmc.h5m` & `openmc_plot-0.3.2/src/openmc_plot/pages/dagmc.h5m`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot/utils.py` & `openmc_plot-0.3.2/src/openmc_plot/utils.py`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.3.1/src/openmc_plot.egg-info/PKG-INFO` & `openmc_plot-0.3.2/src/openmc_plot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openmc-plot
-Version: 0.3.1
+Name: openmc_plot
+Version: 0.3.2
 Summary: A Python package containing a collection of scripts for producing and downloading data for OpenMC
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,25 @@
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_plot/issues
 Keywords: openmc,plot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: streamlit
+Requires-Dist: openmc_source_plotter>=0.6.2
+Requires-Dist: dagmc_geometry_slice_plotter>=0.3.1
+Requires-Dist: openmc_geometry_plot>=0.4.3
+Requires-Dist: regular_mesh_plotter>=0.5.3
+Requires-Dist: openmc_depletion_plotter>=0.3.1
+Requires-Dist: openmc_cylindrical_mesh_plotter>=0.1.2
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: requests; extra == "tests"
 
 A Python app for plotting OpenMC.
 
 This repository contains the source code for the OpenMC plot.
 
 Try the web app at [http://openmc-plot.xsplot.com](http://openmc-plot.xsplot.com)
```

### Comparing `openmc_plot-0.3.1/src/openmc_plot.egg-info/SOURCES.txt` & `openmc_plot-0.3.2/src/openmc_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

