# Comparing `tmp/parallax_app-0.37.5.tar.gz` & `tmp/parallax_app-0.37.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.5.tar", last modified: Wed May  1 18:25:06 2024, max compression
+gzip compressed data, was "parallax_app-0.37.6.tar", last modified: Thu May  9 18:18:04 2024, max compression
```

## Comparing `parallax_app-0.37.5.tar` & `parallax_app-0.37.6.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.672980 parallax_app-0.37.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.676980 parallax_app-0.37.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 18:24:24.000000 parallax_app-0.37.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 18:24:24.000000 parallax_app-0.37.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:25:06.688980 parallax_app-0.37.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-01 18:24:24.000000 parallax_app-0.37.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.676980 parallax_app-0.37.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/ReadMe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/parallax.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 18:24:24.000000 parallax_app-0.37.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.680980 parallax_app-0.37.5/img/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-01 18:24:24.000000 parallax_app-0.37.5/img/target.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/parallax/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/calibration_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27694 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/curr_bg_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/curr_prev_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    32394 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/main_window_wip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/mask_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5120 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/no_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/probe_fine_tip_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/recording_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/reticle_detection_coords_interests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12228 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/screen_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/user_setting_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-01 18:24:24.000000 parallax_app-0.37.5/parallax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/parallax_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 18:25:06.000000 parallax_app-0.37.5/parallax_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-01 18:24:24.000000 parallax_app-0.37.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:25:06.688980 parallax_app-0.37.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 18:24:24.000000 parallax_app-0.37.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-01 18:24:24.000000 parallax_app-0.37.5/tests/test_screen_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/ParallaxReadME.JPG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.684980 parallax_app-0.37.5/ui/font/
--rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/font/FiraCode-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/mainWindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/probe_calib.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:25:06.688980 parallax_app-0.37.5/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/check.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/recordingButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_green.png
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/target.png
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/resources/x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/reticle_calib.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/settingPopUpMenu.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-01 18:24:24.000000 parallax_app-0.37.5/ui/stage_info.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.663052 parallax_app-0.37.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 18:17:27.000000 parallax_app-0.37.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 18:18:04.679052 parallax_app-0.37.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 18:17:27.000000 parallax_app-0.37.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/ReadMe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/parallax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/target.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/parallax/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/axis_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/calibration_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27694 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/curr_bg_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/curr_prev_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/main_window_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/mask_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_fine_tip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/recording_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detection_coords_interests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13394 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/screen_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34101 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/user_setting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/parallax_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-09 18:17:27.000000 parallax_app-0.37.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:18:04.679052 parallax_app-0.37.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 18:17:27.000000 parallax_app-0.37.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_screen_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/ParallaxReadME.JPG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/ui/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/mainWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/probe_calib.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/recordingButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/target.png
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/reticle_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/settingPopUpMenu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.5/.github/workflows/ci.yml` & `parallax_app-0.37.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/.github/workflows/tag_and_publish.yml` & `parallax_app-0.37.6/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/LICENSE` & `parallax_app-0.37.6/LICENSE`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/PKG-INFO` & `parallax_app-0.37.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.5
+Version: 0.37.6
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.5/README.md` & `parallax_app-0.37.6/README.md`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/docs/Makefile` & `parallax_app-0.37.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/docs/ReadMe.rst` & `parallax_app-0.37.6/docs/ReadMe.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/docs/conf.py` & `parallax_app-0.37.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/docs/make.bat` & `parallax_app-0.37.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/docs/parallax.rst` & `parallax_app-0.37.6/docs/parallax.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/arrow-right.png` & `parallax_app-0.37.6/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/gear.png` & `parallax_app-0.37.6/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/recordingButton.png` & `parallax_app-0.37.6/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/sextant.png` & `parallax_app-0.37.6/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/snapshotButton_white.png` & `parallax_app-0.37.6/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/stop-sign.png` & `parallax_app-0.37.6/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/img/target.png` & `parallax_app-0.37.6/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/__main__.py` & `parallax_app-0.37.6/parallax/__main__.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/calibration_camera.py` & `parallax_app-0.37.6/parallax/calibration_camera.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,55 +255,59 @@
         self.mtxA, self.distA = intrinsicA[0], intrinsicA[1]
         self.mtxB, self.distB = intrinsicB[0], intrinsicB[1]
         self.criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 100, 0.001)
         self.flags = cv2.CALIB_FIX_INTRINSIC
         self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB = None, None, None, None, None 
         self.P_A, self.P_B = None, None
 
-    def calibrate_stereo(self):
-        """Calibrate stereo cameras.
-
-        Returns:
-            tuple: Stereo calibration results (retval, R_AB, T_AB, E_AB, F_AB).
-        """
-        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = (
-            cv2.stereoCalibrate(
-                self.objpoints,
-                self.imgpointsA,
-                self.imgpointsB,
-                self.mtxA,
-                self.distA,
-                self.mtxB,
-                self.distB,
-                SIZE,
-                criteria=self.criteria,
-                flags=self.flags,
-            )
-        )
-
+    def print_calibrate_stereo_results(self):
+        if self.retval is None or self.R_AB is None or self.T_AB is None:
+            return
         print("\n== Stereo Calibration ==")
         print("AB")
         print(self.retval)
         print(f"R: \n{self.R_AB}")
         print(f"T: \n{self.T_AB}")
         print(np.linalg.norm(self.T_AB))
 
+        if self.F_AB is None or self.E_AB is None:
+            return
         formatted_F = (
             "F_AB:\n"
             + "\n".join(
                 [" ".join([f"{val:.5f}" for val in row]) for row in self.F_AB]
             ) + "\n")
         formatted_E = (
             "E_AB:\n"
             + "\n".join(
                 [" ".join([f"{val:.5f}" for val in row]) for row in self.E_AB]
             ) + "\n")
         print(formatted_F)
         print(formatted_E)
 
+    def calibrate_stereo(self):
+        """Calibrate stereo cameras.
+
+        Returns:
+            tuple: Stereo calibration results (retval, R_AB, T_AB, E_AB, F_AB).
+        """
+        self.retval, _, _, _, _, self.R_AB, self.T_AB, self.E_AB, self.F_AB = (
+            cv2.stereoCalibrate(
+                self.objpoints,
+                self.imgpointsA,
+                self.imgpointsB,
+                self.mtxA,
+                self.distA,
+                self.mtxB,
+                self.distB,
+                SIZE,
+                criteria=self.criteria,
+                flags=self.flags,
+            )
+        )
         self.P_A = self.mtxA @ np.hstack((np.eye(3), np.zeros((3, 1))))
         self.P_B = self.mtxB @ np.hstack((self.R_AB, self.T_AB.reshape(-1, 1)))
 
         return self.retval, self.R_AB, self.T_AB, self.E_AB, self.F_AB
 
     def _matching_camera_order(self, camA, coordA, camB, coordB):
         """Match camera order based on initialization order.
@@ -453,15 +457,15 @@
         l2_y = np.sqrt(mean_squared_diff_y)
         l2_z = np.sqrt(mean_squared_diff_z)
 
         print(
             f"x: {l2_x*1000}µm³, y: {l2_y*1000}µm³, z:{l2_z*1000}µm³"
         )
 
-    def test_performance(self, camA, coordA, camB, coordB):
+    def test_performance(self, camA, coordA, camB, coordB, print_results=False):
         """Test stereo calibration.
 
         Args:
             camA (str): Camera A name.
             coordA (tuple): Coordinates from camera A.
             camB (str): Camera B name.
             coordB (tuple): Coordinates from camera B.
@@ -478,27 +482,29 @@
             self.P_B, self.P_A, self.imgpointsB, self.imgpointsA
         )
         np.set_printoptions(suppress=True, precision=8)
 
         points_3d_G = self.change_coords_system_from_camA_to_global_iterative(
             points_3d_AB
         )
-        print("\n=solvePnP SOLVEPNP_ITERATIVE=")
+        
         differences = points_3d_G - self.objpoints[0]
         squared_distances = np.sum(np.square(differences), axis=1)
         euclidean_distances = np.sqrt(squared_distances)
         average_L2_distance = np.mean(euclidean_distances)
-        print(
-            f"(Reprojection error) Object points L2 diff: \
-            {average_L2_distance*1000} µm³"
-        )
-        self.test_x_y_z_performance(points_3d_G)
-        print(f"Object points predict:\n{np.around(points_3d_G, decimals=5)}")
+        if print_results:
+            print("\n=solvePnP SOLVEPNP_ITERATIVE=")
+            print(
+                f"(Reprojection error) Object points L2 diff: \
+                {average_L2_distance*1000} µm³"
+            )
+            self.test_x_y_z_performance(points_3d_G)
+            print(f"Object points predict:\n{np.around(points_3d_G, decimals=5)}")
 
