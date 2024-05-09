# Comparing `tmp/ansys_aedt_toolkits_common-0.4.1.tar.gz` & `tmp/ansys_aedt_toolkits_common-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_aedt_toolkits_common-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_aedt_toolkits_common-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_aedt_toolkits_common-0.4.1.tar` & `ansys_aedt_toolkits_common-0.4.2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1089 2024-05-08 12:10:02.727355 ansys_aedt_toolkits_common-0.4.1/LICENSE
--rw-r--r--   0        0        0     3531 2024-05-08 12:10:02.727355 ansys_aedt_toolkits_common-0.4.1/README.rst
--rw-r--r--   0        0        0     2684 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1230 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/__init__.py
--rw-r--r--   0        0        0    37347 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/api.py
--rw-r--r--   0        0        0      265 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/common_properties.toml
--rw-r--r--   0        0        0     1976 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/constants.py
--rw-r--r--   0        0        0     2517 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/logger_handler.py
--rw-r--r--   0        0        0     2541 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/models.py
--rw-r--r--   0        0        0     3706 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
--rw-r--r--   0        0        0     7884 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/rest_api.py
--rw-r--r--   0        0        0     3339 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/thread_manager.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/__init__.py
--rw-r--r--   0        0        0    21177 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/actions_generic.py
--rw-r--r--   0        0        0     1051 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_properties.toml
--rw-r--r--   0        0        0        0 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
--rw-r--r--   0        0        0     4997 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
--rw-r--r--   0        0        0     8951 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
--rw-r--r--   0        0        0     2381 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/logger_handler.py
--rw-r--r--   0        0        0        0 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
--rw-r--r--   0        0        0    19844 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
--rw-r--r--   0        0        0     2997 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/models.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
--rw-r--r--   0        0        0     2406 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
--rw-r--r--   0        0        0     2487 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
--rw-r--r--   0        0        0    57746 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
--rw-r--r--   0        0        0    35360 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
--rw-r--r--   0        0        0     2379 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
--rw-r--r--   0        0        0      982 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
--rw-r--r--   0        0        0     1007 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
--rw-r--r--   0        0        0     5074 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
--rw-r--r--   0        0        0      819 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
--rw-r--r--   0        0        0     6058 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
--rw-r--r--   0        0        0     1124 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
--rw-r--r--   0        0        0     2436 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
--rw-r--r--   0        0        0     8449 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
--rw-r--r--   0        0        0     1615 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
--rw-r--r--   0        0        0     6064 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
--rw-r--r--   0        0        0    24133 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
--rw-r--r--   0        0        0     2300 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
--rw-r--r--   0        0        0     4241 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
--rw-r--r--   0        0        0     5091 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
--rw-r--r--   0        0        0     1969 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
--rw-r--r--   0        0        0      797 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
--rw-r--r--   0        0        0     1058 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
--rw-r--r--   0        0        0     2037 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
--rw-r--r--   0        0        0     3207 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
--rw-r--r--   0        0        0     1857 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
--rw-r--r--   0        0        0      344 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
--rw-r--r--   0        0        0     1877 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
--rw-r--r--   0        0        0     1749 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
--rw-r--r--   0        0        0     7977 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
--rw-r--r--   0        0        0      959 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
--rw-r--r--   0        0        0     1263 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
--rw-r--r--   0        0        0     3615 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
--rw-r--r--   0        0        0      448 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
--rw-r--r--   0        0        0     2255 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
--rw-r--r--   0        0        0      423 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
--rw-r--r--   0        0        0     3184 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
--rw-r--r--   0        0        0     8477 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
--rw-r--r--   0        0        0     2024 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
--rw-r--r--   0        0        0     3641 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
--rw-r--r--   0        0        0      897 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
--rw-r--r--   0        0        0      899 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
--rw-r--r--   0        0        0      868 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
--rw-r--r--   0        0        0      894 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
--rw-r--r--   0        0        0     1986 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
--rw-r--r--   0        0        0     1947 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
--rw-r--r--   0        0        0     1963 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
--rw-r--r--   0        0        0     2421 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
--rw-r--r--   0        0        0     2503 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
--rw-r--r--   0        0        0     5116 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
--rw-r--r--   0        0        0     4927 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
--rw-r--r--   0        0        0     2780 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
--rw-r--r--   0        0        0      603 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
--rw-r--r--   0        0        0     3871 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
--rw-r--r--   0        0        0     1821 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
--rw-r--r--   0        0        0     2587 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
--rw-r--r--   0        0        0      172 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
--rw-r--r--   0        0        0     7191 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
--rw-r--r--   0        0        0     6578 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
--rw-r--r--   0        0        0    10452 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
--rw-r--r--   0        0        0      471 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
--rw-r--r--   0        0        0     4120 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
--rw-r--r--   0        0        0      405 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
--rw-r--r--   0        0        0     2165 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
--rw-r--r--   0        0        0     1463 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
--rw-r--r--   0        0        0    12519 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
--rw-r--r--   0        0        0    11434 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
--rw-r--r--   0        0        0     4599 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
--rw-r--r--   0        0        0     4408 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
--rw-r--r--   0        0        0      290 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
--rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
--rw-r--r--   0        0        0    21788 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
--rw-r--r--   0        0        0     7012 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/utils.py
--rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-09 12:15:52.269873 ansys_aedt_toolkits_common-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3531 2024-05-09 12:15:52.269873 ansys_aedt_toolkits_common-0.4.2/README.rst
+-rw-r--r--   0        0        0     2684 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1230 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/__init__.py
+-rw-r--r--   0        0        0    37347 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/api.py
+-rw-r--r--   0        0        0      265 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/common_properties.toml
+-rw-r--r--   0        0        0     1976 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/constants.py
+-rw-r--r--   0        0        0     2517 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/logger_handler.py
+-rw-r--r--   0        0        0     2541 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/models.py
+-rw-r--r--   0        0        0     3706 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
+-rw-r--r--   0        0        0     7884 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/rest_api.py
+-rw-r--r--   0        0        0     3339 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/thread_manager.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/__init__.py
+-rw-r--r--   0        0        0    21177 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/actions_generic.py
+-rw-r--r--   0        0        0     1051 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_properties.toml
+-rw-r--r--   0        0        0        0 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
+-rw-r--r--   0        0        0     4997 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
+-rw-r--r--   0        0        0     8951 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
+-rw-r--r--   0        0        0     2381 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/logger_handler.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
+-rw-r--r--   0        0        0    19844 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
+-rw-r--r--   0        0        0     2997 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/models.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
+-rw-r--r--   0        0        0     2406 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
+-rw-r--r--   0        0        0     2487 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
+-rw-r--r--   0        0        0    57746 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
+-rw-r--r--   0        0        0    35360 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
+-rw-r--r--   0        0        0     2379 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
+-rw-r--r--   0        0        0      982 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
+-rw-r--r--   0        0        0     1007 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
+-rw-r--r--   0        0        0     5074 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
+-rw-r--r--   0        0        0      819 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
+-rw-r--r--   0        0        0     6058 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
+-rw-r--r--   0        0        0     1124 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
+-rw-r--r--   0        0        0     2436 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
+-rw-r--r--   0        0        0     8449 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
+-rw-r--r--   0        0        0     1615 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
+-rw-r--r--   0        0        0     6064 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
+-rw-r--r--   0        0        0    24133 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
+-rw-r--r--   0        0        0     2300 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
+-rw-r--r--   0        0        0     4241 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
+-rw-r--r--   0        0        0     5091 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
+-rw-r--r--   0        0        0     1969 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
+-rw-r--r--   0        0        0      797 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
+-rw-r--r--   0        0        0     1058 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
+-rw-r--r--   0        0        0     2037 2024-05-09 12:15:52.277873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
+-rw-r--r--   0        0        0     3207 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
+-rw-r--r--   0        0        0     1857 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
+-rw-r--r--   0        0        0      344 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
+-rw-r--r--   0        0        0     1877 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
+-rw-r--r--   0        0        0     1749 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
+-rw-r--r--   0        0        0     7977 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
+-rw-r--r--   0        0        0      959 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
+-rw-r--r--   0        0        0     1263 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
+-rw-r--r--   0        0        0     3615 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
+-rw-r--r--   0        0        0      448 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
+-rw-r--r--   0        0        0     2255 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
+-rw-r--r--   0        0        0      423 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
+-rw-r--r--   0        0        0     3184 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
+-rw-r--r--   0        0        0     8477 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
+-rw-r--r--   0        0        0     2024 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
+-rw-r--r--   0        0        0     3641 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
+-rw-r--r--   0        0        0      899 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
+-rw-r--r--   0        0        0      868 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
+-rw-r--r--   0        0        0      894 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
+-rw-r--r--   0        0        0     1986 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
+-rw-r--r--   0        0        0     1947 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
+-rw-r--r--   0        0        0     1963 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
+-rw-r--r--   0        0        0     2421 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
+-rw-r--r--   0        0        0     2503 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
+-rw-r--r--   0        0        0     5116 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
+-rw-r--r--   0        0        0     4927 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
+-rw-r--r--   0        0        0     2780 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
+-rw-r--r--   0        0        0      603 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
+-rw-r--r--   0        0        0     3871 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
+-rw-r--r--   0        0        0     1821 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
+-rw-r--r--   0        0        0      172 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
+-rw-r--r--   0        0        0     7191 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
+-rw-r--r--   0        0        0     6578 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
+-rw-r--r--   0        0        0    10452 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
+-rw-r--r--   0        0        0      471 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
+-rw-r--r--   0        0        0     4120 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
+-rw-r--r--   0        0        0      405 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
+-rw-r--r--   0        0        0     2165 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
+-rw-r--r--   0        0        0     1463 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
+-rw-r--r--   0        0        0    12519 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
+-rw-r--r--   0        0        0    11434 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
+-rw-r--r--   0        0        0     4599 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
+-rw-r--r--   0        0        0     4408 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
+-rw-r--r--   0        0        0      290 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
+-rw-r--r--   0        0        0    21788 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
+-rw-r--r--   0        0        0     7009 2024-05-09 12:15:52.281873 ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/utils.py
+-rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.2/PKG-INFO
```

### Comparing `ansys_aedt_toolkits_common-0.4.1/LICENSE` & `ansys_aedt_toolkits_common-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/README.rst` & `ansys_aedt_toolkits_common-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/pyproject.toml` & `ansys_aedt_toolkits_common-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 """
 pyaedt-toolkits.
 
 ansys.aedt.toolkits.common
 """
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/api.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/api.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/constants.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/models.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/multithreading_server.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/multithreading_server.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/rest_api.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/rest_api.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/thread_manager.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/backend/thread_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/actions_generic.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/actions_generic.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_properties.toml` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_properties.toml`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/models.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/utils.py` & `ansys_aedt_toolkits_common-0.4.2/src/ansys/aedt/toolkits/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 def check_backend_communication(url_call):
     """Check backend communication."""
     try:
         response = requests.get(url_call + "/health")
         return response.ok
     except requests.exceptions.RequestException:
-        logger.error("Failed to check backend communication.")
+        print("Failed to check backend communication.")
         return False
 
 
 def process_desktop_properties(is_linux, url_call):
     """Process desktop properties."""
     desktop_pid = None
     desktop_version = None
@@ -179,15 +179,15 @@
             response = requests.put(url_call + "/properties", json=new_properties)
             if not response.ok:
                 return
             print("Connect to AEDT session.")
             requests.post(url_call + "/launch_aedt")
             requests.post(url_call + "/wait_thread")
         except requests.exceptions.RequestException:
-            logger.error("Properties update failed")
+            raise Exception("Properties update failed.")
 
 
 class ToolkitThreadStatus(str, Enum):
     """Provides an enumeration of statuses for a toolkit thread."""
 
     IDLE = "Toolkit is idle and ready to accept a new task."
     BUSY = "Toolkit is busy and processing a task."
```

### Comparing `ansys_aedt_toolkits_common-0.4.1/PKG-INFO` & `ansys_aedt_toolkits_common-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-aedt-toolkits-common
-Version: 0.4.1
+Version: 0.4.2
 Summary: User interface example repository to create your toolkit.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

