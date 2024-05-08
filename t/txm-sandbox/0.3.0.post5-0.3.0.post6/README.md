# Comparing `tmp/txm_sandbox-0.3.0.post5.tar.gz` & `tmp/txm_sandbox-0.3.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.0.post5.tar", last modified: Sun Apr 28 16:59:24 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.0.post6.tar", last modified: Wed May  8 23:43:43 2024, max compression
```

## Comparing `txm_sandbox-0.3.0.post5.tar` & `txm_sandbox-0.3.0.post6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/LICENSE
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/MANIFEST.in
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      257 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/README.md
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post5/TXM_GUI2.ipynb
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-28 16:59:24.920873 txm_sandbox-0.3.0.post5/setup.cfg
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1130 2024-04-28 16:58:54.000000 txm_sandbox-0.3.0.post5/setup.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.892873 txm_sandbox-0.3.0.post5/txm_sandbox/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/config/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.896873 txm_sandbox-0.3.0.post5/txm_sandbox/external/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/external/user_io.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.904873 txm_sandbox-0.3.0.post5/txm_sandbox/gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_fitting_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.904873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      786 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      957 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      899 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2389 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1362 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.908873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15328 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    25747 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    23715 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    49041 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16610 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/txm_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/misc.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.912873 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/tmp/readme.txt
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.916873 txm_sandbox-0.3.0.post5/txm_sandbox/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/io.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_spectra_filters.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-28 16:59:24.892873 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      257 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3045 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/SOURCES.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/dependency_links.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/not-zip-safe
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/requires.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-28 16:59:24.000000 txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.220583 txm_sandbox-0.3.0.post6/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post6/LICENSE
+-rw-rw-r--   0 xianghui   (501) staff       (20)      147 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post6/MANIFEST.in
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-08 23:43:43.220394 txm_sandbox-0.3.0.post6/PKG-INFO
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1639 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post6/README.md
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.0.post6/TXM_GUI2.ipynb
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.197731 txm_sandbox-0.3.0.post6/TXM_Sandbox/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.198605 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.200049 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/xanes_analysis_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.200346 txm_sandbox-0.3.0.post6/TXM_Sandbox/external/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/external/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/external/user_io.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.206057 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    79463 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/gui_components.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/main_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   203257 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes_fitting_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.206787 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.208182 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      786 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.208485 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     5528 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/dicts/data_struct_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.210867 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-08 14:31:59.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-08 14:04:01.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    27222 2024-05-07 07:45:10.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    24243 2024-05-08 12:40:21.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    54769 2024-05-08 11:49:58.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-08 13:04:07.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.212743 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      605 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2428 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2029 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/txm_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.213811 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    10590 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/misc.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.214090 txm_sandbox-0.3.0.post6/TXM_Sandbox/tmp/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/tmp/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/tmp/readme.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.219526 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/io.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/misc.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/plotlib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    41021 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    23436 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    84774 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_spectra_filters.py
+-rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-08 23:43:43.220623 txm_sandbox-0.3.0.post6/setup.cfg
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-08 22:55:54.000000 txm_sandbox-0.3.0.post6/setup.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-08 23:43:43.220177 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 xianghui   (501) staff       (20)     3317 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/not-zip-safe
+-rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/requires.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-08 23:43:43.000000 txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.0.post5/LICENSE` & `txm_sandbox-0.3.0.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/README.md` & `txm_sandbox-0.3.0.post6/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/TXM_GUI2.ipynb` & `txm_sandbox-0.3.0.post6/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/setup.py` & `txm_sandbox-0.3.0.post6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.0.post5',
+      version='0.3.0.post6',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,22 +86,18 @@
         self.apply = widgets.PushButton(text="apply", enabled=False)
         self.appl_mk_info_board = widgets.TextEdit(
             label="data info", value="", enabled=False
         )
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.appl_mk_in_data_type.changed.connect(self._sel_appl_mk_in_data_type)
-        self.appl_mk_in_data_file.changed.connect(self._sel_appl_mk_in_data_file)
-        self.appl_mk_data_avail_items.changed.connect(
-            self._sel_appl_mk_data_avail_items
-        )
-        self.appl_mk_mask_avail_items.changed.connect(
-            self._sel_appl_mk_mask_avail_items
-        )
+        self.appl_mk_in_data_type.changed.connect(self._sel_in_data_type)
+        self.appl_mk_in_data_file.changed.connect(self._sel_in_data_file)
+        self.appl_mk_data_avail_items.changed.connect(self._sel_data_avail_items)
+        self.appl_mk_mask_avail_items.changed.connect(self._sel_mask_avail_items)
         self.apply.changed.connect(self._apply)
         self.close_file.changed.connect(self._close_file)
 
         self.gui_layout = widgets.VBox(
             widgets=[
                 self.label1,
                 self.appl_mk_in_data_type,
@@ -164,15 +160,19 @@
                             self.viewer, self._appl_mk_data, "appl_mk_data"
                         )
                         show_layers_in_viewer(self.viewer, ["appl_mk_data"])
                         self._appl_mk_data_ready = True
                     else:
                         rm_gui_viewers(self.viewer, ["appl_mk_data"])
                         self._appl_mk_data_ready = False
-                except:
+                except Exception as e:
+                    self.op_status.value = (
+                        "Invalid file. Check terminal for error message ..."
+                    )
+                    print(e)
                     self.__close_file(mode="data", kill=True)
                     self.__close_file(mode="mask", kill=False)
                     self._appl_mk_data_ready = False
             else:
                 (self._in_mask_path_in_h5, _in_dat_desc, _in_dat_dtype) = (
                     get_slcd_ds_path(
                         self.appl_mk_in_data_file.value,
@@ -201,18 +201,31 @@
                             self.viewer, self._appl_mk_mask, "appl_mk_mask"
                         )
                         show_layers_in_viewer(self.viewer, ["appl_mk_mask"])
                         self._appl_mk_data_ready = True
                     else:
                         rm_gui_viewers(self.viewer, ["appl_mk_mask"])
                         self._appl_mk_data_ready = False
-                except:
+                except Exception as e:
+                    self.op_status.value = (
+                        "Invalid file. Check terminal for error message ..."
+                    )
+                    print(e)
                     self.__close_file(mode="mask", kill=True)
                     self.__close_file(mode="data", kill=False)
                     self._appl_mk_data_ready = False
+        else:
+            if _APPL_DATA_ITEM_CHOICES:
+                pass
+            else:
+                self.op_status.value = "No valid data items in the input file ..."
+            if _APPL_MASK_ITEM_CHOICES:
+                pass
+            else:
+                self.op_status.value = "No valid mask items in the input file ..."
 
     def __dflt_out_file_type(self):
         if (self._appl_mk_data is None) or (len(self._appl_mk_data.shape) <= 2):
             self.appl_mk_out_file_type.enabled = False
         else:
             self.appl_mk_out_file_type.enabled = True
         self.appl_mk_out_file_type.value = "tif"
@@ -250,31 +263,40 @@
                 0,
             )
             self.viewer.layers["appl_mk_mask"].opacity = 0.2
             self.viewer.layers["appl_mk_mask"].colormap = "yellow"
             self.viewer.layers["appl_mk_data"].visible = True
             self.viewer.layers["appl_mk_mask"].visible = True
 
-    def _sel_appl_mk_in_data_type(self):
-        self.appl_mk_in_data_file.value = ""
+    def __reset_widget_val(self):
         global _APPL_MASK_ITEM_CHOICES
         _APPL_MASK_ITEM_CHOICES = []
         self.appl_mk_mask_avail_items.reset_choices()
         global _APPL_DATA_ITEM_CHOICES
         _APPL_DATA_ITEM_CHOICES = []
         self.appl_mk_data_avail_items.reset_choices()
         self.appl_mk_out_file_type.value = "tif"
         self.appl_mk_out_dir.value = ""
         self.appl_mk_info_board.value = ""
         self.op_status.value = ""
+
+    def __reset_data_states(self):
         self._appl_mk_data_ready
+
+    def _sel_in_data_type(self):
+        self.appl_mk_in_data_file.value = ""
+        self.__reset_widget_val()
+        self.__reset_data_states()
         self._close_file()
         self.__lock_appl_mk_gui_widgets()
 
-    def _sel_appl_mk_in_data_file(self):
+    def _sel_in_data_file(self):
+        self.__reset_widget_val()
+        self.__reset_data_states()
+        self._close_file()
         choices = check_avail_items(
             self.appl_mk_in_data_file.value, self.appl_mk_in_data_type.value
         )
         masks = [mask for mask in choices if "mk" in mask]
         datas = list(set(choices) - set(masks))
         if "eng_list" in datas:
             datas.remove("eng_list")
@@ -291,25 +313,25 @@
             self._appl_mk_data_ready = False
             self.__dflt_out_path(dflt=True)
         self.__avail_item_slcd(mode="data")
         self.__avail_item_slcd(mode="mask")
         self.__set_layers_order()
         self.__lock_appl_mk_gui_widgets()
 
-    def _sel_appl_mk_data_avail_items(self):
+    def _sel_data_avail_items(self):
         self.__avail_item_slcd(mode="data")
         self.__set_layers_order()
         self.__lock_appl_mk_gui_widgets()
         self.__dflt_out_file_type()
         try:
             self.__dflt_out_path(dflt=False)
         except:
             self.__dflt_out_path(dflt=True)
 
-    def _sel_appl_mk_mask_avail_items(self):
+    def _sel_mask_avail_items(self):
         self.__avail_item_slcd(mode="mask")
         self.__set_layers_order()
         self.__lock_appl_mk_gui_widgets()
         self.__dflt_out_file_type()
         try:
             self.__dflt_out_path(dflt=False)
         except:
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         self.convt = widgets.PushButton(text="convert", enabled=False)
         self.convt_info_board = widgets.TextEdit(
             label="data info", value="", enabled=False
         )
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.convt_in_data_type.changed.connect(self._sel_convt_in_data_type)
-        self.convt_in_data_file.changed.connect(self._sel_convt_in_data_file)
+        self.convt_in_data_type.changed.connect(self._sel_in_data_type)
+        self.convt_in_data_file.changed.connect(self._sel_in_data_file)
         self.convt_avail_items.changed.connect(self._sel_convt_in_avail_items)
         self.convt.changed.connect(self._convt)
         self.close_file.changed.connect(self._close_file)
 
         self.gui_layout = widgets.VBox(
             widgets=[
                 self.label1,
@@ -157,29 +157,38 @@
     def __dflt_out_file_type(self):
         if (self._convt_data is None) or (len(self._convt_data.shape) <= 2):
             self.convt_out_file_type.enabled = False
         else:
             self.convt_out_file_type.enabled = True
         self.convt_out_file_type.value = "tif"
 
-    def _sel_convt_in_data_type(self):
-        self.convt_in_data_file.value = ""
+    def __reset_widget_val(self):
         global _CONVT_DATA_ITEM_CHOICES
         _CONVT_DATA_ITEM_CHOICES = []
         self.convt_avail_items.reset_choices()
         self.convt_out_file_type.value = "tif"
         self.convt_out_dir.value = ""
         self.convt_info_board.value = ""
         self.op_status.value = ""
+
+    def __reset_data_states(self):
         self._convt_data_ready = False
+
+    def _sel_in_data_type(self):
+        self.convt_in_data_file.value = ""
+        self.__reset_widget_val()
+        self.__reset_data_states()
         self._close_file()
         self.__lock_convt_gui_widgets()
 
     @disp_progress_info("data loading")
-    def _sel_convt_in_data_file(self):
+    def _sel_in_data_file(self):
+        self.__reset_widget_val()
+        self.__reset_data_states()
+        self._close_file()
         choices = check_avail_items(
             self.convt_in_data_file.value, self.convt_in_data_type.value
         )
         global _CONVT_DATA_ITEM_CHOICES
         _CONVT_DATA_ITEM_CHOICES = choices
         self.convt_avail_items.reset_choices()
         if _CONVT_DATA_ITEM_CHOICES:
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/tomo_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from ...utils.io import data_reader, tomo_h5_reader
 from ...utils.tomo_recon_tools import rm_redundant
 from ...gui.gui_components import (
     check_file_availability,
 )
 from ..utils.misc import (
+    set_data_widget,
     rm_gui_viewers,
     disp_progress_info,
     info_reader,
     update_layer_in_viewer,
     show_layers_in_viewer,
 )
 from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
@@ -55,15 +56,15 @@
 ################################################################################
 #             do trial recon for a single slice of a given scan                #
 ################################################################################
 class tomo_gui:
     def __init__(self, viewer):
         self.viewer = viewer
         self._tomo_cfg = ZFLY_CFG["io_data_structure_tomo"]
-        self.scn_fn = None
+        self._scn_fn = None
         self._wedge_data_avg = 0
         self._trial_cen_rec_done = False
         self._multi_trial_cen_rec_done = False
         self._cen = None
         self._wedge_autodet_fig = None
         self._viewers = ["proj_prev", "data_center", "tomo_viewer"]
 
@@ -106,28 +107,27 @@
         )
         self.label2 = widgets.Label(
             name="Step 2",
             value="--------------------     Vol Recon    --------------------",
         )
         self.cen = widgets.LineEdit(name="picked cen", enabled=False)
         self.pick_cen = widgets.PushButton(text="pick center", enabled=False)
-        self.trial_cen_done = widgets.PushButton(text="trial cen done", enabled=False)
         self.trial_cen_done = widgets.RadioButtons(
             name="trial cen done",
             choices=["Yes", "No"],
             orientation="horizontal",
             value="No",
             tooltip="confirm if all trial centering works are finished",
             enabled=False,
         )
         self.vol_rec = widgets.PushButton(text="vol recon", enabled=False)
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.file_type.changed.connect(self._sel_file_type)
+        self.file_type.changed.connect(self._sel_in_file_type)
         self.top_dir.changed.connect(self._sel_top_dir)
         self.find_multi_cen.changed.connect(self._find_multi_cen)
         self.scan_id.changed.connect(self._sel_scn_id)
         self.proj_prev.changed.connect(self._proj_prev)
         self.is_wedge.changed.connect(self._is_wedge)
         self.wedge_thsh.changed.connect(self._set_wedge_thsh)
         self.phase_retrieval.changed.connect(self._use_phase_retrieval)
@@ -177,35 +177,38 @@
             _TOMO_TRL_SCN_ID_CHOICES = ids
         else:
             _TOMO_TRL_SCN_ID_CHOICES = []
         self.scan_id.reset_choices()
 
     def __comp_scn_fn(self):
         if self.scan_id.value:
-            self.scn_fn = self.top_dir.value / self._tomo_cfg[
+            self._scn_fn = self.top_dir.value / self._tomo_cfg[
                 "tomo_raw_fn_template"
             ].format(self.scan_id.value)
         else:
-            self.scn_fn = None
+            self._scn_fn = None
 
     def __set_trial_cen_rec_widgets(self):
-        if not self.scn_fn.exists():
+        if (self._scn_fn is None) or (not self._scn_fn.exists()):
+            """
             self.find_multi_cen.enabled = False
             self.scan_id.enabled = False
             self.proj_prev.enabled = False
             self.cen_sch_s.enabled = False
             self.ref_sli.enabled = False
             self.is_wedge.enabled = False
             self.wedge_thsh.enabled = False
             self.phase_retrieval.enabled = False
             self.beta_gamma_ratio.enabled = False
             self.trial_cen_rec.enabled = False
             self.pick_cen.enabled = False
             self.vol_rec.enabled = False
             self.close_file.enabled = False
+            """
+            self.__reset_widgets()
         else:
             self.find_multi_cen.enabled = True
             self.scan_id.enabled = True
             self.proj_prev.enabled = True
             self.cen_sch_s.enabled = True
             self.ref_sli.enabled = True
             self.is_wedge.enabled = True
@@ -246,34 +249,81 @@
                 self.vol_rec.enabled = False
             else:
                 self.vol_rec.enabled = True
             self.trial_cen_done.enabled = False
         self.close_file.enabled = True
 
     def __preset_dflt(self):
-        self._data_dim = info_reader(self.scn_fn, dtype="data", cfg=self._tomo_cfg)
+        self._data_dim = info_reader(self._scn_fn, dtype="data", cfg=self._tomo_cfg)
         if (self._data_dim[2] / 2 - self.cen_sch_s.value) > (self._data_dim[2] / 6):
             self.cen_sch_s.value = int(self._data_dim[2] / 2 - 40)
         self.ref_sli.value = int(self._data_dim[1] / 2)
 
-    def _sel_file_type(self):
-        self._cen = None
+    def __reset_widgets(self):
+        self._scn_fn = None
+        self._wedge_data_avg = 0
         self._trial_cen_rec_done = False
+        self._multi_trial_cen_rec_done = False
+        self._cen = None
+        self._wedge_autodet_fig = None
+        self._trial_cen_dir = None
+
+        self.find_multi_cen.enabled = False        
+        self.scan_id.enabled = False
+        self.proj_prev.enabled = False
+        self.cen_sch_s.enabled = False
+        self.ref_sli.enabled = False
+        self.is_wedge.enabled = False
+        self.wedge_thsh.enabled = False
+        self.phase_retrieval.enabled = False
+        self.beta_gamma_ratio.enabled = False
+        self.trial_cen_done.enabled = False
+        self.trial_cen_rec.enabled = False
+        self.pick_cen.enabled = False
+        self.vol_rec.enabled = False
+        self.close_file.enabled = False
+
+        set_data_widget(
+            self.cen_sch_s,
+            1,
+            600,
+            2500,
+        )
+        set_data_widget(
+            self.ref_sli,
+            1,
+            540,
+            2560,
+        )
+        self.find_multi_cen.value = False
+        self.proj_prev.value = False
+        self.is_wedge.value = False
+        self.phase_retrieval.value = False
+        self.wedge_thsh.value = 0.1
+        self.beta_gamma_ratio.value = 0.01
+        self.cen.value = ""
+        self.trial_cen_done.value = "No"
+        global _TOMO_TRL_SCN_ID_CHOICES
+        _TOMO_TRL_SCN_ID_CHOICES = []
+        self.scan_id.reset_choices()
+
+        self._close_file()
+
+    def _sel_in_file_type(self):
         if self.file_type.value == "tomo_zfly":
             self._tomo_cfg = ZFLY_CFG["io_data_structure_tomo"]
         else:
             self._tomo_cfg = FLY_CFG["io_data_structure_tomo"]
         self.__check_avail_data()
         self.__comp_scn_fn()
         self.__set_trial_cen_rec_widgets()
         self.__set_vol_rec_widgets()
 
     def _sel_top_dir(self):
-        self._cen = None
-        self._trial_cen_rec_done = False
+        self.__reset_widgets()
         self._trial_cen_dir = self.top_dir.value / "data_center"
         self.__check_avail_data()
         self.__comp_scn_fn()
         self.__set_trial_cen_rec_widgets()
         self.__set_vol_rec_widgets()
 
     def _find_multi_cen(self):
@@ -304,26 +354,26 @@
     @disp_progress_info("data file read")
     def _proj_prev(self):
         rm_gui_viewers(self.viewer, ["proj_prev"])
         if self.proj_prev.value:
             if self.file_type.value == "tomo_zfly":
                 update_layer_in_viewer(
                     self.viewer,
-                    h5py.File(self.scn_fn, "r")[
+                    h5py.File(self._scn_fn, "r")[
                         ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
                             "io_data_structure"
                         ]["data_path"]
                     ],
                     "proj_prev",
                 )
                 show_layers_in_viewer(self.viewer, ["proj_prev"])
             else:
                 update_layer_in_viewer(
                     self.viewer,
-                    h5py.File(self.scn_fn, "r")[
+                    h5py.File(self._scn_fn, "r")[
                         FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
                             "io_data_structure"
                         ]["data_path"]
                     ],
                     "proj_prev",
                 )
                 show_layers_in_viewer(self.viewer, ["proj_prev"])
@@ -333,56 +383,56 @@
         self._cen = None
         self._trial_cen_rec_done = False
         self.__set_vol_rec_widgets()
         if self.is_wedge.value:
             self.wedge_thsh.enabled = True
 
             theta = h5_reader(
-                self.scn_fn, dtype="theta", sli=[None], cfg=self._tomo_cfg
+                self._scn_fn, dtype="theta", sli=[None], cfg=self._tomo_cfg
             ).astype(np.float32)
             if self.file_type.value == "tomo_zfly":
                 idx = np.ones(self._data_dim[0], dtype=bool)
             else:
                 idx = rm_redundant(theta)
                 theta = theta[idx]
                 if self._data_dim[0] > theta.shape[0]:
                     idx = np.concatenate(
                         (
                             idx,
                             np.zeros(self._data_dim[0] - theta.shape[0], dtype=bool),
                         )
                     )
             data = h5_reader(
-                self.scn_fn,
+                self._scn_fn,
                 dtype="data",
                 sli=[
                     None,
                     [self.ref_sli.value, self.ref_sli.value + 1],
                     [0, self._data_dim[2] - 1],
                 ],
                 cfg=self._tomo_cfg,
             ).astype(np.float32)[idx]
             white = (
                 h5_reader(
-                    self.scn_fn,
+                    self._scn_fn,
                     dtype="flat",
                     sli=[
                         None,
                         [self.ref_sli.value, self.ref_sli.value + 1],
                         [0, self._data_dim[2] - 1],
                     ],
                     cfg=self._tomo_cfg,
                 )
                 .mean(axis=0)
                 .astype(np.float32)
             )
 
             dark = (
                 h5_reader(
-                    self.scn_fn,
+                    self._scn_fn,
                     dtype="dark",
                     sli=[
                         None,
                         [self.ref_sli.value, self.ref_sli.value + 1],
                         [0, self._data_dim[2] - 1],
                     ],
                     cfg=self._tomo_cfg,
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self.save_items = widgets.Select(
             choices=get_xanes_fit_save_items_choices, name="save items"
         )
         self.fit = widgets.PushButton(text="fit", enabled=False)
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.data_type.changed.connect(self._data_type)
+        self.data_type.changed.connect(self._sel_in_data_type)
         self.xanes_file.changed.connect(self._sel_xanes_file)
         self.reload.changed.connect(self._reload_xanes_data)
         self.sli.changed.connect(self._vis_sli_chgd)
         self.E.changed.connect(self._vis_E_chgd)
         self.spec_in_roi.changed.connect(self._spec_in_roi_chkd)
         self.roi_cen_x.changed.connect(self._spec_roi_cen_x_chgd)
         self.roi_cen_y.changed.connect(self._spec_roi_cen_y_chgd)
@@ -151,37 +151,14 @@
                 self.save_items,
                 self.fit,
                 self.close_file,
                 self.op_status,
             ]
         )
 
-    def _data_type(self):
-        self.xanes_file.value = ""
-        self.eng_eV.value = ""
-        self.sli.value = 0
-        self.E.value = 0
-        self.spec_in_roi.value = False
-        self.roi_cen_x.value = 0
-        self.roi_cen_y.value = 0
-        self.element.value = ""
-        self.analysis_type = "wl"
-        self.edge_eng = ""
-        self.wl_s.value = ""
-        self.wl_e.value = ""
-        self.edge_s.value = ""
-        self.edge_e.value = ""
-        self.downsample_factor.value = 1
-        global _XANES_FIT_SAVE_ITEMS_CHOICES
-        _XANES_FIT_SAVE_ITEMS_CHOICES = []
-        self.save_items.reset_choices()
-        self.op_status.value = ""
-        self._reg_done = False
-        self.__lock_xanes_gui_widgets()
-
     def __lock_xanes_gui_widgets(self):
         if self._reg_done:
             self.E.enabled = True
             if self._elem is not None:
                 self.spec_in_roi.enabled = True
                 if self.spec_in_roi.value:
                     self.roi_cen_x.enabled = True
@@ -202,35 +179,21 @@
                 self.analysis_type.enabled = True
                 self.wl_s.enabled = True
                 self.wl_e.enabled = True
                 self.fit.enabled = True
                 self.enabled = True
             else:
                 self.enabled = False
-                self.spec_in_roi.enabled = False
-                self.roi_cen_x.enabled = False
-                self.roi_cen_y.enabled = False
-                self.def_fit_range.enabled = False
-                self.data_type.enabled = True
-            self.xanes_file.enabled = True
             if self._xanes_type == "2D XANES":
                 self.sli.enabled = False
             else:
                 self.sli.enabled = True
             self.close_file.enabled = True
         else:
             self.enabled = False
-            self.reload.enabled = False
-            self.sli.enabled = False
-            self.E.enabled = False
-            self.spec_in_roi.enabled = False
-            self.roi_cen_x.enabled = False
-            self.roi_cen_y.enabled = False
-            self.def_fit_range.enabled = False
-            self.close_file.enabled = False
         self.data_type.enabled = True
         self.xanes_file.enabled = True
 
     def __set_xanes_gui_widgets(self):
         if self._reg_done:
             if self._xanes_type == "2D XANES":
                 self.sli.enabled = False
@@ -330,50 +293,109 @@
         if self._spec_in_roi_fig is not None:
             plt.close(self._spec_in_roi_fig)
         self._spec_in_roi_fig, ax = plt.subplots()
         ax.plot(self._eng_lst, self._spec_in_roi)
         ax.set_title("spec in roi")
         plt.show()
 
+    def __set_analysis_type(self):
+        if (self._eng_lst.min() > (float(self.edge_eng.value) - 50)) and (
+            self._eng_lst.max() < (float(self.edge_eng.value) + 50)
+        ):
+            self.analysis_type.value = "wl"
+
+    def __reset_widget_val(self):
+        self.xanes_file.value = ""
+        self.eng_eV.value = ""
+        self.sli.value = 0
+        self.E.value = 0
+        self.spec_in_roi.value = False
+        self.roi_cen_x.value = self.roi_cen_x.min
+        self.roi_cen_y.value = self.roi_cen_y.min
+        self.element.value = ""
+        self.analysis_type = "wl"
+        self.edge_eng = ""
+        self.wl_s.value = ""
+        self.wl_e.value = ""
+        self.edge_s.value = ""
+        self.edge_e.value = ""
+        self.downsample_factor.value = 1
+        global _XANES_FIT_SAVE_ITEMS_CHOICES
+        _XANES_FIT_SAVE_ITEMS_CHOICES = []
+        self.save_items.reset_choices()
+        self.op_status.value = ""
+
+    def __reset_run_states(self):
+        self._reg_done = False
+
+    def __reset_data_states(self):
+        self._elem = None
+        self._xanes_data = None
+
+    def _sel_in_data_type(self):
+        self.__reset_run_states()
+        self.__reset_data_states()
+        self.__reset_widget_val()
+        self._close_file()
+        self.__lock_xanes_gui_widgets()
+
     @disp_progress_info("xanes data loading")
     def _sel_xanes_file(self):
-        with h5py.File(self.xanes_file.value, "r") as f:
-            if (
-                f"/registration_results/reg_results/registered_{self._anal_type_dict[self.data_type.value]}"
-                in f
-            ):
-                self._reg_done = True
-                self._xanes_type = self.data_type.value
-                self._xanes_data_fn = self.xanes_file.value
-                self._xanes_data_dim = f[
+        self.__reset_run_states()
+        self.__reset_data_states()
+        self._close_file()
+        self.op_status.value = "doing xanes data loading ..."
+        try:
+            with h5py.File(self.xanes_file.value, "r") as f:
+                if (
                     f"/registration_results/reg_results/registered_{self._anal_type_dict[self.data_type.value]}"
-                ].shape
-                self._eng_lst = scale_eng_list(
-                    f["/registration_results/reg_results/eng_list"][:]
-                )
-            else:
-                self._reg_done = False
-                self._xanes_type = None
-                self._xanes_data_fn = None
-                self._xanes_data = None
-                self._xanes_data_dim = None
-                self._eng_lst = None
+                    in f
+                ):
+                    self._reg_done = True
+                    self._xanes_type = self.data_type.value
+                    self._xanes_data_fn = self.xanes_file.value
+                    self._xanes_data_dim = f[
+                        f"/registration_results/reg_results/registered_{self._anal_type_dict[self.data_type.value]}"
+                    ].shape
+                    self._eng_lst = scale_eng_list(
+                        f["/registration_results/reg_results/eng_list"][:]
+                    )
+                else:
+                    self._reg_done = False
+                    self._xanes_type = None
+                    self._xanes_data_fn = None
+                    self._xanes_data = None
+                    self._xanes_data_dim = None
+                    self._eng_lst = None
+        except Exception as e:
+            self.op_status.value = "Invalid file!"
+            self._reg_done = False
+            self._xanes_type = None
+            self._xanes_data_fn = None
+            self._xanes_data = None
+            self._xanes_data_dim = None
+            self._eng_lst = None
+            print(e)
         if self._reg_done:
             rm_gui_viewers(self.viewer, ["xanes_data"])
             try:
                 self._xanes_data_fn_p = h5py.File(self._xanes_data_fn, "r")
                 self._xanes_data = da.from_array(
                     self._xanes_data_fn_p[
                         f"/registration_results/reg_results/registered_{self._anal_type_dict[self.data_type.value]}"
                     ]
                 )
                 update_layer_in_viewer(self.viewer, self._xanes_data, "xanes_data")
                 show_layers_in_viewer(self.viewer, ["xanes_data"])
+                self.op_status.value = "xanes data loading finished ..."
             except Exception as e:
-                self.viewer.status = (
+                # vself.viewer.status = (
+                #     "Something is wrong. Please check terminal for more information."
+                # )
+                self.op_status.value = (
                     "Something is wrong. Please check terminal for more information."
                 )
                 print(str(e))
                 self._xanes_data_fn_p = None
                 self._xanes_data = None
 
         self._spec_in_roi = None
@@ -383,58 +405,53 @@
 
     @disp_progress_info("xanes data reloading")
     def _reload_xanes_data(self):
         if self._xanes_data_fn_p is None:
             self._sel_xanes_file()
 
     def _vis_sli_chgd(self):
-        self.__vis_xanes_data()
+        if self._reg_done:
+            self.__vis_xanes_data()
 
     def _vis_E_chgd(self):
-        self.eng_eV.value = str(self._eng_lst[self.E.value])
-        self.__vis_xanes_data()
+        if self._reg_done:
+            self.eng_eV.value = str(self._eng_lst[self.E.value])
+            self.__vis_xanes_data()
 
     def _spec_in_roi_chkd(self):
         if self.spec_in_roi.value:
             self.roi_cen_x.enabled = True
             self.roi_cen_y.enabled = True
             self.def_fit_range.enabled = True
         else:
             self.roi_cen_x.enabled = False
             self.roi_cen_y.enabled = False
             self.def_fit_range.enabled = False
 
     def _spec_roi_cen_x_chgd(self):
-        overlap_roi(self.viewer, self, mode="xanes_spec_roi")
-        self.__plot_spec_in_roi()
+        if self._reg_done:
+            overlap_roi(self.viewer, self, mode="xanes_spec_roi")
+            self.__plot_spec_in_roi()
 
     def _spec_roi_cen_y_chgd(self):
-        overlap_roi(self.viewer, self, mode="xanes_spec_roi")
-        self.__plot_spec_in_roi()
+        if self._reg_done:
+            overlap_roi(self.viewer, self, mode="xanes_spec_roi")
+            self.__plot_spec_in_roi()
 
     def _def_fit_eng_rgn(self):
         (_, wl_fit_s, wl_fit_e, edge_fit_s, edge_fit_e, edge_eng, fit_type) = (
             def_dflt_eng_rgn(self._spec_in_roi, self._eng_lst)
         )
         self.analysis_type.value = fit_type
-        if fit_type == "wl":
-            self.wl_s.value = wl_fit_s
-            self.wl_e.value = wl_fit_e
-        else:
-            self.edge_eng.value = edge_eng
-            self.wl_s.value = wl_fit_s
-            self.wl_e.value = wl_fit_e
-            self.edge_s.value = edge_fit_s
-            self.edge_e.value = edge_fit_e
 
-    def __set_analysis_type(self):
-        if (self._eng_lst.min() > (float(self.edge_eng.value) - 50)) and (
-            self._eng_lst.max() < (float(self.edge_eng.value) + 50)
-        ):
-            self.analysis_type.value = "wl"
+        self.edge_eng.value = edge_eng
+        self.wl_s.value = wl_fit_s
+        self.wl_e.value = wl_fit_e
+        self.edge_s.value = edge_fit_s
+        self.edge_e.value = edge_fit_e
 
     def _xanes_fit_type_chgd(self):
         self.__set_analysis_type()
         self.wl_s.enabled = True
         self.wl_e.enabled = True
         global _XANES_FIT_SAVE_ITEMS_CHOICES
         if self.analysis_type.value == "wl":
@@ -585,12 +602,12 @@
             sig = os.system(f"ipython {xanes3d_fit_script_fn}")
         elif self.data_type.value == "2D XANES":
             sig = os.system(f"ipython {xanes2d_fit_script_fn}")
 
     def _close_file(self):
         if self._spec_in_roi_fig is not None:
             plt.close(self._spec_in_roi_fig)
+            self._spec_in_roi_fig = None
         rm_gui_viewers(self.viewer, self._viewers)
         if self._xanes_data_fn_p is not None:
             self._xanes_data_fn_p.close()
             self._xanes_data_fn_p = None
-            self._xanes_data = None
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,32 +84,35 @@
 #             auto reconstruction and alignment for XANES3D                    #
 ################################################################################
 class xanes_reg_gui:
     def __init__(self, viewer):
         self.viewer = viewer
         self._tomo_cfg = None
         self.scn_fntpl = None
+        self.rec_fntpl = None
         self._ref_rec_tplt = {"file_params": {"raw_data_top_dir": Path("")}}
         self._tomo_recon_tplt = None
         self._test_run_done = False
         self._continue_run_confirmed = False
         self._tomo_tplt_fn_old_val = ""
         self._3dxanes_new_rec_info = ""
         self._3dxanes_rec_roix_old_val = [0, 1]
         self._3dxanes_rec_roiy_old_val = [0, 1]
         self._3dxanes_rec_roiz_old_val = [0, 1]
         self._scn_id_s_old_val = ""
         self._scn_id_e_old_val = ""
         self._2dxanes_if_new_reg = True
         self._2dxanes_data = None
         self._2dxanes_eng_lst = None
+        self._2dxanes_reg_fn = None
+        self._2dxanes_reg_fn_p = None
+        self._2dxanes_fn = None
         self._2dxanes_fn_p = None
         self._2dxanes_data_ready = False
         self._2dxanes_new_reg_info = ""
-        self._2dxanes_reg_fn_p = None
         self._2dxanes_reg_roix_old_val = [0, 1]
         self._2dxanes_reg_roiy_old_val = [0, 1]
         self._2dxanes_reg_roiz_old_val = [0, 1]
         self._2dxanes_reg_ref_im_old_val = 0
         self._2dxanes_if_new_align = False
         self._2dxanes_align_roix_old_val = [0, 1]
         self._2dxanes_align_roiy_old_val = [0, 1]
@@ -187,15 +190,15 @@
             tooltip="confirm if the autocen results are good",
             enabled=False,
         )
         self.reg_run = widgets.PushButton(text="run")
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.data_type.changed.connect(self._xanes_data_type)
+        self.data_type.changed.connect(self._sel_in_data_type)
         self.tomo_tplt_fn.changed.connect(self._xanes_set_fn)
         self.scan_id_s.changed.connect(self._3dxanes_check_scan_id_s)
         self.scan_id_e.changed.connect(self._3dxanes_check_scan_id_e)
         self.auto_cen_dft_roi.changed.connect(self._3dxanes_tomo_auto_cen_dft_roi)
         self.auto_cen_roix.changed.connect(self._xanes_tomo_auto_cen_roix)
         self.auto_cen_roiy.changed.connect(self._xanes_tomo_auto_cen_roiy)
         self.ref_sli.changed.connect(self._xanes_tomo_auto_cen_ref_sli)
@@ -355,73 +358,82 @@
                 self.ang_corr_range.enabled = True
             else:
                 self.ang_corr_range.enabled = False
             self.test_run.enabled = True
             self.close_file.enabled = True
 
     def __3dxanes_tomo_show_sli(self, mode="auto_cen"):
+        sta = False
         if mode == "auto_cen":
+            # print("signature: auto_cen")
             try:
                 update_layer_in_viewer(
                     self.viewer,
                     tifffile.imread(
                         str(self.rec_fntpl).format(
                             self.ref_scan_id.value,
                             str(self.ref_sli.value).zfill(5),
                         )
                     ),
                     "xanes_raw_viewer",
                 )
+                sta = True
             except Exception as e:
                 self.op_status.value = (
                     "Something is wrong. Please check terminal for more information."
                 )
                 print(f"{str(e)=}")
+                sta = False
         elif mode == "recon_roi":
-            print("signature")
+            # print("signature: recon_roi")
             if self._3dxanes_rec_roiz_old_val[0] != self.rec_roiz.value[0]:
                 try:
                     update_layer_in_viewer(
                         self.viewer,
                         tifffile.imread(
                             str(self.rec_fntpl).format(
                                 self.ref_scan_id.value,
                                 str(self.rec_roiz.value[0]).zfill(5),
                             )
                         ),
                         "xanes_raw_viewer",
                     )
+                    sta = True
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
+                    sta = False
             elif self._3dxanes_rec_roiz_old_val[1] != self.rec_roiz.value[1]:
                 try:
                     update_layer_in_viewer(
                         self.viewer,
                         tifffile.imread(
                             str(self.rec_fntpl).format(
                                 self.ref_scan_id.value,
                                 str(self.rec_roiz.value[1]).zfill(5),
                             )
                         ),
                         "xanes_raw_viewer",
                     )
+                    sta = True
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
-        rng = (
-            self.viewer.layers["xanes_raw_viewer"].data.max()
-            - self.viewer.layers["xanes_raw_viewer"].data.min()
-        )
-        self.viewer.layers["xanes_raw_viewer"].contrast_limits = [
-            self.viewer.layers["xanes_raw_viewer"].data.min() + 0.1 * rng,
-            self.viewer.layers["xanes_raw_viewer"].data.max() - 0.1 * rng,
-        ]
-        self._3dxanes_rec_roiz_old_val = self.rec_roiz.value
-        self.viewer.reset_view()
+                    sta = False
+        if sta:
+            rng = (
+                self.viewer.layers["xanes_raw_viewer"].data.max()
+                - self.viewer.layers["xanes_raw_viewer"].data.min()
+            )
+            self.viewer.layers["xanes_raw_viewer"].contrast_limits = [
+                self.viewer.layers["xanes_raw_viewer"].data.min() + 0.1 * rng,
+                self.viewer.layers["xanes_raw_viewer"].data.max() - 0.1 * rng,
+            ]
+            self._3dxanes_rec_roiz_old_val = self.rec_roiz.value
+            self.viewer.reset_view()
 
     def __3dxnaes_tomo_def_autocent_cfg(self):
         with open(cfg_fn, "r") as f:
             tem = json.load(f)
             tem["xanes3d_auto_cen"]["cfg_file"] = str(
                 Path(self._ref_rec_tplt["file_params"]["raw_data_top_dir"])
                 / f"xanes3d_autocen&reg-{self._3dxanes_new_rec_info}.json"
@@ -578,49 +590,60 @@
                 [
                     int(dim[0] / 4),
                     int(dim[0] * 3 / 4),
                 ],
                 dim[0] - 1,
             )
 
-    @disp_progress_info("data directory info read")
     def _3dxanes_check_scan_id_s(self):
         if int(self.scan_id_s.value) > int(self.ref_scan_id.value):
             self.scan_id_s.value = self.ref_scan_id.value
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
-    @disp_progress_info("data directory info read")
     def _3dxanes_check_scan_id_e(self):
         if int(self.scan_id_e.value) < int(self.ref_scan_id.value):
             self.scan_id_e.value = self.ref_scan_id.value
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     def _3dxanes_tomo_auto_cen_dft_roi(self):
         if self.auto_cen_dft_roi.value:
             self.auto_cen_roix.enabled = False
             self.auto_cen_roiy.enabled = False
         else:
             self.auto_cen_roix.enabled = True
             self.auto_cen_roiy.enabled = True
-        overlap_roi(self.viewer, self, mode="auto_cen")
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+        if (self.rec_fntpl is not None) and (
+            Path(
+                str(self.rec_fntpl).format(
+                    self.ref_scan_id.value,
+                    str(self.ref_sli.value).zfill(5),
+                )
+            ).exists()
+        ):
+            overlap_roi(self.viewer, self, mode="auto_cen")
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     @disp_progress_info("xanes2d data loading")
     def __2dxanes_check_in_file(self):
-        self._2dxanes_fn = self.tomo_tplt_fn.value
         if self._2dxanes_fn_p is None:
-            self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
+            try:
+                self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
+            except Exception as e:
+                self._2dxanes_fn_p = None
+                self.op_status.value = "Invalid data file!"
+                print(e)
         else:
             self._2dxanes_fn_p.close()
             self._2dxanes_fn_p = h5py.File(self._2dxanes_fn, "r")
         if (
-            (self._2dxanes_fn_p["X_eng"].shape[0] > 1)
+            (self._2dxanes_fn_p is not None)
+            and (self._2dxanes_fn_p["X_eng"].shape[0] > 1)
             and len(self._2dxanes_fn_p["img_xanes"].shape) == 3
             and self._2dxanes_fn_p["X_eng"].shape[0]
             == self._2dxanes_fn_p["img_xanes"].shape[0]
         ):
             try:
                 self._2dxanes_eng_lst = self._2dxanes_fn_p["X_eng"][:]
                 dark = self._2dxanes_fn_p["img_dark"][:].squeeze()
@@ -643,14 +666,20 @@
                 print(str(e))
                 self._2dxanes_fn_p.close()
                 self._2dxanes_fn_p = None
                 self._2dxanes_data = None
                 self._2dxanes_eng_lst = None
                 self._2dxanes_fn = None
                 self._2dxanes_data_ready = False
+        else:
+            self._2dxanes_fn_p = None
+            self._2dxanes_data = None
+            self._2dxanes_eng_lst = None
+            self._2dxanes_fn = None
+            self._2dxanes_data_ready = False
         self._test_run_done = False
         self._continue_run_confirmed = False
 
     def __2dxanes_set_widget(self):
         if self._2dxanes_data_ready:
             self.scan_id_s.enabled = False
             self.scan_id_e.enabled = False
@@ -693,71 +722,78 @@
             self.ang_corr_range.enabled = False
             self.test_run.enabled = False
             self.confirm_test_run.enabled = False
             self.reg_run.enabled = False
             self.close_file.enabled = False
 
     def __2dxanes_show_sli(self, mode="auto_reg"):
+        sta = False
         if mode == "auto_reg":
             if self.ref_sli.value < self.rec_roiz.value[0]:
                 if self.rec_roiz.value[0] < len(self._2dxanes_eng_lst):
                     self.ref_sli.value = self.rec_roiz.value[0]
             if self.ref_sli.value > self.rec_roiz.value[1]:
                 if self.rec_roiz.value[1] < len(self._2dxanes_eng_lst):
                     self.ref_sli.value = self.rec_roiz.value[1]
-
-            tem = self.viewer.dims.current_step
             try:
+                tem = self.viewer.dims.current_step
                 self.viewer.dims.current_step = [
                     self.ref_sli.value,
                     int(tem[1]),
                     int(tem[2]),
                 ]
+                self.ref_scan_id.value = (
+                    f"{float(self._2dxanes_eng_lst[self.ref_sli.value]) * 1000}eV"
+                )
+                sta = True
             except Exception as e:
                 self.op_status.value = (
                     "Something is wrong. Please check terminal for more information."
                 )
                 print(str(e))
-
-            self.ref_scan_id.value = (
-                f"{float(self._2dxanes_eng_lst[self.ref_sli.value]) * 1000}eV"
-            )
+                sta = False
         elif mode == "auto_algn":
             if self._2dxanes_reg_roiz_old_val[0] != self.rec_roiz.value[0]:
                 if self.rec_roiz.value[0] > self.ref_sli.value:
                     self.rec_roiz.value = [self.ref_sli.value, self.rec_roiz.value[1]]
-                tem = self.viewer.dims.current_step
                 try:
+                    tem = self.viewer.dims.current_step
                     self.viewer.dims.current_step = [
                         self.rec_roiz.value[0],
                         int(tem[1]),
                         int(tem[2]),
                     ]
                     self.ref_scan_id.value = f"{float(self._2dxanes_eng_lst[self.rec_roiz.value[0]]) * 1000}eV"
+                    sta = True
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
+                    sta = False
             elif self._2dxanes_reg_roiz_old_val[1] != self.rec_roiz.value[1]:
                 if self.rec_roiz.value[1] < self.ref_sli.value:
                     self.rec_roiz.value = [self.rec_roiz.value[0], self.ref_sli.value]
-                tem = self.viewer.dims.current_step
                 try:
+                    tem = self.viewer.dims.current_step
                     self.viewer.dims.current_step = [
                         self.rec_roiz.value[1],
                         int(tem[1]),
                         int(tem[2]),
                     ]
                     self.ref_scan_id.value = f"{float(self._2dxanes_eng_lst[self.rec_roiz.value[1]]) * 1000}eV"
+                    sta = True
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
+                    sta = False
+        if sta:
             self._2dxanes_reg_roiz_old_val = self.rec_roiz.value
-        self.viewer.reset_view()
+            self.viewer.reset_view()
 
     def __2dxanes_set_roi_lims(self):
+        # if self._2dxanes_data_ready:
         dim = self._2dxanes_data.shape
         set_data_widget(
             self.ref_sli,
             0,
             int(dim[0] / 2),
             dim[0] - 1,
         )
@@ -891,65 +927,107 @@
         xanes2d_image_autocent_cfg["meta"]["eng_list"] = list(
             self._2dxanes_eng_lst[self.rec_roiz.value[0] : self.rec_roiz.value[1]]
         )
 
         with open(tem["xanes2d_reg"]["cfg_file"], "w") as f:
             json.dump(xanes2d_image_autocent_cfg, f, indent=4, separators=(",", ": "))
 
-    def __xanes_reset_run_status(self):
-        self._test_run_done = False
-        self.confirm_test_run.value == "No"
-        self._continue_run_confirmed = False
-
-    def __xanes_reset_run_buttons(self):
-        if self._test_run_done:
-            self.confirm_test_run.enabled = True
-        else:
-            self.confirm_test_run.enabled = False
-            self.confirm_test_run.value == "No"
-            self._continue_run_confirmed = False
-        if self._continue_run_confirmed:
-            self.reg_run.enabled = True
-        else:
-            self.reg_run.enabled = False
-
-    def _xanes_data_type(self):
-        self.tomo_tplt_fn.value = ""
+    def __reset_widgets_val(self):
         self.ref_scan_id.value = ""
         global _TOMO_XANES3D_REC_ID_S_CHOICES
         _TOMO_XANES3D_REC_ID_S_CHOICES = []
         self.scan_id_s.reset_choices()
         global _TOMO_XANES3D_REC_ID_E_CHOICES
         _TOMO_XANES3D_REC_ID_E_CHOICES = []
         self.scan_id_e.reset_choices()
         self.auto_cen_dft_roi.value = False
-        self.auto_cen_roix.value = [540, 740]
-        self.auto_cen_roiy.value = [540, 740]
+        set_data_widget(
+            self.auto_cen_roix,
+            1,
+            [540, 740],
+            1280,
+        )
+        set_data_widget(
+            self.auto_cen_roiy,
+            1,
+            [540, 740],
+            1280,
+        )
         self.ref_sli.value = 540
-        self.rec_roix.value = [540, 740]
-        self.rec_roiy.value = [540, 740]
-        self.rec_roiz.value = [440, 640]
+        set_data_widget(
+            self.rec_roix,
+            1,
+            [540, 740],
+            1280,
+        )
+        set_data_widget(
+            self.rec_roiy,
+            1,
+            [540, 740],
+            1280,
+        )
+        set_data_widget(
+            self.rec_roiz,
+            1,
+            [440, 640],
+            1080,
+        )
         self.sli_srch_range.value = 10
         self.cen_srch_range.value = 15
         self.ang_corr.value = False
         self.ang_corr_range.value = 2.0
-        self.confirm_test_run.value = "No"
         self.op_status.value = ""
-        self.rec_fntpl = None
+
+    def __reset_run_states(self):
         self._test_run_done = False
+        self.confirm_test_run.value == "No"
         self._continue_run_confirmed = False
+
+    def __reset_run_buttons(self):
+        if self._test_run_done:
+            self.confirm_test_run.enabled = True
+        else:
+            self.confirm_test_run.enabled = False
+            self.confirm_test_run.value == "No"
+            self._continue_run_confirmed = False
+        if self._continue_run_confirmed:
+            self.reg_run.enabled = True
+        else:
+            self.reg_run.enabled = False
+
+    def __reset_data_states(self):
+        self.rec_fntpl = None
+
+        self._2dxanes_data_ready = False
+        if self._2dxanes_fn_p is not None:
+            self._2dxanes_fn_p.close()
+            self._2dxanes_fn_p = None
+        self._2dxanes_fn = None
+        if self._2dxanes_reg_fn_p is not None:
+            self._2dxanes_reg_fn_p.close()
+            self._2dxanes_reg_fn_p = None
+        self._2dxanes_reg_fn = None
+
+    def _sel_in_data_type(self):
+        self.__reset_data_states()
+        self.__reset_widgets_val()
         if self.data_type.value == "3D XANES":
             self.tomo_tplt_fn.filter = "*.json"
             self.__3dxanes_set_widget()
         else:
             self.tomo_tplt_fn.filter = "*.h5"
             self.__2dxanes_set_widget()
-        self.__xanes_reset_run_buttons()
+        self.__reset_run_states()
+        self.__reset_run_buttons()
+        self._close_file()
 
+    @disp_progress_info("data directory info read")
     def _xanes_set_fn(self):
+        self.__reset_data_states()
+        self.__reset_widgets_val()
         if self.data_type.value == "3D XANES":
             self._tomo_tplt_fn = self.tomo_tplt_fn.value
             cfg_type = check_cfg_type(self._tomo_tplt_fn)
             if cfg_type == "xanes3d_tomo_tplt":
                 with open(self._tomo_tplt_fn, "r") as f:
                     tem = json.load(f)
                     self.ref_scan_id.value = list(tem.keys())[0]
@@ -970,71 +1048,148 @@
                     self._tomo_cfg = FLY_CFG["io_data_structure_xanes3D"]
                 self.__3dxanes_comp_tomo_fntpl()
                 self.__3dxanes_tomo_check_avail_id_s()
                 self.__3dxanes_tomo_check_avail_id_e()
                 self.__3dxanes_set_scan_id_lims()
                 self.__3dxanes_set_widget()
                 self.__3dxanes_set_roi_lims()
-                self.__3dxanes_tomo_show_sli(mode="auto_cen")
-                self.__xanes_reset_run_status()
-                self.__xanes_reset_run_buttons()
+                if (self.rec_fntpl is None) or (
+                    not Path(
+                        str(self.rec_fntpl).format(
+                            self.ref_scan_id.value,
+                            str(self.ref_sli.value).zfill(5),
+                        )
+                    ).exists()
+                ):
+                    self.__3dxanes_tomo_show_sli(mode="auto_cen")
             else:
                 self.op_status.value = (
                     "wrong type of json cfg file. check error message in terminal"
                 )
                 print(
                     "The required json file should have file name starting with 'xanes3d_tomo_tplt_cfg'."
                 )
         else:
+            self._2dxanes_fn = self.tomo_tplt_fn.value
             self.__2dxanes_check_in_file()
             self.__2dxanes_set_widget()
-            self.__2dxanes_set_roi_lims()
-            self.__2dxanes_show_sli(mode="auto_reg")
-            _min = self.viewer.layers["xanes_raw_viewer"].data[self.ref_sli.value].min()
-            _max = self.viewer.layers["xanes_raw_viewer"].data[self.ref_sli.value].max()
-            rng = _max - _min
-            self.viewer.layers["xanes_raw_viewer"].contrast_limits = [
-                _min + 0.1 * rng,
-                _max - 0.1 * rng,
-            ]
-            self.__xanes_reset_run_status()
-            self.__xanes_reset_run_buttons()
+            if self._2dxanes_data_ready:
+                self.__2dxanes_set_roi_lims()
+                self.__2dxanes_show_sli(mode="auto_reg")
+                _min = (
+                    self.viewer.layers["xanes_raw_viewer"]
+                    .data[self.ref_sli.value]
+                    .min()
+                )
+                _max = (
+                    self.viewer.layers["xanes_raw_viewer"]
+                    .data[self.ref_sli.value]
+                    .max()
+                )
+                rng = _max - _min
+                self.viewer.layers["xanes_raw_viewer"].contrast_limits = [
+                    _min + 0.1 * rng,
+                    _max - 0.1 * rng,
+                ]
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_roix(self):
-        overlap_roi(self.viewer, self, mode="auto_cen")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+        if self.data_type.value == "3D XANES":
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
+        else:
+            if self._2dxanes_data_ready:
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_roiy(self):
-        overlap_roi(self.viewer, self, mode="auto_cen")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+        if self.data_type.value == "3D XANES":
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
+        else:
+            if self._2dxanes_data_ready:
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     def _xanes_tomo_auto_cen_ref_sli(self):
         if self.data_type.value == "3D XANES":
-            self.__3dxanes_tomo_show_sli(mode="auto_cen")
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                self.__3dxanes_tomo_show_sli(mode="auto_cen")
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
         else:
-            self.__2dxanes_show_sli(mode="auto_reg")
-        overlap_roi(self.viewer, self, mode="auto_cen")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
-        self.__xanes_reset_run_status()
-        self.__xanes_reset_run_buttons()
+            if self._2dxanes_data_ready:
+                self.__2dxanes_show_sli(mode="auto_reg")
+                overlap_roi(self.viewer, self, mode="auto_cen")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "auto_cen_roi"])
+        self.__reset_run_states()
+        self.__reset_run_buttons()
 
     def _xanes_tomo_rec_roix(self):
-        overlap_roi(self.viewer, self, mode="recon_roi")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
-        if self.data_type.value == "2D XANES":
+        if self.data_type.value == "3D XANES":
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
+        else:
+            if self._2dxanes_data_ready:
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
             self.confirm_test_run.value = "No"
 
     def _xanes_tomo_rec_roiy(self):
-        overlap_roi(self.viewer, self, mode="recon_roi")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
-        if self.data_type.value == "2D XANES":
+        if self.data_type.value == "3D XANES":
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
+        else:
+            if self._2dxanes_data_ready:
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
             self.confirm_test_run.value = "No"
 
     def _xanes_tomo_rec_roiz(self):
         if self.data_type.value == "3D XANES":
             if self.rec_roiz.value[0] > (
                 self.ref_sli.value - self.sli_srch_range.value
             ):
@@ -1045,20 +1200,31 @@
             if self.rec_roiz.value[1] < (
                 self.ref_sli.value + self.sli_srch_range.value
             ):
                 self.rec_roiz.value = [
                     self.rec_roiz.value[0],
                     self.ref_sli.value + self.sli_srch_range.value,
                 ]
-            self.__3dxanes_tomo_show_sli(mode="recon_roi")
+            if (self.rec_fntpl is not None) and (
+                Path(
+                    str(self.rec_fntpl).format(
+                        self.ref_scan_id.value,
+                        str(self.ref_sli.value).zfill(5),
+                    )
+                ).exists()
+            ):
+                self.__3dxanes_tomo_show_sli(mode="recon_roi")
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
         else:
-            self.__2dxanes_show_sli(mode="auto_algn")
+            if self._2dxanes_data_ready:
+                self.__2dxanes_show_sli(mode="auto_algn")
+                overlap_roi(self.viewer, self, mode="recon_roi")
+                show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
             self.confirm_test_run.value = "No"
-        overlap_roi(self.viewer, self, mode="recon_roi")
-        show_layers_in_viewer(self.viewer, ["xanes_raw_viewer", "recon_roi"])
 
     @disp_progress_info("xanes auto registration test run")
     def _xanes_test_run(self):
         if self.data_type.value == "3D XANES":
             self.__3dxanes_tomo_if_new_rec()
             self.__3dxnaes_tomo_def_autocent_cfg()
 
@@ -1086,15 +1252,15 @@
                 self._test_run_done = True
             else:
                 self._test_run_done = False
                 self.op_status.value = "auto centering fails"
                 print("auto centering fails")
             self.confirm_test_run.value == "No"
             self._continue_run_confirmed = False
-            self.__xanes_reset_run_buttons()
+            self.__reset_run_buttons()
         else:
             self.__2dxanes_check_if_new_reg()
             self.__2dxanes_def_img_autoreg_cfg()
 
             if self._2dxanes_if_new_reg:
                 sig = os.system(f"ipython {xanes2d_img_auto_cen_script_fn}")
 
@@ -1119,15 +1285,15 @@
                     self._test_run_done = True
                 else:
                     self._test_run_done = False
                     self.op_status.value = "auto alignment fails"
                     print("auto alignment fails")
                 self.confirm_test_run.value == "No"
                 self._continue_run_confirmed = False
-                self.__xanes_reset_run_buttons()
+                self.__reset_run_buttons()
             else:
                 self.op_status.value = "Nothing is changed from last auto-registration."
                 print("Nothing is changed from last auto-registration.")
 
     def _xanes_confirm_to_run(self):
         if self.confirm_test_run.value == "Yes":
             self._continue_run_confirmed = True
@@ -1203,14 +1369,14 @@
                     self.op_status.value = "Alignment fails"
                     print("Alignment fails")
             else:
                 self.op_status.value = "Nothing is changed from last alignment."
                 print("Nothing is changed from last alignment.")
 
     def _close_file(self):
-        if self._2dxanes_reg_fn is not None:
-            self._2dxanes_reg_fn.close()
+        if self._2dxanes_reg_fn_p is not None:
+            self._2dxanes_reg_fn_p.close()
             self._2dxanes_reg_fn = None
         if self._2dxanes_fn_p is not None:
             self._2dxanes_fn_p.close()
             self._2dxanes_fn_p = None
         rm_gui_viewers(self.viewer, self._viewers)
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
         self.vis_mk_mask = widgets.PushButton(text="make mask", enabled=False)
         self.vis_info_board = widgets.TextEdit(
             label="data info", value="", enabled=False
         )
         self.close_file = widgets.PushButton(text="close file", enabled=False)
         self.op_status = widgets.LineEdit(name="operation status", enabled=False)
 
-        self.vis_in_data_type.changed.connect(self._sel_vis_in_data_type)
-        self.vis_data_file.changed.connect(self._sel_vis_in_data_file)
-        self.vis_avail_items.changed.connect(self._sel_vis_in_avail_items)
+        self.vis_in_data_type.changed.connect(self._sel_in_data_type)
+        self.vis_data_file.changed.connect(self._sel_in_data_file)
+        self.vis_avail_items.changed.connect(self._sel_in_avail_items)
         self.vis_rd_contr_lims.changed.connect(self._read_contr_lims)
         self.vis_mk_mask.changed.connect(self._mk_mask)
         self.vis_test_mask_thsh.changed.connect(self._test_mask_thsh)
         self.confirm_mask_thsh.changed.connect(self._confirm_thsh)
         self.close_file.changed.connect(self._close_file)
 
         self.gui_layout = widgets.VBox(
@@ -175,44 +175,59 @@
                     self._vis_data_ready = False
             except Exception as e:
                 self.viewer.status = "Something wrong happened during openning data file. Please check the terminal for more information."
                 print(str(e))
                 self._close_file()
                 self._vis_data_ready = False
 
-    def _sel_vis_in_data_type(self):
+    def __reset_widget_val(self):
         self.vis_data_file.value = ""
         global _AVAIL_DATA_ITEM_CHOICES
         _AVAIL_DATA_ITEM_CHOICES = []
         self.vis_avail_items.reset_choices()
         self.vis_data_cntrst_lowlim.value = ""
         self.vis_data_cntrst_highlim.value = ""
         self.confirm_mask_thsh.value = "No"
         self.vis_info_board.value = ""
         self.op_status.value = ""
+
+    def __reset_data_states(self):
         self._vis_data_ready = False
+        self._vis_data = None
+        self._thsh_for_mask = None
+
+    def __reset_run_states(self):
+        self._mask_thsh_confirmed = False
+
+    def _sel_in_data_type(self):
+        self.__reset_run_states()
+        self.__reset_data_states()
+        self.__reset_widget_val()
         self._close_file()
         self.__lock_vis_gui_widgets()
 
     @disp_progress_info("data loading")
-    def _sel_vis_in_data_file(self):
+    def _sel_in_data_file(self):
+        self.__reset_run_states()
+        self.__reset_data_states()
+        self._close_file()
         choices = check_avail_items(
             self.vis_data_file.value, self.vis_in_data_type.value
         )
         global _AVAIL_DATA_ITEM_CHOICES
         _AVAIL_DATA_ITEM_CHOICES = choices
         self.vis_avail_items.reset_choices()
         if _AVAIL_DATA_ITEM_CHOICES:
             self._vis_data_ready = True
         else:
             self._vis_data_ready = False
         self.__avail_item_slcd()
         self.__lock_vis_gui_widgets()
 
-    def _sel_vis_in_avail_items(self):
+    def _sel_in_avail_items(self):
         self.__avail_item_slcd()
         self.__lock_vis_gui_widgets()
 
     def _read_contr_lims(self):
         self.vis_data_cntrst_lowlim.value = self.viewer.layers[
             "vis_data"
         ].contrast_limits[0]
@@ -372,9 +387,8 @@
             self.vis_mk_mask.enabled = False
             self._thsh_for_mask = None
 
     def _close_file(self):
         if self._vis_fn_p is not None:
             self._vis_fn_p.close()
             self._vis_fn_p = None
-            self._vis_data = None
             rm_gui_viewers(self.viewer, self._viewers)
```

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.0.post6/TXM_Sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post5/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.0.post6/txm_sandbox.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 TXM_GUI2.ipynb
 setup.py
+TXM_Sandbox/config/XANES2D_GUI_config.json
+TXM_Sandbox/config/analysis_tool_gui_cfg.json
+TXM_Sandbox/config/io_tomo_h5_data_structure.json
+TXM_Sandbox/config/io_xanes2D_h5_data_structure.json
+TXM_Sandbox/config/io_xanes3D_h5_data_structure.json
+TXM_Sandbox/tmp/readme.txt
 txm_sandbox/__init__.py
 txm_sandbox.egg-info/PKG-INFO
 txm_sandbox.egg-info/SOURCES.txt
 txm_sandbox.egg-info/dependency_links.txt
 txm_sandbox.egg-info/not-zip-safe
 txm_sandbox.egg-info/requires.txt
 txm_sandbox.egg-info/top_level.txt
```