-        self.test_pixel_error()
+            self.test_pixel_error()
         return average_L2_distance
 
     def test_pixel_error(self):
         """Test pixel reprojection error."""
         mean_error = 0
         for i in range(len(self.objpoints)):
             imgpointsA_converted = np.array(
```

### Comparing `parallax_app-0.37.5/parallax/camera.py` & `parallax_app-0.37.6/parallax/camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.6/parallax/curr_bg_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.6/parallax/curr_prev_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/main_window_wip.py` & `parallax_app-0.37.6/parallax/main_window_wip.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,29 +573,28 @@
         # Get the prev camera lists displaying on the screen
         prev_camera, curr_camera = screen.get_camera_name(), selected_sn
         prev_lists = [
             screen.get_camera_name()
             for screen in self.screen_widgets
             if screen.get_camera_name()
         ]
-        if (
-            0 <= screen_index < len(prev_lists)
-        ):  # Ensure screen_index is within valid range
+
+        # Ensure screen_index is within valid range
+        if (0 <= screen_index < len(prev_lists)):  
             curr_list = prev_lists[:]
             curr_list.pop(screen_index)
             curr_list.insert(screen_index, curr_camera)
         else:
             logger.error(f"Invalid screen index: {screen_index}")
         logger.debug(f"prev_list: {prev_lists}")
         logger.debug(f"curr_list: {curr_list}")
 
         # Handle updates based on the current state of the application
-        if (
-            self.startButton.isChecked()
-        ):  # If the 'Start' button is enabled (continuous acquisition mode)
+        # If the 'Start' button is enabled (continuous acquisition mode)
+        if (self.startButton.isChecked()):  
             if set(prev_lists) == set(curr_list):
                 # If the list of cameras hasn't changed, just update the current screen's camera
                 screen.set_camera(camera_list.get(curr_camera))
             else:
                 if prev_camera not in curr_list:
                     # If the previous camera has been removed from the list, stop its acquisition
                     screen.stop_acquisition_camera()
```

### Comparing `parallax_app-0.37.5/parallax/mask_generator.py` & `parallax_app-0.37.6/parallax/mask_generator.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/model.py` & `parallax_app-0.37.6/parallax/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self.stage_listener_url = "http://localhost:8080/"
 
         # probe detector
         self.probeDetectors = []
 
         # coords axis
         self.coords_axis = {}
+        self.pos_x = {}
         self.camera_intrinsic = {}
         self.camera_extrinsic = {}
         self.calibration = None
         self.calibrations = {}
 
         self.cal_in_progress = False
         self.accutest_in_progress = False
@@ -127,14 +128,32 @@
         """Get a stage."""
         return self.stages.get(stage_sn)
 
     def add_probe_detector(self, probeDetector):
         """Add a probe detector."""
         self.probeDetectors.append(probeDetector)
 
+    def reset_coords_intrinsic_extrinsic(self):
+        """Reset coordinates intrinsic extrinsic."""
+        self.coords_axis = {}
+        self.camera_intrinsic = {}
+        self.camera_extrinsic = {}
+    
+    def add_pos_x(self, camera_name, pt):
+        """Add position x."""
+        self.pos_x[camera_name] = pt
+
+    def get_pos_x(self, camera_name):
+        """Add position x."""
+        return self.pos_x.get(camera_name)
+    
+    def reset_pos_x(self):
+        """Reset position x."""
+        self.pos_x = {}
+    
     def add_coords_axis(self, camera_name, coords):
         """Add coordinates axis."""
         self.coords_axis[camera_name] = coords
 
     def get_coords_axis(self, camera_name):
         """Get coordinates axis."""
         return self.coords_axis.get(camera_name)
```

### Comparing `parallax_app-0.37.5/parallax/no_filter.py` & `parallax_app-0.37.6/parallax/no_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
 NoFilter serves as a pass-through component in a frame processing pipeline, 
 employing a worker-thread model to asynchronously handle frames without modification, 
 facilitating integration and optional processing steps.
 """
 
+import logging
 import time
 
+import cv2
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
+# Set logger name
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 
 class NoFilter(QObject):
     """Class representing no filter."""
 
     name = "None"
     frame_processed = pyqtSignal(object)
 
@@ -23,14 +28,15 @@
 
         def __init__(self, name):
             """Initialize the worker object."""
             QObject.__init__(self)
             self.name = name
             self.running = True
             self.new = False
+            self.frame = None
 
         def update_frame(self, frame):
             """Update the frame to be processed.
 
             Args:
                 frame: The frame to be processed.
             """
@@ -58,62 +64,94 @@
             while self.running:
                 if self.new:
                     self.process(self.frame)
                     self.new = False
                 time.sleep(0.001)
             self.finished.emit()
 
-    def __init__(self):
+        def set_name(self, name):
+            """Set name as camera serial number."""
+            self.name = name
+
+    def __init__(self, camera_name):
         """Initialize the filter object."""
+        logger.debug(f"{self.name} Init no filter manager")
         super().__init__()
         self.worker = None
+        self.name = camera_name
         self.thread = None
-        self.init_thread()
+        self.start()
 
     def init_thread(self):
         """Initialize or reinitialize the worker and thread"""
+        if self.thread is not None:
+            self.clean()  # Clean up existing thread and worker before reinitializing 
         self.thread = QThread()
         self.worker = self.Worker(self.name)
         self.worker.moveToThread(self.thread)
 
         self.thread.started.connect(self.worker.run)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.thread.destroyed.connect(self.onThreadDestroyed)
+        self.threadDeleted = False
+
         self.worker.frame_processed.connect(self.frame_processed.emit)
         self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(lambda: self.thread_deleted)
         self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
-
-        self.thread.start()
+        self.worker.destroyed.connect(self.onWorkerDestroyed) # Debug msg
+        logger.debug(f"{self.name} init camera name")
 
     def process(self, frame):
         """Process the frame using the worker.
 
         Args:
             frame: The frame to be processed.
         """
         if self.worker is not None:
             self.worker.update_frame(frame)
 
     def start(self):
         """Start the filter by reinitializing and starting the worker and thread."""
+        logger.debug(f" {self.name} Starting thread")
         self.init_thread()  # Reinitialize and start the worker and thread
+        self.thread.start()
+        self.worker.start_running()
 
     def stop(self):
         """Stop the filter by stopping the worker."""
+        logger.debug(f" {self.name} Stopping thread")
         if self.worker is not None:
             self.worker.stop_running()
 
+    def onWorkerDestroyed(self):
+        """Cleanup after worker finishes."""
+        logger.debug(f"{self.name} worker destroyed")
+
+    def onThreadDestroyed(self):
+        """Flag if thread is deleted"""
+        logger.debug(f"{self.name} thread destroyed")
+        self.threadDeleted = True
+        self.thread = None
+
+    def set_name(self, camera_name):
+        """Set camera name."""
+        self.name = camera_name
+        if self.worker is not None:
+            self.worker.set_name(self.name)
+        logger.debug(f"{self.name} set camera name")
+
     def clean(self):
-        """Clean up the filter by stopping the worker and waiting for the thread to finish."""
+        """Safely clean up the reticle detection manager."""
+        logger.debug(f"{self.name} Cleaning the thread")
         if self.worker is not None:
-            self.worker.stop_running()
-        if self.thread is not None:
-            self.thread.quit()
-            self.thread.wait()
+            self.worker.stop_running()  # Signal the worker to stop
+        
+        if not self.threadDeleted and self.thread.isRunning():
+            self.thread.quit()  # Ask the thread to quit
+            self.thread.wait()  # Wait for the thread to finish
+        self.thread = None  # Clear the reference to the thread
+        self.worker = None  # Clear the reference to the worker
+        logger.debug(f"{self.name} Cleaned the thread")
 
     def __del__(self):
         """Destructor for the filter object."""
-        self.clean()
-
-    def thread_deleted(self):
-        """Placeholder method for when the thread is deleted."""
-        pass
+        self.clean()
```

### Comparing `parallax_app-0.37.5/parallax/probe_calibration.py` & `parallax_app-0.37.6/parallax/probe_calibration.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,14 +102,20 @@
             column_names = [
                 "local_x",
                 "local_y",
                 "local_z",
                 "global_x",
                 "global_y",
                 "global_z",
+                "ts_local_coords",
+                "ts_img_captured",
+                "cam0",
+                "pt0",
+                "cam1",
+                "pt1"
             ]
             writer.writerow(column_names)
 
     def clear(self):
         """
         Clears all stored data and resets the transformation matrix to its default state.
         """
@@ -156,30 +162,43 @@
         # Combine weights and bias to form the transformation matrix
         transformation_matrix = np.hstack([weights, bias.reshape(-1, 1)])
         # Adding the extra row to complete the affine transformation matrix
         transformation_matrix = np.vstack([transformation_matrix, [0, 0, 0, 1]])
 
         return model, transformation_matrix
 
-    def _update_local_global_point(self):
+    def _update_local_global_point(self, debug_info=None):
         """
         Updates the CSV file with a new set of local and global points from the current stage position.
         """
-        with open(self.csv_file, "a", newline="") as file:
+        with open(self.csv_file, "a", newline='') as file:
             writer = csv.writer(file)
-            writer.writerow(
-                [
-                    self.stage.stage_x,
-                    self.stage.stage_y,
-                    self.stage.stage_z,
-                    self.stage.stage_x_global,
-                    self.stage.stage_y_global,
-                    self.stage.stage_z_global,
-                ]
-            )
+            row_data = [
+                self.stage.stage_x,
+                self.stage.stage_y,
+                self.stage.stage_z,
+                self.stage.stage_x_global,
+                self.stage.stage_y_global,
+                self.stage.stage_z_global,
+            ]
+
+            # Check if debug information needs to be added
+            if debug_info is not None:
+                # Append debug information as needed
+                row_data.extend([
+                    debug_info.get("ts_local_coords", ''),
+                    debug_info.get("ts_img_captured", ''),
+                    debug_info.get("cam0", ''),
+                    debug_info.get("pt0", ''),
+                    debug_info.get("cam1", ''),
+                    debug_info.get("pt1", '')
+                ])
+
+            # Write the complete row to the CSV
+            writer.writerow(row_data)
 
     def _is_criteria_met_transM(self):
         """
         Checks if the transformation matrix has stabilized within certain thresholds.
 
         Returns:
             bool: True if the criteria are met, otherwise False.
@@ -307,24 +326,24 @@
         z_diff = self.max_z - self.min_z
         self.transM_info.emit(
             self.transM_LR,
             self.LR_err_L2_current,
             np.array([x_diff, y_diff, z_diff]),
         )
 
-    def update(self, stage):
+    def update(self, stage, debug_info=None):
         """
         Main method to update calibration with a new stage position and check if calibration is complete.
 
         Args:
             stage (Stage): The current stage object with new position data.
         """
         # update points in the file
         self.stage = stage
-        self._update_local_global_point()
+        self._update_local_global_point(debug_info)
         # get whole list of local and global points in pd format
         local_points, global_points = self._get_local_global_points()
         self.model_LR, self.transM_LR = self._get_transM_LR(
             local_points, global_points
         )
         self.LR_err_L2_current = self._l2_error_current_point()
         self._update_min_max_x_y_z()  # update min max x,y,z
```

### Comparing `parallax_app-0.37.5/parallax/probe_detect_manager.py` & `parallax_app-0.37.6/parallax/reticle_detect_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,323 +1,324 @@
 """
-ProbeDetectManager coordinates probe detection in images, leveraging PyQt threading 
-and signals for real-time processing. It handles frame updates, detection, 
-and result communication, utilizing components like MaskGenerator and ProbeDetector.
+Manages reticle detection in images through a worker thread, integrating line detection, 
+masking, coordinate analysis, and camera calibration. Uses PyQt's signals 
+for thread-safe operations and real-time processing feedback.
 """
 
 import logging
 import time
 
 import cv2
 import numpy as np
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
-from .curr_bg_cmp_processor import CurrBgCmpProcessor
-from .curr_prev_cmp_processor import CurrPrevCmpProcessor
+from .calibration_camera import CalibrationCamera
 from .mask_generator import MaskGenerator
-from .probe_detector import ProbeDetector
 from .reticle_detection import ReticleDetection
+from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
 
 # Set logger name
 logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
 
 
-class ProbeDetectManager(QObject):
-    """Manager class for probe detection."""
+class ReticleDetectManager(QObject):
+    """Reticle detection class"""
 
     name = "None"
     frame_processed = pyqtSignal(object)
-    found_coords = pyqtSignal(str, str, tuple, tuple)
+    found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
 
     class Worker(QObject):
-        """Worker class for probe detection."""
+        """Reticle detection Worker Thread"""
 
         finished = pyqtSignal()
         frame_processed = pyqtSignal(object)
-        found_coords = pyqtSignal(str, str, tuple)
+        found_coords = pyqtSignal(
+            np.ndarray, np.ndarray, np.ndarray, np.ndarray
+        )
 
-        def __init__(self, name, model):
-            """Initialize Worker object"""
+        def __init__(self, name):
+            """Initialize the worker"""
             QObject.__init__(self)
-            self.model = model
             self.name = name
             self.running = False
             self.is_detection_on = False
             self.new = False
             self.frame = None
-            self.reticle_coords = self.model.get_coords_axis(self.name)
-
-            # TODO move to model structure
-            self.prev_img = None
-            self.reticle_zone = None
-            self.is_probe_updated = True
-            self.probes = {}
-            self.sn = None
-
-            self.IMG_SIZE = (1000, 750)
             self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
-            self.CROP_INIT = 50
-            self.mask_detect = MaskGenerator()
+            self.frame_success = None
 
-        def update_sn(self, sn):
-            """Update the serial number and initialize probe detectors.
+            self.mask_detect = MaskGenerator(initial_detect = True)
+            self.reticleDetector = ReticleDetection(
+                self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name
+            )
+            self.coordsInterests = ReticleDetectCoordsInterest()
+            self.calibrationCamera = CalibrationCamera(self.name)
 
-            Args:
-                sn (str): Serial number.
-            """
-            if sn not in self.probes.keys():
-                self.sn = sn
-                self.probeDetect = ProbeDetector(self.sn, self.IMG_SIZE)
-                self.currPrevCmpProcess = CurrPrevCmpProcessor(
-                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
-                )
-                self.currBgCmpProcess = CurrBgCmpProcessor(
-                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
-                )
-                self.probes[self.sn] = {
-                    "probeDetector": self.probeDetect,
-                    "currPrevCmpProcess": self.currPrevCmpProcess,
-                    "currBgCmpProcess": self.currBgCmpProcess,
-                }
-            else:
-                if sn != self.sn:
-                    self.sn = sn
-                    self.probeDetect = self.probes[self.sn]["probeDetector"]
-                    self.currPrevCmpProcess = self.probes[self.sn][
-                        "currPrevCmpProcess"
-                    ]
-                    self.currBgCmpProcess = self.probes[self.sn][
-                        "currBgCmpProcess"
-                    ]
-                else:
-                    pass
+        def update_frame(self, frame):
+            """Update the frame to be processed."""
+            self.frame = frame
+            # Deal with one frame at a time. This may cause the frame drop
+            if self.new is False:
+                self.new = True
 
-        def update_frame(self, frame, timestamp):
-            """Update the frame and timestamp.
+        def draw(self, frame, x_axis_coords, y_axis_coords):
+            """Draw the coordinates on the frame.
 
             Args:
                 frame (numpy.ndarray): Input frame.
-                timestamp (str): Timestamp of the frame.
+                x_axis_coords (numpy.ndarray): X-axis coordinates.
+                y_axis_coords (numpy.ndarray): Y-axis coordinates.
+
+            Returns:
+                numpy.ndarray: Frame with coordinates drawn.
             """
-            self.frame = frame
-            self.new = True
-            self.timestamp = timestamp
+            if x_axis_coords is None or y_axis_coords is None:
+                return frame
+            for pixel in x_axis_coords:
+                pt = tuple(pixel)
+                cv2.circle(frame, pt, 7, (255, 255, 0), -1)
+            for pixel in y_axis_coords:
+                pt = tuple(pixel)
+                cv2.circle(frame, pt, 7, (0, 255, 255), -1)
+            return frame
 
-        def process(self, frame, timestamp):
-            """Process the frame for probe detection.
-            1. First run currPrevCmpProcess
-            2. If it fails on 1, run currBgCmpProcess
+        def draw_xyz(self, frame, origin, x, y, z):
+            """Draw the XYZ axes on the frame."""
+            frame = cv2.line(frame, origin, x, (0, 0, 255), 3)  # Blue line
+            frame = cv2.line(frame, origin, y, (0, 255, 0), 3)  # Green line
+            frame = cv2.line(frame, origin, z, (255, 0, 0), 3)  # Red line
+            return frame
 
-            Args:
-                frame (numpy.ndarray): Input frame.
-                timestamp (str): Timestamp of the frame.
+        def draw_calibration_info(self, frame, ret, mtx, dist):
+            """
+            Draw calibration information on the frame.
 
-            Returns:
-                tuple: Processed frame and timestamp.
+            Parameters:
+            - frame: The image frame on which to draw.
+            - ret: Boolean indicating if calibration was successful.
+            - mtx: The camera matrix obtained from calibration.
+            - dist: The distortion coefficients obtained from calibration.
             """
-            if frame.ndim > 2:
-                gray_img = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-            else:
-                gray_img = frame
 
-            resized_img = cv2.resize(gray_img, self.IMG_SIZE)
-            self.curr_img = cv2.GaussianBlur(resized_img, (9, 9), 0)
-            mask = self.mask_detect.process(resized_img)  # Generate Mask
-
-            if self.mask_detect.is_reticle_exist and self.reticle_zone is None:
-                reticle = ReticleDetection(
-                    self.IMG_SIZE, self.mask_detect, self.name
+            # Starting position for the text
+            offset_start = 50
+            line_height = 60
+
+            # Basic settings for the text
+            font = cv2.FONT_HERSHEY_SIMPLEX
+            font_scale = 1.5
+            font_color = (255, 255, 255)  # White color
+            line_type = 2
+
+            # Status text
+            status_text = f"Overall RMS re-projection error: {ret}"
+            cv2.putText(
+                frame,
+                status_text,
+                (10, offset_start),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
+            # Camera matrix text
+            mtx_lines = [
+                f"Camera Matrix:",
+                f"[{mtx[0][0]:.2f}, {mtx[0][1]:.2f}, {mtx[0][2]:.2f}]",
+                f"[{mtx[1][0]:.2f}, {mtx[1][1]:.2f}, {mtx[1][2]:.2f}]",
+                f"[{mtx[2][0]:.2f}, {mtx[2][1]:.2f}, {mtx[2][2]:.2f}]"
+            ]
+            # Draw each line of the camera matrix
+            for i, line in enumerate(mtx_lines):
+                cv2.putText(
+                    frame,
+                    line,
+                    (10, offset_start + line_height + i * line_height),
+                    font,
+                    font_scale,
+                    font_color,
+                    line_type,
                 )
-                self.reticle_zone = reticle.get_reticle_zone(
-                    frame
-                )  # Generate X and Y Coordinates zone
-                self.currBgCmpProcess.update_reticle_zone(self.reticle_zone)
-
-            if self.prev_img is not None:
-                if (
-                    self.probeDetect.angle is None
-                ):  # Detecting probe for the first time
-                    ret = self.currPrevCmpProcess.first_cmp(
-                        self.curr_img, self.prev_img, mask, gray_img
-                    )
-                    if ret is False:
-                        ret = self.currBgCmpProcess.first_cmp(
-                            self.curr_img, mask, gray_img
-                        )
-                    if ret:
-                        logger.debug("First detect")
-                        logger.debug(
-                            f"angle: {self.probeDetect.angle}, \
-                            tip: {self.probeDetect.probe_tip}, \
-                            base: {self.probeDetect.probe_base}"
-                        )
-                else:  # Tracking for the known probe
-                    ret = self.currPrevCmpProcess.update_cmp(
-                        self.curr_img, self.prev_img, mask, gray_img
-                    )
-                    if ret is False:
-                        ret = self.currBgCmpProcess.update_cmp(
-                            self.curr_img, mask, gray_img
-                        )
-
-                    if ret:  # Found
-                        self.found_coords.emit(
-                            timestamp, self.sn, self.probeDetect.probe_tip_org
-                        )
-                        cv2.circle(
-                            frame,
-                            self.probeDetect.probe_tip_org,
-                            5,
-                            (255, 255, 0),
-                            -1,
-                        )
 
-                if ret:
-                    self.prev_img = self.curr_img
+            # Distortion coefficients text
+            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, \
+                {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
+            cv2.putText(
+                frame,
+                dist_text,
+                (10, offset_start + line_height * 5),
+                font,
+                font_scale,
+                font_color,
+                line_type,
+            )
+
+            return frame
+
+        def process(self, frame):
+            """Process the frame for reticle detection."""
+            # cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
+            ret, frame_, _, inliner_lines_pixels = (
+                self.reticleDetector.get_coords(frame)
+            )
+            if not ret:
+                logger.debug(f"{ self.name} get_coords fails ")
             else:
-                self.prev_img = self.curr_img
+                ret, x_axis_coords, y_axis_coords = (
+                    self.coordsInterests.get_coords_interest(
+                        inliner_lines_pixels
+                    )
+                )
 
-            return frame, timestamp
+            if not ret:
+                logger.debug(f"{ self.name} get_coords_interest fails ")
+            else:
+                # TODO
+                # ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
+                # if not ret:
+                ret, mtx, dist = self.calibrationCamera.calibrate_camera(
+                    x_axis_coords, y_axis_coords
+                )
+                if not ret:
+                    logger.debug(f"{ self.name} calibrate_camera fails ")
+                else:
+                    # Draw
+                    self.found_coords.emit(
+                        x_axis_coords, y_axis_coords, mtx, dist
+                    )
+                    origin, x, y, z = self.calibrationCamera.get_origin_xyz()
+                    frame = self.draw_xyz(frame, origin, x, y, z)
+                    frame = self.draw(frame, x_axis_coords, y_axis_coords)
+                    frame = self.draw_calibration_info(frame, ret, mtx, dist)
+                self.frame_success = frame
+            
+            if self.frame_success is None:
+                logger.debug(f"{ self.name} reticle detection fail ")
+                return frame
+            else:
+                logger.debug(f"{ self.name} reticle detection success \n")
+                self.stop_running() # If found, stop processing
+                return self.frame_success
 
         def stop_running(self):
             """Stop the worker from running."""
             self.running = False
 
         def start_running(self):
             """Start the worker running."""
             self.running = True
 
         def start_detection(self):
-            """Start the probe detection."""
+            """Start the reticle detection."""
             self.is_detection_on = True
 
         def stop_detection(self):
-            """Stop the probe detection."""
+            """Stop the reticle detection."""
             self.is_detection_on = False
 
-        def process_draw_reticle(self, frame):
-            if self.reticle_coords is not None:
-                for idx, coords in enumerate(self.reticle_coords):
-                    # Normalize indices to 0-255 for colormap application.
-                    indices = np.linspace(
-                        0, 255, len(coords), endpoint=True, dtype=np.uint8
-                    )
-                    # Apply 'jet' colormap to x-coords, 'winter' to the y-coords.
-                    colormap = cv2.applyColorMap(
-                        indices,
-                        cv2.COLORMAP_JET if idx == 0 else cv2.COLORMAP_WINTER,
-                    )
-
-                    for point_idx, (x, y) in enumerate(coords):
-                        color = colormap[point_idx][0].tolist()
-                        cv2.circle(frame, (x, y), 2, color, -1)
-            return frame
-
         def run(self):
             """Run the worker thread."""
-            print("probe_detect_manager running ")
             while self.running:
                 if self.new:
-                    if self.is_detection_on:
-                        self.frame, self.timestamp = self.process(
-                            self.frame, self.timestamp
-                        )
-                    self.frame = self.process_draw_reticle(self.frame)
+                    self.frame = self.process(self.frame)
                     self.frame_processed.emit(self.frame)
-                    self.new = False
+                self.new = False
                 time.sleep(0.001)
-            print("probe_detect_manager running done")
             self.finished.emit()
 
-    def __init__(self, model, camera_name):
-        """Initialize ProbeDetectManager object"""
+        def set_name(self, name):
+            """Set name as camera serial number."""
+            self.name = name
+
+    def __init__(self, camera_name):
+        """Initialize the reticle detection manager."""
+        logger.debug(f"{self.name} Init reticle detect manager")
         super().__init__()
-        self.model = model
         self.worker = None
         self.name = camera_name
         self.thread = None
-        self.init_thread()
 
     def init_thread(self):
         """Initialize the worker thread."""
+        if self.thread is not None:
+            self.clean()  # Clean up existing thread and worker before reinitializing
         self.thread = QThread()
-        self.worker = self.Worker(self.name, self.model)
+        self.worker = self.Worker(self.name)
         self.worker.moveToThread(self.thread)
+
         self.thread.started.connect(self.worker.run)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.thread.destroyed.connect(self.onThreadDestroyed) # Debug msg
+        self.threadDeleted = False
+
         self.worker.frame_processed.connect(self.frame_processed)
-        self.worker.found_coords.connect(self.found_coords_print)
+        self.worker.found_coords.connect(self.found_coords)
         self.worker.finished.connect(self.thread.quit)
         self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
+        self.worker.destroyed.connect(self.onWorkerDestroyed)
+        logger.debug(f"{self.name} init camera")
 
-    def process(self, frame, timestamp):
+    def process(self, frame):
         """Process the frame using the worker.
 
         Args:
             frame (numpy.ndarray): Input frame.
-            timestamp (str): Timestamp of the frame.
         """
         if self.worker is not None:
-            self.worker.update_frame(frame, timestamp)
-
-    def found_coords_print(self, timestamp, sn, pixel_coords):
-        """Emit the found coordinates signal.
-
-        Args:
-            timestamp (str): Timestamp of the frame.
-            sn (str): Serial number.
-            pixel_coords (tuple): Pixel coordinates of the probe tip.
-        """
-        moving_stage = self.model.get_stage(sn)
-        if moving_stage is not None:
-            stage_info = (
-                moving_stage.stage_x,
-                moving_stage.stage_y,
-                moving_stage.stage_z,
-            )
-        # print(timestamp, sn, stage_info, pixel_coords)
-        self.found_coords.emit(timestamp, sn, stage_info, pixel_coords)
+            self.worker.update_frame(frame)
 
     def start(self):
-        """Start the probe detection manager."""
+        """Start the reticle detection manager."""
+        logger.debug(f"{self.name} Starting thread in {self.__class__.__name__}")
         self.init_thread()  # Reinitialize and start the worker and thread
         self.worker.start_running()
         self.thread.start()
 
     def stop(self):
-        """Stop the probe detection manager."""
+        """Stop the reticle detection manager."""
         if self.worker is not None:
             self.worker.stop_running()
+        
+    def onWorkerDestroyed(self):
+        """Cleanup after worker finishes."""
+        logger.debug(f"{self.name} worker finished")
+
+    def onThreadDestroyed(self):
+        """Flag if thread is deleted"""
+        logger.debug(f"{self.name} thread destroyed")
+        self.threadDeleted = True
+        self.thread = None
 
-    def start_detection(self, sn):  # Call from stage listener.
-        """Start the probe detection for a specific serial number.
-
-        Args:
-            sn (str): Serial number.
-        """
-        if self.worker is not None:
-            self.worker.update_sn(sn)
-            self.worker.start_detection()
-
-    def stop_detection(self, sn):  # Call from stage listener.
-        """Stop the probe detection for a specific serial number.
-
-        Args:
-            sn (str): Serial number.
-        """
+    def set_name(self, camera_name):
+        """Set camera name."""
+        self.name = camera_name
         if self.worker is not None:
-            self.worker.stop_detection()
+            self.worker.set_name(self.name)
+        logger.debug(f"{self.name} set camera name")
 
     def clean(self):
-        """Clean up the probe detection manager."""
+        """Safely clean up the reticle detection manager."""
+        logger.debug(f"{self.name} Cleaning the thread")
         if self.worker is not None:
-            self.worker.stop_running()
-        if self.thread is not None:
-            self.thread.quit()
-            self.thread.wait()
+            self.worker.stop_running()  # Signal the worker to stop
+        
+        if not self.threadDeleted and self.thread.isRunning():
+            logger.debug(f"{self.name} Stopping thread in {self.__class__.__name__}")
+            self.thread.quit()  # Ask the thread to quit
+            self.thread.wait()  # Wait for the thread to finish
+        self.thread = None  # Clear the reference to the thread
+        self.worker = None  # Clear the reference to the worker
+        logger.debug(f"{self.name} Cleaned the thread")
+
+    def onThreadDestroyed(self):
+        """Flag if thread is deleted"""
+        self.threadDeleted = True
 
     def __del__(self):
-        """Destructor for the probe detection manager."""
+        """Destructor for the reticle detection manager."""
         self.clean()
```

### Comparing `parallax_app-0.37.5/parallax/probe_detector.py` & `parallax_app-0.37.6/parallax/probe_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.6/parallax/probe_fine_tip_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/recording_manager.py` & `parallax_app-0.37.6/parallax/recording_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/reticle_detect_manager.py` & `parallax_app-0.37.6/parallax/probe_detect_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,310 +1,359 @@
 """
-Manages reticle detection in images through a worker thread, integrating line detection, 
-masking, coordinate analysis, and camera calibration. Uses PyQt's signals 
-for thread-safe operations and real-time processing feedback.
+ProbeDetectManager coordinates probe detection in images, leveraging PyQt threading 
+and signals for real-time processing. It handles frame updates, detection, 
+and result communication, utilizing components like MaskGenerator and ProbeDetector.
 """
 
 import logging
 import time
 
 import cv2
 import numpy as np
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
-from .calibration_camera import CalibrationCamera
+from .curr_bg_cmp_processor import CurrBgCmpProcessor
+from .curr_prev_cmp_processor import CurrPrevCmpProcessor
 from .mask_generator import MaskGenerator
+from .probe_detector import ProbeDetector
 from .reticle_detection import ReticleDetection
-from .reticle_detection_coords_interests import ReticleDetectCoordsInterest
 
 # Set logger name
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
-logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.DEBUG)
-logging.getLogger("PyQt5.uic.properties").setLevel(logging.DEBUG)
+logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
+logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
 
-class ReticleDetectManager(QObject):
-    """Reticle detection class"""
+class ProbeDetectManager(QObject):
+    """Manager class for probe detection."""
 
     name = "None"
     frame_processed = pyqtSignal(object)
-    found_coords = pyqtSignal(np.ndarray, np.ndarray, np.ndarray, np.ndarray)
+    found_coords = pyqtSignal(str, str, tuple, tuple)
 
     class Worker(QObject):
-        """Reticle detection Worker Thread"""
+        """Worker class for probe detection."""
 
         finished = pyqtSignal()
         frame_processed = pyqtSignal(object)
-        found_coords = pyqtSignal(
-            np.ndarray, np.ndarray, np.ndarray, np.ndarray
-        )
+        found_coords = pyqtSignal(str, str, tuple)
 
-        def __init__(self, name):
-            """Initialize the worker"""
+        def __init__(self, name, model):
+            """Initialize Worker object"""
             QObject.__init__(self)
+            self.model = model
             self.name = name
             self.running = False
             self.is_detection_on = False
             self.new = False
             self.frame = None
-            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
-            self.frame_success = None
+            self.reticle_coords = self.model.get_coords_axis(self.name)
 
-            self.mask_detect = MaskGenerator(initial_detect = True)
-            self.reticleDetector = ReticleDetection(
-                self.IMG_SIZE_ORIGINAL, self.mask_detect, self.name
-            )
-            self.coordsInterests = ReticleDetectCoordsInterest()
-            self.calibrationCamera = CalibrationCamera(self.name)
+            # TODO move to model structure
+            self.prev_img = None
+            self.reticle_zone = None
+            self.is_probe_updated = True
+            self.probes = {}
+            self.sn = None
 
-        def update_frame(self, frame):
-            """Update the frame to be processed."""
-            self.frame = frame
-            # Deal with one frame at a time. This may cause the frame drop
-            if self.new is False:
-                self.new = True
+            self.IMG_SIZE = (1000, 750)
+            self.IMG_SIZE_ORIGINAL = (4000, 3000)  # TODO
+            self.CROP_INIT = 50
+            self.mask_detect = MaskGenerator()
 
-        def draw(self, frame, x_axis_coords, y_axis_coords):
-            """Draw the coordinates on the frame.
+        def update_sn(self, sn):
+            """Update the serial number and initialize probe detectors.
 
             Args:
-                frame (numpy.ndarray): Input frame.
-                x_axis_coords (numpy.ndarray): X-axis coordinates.
-                y_axis_coords (numpy.ndarray): Y-axis coordinates.
-
-            Returns:
-                numpy.ndarray: Frame with coordinates drawn.
+                sn (str): Serial number.
             """
-            if x_axis_coords is None or y_axis_coords is None:
-                return frame
-            for pixel in x_axis_coords:
-                pt = tuple(pixel)
-                cv2.circle(frame, pt, 7, (255, 255, 0), -1)
-            for pixel in y_axis_coords:
-                pt = tuple(pixel)
-                cv2.circle(frame, pt, 7, (0, 255, 255), -1)
-            return frame
-
-        def draw_xyz(self, frame, origin, x, y, z):
-            """Draw the XYZ axes on the frame."""
-            frame = cv2.line(frame, origin, x, (0, 0, 255), 3)  # Blue line
-            frame = cv2.line(frame, origin, y, (0, 255, 0), 3)  # Green line
-            frame = cv2.line(frame, origin, z, (255, 0, 0), 3)  # Red line
-            return frame
+            if sn not in self.probes.keys():
+                self.sn = sn
+                self.probeDetect = ProbeDetector(self.sn, self.IMG_SIZE)
+                self.currPrevCmpProcess = CurrPrevCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.currBgCmpProcess = CurrBgCmpProcessor(
+                    self.probeDetect, self.IMG_SIZE_ORIGINAL, self.IMG_SIZE
+                )
+                self.probes[self.sn] = {
+                    "probeDetector": self.probeDetect,
+                    "currPrevCmpProcess": self.currPrevCmpProcess,
+                    "currBgCmpProcess": self.currBgCmpProcess,
+                }
+            else:
+                if sn != self.sn:
+                    self.sn = sn
+                    self.probeDetect = self.probes[self.sn]["probeDetector"]
+                    self.currPrevCmpProcess = self.probes[self.sn][
+                        "currPrevCmpProcess"
+                    ]
+                    self.currBgCmpProcess = self.probes[self.sn][
+                        "currBgCmpProcess"
+                    ]
+                else:
+                    pass
 
-        def draw_calibration_info(self, frame, ret, mtx, dist):
-            """
-            Draw calibration information on the frame.
+        def update_frame(self, frame, timestamp):
+            """Update the frame and timestamp.
 
-            Parameters:
-            - frame: The image frame on which to draw.
-            - ret: Boolean indicating if calibration was successful.
-            - mtx: The camera matrix obtained from calibration.
-            - dist: The distortion coefficients obtained from calibration.
+            Args:
+                frame (numpy.ndarray): Input frame.
+                timestamp (str): Timestamp of the frame.
             """
+            self.frame = frame
+            self.new = True
+            self.timestamp = timestamp
 
-            # Starting position for the text
-            offset_start = 50
-            line_height = 60
-
-            # Basic settings for the text
-            font = cv2.FONT_HERSHEY_SIMPLEX
-            font_scale = 1.5
-            font_color = (255, 255, 255)  # White color
-            line_type = 2
-
-            # Status text
-            status_text = f"Overall RMS re-projection error: {ret}"
-            cv2.putText(
-                frame,
-                status_text,
-                (10, offset_start),
-                font,
-                font_scale,
-                font_color,
-                line_type,
-            )
-
-            # Camera matrix text
-            mtx_lines = [
-                f"Camera Matrix:",
-                f"[{mtx[0][0]:.2f}, {mtx[0][1]:.2f}, {mtx[0][2]:.2f}]",
-                f"[{mtx[1][0]:.2f}, {mtx[1][1]:.2f}, {mtx[1][2]:.2f}]",
-                f"[{mtx[2][0]:.2f}, {mtx[2][1]:.2f}, {mtx[2][2]:.2f}]"
-            ]
-            # Draw each line of the camera matrix
-            for i, line in enumerate(mtx_lines):
-                cv2.putText(
-                    frame,
-                    line,
-                    (10, offset_start + line_height + i * line_height),
-                    font,
-                    font_scale,
-                    font_color,
-                    line_type,
-                )
-
-            # Distortion coefficients text
-            dist_text = f"Dist Coeffs: [{dist[0][0]:.4f}, {dist[0][1]:.4f}, \
-                {dist[0][2]:.4f}, {dist[0][3]:.4f} {dist[0][4]:.4f}]"
-            cv2.putText(
-                frame,
-                dist_text,
-                (10, offset_start + line_height * 5),
-                font,
-                font_scale,
-                font_color,
-                line_type,
-            )
+        def process(self, frame, timestamp):
+            """Process the frame for probe detection.
+            1. First run currPrevCmpProcess
+            2. If it fails on 1, run currBgCmpProcess
 
-            return frame
+            Args:
+                frame (numpy.ndarray): Input frame.
+                timestamp (str): Timestamp of the frame.
 
-        def process(self, frame):
-            """Process the frame for reticle detection."""
-            # cv2.circle(frame, (2000,1500), 10, (255, 0, 0), -1)
-            ret, frame_, _, inliner_lines_pixels = (
-                self.reticleDetector.get_coords(frame)
-            )
-            if not ret:
-                logger.debug(f"{ self.name} get_coords fails ")
+            Returns:
+                tuple: Processed frame and timestamp.
+            """
+            if frame.ndim > 2:
+                gray_img = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
             else:
-                ret, x_axis_coords, y_axis_coords = (
-                    self.coordsInterests.get_coords_interest(
-                        inliner_lines_pixels
-                    )
-                )
+                gray_img = frame
 
-            if not ret:
-                logger.debug(f"{ self.name} get_coords_interest fails ")
-            else:
-                # TODO
-                # ret, mtx, dist = self.calibrationCamera.get_predefined_intrinsic(x_axis_coords, y_axis_coords)
-                # if not ret:
-                ret, mtx, dist = self.calibrationCamera.calibrate_camera(
-                    x_axis_coords, y_axis_coords
+            resized_img = cv2.resize(gray_img, self.IMG_SIZE)
+            self.curr_img = cv2.GaussianBlur(resized_img, (9, 9), 0)
+            mask = self.mask_detect.process(resized_img)  # Generate Mask
+
+            if self.mask_detect.is_reticle_exist and self.reticle_zone is None:
+                reticle = ReticleDetection(
+                    self.IMG_SIZE, self.mask_detect, self.name
                 )
-                if not ret:
-                    logger.debug(f"{ self.name} calibrate_camera fails ")
-                else:
-                    # Draw
-                    self.found_coords.emit(
-                        x_axis_coords, y_axis_coords, mtx, dist
+                self.reticle_zone = reticle.get_reticle_zone(
+                    frame
+                )  # Generate X and Y Coordinates zone
+                self.currBgCmpProcess.update_reticle_zone(self.reticle_zone)
+
+            if self.prev_img is not None:
+                if (
+                    self.probeDetect.angle is None
+                ):  # Detecting probe for the first time
+                    ret = self.currPrevCmpProcess.first_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
                     )
-                    origin, x, y, z = self.calibrationCamera.get_origin_xyz()
-                    frame = self.draw_xyz(frame, origin, x, y, z)
-                    frame = self.draw(frame, x_axis_coords, y_axis_coords)
-                    frame = self.draw_calibration_info(frame, ret, mtx, dist)
-                self.frame_success = frame
-            
-            if self.frame_success is None:
-                logger.debug(f"{ self.name} reticle detection fail ")
-                return frame
+                    if ret is False:
+                        ret = self.currBgCmpProcess.first_cmp(
+                            self.curr_img, mask, gray_img
+                        )
+                    if ret:
+                        logger.debug("First detect")
+                        logger.debug(
+                            f"angle: {self.probeDetect.angle}, \
+                            tip: {self.probeDetect.probe_tip}, \
+                            base: {self.probeDetect.probe_base}"
+                        )
+                else:  # Tracking for the known probe
+                    ret = self.currPrevCmpProcess.update_cmp(
+                        self.curr_img, self.prev_img, mask, gray_img
+                    )
+                    if ret is False:
+                        ret = self.currBgCmpProcess.update_cmp(
+                            self.curr_img, mask, gray_img
+                        )
+
+                    if ret:  # Found
+                        self.found_coords.emit(
+                            timestamp, self.sn, self.probeDetect.probe_tip_org
+                        )
+                        cv2.circle(
+                            frame,
+                            self.probeDetect.probe_tip_org,
+                            5,
+                            (255, 255, 0),
+                            -1,
+                        )
+
+                if ret:
+                    self.prev_img = self.curr_img
             else:
-                logger.debug(f"{ self.name} reticle detection success \n")
-                return self.frame_success
+                self.prev_img = self.curr_img
+
+            return frame, timestamp
 
         def stop_running(self):
             """Stop the worker from running."""
             self.running = False
 
         def start_running(self):
             """Start the worker running."""
             self.running = True
 
         def start_detection(self):
-            """Start the reticle detection."""
+            """Start the probe detection."""
             self.is_detection_on = True
 
         def stop_detection(self):
-            """Stop the reticle detection."""
+            """Stop the probe detection."""
             self.is_detection_on = False
 
+        def process_draw_reticle(self, frame):
+            if self.reticle_coords is not None:
+                for idx, coords in enumerate(self.reticle_coords):
+                    # Normalize indices to 0-255 for colormap application.
+                    indices = np.linspace(
+                        0, 255, len(coords), endpoint=True, dtype=np.uint8
+                    )
+                    # Apply 'jet' colormap to x-coords, 'winter' to the y-coords.
+                    colormap = cv2.applyColorMap(
+                        indices,
+                        cv2.COLORMAP_JET if idx == 0 else cv2.COLORMAP_WINTER,
+                    )
+
+                    for point_idx, (x, y) in enumerate(coords):
+                        color = colormap[point_idx][0].tolist()
+                        cv2.circle(frame, (x, y), 2, color, -1)
+            return frame
+
         def run(self):
             """Run the worker thread."""
+            print("probe_detect_manager running ")
             while self.running:
                 if self.new:
-                    self.frame = self.process(self.frame)
+                    if self.is_detection_on:
+                        self.frame, self.timestamp = self.process(
+                            self.frame, self.timestamp
+                        )
+                    self.frame = self.process_draw_reticle(self.frame)
                     self.frame_processed.emit(self.frame)
-                self.new = False
+                    self.new = False
                 time.sleep(0.001)
+            print("probe_detect_manager running done")
             self.finished.emit()
-            logger.debug(f"thread finished {self.name}")
 
         def set_name(self, name):
             """Set name as camera serial number."""
             self.name = name
+            self.reticle_coords = self.model.get_coords_axis(self.name)
 
-    def __init__(self, camera_name):
-        """Initialize the reticle detection manager."""
-        logger.debug("Init reticle detect manager")
+    def __init__(self, model, camera_name):
+        """Initialize ProbeDetectManager object"""
         super().__init__()
+        self.model = model
         self.worker = None
         self.name = camera_name
         self.thread = None
 
     def init_thread(self):
         """Initialize the worker thread."""
         if self.thread is not None:
-            self.clean()  # Clean up existing thread and worker before reinitializing
+            self.clean()  # Clean up existing thread and worker before reinitializing 
         self.thread = QThread()
-        self.worker = self.Worker(self.name)
+        self.worker = self.Worker(self.name, self.model)
         self.worker.moveToThread(self.thread)
-
+        
         self.thread.started.connect(self.worker.run)
         self.thread.finished.connect(self.thread.deleteLater)
         self.thread.destroyed.connect(self.onThreadDestroyed)
         self.threadDeleted = False
 
         self.worker.frame_processed.connect(self.frame_processed)
-        self.worker.found_coords.connect(self.found_coords)
+        self.worker.found_coords.connect(self.found_coords_print)
         self.worker.finished.connect(self.thread.quit)
         self.worker.finished.connect(self.worker.deleteLater)
-        logger.debug(f"init camera name: {self.name}")
+        self.worker.destroyed.connect(self.onWorkerDestroyed)
+        logger.debug(f"{self.name} init camera name")
 
-    def process(self, frame):
+    def process(self, frame, timestamp):
         """Process the frame using the worker.
 
         Args:
             frame (numpy.ndarray): Input frame.
+            timestamp (str): Timestamp of the frame.
         """
         if self.worker is not None:
-            self.worker.update_frame(frame)
+            self.worker.update_frame(frame, timestamp)
+
+    def found_coords_print(self, timestamp, sn, pixel_coords):
+        """Emit the found coordinates signal.
+
+        Args:
+            timestamp (str): Timestamp of the frame.
+            sn (str): Serial number.
+            pixel_coords (tuple): Pixel coordinates of the probe tip.
+        """
+        moving_stage = self.model.get_stage(sn)
+        if moving_stage is not None:
+            stage_info = (
+                moving_stage.stage_x,
+                moving_stage.stage_y,
+                moving_stage.stage_z,
+            )
+        # print(timestamp, sn, stage_info, pixel_coords)
+        self.found_coords.emit(timestamp, sn, stage_info, pixel_coords)
 
     def start(self):
-        """Start the reticle detection manager."""
+        """Start the probe detection manager."""
+        logger.debug(f" {self.name} Starting thread")
         self.init_thread()  # Reinitialize and start the worker and thread
         self.worker.start_running()
         self.thread.start()
-        logger.debug(f"thread started {self.name}")
 
     def stop(self):
-        """Stop the reticle detection manager."""
+        """Stop the probe detection manager."""
+        logger.debug(f" {self.name} Stopping thread")
         if self.worker is not None:
             self.worker.stop_running()
 
+    def onWorkerDestroyed(self):
+        """Cleanup after worker finishes."""
+        logger.debug(f"{self.name} worker destroyed")
+
+    def onThreadDestroyed(self):
+        """Flag if thread is deleted"""
+        logger.debug(f"{self.name} thread destroyed")
+        self.threadDeleted = True
+        self.thread = None
+
+    def start_detection(self, sn):  # Call from stage listener.
+        """Start the probe detection for a specific serial number.
+
+        Args:
+            sn (str): Serial number.
+        """
+        if self.worker is not None:
+            self.worker.update_sn(sn)
+            self.worker.start_detection()
+
+    def stop_detection(self, sn):  # Call from stage listener.
+        """Stop the probe detection for a specific serial number.
+
+        Args:
+            sn (str): Serial number.
+        """
+        if self.worker is not None:
+            self.worker.stop_detection()
+
     def set_name(self, camera_name):
         """Set camera name."""
         self.name = camera_name
         if self.worker is not None:
             self.worker.set_name(self.name)
-        logger.debug(f"camera name: {self.name}")
+        logger.debug(f"{self.name} set camera name")
 
     def clean(self):
-        """Safely clean up the reticle detection manager."""
-        logger.debug("Cleaning the thread")
+        """Clean up the probe detection manager."""
+        logger.debug(f"{self.name} Cleaning the thread")
         if self.worker is not None:
-            self.worker.stop_running()  # Signal the worker to stop
+            self.worker.stop_running()
+
         if not self.threadDeleted and self.thread.isRunning():
             self.thread.quit()  # Ask the thread to quit
             self.thread.wait()  # Wait for the thread to finish
         self.thread = None  # Clear the reference to the thread
         self.worker = None  # Clear the reference to the worker
-
-    def onThreadDestroyed(self):
-        """Flag if thread is deleted"""
-        self.threadDeleted = True
+        logger.debug(f"{self.name} Cleaned the thread")
 
     def __del__(self):
-        """Destructor for the reticle detection manager."""
+        """Destructor for the probe detection manager."""
         self.clean()
```

### Comparing `parallax_app-0.37.5/parallax/reticle_detection.py` & `parallax_app-0.37.6/parallax/reticle_detection.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.6/parallax/reticle_detection_coords_interests.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/screen_widget.py` & `parallax_app-0.37.6/parallax/screen_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pyqtgraph as pg
 from PyQt5 import QtCore
 from PyQt5.QtCore import Qt, pyqtSignal
 
 from .no_filter import NoFilter
 from .probe_detect_manager import ProbeDetectManager
 from .reticle_detect_manager import ReticleDetectManager
+from .axis_filter import AxisFilter
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
@@ -70,17 +71,21 @@
 
         # camera
         self.camera = camera
         camera_name = self.get_camera_name()
         self.focochan = None
 
         # No filter
-        self.filter = NoFilter()
+        self.filter = NoFilter(camera_name)
         self.filter.frame_processed.connect(self.set_image_item_from_data)
 
+        # Axis Filter
+        self.axisFilter = AxisFilter(self.model, camera_name)
+        self.axisFilter.frame_processed.connect(self.set_image_item_from_data)
+
         # Reticle Detection
         self.reticleDetector = ReticleDetectManager(camera_name)
         self.reticleDetector.frame_processed.connect(
             self.set_image_item_from_data
         )
         self.reticleDetector.found_coords.connect(self.found_reticle_coords)
         self.reticleDetector.found_coords.connect(self.reticle_coords_detected)
@@ -142,14 +147,15 @@
             self.camera.end_singleframe_acquisition()
 
     def set_data(self, data):
         """
         Set the data displayed in the screen widget.
         """
         self.filter.process(data)
+        self.axisFilter.process(data)
         self.reticleDetector.process(data)
         captured_time = self.camera.get_last_capture_time(millisecond=True)
         self.probeDetector.process(data, captured_time)
 
     def is_camera(self):
         """
         Return True if the camera is 'Blackfly' camera.
@@ -245,20 +251,27 @@
 
         Returns:
             str: The color type of the camera.
         """
         if self.camera:
             return self.camera.device_color_type
 
+    def send_clicked_position(self, pos):
+        self.axisFilter.clicked_position(pos)
+
     def image_clicked(self, event):
         """
         Handle the image click event.
         """
         if event.button() == QtCore.Qt.MouseButton.LeftButton:
-            self.select(event.pos())
+            x, y = event.pos().x(), event.pos().y()
+            x, y = int(round(x)), int(round(y))
+            self.select((x,y))
+            print(f"Clicked position on {self.get_camera_name()}: ({x}, {y})")
+            self.send_clicked_position((x, y))
         elif event.button() == QtCore.Qt.MouseButton.MiddleButton:
             self.zoom_out()
 
     def select(self, pos):
         """Select a position and emit the selected coordinates."""
         self.click_target.setPos(pos)
         self.click_target.setVisible(True)
@@ -276,44 +289,61 @@
         self.view_box.autoRange()
 
     def set_camera(self, camera):
         """
         Set the camera.
         """
         self.camera = camera
-        self.reticleDetector.set_name(self.get_camera_name())
+        camera_sn = self.get_camera_name()
+        self.reticleDetector.set_name(camera_sn)
+        self.probeDetector.set_name(camera_sn)
+        self.axisFilter.set_name(camera_sn)
+        self.filter.set_name(camera_sn)
 
     def run_reticle_detection(self):
         """Run reticle detection by stopping the filter and starting the reticle detector."""
         logger.debug("run_reticle_detection")
         self.filter.stop()
+        self.axisFilter.stop()
         self.reticleDetector.start()
 
     def run_probe_detection(self):
         """Run probe detection by stopping the filter and starting the probe detector."""
         logger.debug("run_probe_detection")
         self.filter.stop()
+        self.axisFilter.stop()
         self.probeDetector.start()
 
     def run_no_filter(self):
         """Run without any filter by stopping the reticle detector and probe detector."""
         logger.debug("run_no_filter")
         self.reticleDetector.stop()
         self.probeDetector.stop()
+        self.axisFilter.stop()
         self.filter.start()
 
+    def run_axis_filter(self):
+        """Run without any filter by stopping the reticle detector and probe detector."""
+        logger.debug("run_axis_filter")
+        self.filter.stop()
+        self.reticleDetector.stop()
+        logger.debug("reticleDetector stopped")
+        self.axisFilter.start()
+
     def found_reticle_coords(self, x_coords, y_coords, mtx, dist):
         """Store the found reticle coordinates, camera matrix, and distortion coefficients."""
         self.reticle_coords = [x_coords, y_coords]
         self.mtx = mtx
         self.dist = dist
 
     def reset_reticle_coords(self):
         """Reset reticle coordinates."""
         self.reticle_coords = None
+        self.mtx = None
+        self.dist = None
 
     def found_probe_coords(self, timestamp, probe_sn, stage_info, tip_coords):
         """Store the found probe coordinates and related information."""
         self.probe_detect_last_timestamp = timestamp
         self.probe_detect_last_sn = probe_sn
         self.stage_info = stage_info
         self.probe_detect_last_coords = tip_coords
```

### Comparing `parallax_app-0.37.5/parallax/stage_listener.py` & `parallax_app-0.37.6/parallax/stage_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
                 return True
         return False
 
 
 class StageListener(QObject):
     """Class for listening to stage updates."""
 
-    probeCalibRequest = pyqtSignal(QObject)
+    probeCalibRequest = pyqtSignal(QObject, dict)
 
     def __init__(self, model, stage_ui):
         """Initialize Stage Listener object"""
         super().__init__()
         self.model = model
         self.timestamp_local, self.timestamp_img_captured = None, None
         self.worker = Worker(self.model.stage_listener_url)
@@ -381,15 +381,16 @@
             if 0 <= time_diff < smallest_time_diff:
                 smallest_time_diff = time_diff
                 closest_ts = ts
                 closest_coords = local_coords
 
         return closest_ts, closest_coords
 
-    def handleGlobalDataChange(self, sn, global_coords, ts_img_captured):
+    #def handleGlobalDataChange(self, sn, global_coords, ts_img_captured):
+    def handleGlobalDataChange(self, sn, global_coords, ts_img_captured, cam0, pt0, cam1, pt1):
         """Handle changes in global stage data.
 
         Args:
             sn (str): Serial number of the stage.
             coords (list): Global coordinates.
             ts_img_captured (str): Timestamp of the captured image.
         """
@@ -418,15 +419,25 @@
             self.stage_global_data.stage_x = local_coords[0]
             self.stage_global_data.stage_y = local_coords[1]
             self.stage_global_data.stage_z = local_coords[2]
             self.stage_global_data.stage_x_global = global_coords_x
             self.stage_global_data.stage_y_global = global_coords_y
             self.stage_global_data.stage_z_global = global_coords_z
 
-            self.probeCalibRequest.emit(self.stage_global_data)
+            # Debug info
+            debug_info = {}
+            debug_info["ts_local_coords"] = ts_local_coords
+            debug_info["ts_img_captured"] = ts_img_captured
+            debug_info["cam0"] = cam0
+            debug_info["pt0"] = pt0
+            debug_info["cam1"] = cam1
+            debug_info["pt1"] = pt1
+
+            #self.probeCalibRequest.emit(self.stage_global_data)
+            self.probeCalibRequest.emit(self.stage_global_data, debug_info)
 
             # Update into UI
             moving_stage = self.model.stages.get(sn)
             if moving_stage is not None:
                 moving_stage.stage_x_global = global_coords_x
                 moving_stage.stage_y_global = global_coords_y
                 moving_stage.stage_z_global = global_coords_z
```

### Comparing `parallax_app-0.37.5/parallax/stage_ui.py` & `parallax_app-0.37.6/parallax/stage_ui.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/stage_widget.py` & `parallax_app-0.37.6/parallax/stage_widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 to manage calibration data and provides UI functionalities for reticle and probe detection, 
 and camera calibration. The class integrates with PyQt5 for the UI, handling UI loading, 
 initializing components, and linking user actions to calibration processes.
 """
 
 import logging
 import os
+import math
+import time
 
 import numpy as np
 from PyQt5.QtCore import QTimer
 from PyQt5.QtWidgets import (QLabel, QMessageBox, QPushButton, QSizePolicy,
                              QSpacerItem, QWidget)
 from PyQt5.uic import loadUi
 
 from .calibration_camera import CalibrationStereo
 from .probe_calibration import ProbeCalibration
 from .stage_listener import StageListener
 from .stage_ui import StageUI
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.WARNING)
-
+logger.setLevel(logging.DEBUG)
 
 class StageWidget(QWidget):
     """Widget for stage control and calibration."""
 
     def __init__(self, model, ui_dir, screen_widgets):
         """Initializes the StageWidget instance.
 
@@ -81,15 +82,15 @@
         self.calib_z = self.probe_calib_widget.findChild(QPushButton, "calib_z")
         self.probeCalibrationLabel = self.probe_calib_widget.findChild(
             QLabel, "probeCalibrationLabel"
         )
 
         # Reticle Widget
         self.reticle_detection_status = (
-            None  # options: default, process, detected, accepted
+            "default"  # options: default, process, detected, accepted, request_axis
         )
         self.reticle_calibration_btn.clicked.connect(
             self.reticle_detection_button_handler
         )
         self.calibrationStereo = None
         # Hide Accept and Reject Button in Reticle Detection
         self.acceptButton.hide()
@@ -99,14 +100,16 @@
         )
         self.rejectButton.clicked.connect(self.reticle_detect_default_status)
         # Add a QTimer for delayed check
         self.reticle_calibration_timer = QTimer(self)
         self.reticle_calibration_timer.timeout.connect(
             self.reticle_detect_default_status
         )
+        self.get_pos_x_from_user_timer = QTimer()
+        self.get_pos_x_from_user_timer.timeout.connect(self.check_positive_x_axis)
 
         # Stage widget
         self.stageUI = StageUI(self.model, self)
         self.probe_calibration_btn.setEnabled(False)
         self.probe_calibration_btn.clicked.connect(
             self.probe_detection_button_handler
         )
@@ -127,26 +130,27 @@
         self.probeCalibration.transM_info.connect(
             self.update_probe_calib_status
         )
         self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
         self.probe_detection_status = None    # options: default, process, x_y_z_detected, accepted
 
         self.filter = "no_filter"
+        logger.debug(f"filter: {self.filter}")
 
     def reticle_detection_button_handler(self):
         """
         Handles clicks on the reticle detection button, initiating or canceling reticle detection.
         """
         logger.debug(f"\n reticle_detection_button_handler {self.reticle_detection_status}")
         if self.reticle_calibration_btn.isChecked():
             # Run reticle detectoin
             self.reticle_detect_process_status()
         else:
             if self.reticle_detection_status == "accepted":
-                response = self.overwrite_popup_window()
+                response = self.reticle_overwrite_popup_window()
                 if response:
                     # Overwrite the result
                     self.reticle_detect_default_status()
                 else:
                     # Keep the last calibration result
                     self.reticle_calibration_btn.setChecked(True)
 
@@ -160,21 +164,23 @@
 
         if self.reticle_detection_status == "process":
             self.reticle_detect_fail_popup_window()
 
         # Stop reticle detectoin, and run no filter
         self.reticle_calibration_timer.stop()
 
-        if self.reticle_detection_status != "accepted":
-            for screen in self.screen_widgets:
-                screen.reticle_coords_detected.disconnect(
-                    self.reticle_detect_all_screen
-                )
+        for screen in self.screen_widgets:
+            if self.filter != "no_filter":
                 screen.run_no_filter()
-            self.filter = "no_filter"
+            if self.reticle_detection_status != "accepted":
+                screen.reticle_coords_detected.disconnect(
+                    self.reticle_detect_two_screens
+                )    
+        self.filter = "no_filter"
+        logger.debug(f"filter: {self.filter}")
 
         # Hide Accept and Reject Button
         self.acceptButton.hide()
         self.rejectButton.hide()
 
         self.reticle_calibration_btn.setStyleSheet(
             """
@@ -188,27 +194,28 @@
         """)
         self.reticle_detection_status = "default"
         self.reticleCalibrationLabel.setText("")
         if self.probe_calibration_btn.isEnabled():
             # Disable probe calibration
             self.probe_detect_default_status()
 
-    def overwrite_popup_window(self):
+    def reticle_overwrite_popup_window(self):
         """
         Displays a confirmation dialog to decide whether to overwrite the current reticle position.
 
         Returns:
             bool: True if the user chooses to overwrite, False otherwise.
         """
         message = (
             f"Are you sure you want to overwrite the current reticle position?"
         )
+        logger.debug(f"Are you sure you want to overwrite the current reticle position?")
         response = QMessageBox.warning(
             self,
-            "Reticle Detection Failed",
+            "Reticle Detection",
             message,
             QMessageBox.Yes | QMessageBox.No,
             QMessageBox.No,
         )
 
         # Check which button was clicked
         if response == QMessageBox.Yes:
@@ -243,21 +250,26 @@
             self.reticle_calibration_btn.setEnabled(False)
 
         # Run reticle detectoin
         self.reticle_calibration_btn.setStyleSheet(
             "color: gray;"
             "background-color: #ffaaaa;"
         )
+
+        # Reset models
+        self.model.reset_coords_intrinsic_extrinsic()
+
         for screen in self.screen_widgets:
             screen.reset_reticle_coords()
             screen.reticle_coords_detected.connect(
-                self.reticle_detect_all_screen
+                self.reticle_detect_two_screens
             )
             screen.run_reticle_detection()
         self.filter = "reticle_detection"
+        logger.debug(f"filter: {self.filter}")
 
         # Hide Accept and Reject Button
         self.acceptButton.hide()
         self.rejectButton.hide()
 
         # Start the timer for 10 seconds to check the status later
         self.reticle_detection_status = "process"
@@ -278,96 +290,187 @@
 
         # Change the button to brown.
         self.reticle_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #bc9e44;"
         )
 
+    def select_positive_x_popup_window(self):
+        message = (
+            f"Click positive x-axis on each screen"
+        )
+        QMessageBox.warning(self, "Calibration", message)
+
+    def get_coords_detected_screens(self):
+        coords_detected_cam_name = []
+        for screen in self.screen_widgets:
+            cam_name = screen.get_camera_name()
+            coords = self.model.get_coords_axis(cam_name) 
+            if coords is not None:
+                coords_detected_cam_name.append(cam_name)
+
+        return coords_detected_cam_name
+    
+    def is_positive_x_axis_detected(self):
+        pos_x_detected_screens = []
+        for cam_name in self.coords_detected_screens:
+            pos_x = self.model.get_pos_x(cam_name)
+            if pos_x is not None:
+                pos_x_detected_screens.append(cam_name)
+        
+        return set(self.coords_detected_screens) == set(pos_x_detected_screens)
+    
+    def check_positive_x_axis(self):
+        if self.is_positive_x_axis_detected():
+            self.get_pos_x_from_user_timer.stop()  # Stop the timer if the positive x-axis has been detected
+            # Continue to calibrate stereo
+            self.start_calibrate_streo()
+            self.enable_reticle_probe_calibration_buttons()
+            logger.debug("Positive x-axis detected on all screens.")
+        else:
+            self.coords_detected_screens = self.get_coords_detected_screens()
+            logger.debug("Checking again for user input of positive x-axis...")
+
+    def continue_if_positive_x_axis_from_user(self):
+        """Get the positive x-axis coordinate of the reticle from the user."""
+        for screen in self.screen_widgets:
+            screen.reticle_coords_detected.disconnect(
+                self.reticle_detect_two_screens
+            )
+            screen.run_axis_filter()
+        
+        self.select_positive_x_popup_window()
+        self.coords_detected_screens = self.get_coords_detected_screens()
+        self.get_pos_x_from_user_timer.start(1000)
+
     def reticle_detect_accept_detected_status(self):
         """
-        Finalizes the reticle detection process, accepting the detected reticle position and updating the UI accordingly.
+        Finalizes the reticle detection process, accepting the detected 
+        reticle position and updating the UI accordingly.
         """
         self.reticle_detection_status = "accepted"
+        logger.debug(f"1 self.filter: {self.filter}")
 
         # Change the button to green.
         self.reticle_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
         # Show Accept and Reject Button
         self.acceptButton.hide()
         self.rejectButton.hide()
 
+        # TODO Get user input of positive x coor distance of the reticle
+        self.continue_if_positive_x_axis_from_user()
+        logger.debug(f"2 self.filter: {self.filter}")
+        
+        """
+        for screen in self.screen_widgets:
+            screen.reticle_coords_detected.disconnect(
+                self.reticle_detect_two_screens
+            )
+            screen.run_no_filter()
+        self.filter = "no_filter"
+        logger.debug(f"filter: {self.filter}")
+        self.start_calibrate_streo()
+        self.enable_reticle_probe_calibration_buttons()
+        """
+
+    def start_calibrate_streo(self):
+        # Perform stereo calibration
         result = self.calibrate_stereo()
         if result:
             self.reticleCalibrationLabel.setText(
                 f"<span style='color:green;'><small>Coords Reproj RMSE:<br></small>"
                 f"<span style='color:green;'>{result*1000:.1f} µm³</span>"
             )
 
-        for screen in self.screen_widgets:
-            screen.reticle_coords_detected.disconnect(
-                self.reticle_detect_all_screen
-            )
-            screen.run_no_filter()
-        self.filter = "no_filter"
-
+    def enable_reticle_probe_calibration_buttons(self):
         # Enable reticle_calibration_btn button
         if not self.reticle_calibration_btn.isEnabled():
             self.reticle_calibration_btn.setEnabled(True)
         logger.debug(self.reticle_detection_status)
 
         # Enable probe calibration
         if not self.probe_calibration_btn.isEnabled():
             self.probe_calibration_btn.setEnabled(True)
 
+    def get_results_calibrate_stereo(self, camA, coordsA, itmxA, camB, coordsB, itmxB):
+        """
+        Returns the results of the stereo calibration process.
+
+        Returns:
+            tuple: A tuple containing the results of the stereo calibration process.
+        """
+        calibrationStereo = CalibrationStereo(camA, coordsA, itmxA, camB, coordsB, itmxB)
+        retval, R_AB, T_AB, E_AB, F_AB = calibrationStereo.calibrate_stereo()
+        err = calibrationStereo.test_performance(camA, coordsA, camB, coordsB) # Test
+        return err, calibrationStereo, retval, R_AB, T_AB, E_AB, F_AB
+        
     def calibrate_stereo(self):
         """
         Performs stereo calibration using the detected reticle positions and updates the model with the calibration data.
         """
+        if len(self.model.coords_axis) < 2 and len(self.model.camera_intrinsic) < 2:
+            return None
+    
         # Streo Camera Calibration
-        if len(self.model.coords_axis) >=2 and len(self.model.camera_intrinsic) >=2:
-            img_coords = []
-            intrinsics = []
-            cam_names = []
+        min_err = math.inf
+        self.calibrationStereo = None
+        self.camA_best, self.camB_best = None, None
+        img_coords = []
+        intrinsics = []
+        cam_names = []
 
-            for screen in self.screen_widgets:
-                camera_name = screen.get_camera_name()
+        # Get coords and intrinsic parameters from the screens
+        for screen in self.screen_widgets:
+            camera_name = screen.get_camera_name()
+            coords = self.model.get_coords_axis(camera_name)
+            intrinsic = self.model.get_camera_intrinsic(camera_name)
+            if coords is not None:
                 cam_names.append(camera_name)
-                img_coords.append(self.model.get_coords_axis(camera_name))
-                intrinsics.append(self.model.get_camera_intrinsic(camera_name))
-
-            if len(intrinsics) >= 2:
-                print("\n== intrinsics ==")
-                print(f" cam {cam_names[0]}:\n  {intrinsics[0]}")
-                print(f" cam {cam_names[1]}:\n  {intrinsics[1]}")
-
-            # TODO
-            self.calibrationStereo = CalibrationStereo(
-                cam_names[0],
-                img_coords[0],
-                intrinsics[0],
-                cam_names[1],
-                img_coords[1],
-                intrinsics[1],
-            )
-            retval, R_AB, T_AB, E_AB, F_AB = (
-                self.calibrationStereo.calibrate_stereo()
-            )
-            self.model.add_camera_extrinsic(
-                cam_names[0], cam_names[1], retval, R_AB, T_AB, E_AB, F_AB
-            )
+                img_coords.append(coords)
+                intrinsics.append(intrinsic)
 
-            # Test
-            err = self.calibrationStereo.test_performance(
-                cam_names[0], img_coords[0], cam_names[1], img_coords[1]
-            )
-            return err
-        else:
+        # Ensure there are at least two cameras  
+        if len(cam_names) < 2:
             return None
+        
+        # Perform calibration between pairs of cameras
+        print(cam_names)
+        for i in range(len(cam_names)-1):
+            for j in range(i+1, len(cam_names)):
+                camA, camB = cam_names[i], cam_names[j]
+                coordsA, coordsB = img_coords[i], img_coords[j]
+                itmxA, itmxB = intrinsics[i], intrinsics[j]
+                
+                err, instance, retval, R_AB, T_AB, E_AB, F_AB = self.get_results_calibrate_stereo(
+                    camA, coordsA, itmxA, camB, coordsB, itmxB
+                )
+                print(f"camA: {camA} camB: {camB} err: {err}")
+                if err < min_err:
+                    self.calibrationStereo = instance
+                    min_err = err
+                    R_AB_best, T_AB_best, E_AB_best, F_AB_best = R_AB, T_AB, E_AB, F_AB
+                    self.camA_best, self.camB_best = camA, camB
+                    coordsA_best, coordsB_best = coordsA, coordsB
+                    itmxA_best, itmxB_best = itmxA, itmxB
+                    
+        self.model.add_camera_extrinsic(
+            self.camA_best, self.camB_best, min_err, R_AB_best, T_AB_best, E_AB_best, F_AB_best
+        )
+
+        print("\n== intrinsics ==")
+        print(f" cam {self.camA_best}:\n  {itmxA_best}")
+        print(f" cam {self.camB_best}:\n  {itmxB_best}")
+        self.calibrationStereo.print_calibrate_stereo_results()
+        err = self.calibrationStereo.test_performance(
+            self.camA_best, coordsA_best, self.camB_best, coordsB_best, print_results=True
+            )
+        return err
 
     def reticle_detect_all_screen(self):
         """
         Checks all screens for reticle detection results and updates the status based on whether the reticle
         has been detected on all screens.
         """
         """Detect reticle coordinates on all screens."""
@@ -384,14 +487,38 @@
             coords = screen.get_reticle_coords()
             mtx, dist = screen.get_camera_intrinsic()
             camera_name = screen.get_camera_name()
             # Retister the reticle coords in the model
             self.model.add_coords_axis(camera_name, coords)
             self.model.add_camera_intrinsic(camera_name, mtx, dist)
 
+    def reticle_detect_two_screens(self):
+        """Detect reticle coordinates on two screens."""
+        reticle_detected_screen_cnt = 0
+        for screen in self.screen_widgets:
+            coords = screen.get_reticle_coords()
+            if coords is not None:
+                reticle_detected_screen_cnt += 1
+
+        if reticle_detected_screen_cnt >= 2:
+            # Found the coords
+            self.reticle_detect_detected_status()
+        else:
+            return
+        
+        # Register into the model
+        for screen in self.screen_widgets:
+            coords = screen.get_reticle_coords()
+            mtx, dist = screen.get_camera_intrinsic()
+            camera_name = screen.get_camera_name()
+            # Retister the reticle coords in the model
+            if coords is not None:
+                self.model.add_coords_axis(camera_name, coords)
+                self.model.add_camera_intrinsic(camera_name, mtx, dist)
+
     def probe_detect_all_screen(self):
         """Detect probe coordinates on all screens."""
         timestamp_cmp, sn_cmp = None, None
         cam_names = []
         tip_coords = []
 
         if self.calibrationStereo is None:
@@ -420,29 +547,82 @@
             cam_names.append(camera_name)
             tip_coords.append(tip_coord)
 
         # All screen has the same timestamp. Proceed the triangulation
         global_coords = self.calibrationStereo.get_global_coords(
             cam_names[0], tip_coords[0], cam_names[1], tip_coords[1]
         )
-        self.stageListener.handleGlobalDataChange(sn, global_coords, timestamp)
+        self.stageListener.handleGlobalDataChange(sn,
+                                global_coords,
+                                timestamp,
+                                cam_names[0],
+                                tip_coords[0],
+                                cam_names[1],
+                                tip_coords[1]
+                            )
+
+    def probe_detect_two_screens(self):
+        """Detect probe coordinates on all screens."""
+        timestamp_cmp, sn_cmp = None, None
+
+        if self.calibrationStereo is None:
+            print("Camera calibration has not done")
+            return
+
+        for screen in self.screen_widgets:
+            camera_name = screen.get_camera_name()
+            if camera_name == self.camA_best or camera_name == self.camB_best:
+                timestamp, sn, tip_coord = screen.get_last_detect_probe_info()
+
+                if (sn is None) or (tip_coord is None) or (timestamp is None):
+                    return
+
+                if timestamp_cmp is None:
+                    timestamp_cmp = timestamp
+                else:  # if timestamp is different between screens, return
+                    if timestamp_cmp[:-2] != timestamp[:-2]:
+                        return
+
+                if sn_cmp is None:
+                    sn_cmp = sn
+                else:  # if sn is different between screens, return
+                    if sn_cmp != sn:
+                        return
+                if camera_name == self.camA_best:
+                    tip_coordsA = tip_coord
+                else:
+                    tip_coordsB = tip_coord
+
+        # All screen has the same timestamp. Proceed the triangulation
+        global_coords = self.calibrationStereo.get_global_coords(
+            self.camA_best, tip_coordsA, self.camB_best, tip_coordsB
+        )
+
+        self.stageListener.handleGlobalDataChange(sn,
+                                global_coords,
+                                timestamp,
+                                self.camA_best, 
+                                tip_coordsA, 
+                                self.camB_best, 
+                                tip_coordsB
+                            )
 
     def probe_overwrite_popup_window(self):
         """
         Displays a confirmation dialog asking the user if they want to overwrite the current probe position.
 
         Returns:
             bool: True if the user confirms the overwrite, False otherwise.
         """
         message = (
             f"Are you sure you want to overwrite the current probe position?"
         )
         response = QMessageBox.warning(
             self,
-            "Reticle Detection Failed",
+            "Probe Detection",
             message,
             QMessageBox.Yes | QMessageBox.No,
             QMessageBox.No,
         )
 
         # Check which button was clicked
         if response == QMessageBox.Yes:
@@ -486,42 +666,53 @@
 
         self.probe_calibration_btn.setChecked(False)
         if self.reticle_detection_status == "default":
             self.probe_calibration_btn.setEnabled(False)
 
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(
-                    self.probe_detect_all_screen
-                )
-                screen.run_no_filter()
-
+                camera_name = screen.get_camera_name()
+                if camera_name == self.camA_best or camera_name == self.camB_best:
+                    print(f"Disconnect probe_detection: {camera_name}")
+                    screen.probe_coords_detected.disconnect(
+                        self.probe_detect_two_screens
+                    )
+                    screen.run_no_filter()
+ 
             self.filter = "no_filter"
+            logger.debug(f"filter: {self.filter}")
             self.probeCalibration.clear()
 
         # update global coords
         self.stageListener.requestClearGlobalDataTransformM()
 
     def probe_detect_process_status(self):
         """
         Updates the UI and internal state to reflect that the probe detection process is underway.
         """
-        self.probe_detection_status = "process"
+        self.probe_detection_status = "                                                                                                                                         "
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #bc9e44;"
         )
         self.calib_x.show()
         self.calib_y.show()
         self.calib_z.show()
 
+        # Connect with only reticle detected screens
         for screen in self.screen_widgets:
-            screen.probe_coords_detected.connect(self.probe_detect_all_screen)
-            screen.run_probe_detection()
+            camera_name = screen.get_camera_name()
+            if camera_name == self.camA_best or camera_name == self.camB_best:
+                print(f"Connect probe_detection: {camera_name}")
+                screen.probe_coords_detected.connect(self.probe_detect_two_screens)
+                screen.run_probe_detection()
+            else:
+                screen.run_no_filter()
         self.filter = "probe_detection"
+        logger.debug(f"filter: {self.filter}")
 
         # message
         message = f"Move probe at least 2mm along X, Y, and Z axes"
         QMessageBox.information(self, "Probe calibration info", message)
 
     def probe_detect_accepted_status(self, stage_sn, transformation_matrix):
         """
@@ -536,20 +727,24 @@
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
         self.hide_x_y_z()
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
-                screen.probe_coords_detected.disconnect(
-                    self.probe_detect_all_screen
-                )
-                screen.run_no_filter()
+                camera_name = screen.get_camera_name()
+                if camera_name == self.camA_best or camera_name == self.camB_best:
+                    print(f"Disconnect probe_detection: {camera_name}")
+                    screen.probe_coords_detected.disconnect(
+                        self.probe_detect_two_screens
+                    )
+                    screen.run_no_filter()
 
             self.filter = "no_filter"
+            logger.debug(f"filter: {self.filter}")
 
         # update global coords
         self.stageListener.requestUpdateGlobalDataTransformM(
             stage_sn, transformation_matrix
         )
 
     def hide_x_y_z(self):
@@ -574,15 +769,15 @@
         if self.calib_z.isVisible():
             self.calib_z.hide()
             # Change the button to green.
             self.calib_z.setStyleSheet(
             "color: white;"
             "background-color: black;"
         )
-            
+
     def calib_x_complete(self):
         """
         Updates the UI to indicate that the calibration for the X-axis is complete.
         """
         if self.calib_x.isVisible():
             # Change the button to green.
             self.calib_x.setStyleSheet(
```

### Comparing `parallax_app-0.37.5/parallax/user_setting_manager.py` & `parallax_app-0.37.6/parallax/user_setting_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax/utils.py` & `parallax_app-0.37.6/parallax/utils.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/parallax_app.egg-info/PKG-INFO` & `parallax_app-0.37.6/parallax_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.5
+Version: 0.37.6
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.5/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.6/parallax_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 img/recordingButton.png
 img/sextant.png
 img/snapshotButton_white.png
 img/stop-sign.png
 img/target.png
 parallax/__init__.py
 parallax/__main__.py
+parallax/axis_filter.py
 parallax/calibration_camera.py
 parallax/camera.py
 parallax/curr_bg_cmp_processor.py
 parallax/curr_prev_cmp_processor.py
 parallax/main_window_wip.py
 parallax/mask_generator.py
 parallax/model.py
```

### Comparing `parallax_app-0.37.5/pyproject.toml` & `parallax_app-0.37.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/tests/test_screen_widget.py` & `parallax_app-0.37.6/tests/test_screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/ParallaxReadME.JPG` & `parallax_app-0.37.6/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.6/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/mainWindow.ui` & `parallax_app-0.37.6/ui/mainWindow.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/probe_calib.ui` & `parallax_app-0.37.6/ui/probe_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/arrow-right.png` & `parallax_app-0.37.6/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/check.png` & `parallax_app-0.37.6/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/gear.png` & `parallax_app-0.37.6/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/recordingButton.png` & `parallax_app-0.37.6/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.6/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/sextant.png` & `parallax_app-0.37.6/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.6/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.6/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.6/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/stop-sign.png` & `parallax_app-0.37.6/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/resources/target.png` & `parallax_app-0.37.6/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/reticle_calib.ui` & `parallax_app-0.37.6/ui/reticle_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/settingPopUpMenu.ui` & `parallax_app-0.37.6/ui/settingPopUpMenu.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.5/ui/stage_info.ui` & `parallax_app-0.37.6/ui/stage_info.ui`

 * *Files identical despite different names*

