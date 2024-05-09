# Comparing `tmp/hello_robot_stretch_factory-0.5.5.tar.gz` & `tmp/hello-robot-stretch-factory-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.5.5.tar", last modified: Fri Mar  8 03:36:23 2024, max compression
+gzip compressed data, was "hello-robot-stretch-factory-0.5.6.tar", last modified: Thu May  9 18:05:44 2024, max compression
```

## Comparing `hello_robot_stretch_factory-0.5.5.tar` & `hello-robot-stretch-factory-0.5.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      931 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/LICENSE.md
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      367 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/README.md
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      253 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/deploy.sh
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/
--rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2024-03-08 03:36:23.000000 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3200 2024-03-08 03:36:23.000000 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-03-08 03:36:23.000000 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       86 2024-03-08 03:36:23.000000 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2024-03-08 03:36:23.000000 hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1010 2024-03-08 03:35:58.000000 hello_robot_stretch_factory-0.5.5/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4641 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5437 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45544 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5406 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21840 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/param_mgmt.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9286 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/stretch_factory/trace_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/test/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-03-08 03:36:23.226133 hello_robot_stretch_factory-0.5.5/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/RE1_migrate_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2149 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/README.md
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2024-01-31 00:25:29.000000 hello_robot_stretch_factory-0.5.5/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7700 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4569 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/tools/REx_camera_set_symlink.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5596 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_comm_rates.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    19982 2024-02-01 00:46:30.000000 hello_robot_stretch_factory-0.5.5/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3680 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dmesg_monitor.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1353 2024-02-01 00:55:48.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5157 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1398 2024-03-08 03:33:05.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2848 2023-12-15 18:21:25.000000 hello_robot_stretch_factory-0.5.5/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5833 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2399 2024-01-26 16:46:42.000000 hello_robot_stretch_factory-0.5.5/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      735 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4449 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3183 2024-01-31 23:36:30.000000 hello_robot_stretch_factory-0.5.5/tools/REx_stepper_type.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1572 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-10-19 22:25:50.000000 hello_robot_stretch_factory-0.5.5/tools/REx_wacc_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8024 2024-03-08 03:27:30.000000 hello_robot_stretch_factory-0.5.5/tools/REx_xrandr_display.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-09 18:05:44.635994 hello-robot-stretch-factory-0.5.6/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      931 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/LICENSE.md
+-rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2024-05-09 18:05:44.635994 hello-robot-stretch-factory-0.5.6/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      367 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/README.md
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      253 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/deploy.sh
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-09 18:05:44.635994 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/
+-rw-r--r--   0 hello-robot  (1000) hello-robot  (1000)     1019 2024-05-09 18:05:44.000000 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3200 2024-05-09 18:05:44.000000 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2024-05-09 18:05:44.000000 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       86 2024-05-09 18:05:44.000000 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2024-05-09 18:05:44.000000 hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2024-05-09 18:05:44.635994 hello-robot-stretch-factory-0.5.6/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1010 2024-05-09 18:05:25.000000 hello-robot-stretch-factory-0.5.6/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-09 18:05:44.631994 hello-robot-stretch-factory-0.5.6/stretch_factory/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4641 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5437 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    45544 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5406 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21840 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/param_mgmt.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9286 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/stretch_factory/trace_mgmt.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-09 18:05:44.631994 hello-robot-stretch-factory-0.5.6/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/test/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/test/test_usb_reset.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2024-05-09 18:05:44.635994 hello-robot-stretch-factory-0.5.6/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/RE1_migrate_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2149 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/README.md
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2024-01-31 00:25:29.000000 hello-robot-stretch-factory-0.5.6/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7700 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4569 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/tools/REx_camera_set_symlink.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5596 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_comm_rates.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    19982 2024-02-01 00:46:30.000000 hello-robot-stretch-factory-0.5.6/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3680 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dmesg_monitor.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1353 2024-02-01 00:55:48.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5157 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1398 2024-03-08 03:33:05.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2848 2023-12-15 18:21:25.000000 hello-robot-stretch-factory-0.5.6/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5833 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2399 2024-01-26 16:46:42.000000 hello-robot-stretch-factory-0.5.6/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      735 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4449 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3183 2024-01-31 23:36:30.000000 hello-robot-stretch-factory-0.5.6/tools/REx_stepper_type.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1572 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-10-19 22:25:50.000000 hello-robot-stretch-factory-0.5.6/tools/REx_wacc_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8024 2024-03-08 03:27:30.000000 hello-robot-stretch-factory-0.5.6/tools/REx_xrandr_display.py
```

### Comparing `hello_robot_stretch_factory-0.5.5/LICENSE.md` & `hello-robot-stretch-factory-0.5.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/PKG-INFO` & `hello-robot-stretch-factory-0.5.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hello_robot_stretch_factory
-Version: 0.5.5
+Name: hello-robot-stretch-factory
+Version: 0.5.6
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hello_robot_stretch_factory
-Version: 0.5.5
+Name: hello-robot-stretch-factory
+Version: 0.5.6
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.5.5/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello-robot-stretch-factory-0.5.6/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/setup.py` & `hello-robot-stretch-factory-0.5.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     long_description = fh.read()
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
-    name="hello_robot_stretch_factory",
-    version="0.5.5",
+    name="hello-robot-stretch-factory",
+    version="0.5.6",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/device_mgmt.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_available.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_available.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_installed.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_recommended.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_updater.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_utils.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/firmware_version.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/hello_device_utils.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/hello_device_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/param_mgmt.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/stretch_factory/trace_mgmt.py` & `hello-robot-stretch-factory-0.5.6/stretch_factory/trace_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/test/test_firmware_updater.py` & `hello-robot-stretch-factory-0.5.6/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/test/test_usb_reset.py` & `hello-robot-stretch-factory-0.5.6/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/RE1_migrate_contacts.py` & `hello-robot-stretch-factory-0.5.6/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/RE1_migrate_params.py` & `hello-robot-stretch-factory-0.5.6/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/README.md` & `hello-robot-stretch-factory-0.5.6/tools/README.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_D435i_check.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_imu_collect.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_imu_process.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_base_calibrate_wheel_separation.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_gravity_comp.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_guarded_contact.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_guarded_contact.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_calibrate_range.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_camera_set_symlink.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_camera_set_symlink.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_cliff_sensor_calibrate.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_comm_rates.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_comm_rates.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_discover_hello_devices.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dmesg_monitor.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dmesg_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_id_change.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_id_scan.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_jog.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_reboot.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_dynamixel_set_baud.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_firmware_flash.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_firmware_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_firmware_updater.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_gamepad_configure.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_gripper_calibrate.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_hello_dynamixel_jog.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_calibration_run.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_ctrl_tuning.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_gains.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_jog.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_mechaduino_menu.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_stepper_type.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_stepper_type.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_trace_firmware.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_trace_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_trace_robot.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_usb_reset.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_wacc_calibrate.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.5.5/tools/REx_xrandr_display.py` & `hello-robot-stretch-factory-0.5.6/tools/REx_xrandr_display.py`

 * *Files identical despite different names*

