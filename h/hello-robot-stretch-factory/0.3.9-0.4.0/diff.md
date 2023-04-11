# Comparing `tmp/hello_robot_stretch_factory-0.3.9.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.3.9.tar", last modified: Mon Sep 26 23:26:26 2022, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.0.tar", last modified: Tue Apr 11 22:29:49 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.3.9.tar` & `hello_robot_stretch_factory-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,59 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2022-09-26 23:26:26.000000 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1447 2022-09-26 23:26:26.000000 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2022-09-26 23:26:26.000000 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       73 2022-09-26 23:26:26.000000 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2022-09-26 23:26:26.000000 hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      992 2022-09-26 23:24:38.000000 hello_robot_stretch_factory-0.3.9/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2022-09-26 22:58:30.000000 hello_robot_stretch_factory-0.3.9/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    40406 2022-09-26 23:19:44.000000 hello_robot_stretch_factory-0.3.9/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    15885 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/stretch_factory/param_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 23:26:26.513807 hello_robot_stretch_factory-0.3.9/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    21784 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7224 2022-09-26 20:01:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5361 2022-09-26 21:04:56.000000 hello_robot_stretch_factory-0.3.9/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.3.9/tools/REx_wacc_calibrate.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.279500 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1796 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-11 22:29:49.000000 hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-11 22:29:27.000000 hello_robot_stretch_factory-0.4.0/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/stretch_factory/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2022-09-26 22:58:30.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37370 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/stretch_factory/param_mgmt.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.283499 hello_robot_stretch_factory-0.4.0/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/test/test_usb_reset.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-11 22:29:49.279500 hello_robot_stretch_factory-0.4.0/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7203 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-03-09 23:32:07.000000 hello_robot_stretch_factory-0.4.0/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4410 2023-04-11 22:29:04.000000 hello_robot_stretch_factory-0.4.0/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-11 22:29:18.000000 hello_robot_stretch_factory-0.4.0/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-11 22:29:02.000000 hello_robot_stretch_factory-0.4.0/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-11 22:29:02.000000 hello_robot_stretch_factory-0.4.0/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2022-09-26 19:48:43.000000 hello_robot_stretch_factory-0.4.0/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.3.9/LICENSE.md` & `hello_robot_stretch_factory-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/PKG-INFO` & `hello_robot_stretch_factory-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.3.9
+Version: 0.4.0
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.3.9
+Version: 0.4.0
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hello_robot_stretch_factory-0.3.9/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.0/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,50 @@
 setup.py
 ./tools/RE1_migrate_contacts.py
 ./tools/RE1_migrate_params.py
 ./tools/REx_D435i_check.py
 ./tools/REx_base_calibrate_imu_collect.py
 ./tools/REx_base_calibrate_imu_process.py
 ./tools/REx_base_calibrate_wheel_separation.py
+./tools/REx_calibrate_gravity_comp.py
 ./tools/REx_calibrate_guarded_contact.py
 ./tools/REx_calibrate_range.py
 ./tools/REx_cliff_sensor_calibrate.py
+./tools/REx_discover_hello_devices.py
 ./tools/REx_dynamixel_id_change.py
 ./tools/REx_dynamixel_id_scan.py
 ./tools/REx_dynamixel_jog.py
 ./tools/REx_dynamixel_reboot.py
 ./tools/REx_dynamixel_set_baud.py
+./tools/REx_firmware_flash.py
 ./tools/REx_firmware_updater.py
 ./tools/REx_gamepad_configure.py
 ./tools/REx_gripper_calibrate.py
 ./tools/REx_hello_dynamixel_jog.py
 ./tools/REx_stepper_calibration_YAML_to_flash.py
 ./tools/REx_stepper_calibration_flash_to_YAML.py
 ./tools/REx_stepper_calibration_run.py
 ./tools/REx_stepper_ctrl_tuning.py
 ./tools/REx_stepper_gains.py
 ./tools/REx_stepper_jog.py
 ./tools/REx_stepper_mechaduino_menu.py
+./tools/REx_trace_firmware.py
+./tools/REx_trace_robot.py
 ./tools/REx_usb_reset.py
 ./tools/REx_wacc_calibrate.py
 hello_robot_stretch_factory.egg-info/PKG-INFO
 hello_robot_stretch_factory.egg-info/SOURCES.txt
 hello_robot_stretch_factory.egg-info/dependency_links.txt
 hello_robot_stretch_factory.egg-info/requires.txt
 hello_robot_stretch_factory.egg-info/top_level.txt
 stretch_factory/__init__.py
 stretch_factory/device_mgmt.py
+stretch_factory/firmware_available.py
+stretch_factory/firmware_installed.py
+stretch_factory/firmware_recommended.py
 stretch_factory/firmware_updater.py
+stretch_factory/firmware_utils.py
+stretch_factory/firmware_version.py
 stretch_factory/hello_device_utils.py
 stretch_factory/param_mgmt.py
 test/test_firmware_updater.py
 test/test_usb_reset.py
```

### Comparing `hello_robot_stretch_factory-0.3.9/setup.py` & `hello_robot_stretch_factory-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.3.9",
+    version="0.4.0",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
     packages=['stretch_factory'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
-    install_requires=['future', 'pyserial','pyusb','gitpython','hello-robot-stretch-body>=0.4.8','tabulate']
+
+    install_requires=['future', 'pyserial','pyusb','gitpython','hello-robot-stretch-body>=0.4.26','tabulate']
+
 )
```

### Comparing `hello_robot_stretch_factory-0.3.9/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.0/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.0/stretch_factory/firmware_updater.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,643 +1,693 @@
 #!/usr/bin/env python
 
 import click
 import os
 from subprocess import Popen, PIPE
-import git
 import stretch_body.stepper
 import stretch_body.pimu
 import stretch_body.wacc
 import stretch_body.device
 import yaml
 import time
 import sys
 import stretch_body.device
-from stretch_factory.device_mgmt import StretchDeviceMgmt
-import stretch_body.hello_utils
 
-# #####################################################################################################
-class FirmwareVersion():
-    """
-    Manage comparision of firmware versions
-    """
-    def __init__(self,version_str):
-        self.device='NONE'
-        self.major=0
-        self.minor=0
-        self.bugfix=0
-        self.protocol=0
-        self.valid=False
-        self.from_string(version_str)
-    def __str__(self):
-        return self.to_string()
-    def to_string(self):
-        """
-        Version is represented as Stepper.v0.0.1p0 for example
-        """
-        return self.device+'.v'+str(self.major)+'.'+str(self.minor)+'.'+str(self.bugfix)+'p'+str(self.protocol)
+import stretch_body.hello_utils
+import shlex
+from stretch_factory.firmware_available import FirmwareAvailable
+from stretch_factory.firmware_recommended import FirmwareRecommended
+from stretch_factory.firmware_installed import FirmwareInstalled
+from stretch_factory.firmware_version import FirmwareVersion
+import stretch_factory.firmware_utils as fwu
 
-    def __gt__(self, other):
-        if not self.valid or not other.valid:
-            return False
-        if self.protocol>other.protocol:
-            return True
-        if self.protocol<other.protocol:
-            return False
-        if self.major > other.major:
-            return True
-        if self.minor > other.minor:
-            return True
-        if self.bugfix > other.bugfix:
-            return True
-        return False
+import stretch_factory.hello_device_utils as hdu
 
-    def __lt__(self, other):
-        if not self.valid or not other.valid:
-            return False
-        if self.protocol<other.protocol:
-            return True
-        if self.protocol>other.protocol:
-            return False
-        if self.major < other.major:
-            return True
-        if self.minor < other.minor:
-            return True
-        if self.bugfix < other.bugfix:
-            return True
-        return False
 
-    def __ne__(self,other):
-        return not self.__eq__(other)
 
-    def __eq__(self,other):
-        if not other or not self.valid or not other.valid:
-            return False
-        return self.major == other.major and self.minor == other.minor and self.bugfix == other.bugfix and self.protocol==other.protocol
+class FirmwareUpdater():
+    def __init__(self, use_device,args):
+        #use_device = {'hello-motor-arm': True, 'hello-motor-right-wheel': True, 'hello-motor-left-wheel': True, 'hello-pimu': True, 'hello-wacc': True,'hello-motor-lift': True}
+        self.ready_to_run = False
+        self.resume_tmp_filename='/tmp/REx_firmware_updater_resume.yaml'
+        self.args=args
+        state_from_yaml = self.from_yaml()
+
+        if args.resume:
+            if not state_from_yaml:
+                click.secho('WARNING: A previous firmware update is not available. Unable to resume', fg="yellow",bold=True)
+                self.ready_to_run = False
+                return
+            else:
 
-    def same_device(self,d):
-        return d==self.device
+                self.state = state_from_yaml  # Use the disk version
+                devs=' '
+                for d in self.state['use_device']:
+                    if self.state['use_device'][d]:
+                        devs=devs+' '+str(d)+' |'
+                devs=devs[:-1]
+                click.secho('\nResuming firmware updates for:%s '%devs, fg="green",bold=True)
+                print('')
+                self.ready_to_run = True
+        else:
+            if state_from_yaml:
+                click.secho('WARNING: A previous firmware update is incomplete', fg="yellow", bold=True)
+                click.secho('WARNING: Run REx_firmware_udpater.py --resume', fg="yellow", bold=True)
+                click.secho('WARNING: Or delete file %s and try again.'%self.resume_tmp_filename, fg="yellow",bold=True)
+                self.ready_to_run = False
+                return
+    
+            self.state = {}
+            self.state['use_device']=use_device
+            self.state['verbose'] = args.verbose
+            self.state['no_prompts'] = args.no_prompts
+            self.state['install_version'] = args.install_version
+            self.state['install_path'] = args.install_path
+            self.state['install_branch'] = args.install_branch
+            if self.state['install_path'] and self.state['install_path'][0] != '/':
+                    self.state['install_path'] = os.getcwd() + '/' + self.state['install_path']
+            self.state['completed']={}
+            for d in use_device:
+                if use_device[d]:
+                    self.state['completed'][d] = {'flash': False,
+                                                            'return_to_bus': False,
+                                                            'establish_comms':False,
+                                                            'version_validate': False,
+                                                            'calibration_flash': False,
+                                                            'return_to_bus2': False}
+
+
+        #Check that all devices targeted can be updated
+        self.fw_installed = FirmwareInstalled(self.state['use_device'])
+        all_valid=True
+        for d in self.state['use_device']:
+            if self.state['use_device'][d] and not self.fw_installed.is_device_valid(d):
+                click.secho('WARNING: Device %s is not valid. Unable to attempt the firmware update. Skipping device.'%d, fg="yellow", bold=True)
+                self.state['use_device'][d]=False
+                all_valid=False
+
+        # if not all_valid:
+        #     mapping = hdu.get_hello_ttyACMx_mapping()
+        #     if len(mapping['missing']):
+        #         print('')
+        #         click.secho('------------------------------------------', fg="yellow", bold=True)
+        #         click.secho('WARNING: Some devices are not on the bus:', fg="yellow", bold=True)
+        #         for k in mapping['hello']:
+        #             print('%s | %s'%(k,mapping['hello'][k]))
+        #         click.secho('------------------------------------------', fg="yellow", bold=True)
+        #         click.secho('WARNING: Power cycle the robot and try again', fg="yellow",bold=True)
+        #         click.secho('WARNING: Otherwise contact Hello Robot support', fg="yellow", bold=True)
+        #         print('')
+        #     self.ready_to_run=False
+        #     return
+
+        self.fw_available = FirmwareAvailable(self.state['use_device'])
+        self.fw_recommended = FirmwareRecommended(self.state['use_device'], self.fw_installed, self.fw_available)
+
+        self.create_arduino_config_file()
+        self.ready_to_run = fwu.check_arduino_cli_install()
+
+        # Set the target version to flash to recommended for each device
+        #This dict has a FirmwareVersion target for each device that has a valid (and desired) update
+        self.target = {}
+
+        if args.resume:
+            for d in self.state['use_device']:
+                if self.state['use_device'][d]:
+                    self.target[d] = FirmwareVersion(self.state['target_str'][d])
+        else:
+            self.state['repo_path']=None
 
-    def from_string(self,x):
-        #X is of form 'Stepper.v0.0.1p0'
-        try:
-            xl=x.split('.')
-            if len(xl) != 4:
-                raise Exception('Invalid version len')
-            device=xl[0]
-            if not (device=='Stepper' or device=='Wacc' or device=='Pimu'):
-                raise Exception('Invalid device name ')
-            major=int(xl[1][1:])
-            minor=int(xl[2])
-            bugfix=int(xl[3][0:xl[3].find('p')])
-            protocol=int(xl[3][(xl[3].find('p')+1):])
-            self.device=device
-            self.major=major
-            self.minor=minor
-            self.bugfix=bugfix
-            self.protocol=protocol
-            self.valid=True
-        except(ValueError,Exception):
-            print('Invalid version format in tag: %s'%x)
-# #####################################################################################################
-class InstalledFirmware():
-    """
-    Pull the current installed firmware off the robot uCs
-    Build config_info of form:
-    {'hello-motor-arm': {'board_info': {'board_version': u'Stepper.Irma.V1',
-       'firmware_version': u'Stepper.v0.0.1p1',
-       'protocol_version': u'p1'},
-      'installed_protocol_valid': True,
-      'supported_protocols': ['p0', 'p1']}}
-    """
-    def __init__(self,use_device):
-        """
-        use_device has form of:
-        {'hello-motor-lift': True, 'hello-motor-arm': True, 'hello-motor-right-wheel': True, 'hello-motor-left-wheel': True, 'hello-pimu': True, 'hello-wacc': True}
-        """
-        self.use_device=use_device
-        self.config_info={'hello-motor-lift': None,'hello-motor-arm':None,'hello-motor-left-wheel':None,'hello-motor-right-wheel':None,'hello-pimu':None,'hello-wacc':None}
-        for device in self.config_info.keys():
-            if self.use_device[device]:
-                if device=='hello-wacc':
-                    dd=stretch_body.wacc.Wacc()
-                elif device == 'hello-pimu':
-                    dd = stretch_body.pimu.Pimu()
+            #Default target is recommended
+            for d in self.state['use_device']:
+                if self.state['use_device'][d]:
+                    if d in self.fw_recommended.recommended:
+                        self.target[d] = self.fw_recommended.recommended[d]
+
+            #Now overwrite default target if given command line options
+            if args.install_version:
+                self.ready_to_run = self.ready_to_run and self.set_target_from_install_version()
+
+            if self.state['install_path']:
+                self.ready_to_run = self.ready_to_run and self.set_target_from_install_path(self.state['install_path'])
+
+            if args.install_branch:
+                self.ready_to_run = self.ready_to_run and self.set_target_from_install_branch()
+
+            # Store updated target for potential future resume
+            self.state['target_str'] = {}
+            for d in self.target:
+                if self.target[d]:
+                    self.state['target_str'][d] = self.target[d].to_string()
                 else:
-                    dd=stretch_body.stepper.Stepper('/dev/'+device)
-                dd.startup()
-                if dd.board_info['firmware_version'] is not None: #Was able to pull board info from device
-                    self.config_info[device]={}
-                    self.config_info[device]['board_info'] = dd.board_info.copy()
-                    try:
-                        self.config_info[device]['supported_protocols']=dd.supported_protocols.keys()
-                    except AttributeError:
-                        #Older versions of stretch body used a different represenation
-                        self.config_info[device]['supported_protocols']=[dd.valid_firmware_protocol]
-                    self.config_info[device]['installed_protocol_valid']=(dd.board_info['protocol_version']in self.config_info[device]['supported_protocols'])
-                    self.config_info[device]['version']=FirmwareVersion(self.config_info[device]['board_info']['firmware_version'])
-                    dd.stop()
-                else:
-                    self.config_info[device]=None
+                    self.state['target_str'][d] ='None'
 
-    def get_supported_protocols(self,device_name):
-        if self.is_device_valid(device_name):
-            return self.config_info[device_name]['supported_protocols']
-        return None
-    def get_version(self,device_name):
-        if self.is_device_valid(device_name):
-            return self.config_info[device_name]['version']
-        return None
-    def is_device_valid(self,device_name):
-        return self.config_info[device_name] is not None
+        # Count how many updates doing
+        num_update = 0
+        for device_name in self.target:
+            if self.fw_installed.is_device_valid(device_name):
+                num_update = num_update + 1
+        self.pretty_print_target()
+        if not num_update:
+            if not args.resume:
+                click.secho('No updates to be done', fg="yellow", bold=True)
+            else:
+                click.secho('WARNING: Unable to resume update. Not all devices returned to bus successfully', fg="red", bold=True)
+                click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+            self.ready_to_run=False
+        #At this point self.state dictionary has all information needed to run an update cycle
+
+    def to_yaml(self):
+        with open(self.resume_tmp_filename, 'w') as yaml_file:
+         yaml.dump(self.state, yaml_file, default_flow_style=False)
 
-    def is_protocol_supported(self,device_name,p):
-        """
-        Provide 'p0', etc
-        """
-        return self.is_device_valid(device_name) and p in self.config_info[device_name]['supported_protocols']
-
-    def max_protocol_supported(self,device_name):
-        x=[int(x[1:]) for x in self.config_info[device_name]['supported_protocols']]
-        return 'p'+str(max(x))
-
-    def pretty_print(self):
-        click.secho(' Currently Installed Firmware '.center(110,'#'),fg="cyan", bold=True)
-        for device in self.config_info:
-            if self.use_device[device]:
-                click.secho('------------ %s ------------'%device.upper(),fg="white", bold=True)
-                if self.config_info[device]:
-                    click.echo('Installed Firmware: %s'%self.config_info[device]['board_info']['firmware_version'])
-                    x=" , ".join(["{}"]*len(self.config_info[device]['supported_protocols'])).format(*self.config_info[device]['supported_protocols'])
-                    click.echo('Installed Stretch Body supports protocols: '+x)
-                    if self.config_info[device]['installed_protocol_valid']:
-                        click.secho('Installed protocol %s : VALID'%self.config_info[device]['board_info']['protocol_version'])
-                    else:
-                        click.secho('Installed protocol %s : INVALID'%self.config_info[device]['board_info']['protocol_version'],fg="yellow")
-                else:
-                    click.secho('Device not found')
-# #####################################################################################################
-class AvailableFirmware():
-    def __init__(self,use_device):
-        self.use_device=use_device
-        self.repo=None
-        self.repo_path=None
-        self.versions = {}
-        for d in self.use_device:
-            if self.use_device[d]:
-                self.versions[d]=[] #List of available versions for that device
-        self.__clone_firmware_repo()
-        self.__get_available_firmware_versions()
-
-    def __clone_firmware_repo(self):
-        print('Collecting information...')
-        self.repo_path = '/tmp/stretch_firmware_update'
-        if not os.path.isdir(self.repo_path):
-            #print('Cloning latest version of Stretch Firmware to %s'% self.repo_path)
-            git.Repo.clone_from('https://github.com/hello-robot/stretch_firmware',  self.repo_path)
-
-        sys.stdout.write('.')
-        sys.stdout.flush()
-        self.repo = git.Repo(self.repo_path)
-        os.chdir(self.repo_path)
-
-        sys.stdout.write('.')
-        sys.stdout.flush()
-        os.system('git checkout master >/dev/null 2>&1')
-
-        sys.stdout.write('.')
-        sys.stdout.flush()
-        os.system('git fetch --tags >/dev/null 2>&1 ')
-
-        sys.stdout.write('.')
-        sys.stdout.flush()
-        os.system('git pull >/dev/null 2>&1 ')
-        sys.stdout.write('.')
-        sys.stdout.flush()
-        print('\n')
-
-
-    def pretty_print(self):
-        click.secho(' Currently Tagged Versions of Stretch Firmware on Master Branch '.center(110,'#'),fg="cyan", bold=True)
-        for device_name in self.versions.keys():
-            click.secho('---- %s ----'%device_name.upper(), fg="white", bold=True)
-            for v in self.versions[device_name]:
-                print(v)
-    # python -m pip install gitpython
-    # https://www.devdungeon.com/content/working-git-repositories-python
-    def __get_available_firmware_versions(self):
-        if self.repo is None:
-            return
-        for t in self.repo.tags:
-            v = FirmwareVersion(t.name)
-            if v.valid:
-                for device_name in self.versions:
-                    if (v.device == 'Stepper' and device_name in ['hello-motor-lift','hello-motor-arm','hello-motor-left-wheel','hello-motor-right-wheel']) or\
-                        (v.device == 'Wacc' and device_name=='hello-wacc') or\
-                        (v.device == 'Pimu' and device_name=='hello-pimu'):
-                            self.versions[device_name].append(v)
-
-
-
-    def get_most_recent_version(self,device_name,supported_protocols):
-        """
-        For the device and supported protocol versions (eg, '['p0','p1']'), return the most recent version (type FirmwareVersion)
-        """
-        if len(self.versions[device_name])==0:
+    def from_yaml(self):
+        try:
+            with open(self.resume_tmp_filename, 'r') as s:
+                return  yaml.load(s, Loader=yaml.FullLoader)
+        except IOError:
             return None
-        recent=None
-        s=[int(x[1:]) for x in supported_protocols ]
-        supported_versions=[]
-        for v in self.versions[device_name]:
-            if v.protocol in s:
-                supported_versions.append(v)
-        for sv in supported_versions:
-            if recent is None or sv>recent:
-                recent=sv
-        return recent
-
-
-    def get_remote_branches(self):
-        branches=[]
-        print('Collecting information...')
-        for ref in self.repo.git.branch('-r').split('\n'):
-            sys.stdout.write('.')
-            sys.stdout.flush()
-            branches.append(ref)
-        print('\n')
-        branches=[b.strip(' ') for b in branches if b.find('HEAD')==-1]
-        branches.remove('origin/master') #Move master to position 0
-        branches=['origin/master']+branches
-        return branches
-
-# #####################################################################################################
-class RecommendedFirmware():
-    def __init__(self,use_device,installed=None,available=None):
-        self.use_device=use_device
-        self.fw_installed = InstalledFirmware(use_device) if installed is None else installed
-        self.fw_available= AvailableFirmware(use_device) if available is None else available
-        self.recommended = {}
-        self.__get_recommend_updates()
-
-    def __get_recommend_updates(self):
-        for device_name in self.use_device.keys():
-            if self.use_device[device_name]:
-                if self.fw_installed.is_device_valid(device_name): #Len 0 if device not found
-                    self.recommended[device_name]=self.fw_available.get_most_recent_version(device_name, self.fw_installed.get_supported_protocols(device_name))
-                else:
-                    self.recommended[device_name]=None
 
-    def pretty_print(self):
-        click.secho(' Recommended Firmware Updates '.center(110,'#'), fg="cyan",bold=True)
-        print('\n')
-        click.secho('%s | %s | %s | %s ' % ('DEVICE'.ljust(25), 'INSTALLED'.ljust(25), 'RECOMMENDED'.ljust(25), 'ACTION'.ljust(25)), fg="cyan", bold=True)
-        click.secho('-'*110,fg="cyan", bold=True)
-
-        for device_name in self.recommended.keys():
-            dev_out=device_name.upper().ljust(25)
-            installed_out=''.ljust(25)
-            rec_out = ''.ljust(25)
-            action_out = ''.ljust(25)
-            if not self.fw_installed.is_device_valid(device_name):
-                installed_out='No device available'.ljust(25)
-            else:
-                version = self.fw_installed.get_version(device_name)
-                installed_out=str(version).ljust(25)
-                if self.recommended[device_name]==None:
-                   rec_out='None (might be on dev branch)'.ljust(25)
-                else:
-                    rec_out=str(self.recommended[device_name]).ljust(25)
-                    if self.recommended[device_name] > version:
-                        action_out='Upgrade recommended'.ljust(25)
-                    elif self.recommended[device_name] < version:
-                        action_out='Downgrade recommended'.ljust(25)
+    def delete_yaml(self):
+        if os.path.exists(self.resume_tmp_filename):
+            os.system('rm %s'%self.resume_tmp_filename)
+
+# ########################################################################################################3
+
+    def get_port_from_user(self):
+        mapping = hdu.get_hello_ttyACMx_mapping()
+        click.secho('-------- Available Ports ------------', fg="cyan",bold=True)
+        m=[]
+        for a in mapping['ACMx']:
+            if mapping['ACMx'][a] is None:
+                print('%d | %s' % (len(m), a))
+                m.append(a)
+        dp = None
+        while dp == None:
+            id = click.prompt('Please enter desired port id', default=0)
+            if id >= 0 and id < len(mapping['ACMx']):
+                dp = m[id]
+            else:
+                click.secho('Invalid ID', fg="red")
+        return dp
+
+    def get_device_from_user(self):
+        click.secho('--------Available Devices ------------' , fg="cyan",bold=True)
+        m=['hello-motor-arm','hello-motor-left-wheel' ,'hello-motor-right-wheel' ,'hello-motor-lift','hello-wacc','hello-pimu']
+        for i in range(len(m)):
+            print('%d | %s ' % (i, m[i]))
+        dp = None
+        while dp == None:
+            id = click.prompt('Please enter desired device id', default=0)
+            if id >= 0 and id < len(m):
+                dp = m[id]
+            else:
+                click.secho('Invalid ID', fg="red")
+        return dp
+
+
+    def run(self):
+        if not self.ready_to_run:
+            click.secho('WARNING: Unable to complete firmware update...', fg="yellow", bold=True)
+            return False
+
+        self.print_upload_warning()
+
+        #self.pretty_print_state()
+        #Advance the state machine
+        if self.state['no_prompts'] or click.confirm('Proceed with update??'):
+            print('\n\n\n')
+            #Flash all devices
+            for d in self.target:
+                click.secho(' %s  '.center(110, '#') % d.upper(), fg="yellow", bold=True)
+                click.secho(' %s |  COMPILE AND FLASH FIRMWARE... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if not self.state['completed'][d]['flash']:
+                    if self.fw_installed.is_device_valid(d):
+                        nretry=3
+                        for i in range(nretry):
+                            self.state['completed'][d]['flash']=self.do_device_flash(d,self.target[d].to_string(),self.state['repo_path'],self.state['verbose'])
+                            if not self.state['completed'][d]['flash']:
+                                #It may get here if the usb bus connectoin fails during flash
+                                #Attempt to reset the device and then try again
+                                print('Retrying firmware flash for %s'%d)
+                                port=fwu.get_port_name(d)
+                                if port is not None:
+                                    hdu.place_arduino_in_bootloader('/dev/'+port)
+                            else:
+                                break
                     else:
-                        action_out = 'At most recent version'.ljust(25)
-            print('%s | %s | %s | %s ' %(dev_out,installed_out,rec_out,action_out))
+                        click.secho('WARNING: Unable to flash %s as device not valid'%d, fg="yellow", bold=True)
+                        self.state['completed'][d]['flash'] =False
 
+                    if not self.state['completed'][d]['flash']:
+                        click.secho('WARNING: Device %s did not flash firmware successfully'%d, fg="red", bold=True)
+                        click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                        click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+                        self.to_yaml()
+                        return False
 
-    def print_recommended_args(self):
-        dev_arg_map={'hello-pimu':' --pimu','hello-wacc':' --wacc','hello-motor-right-wheel':' --right_wheel',
-                     'hello-motor-left-wheel':' --left_wheel','hello-motor-lift':' --lift',
-                     'hello-motor-arm':' --arm'}
-        rec_args=''
-        for device_name in self.recommended.keys():
-            if self.fw_installed.is_device_valid(device_name):
-                version = self.fw_installed.get_version(device_name)
-                if self.recommended[device_name]!=None:
-                    if self.recommended[device_name] > version:
-                        rec_args=rec_args+dev_arg_map[device_name]
-        if len(rec_args):
-            click.secho('\nRun recommended command: \nREx_firmware_updater.py --install %s'%rec_args,fg="green", bold=True)
-        else:
-            click.secho('\nFirmware upgrade not necessary',fg="green", bold=True)
+                click.secho(' %s |   CHECK #1 IF DEVICE RETURNS TO BUS... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if  not self.state['completed'][d]['return_to_bus']:
+                    self.state['completed'][d]['return_to_bus']=self.wait_on_return_to_bus(d)
+
+                    if not self.state['completed'][d]['return_to_bus']:
+                        click.secho('WARNING: Device %s did not return to bus successfully'%d, fg="red", bold=True)
+                        click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                        click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+                        self.to_yaml()
+                        return False
 
-# #####################################################################################################
+                time.sleep(3.0) #Give a chance for devices to become ready for comms
 
-log_device=stretch_body.device.Device(req_params=False)
+                click.secho(' %s |   CHECK IF ESTABLISH COMMS... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if not self.state['completed'][d]['establish_comms']:
+                    self.state['completed'][d]['establish_comms'] = self.verify_establish_comms(d)
+
+                    if not self.state['completed'][d]['establish_comms']:
+                        click.secho('WARNING: Device %s did not establish comms successfully'%d, fg="red", bold=True)
+                        click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                        click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+                        self.to_yaml()
+                        return False
 
-def user_msg_log(msg,user_display=True,fg=None,bg=None,bold=False):
-    if user_display:
-        click.secho(str(msg),fg=fg, bg=bg,bold=bold)
-    log_device.logger.debug(str(msg))
+                click.secho('%s |  CHECK FOR CORRECT VERSION UPDATE... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if not self.state['completed'][d]['version_validate']:
+                    self.state['completed'][d]['version_validate'] = self.verify_firmware_version(d)
+                    if not self.state['completed'][d]['version_validate']: #If failed, force to try upload again
+                        self.state['completed'][d]['flash']=False
+                        self.state['completed'][d]['return_to_bus']=False
+                        self.state['completed'][d]['establish_comms'] = False
+                        click.secho('WARNING: Device %s has not updated to target firmware version'%d, fg="red", bold=True)
+                        click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                        click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+                        self.to_yaml()
+                        return False
 
-class FirmwareUpdater():
-    def __init__(self,use_device):
-        self.use_device=use_device
-        self.fw_installed = InstalledFirmware(use_device)
-        for device_name in self.use_device.keys():
-            self.use_device[device_name]=self.use_device[device_name] and self.fw_installed.is_device_valid(device_name)
-        self.fw_available= AvailableFirmware(use_device)
-        self.fw_recommended=RecommendedFirmware(use_device,self.fw_installed,self.fw_available)
-        self.target=self.fw_recommended.recommended.copy()
-
-    def startup(self):
-        #if not self.__check_ubuntu_version():
-        #    print('Firmware Updater does not work on Ubuntu 20.04 currently. Please try again in Ubuntu 18.04')
-         #   return False
-        if self.__check_arduino_cli_install():
-            self.__create_arduino_config_file()
+                click.secho('%s |  RESTORING CALIBRATION DATA... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if not self.state['completed'][d]['calibration_flash']:
+                    self.state['completed'][d]['calibration_flash'] = self.flash_stepper_calibration(d)
+
+                if not self.state['completed'][d]['calibration_flash']:
+                    click.secho('WARNING: Device %s failed on encoder calibration flash'%d, fg="red", bold=True)
+                    click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                    click.secho('WARNING: Then run: REx_firmware_udpater.py --resume', fg="red", bold=True)
+                    self.to_yaml()
+                    return False
+
+                click.secho('%s |  CHECK #2 IF RETURNED TO BUS... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
+                if  not self.state['completed'][d]['return_to_bus2']:
+                    self.state['completed'][d]['return_to_bus2']=self.wait_on_return_to_bus(d)
+
+                if not self.state['completed'][d]['return_to_bus2']:
+                    click.secho('WARNING: Device %s did not return to bus successfully'%d, fg="red", bold=True)
+                    click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
+                    click.secho('WARNING: Then run: REx_firmware_udpater.py - -resume', fg="red", bold=True)
+                    self.to_yaml()
+                    return False
+                print('\n\n\n')
+
+            print('')
+            click.secho(' CONGRATULATIONS... '.center(110, '#'), fg="cyan", bold=True)
+            for d in self.target:
+                click.secho('%s | No issues encountered. Firmware updated to %s.'%(d.upper().ljust(25),str(self.target[d])), fg="green", bold=True)
+            self.delete_yaml()
             return True
-        return False
 
-    def __create_arduino_config_file(self):
-        arduino_config = {'board_manager': {'additional_urls': []},
-                          'daemon': {'port': '50051'},
-                          'directories': {'data': os.environ['HOME'] + '/.arduino15',
-                                          'downloads': os.environ['HOME'] + '/.arduino15/staging',
-                                          'user': self.fw_available.repo_path + '/arduino'},
-                          'library': {'enable_unsafe_install': False},
-                          'logging': {'file': '', 'format': 'text', 'level': 'info'},
-                          'metrics': {'addr': ':9090', 'enabled': True},
-                          'sketch': {'always_export_binaries': False},
-                          'telemetry': {'addr': ':9090', 'enabled': True}}
-        with open(self.fw_available.repo_path + '/arduino-cli.yaml', 'w') as yaml_file:
-            yaml.dump(arduino_config, yaml_file, default_flow_style=False)
+    # ########################################################################################################3
 
-    def __check_ubuntu_version(self):
-        res = Popen('cat /etc/lsb-release | grep DISTRIB_RELEASE', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().strip(b'\n')
-        return res==b'DISTRIB_RELEASE=18.04'
-        
-    def __check_arduino_cli_install(self):
-        target_version=b'0.24.0'#0.18.3'
-        version='None'
-        res=Popen('arduino-cli version', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
-        do_install=False
-        if not(res[:11]==b'arduino-cli'):
-            do_install=True
-        else:
-            version=res[res.find(b'Version:')+9:res.find(b' Commit')]
-            if version!=target_version:
-                do_install=True
-        if do_install:
-            click.secho('WARNING:---------------------------------------------------------------------------------',fg="yellow", bold=True)
-            click.secho('WARNING: Compatible version of arduino_cli not installed. ',fg="yellow", bold=True)
-            click.secho('Requires version %s. Installed version of %s'%(target_version,version))
-            if click.confirm('Install now?'):
-                os.system('curl -fsSL https://raw.githubusercontent.com/arduino/arduino-cli/master/install.sh | BINDIR=$HOME/.local/bin/ sh -s %s'%target_version.decode('utf-8'))
-                os.system('arduino-cli config init')
-                os.system('arduino-cli core install arduino:samd@1.6.21')
-                return True
-            else:
+    def all_completed(self,state_name):
+        all_completed=True
+        for d in self.target:
+            all_completed=all_completed and self.state['completed'][d][state_name]
+        return all_completed
+
+# ########################################################################################################################
+    def do_device_flash(self, device_name, tag, repo_path=None, verbose=False, port_name=None):
+        #click.secho('-------- FIRMWARE FLASH %s | %s ------------' % (device_name, tag), fg="cyan", bold=True)
+        config_file = self.fw_available.repo_path + '/arduino-cli.yaml'
+
+        fwu.user_msg_log('Config: ' + str(config_file), user_display=verbose)
+        fwu.user_msg_log('Repo: ' + str(repo_path), user_display=verbose)
+
+        sketch_name=fwu.get_sketch_name(device_name)
+
+        if sketch_name == 'hello_stepper' and not fwu.does_stepper_have_encoder_calibration_YAML(device_name):
+            print('Encoder data has not been stored for %s and may be lost. Aborting firmware flash.' % device_name)
+            return False
+
+        if port_name is None:
+            print('Looking for device %s on bus' % device_name)
+            if not fwu.wait_on_device(device_name, timeout=5.0):
+                print('Failure: Device not on bus.')
                 return False
-        return True
+            port_name = fwu.get_port_name(device_name)
 
-    def pretty_print_target(self):
-        click.secho(' UPDATING FIRMWARE TO... '.center(110,'#'), fg="cyan", bold=True)
-        for device_name in self.target.keys():
-            if self.use_device[device_name]:
-                if not self.fw_installed.is_device_valid(device_name):
-                    print('%s | No target available' % device_name.upper().ljust(25))
-                else:
-                    v_curr=self.fw_installed.get_version(device_name)
-                    v_targ=self.target[device_name]
-                    if v_targ is None:
-                        rec = 'No target available'
-                    elif v_curr > v_targ:
-                        rec = 'Downgrading to %s' % self.target[device_name]
-                    elif v_curr<v_targ:
-                        rec = 'Upgrading to %s' % self.target[device_name]
-                    else:
-                        rec = 'Reinstalling %s' % self.target[device_name]
-                    print('%s | %s ' % (device_name.upper().ljust(25), rec.ljust(40)))
+        fwu.user_msg_log('Device: %s Port: %s' % (device_name, port_name), user_display=verbose)
 
-    def print_upload_warning(self):
-        click.secho('------------------------------------------------', fg="yellow", bold=True)
-        click.secho('WARNING: (1) Updating robot firmware should only be done by experienced users', fg="yellow", bold=True)
-        click.secho('WARNING: (2) Do not have other robot processes running during update', fg="yellow", bold=True)
-        click.secho('WARNING: (3) Leave robot powered on during update', fg="yellow", bold=True)
-        if self.use_device['hello-motor-lift']:
-            click.secho('WARNING: (4) Ensure Lift has support clamp in place', fg="yellow", bold=True)
-            click.secho('WARNING: (5) Lift may make a loud noise during programming. This is normal.', fg="yellow", bold=True)
-        click.secho('------------------------------------------------', fg="yellow", bold=True)
+        if port_name is not None and sketch_name is not None:
+            print('Starting programming. This will take about 5s...')
+            if repo_path is None:
+                os.chdir(self.fw_available.repo_path)
+                cmd='git checkout ' + tag + '>/dev/null 2>&1'
+                os.system(cmd)
+                if verbose:
+                    print('Ran: %s from %s'%(cmd,self.fw_available.repo_path))
+                src_path = self.fw_available.repo_path
+            else:
+                src_path = repo_path
 
+            compile_command = 'arduino-cli compile --config-file %s --fqbn hello-robot:samd:%s %s/arduino/%s' % (
+            config_file, sketch_name, src_path, sketch_name)
+            fwu.user_msg_log(compile_command, user_display=verbose)
+            c = Popen(shlex.split(compile_command), shell=False, bufsize=64, stdin=PIPE, stdout=PIPE,
+                      close_fds=True).stdout.read().strip()
+            if type(c) == bytes:
+                c = c.decode("utf-8")
+            cc = c.split('\n')
+            fwu.user_msg_log(c, user_display=verbose)
 
-    def do_update(self,no_prompts=False,repo_path=None,verbose=False):
-        # Return True if system was upgraded
-        # Return False if system was not upgraded / error happened
-        self.num_update=0
+            # In version 0.18.x the last line after compile is: Sketch uses xxx bytes (58%) of program storage space. Maximum is yyy bytes.
+            # In version 0.24.x +this is now on line 0.
+            # Need a more robust way to determine successful compile. Works for now.
+            success = (str(cc[0]).find('Sketch uses') != -1)
+            if not success:
+                print('Firmware failed to compile %s at %s' % (sketch_name, src_path))
+                return False
+            else:
+                print('Success in firmware compile')
 
-        #Count how many updates doing
-        for device_name in self.target.keys():
-            if self.fw_installed.is_device_valid(device_name) and self.target[device_name] is not None:
-                self.num_update=self.num_update+1
+            upload_command = 'arduino-cli upload  --config-file %s -p /dev/%s --fqbn hello-robot:samd:%s %s/arduino/%s' % (
+            config_file, port_name, sketch_name, src_path, sketch_name)
 
-        self.pretty_print_target()
+            fwu.user_msg_log(upload_command, user_display=verbose)
+            u = Popen(shlex.split(upload_command), shell=False, bufsize=64, stdin=PIPE, stdout=PIPE,
+                      close_fds=True).stdout.read().strip()
+
+            if type(u) == bytes:
+                u = u.decode('utf-8')
+            uu = u.split('\n')
+            fwu.user_msg_log(u, user_display=False)
+            if verbose:
+                print(upload_command)
+                # Pretty print the result
+                for l in uu:
+                    k = l.split('\r')
+                    if len(k) == 1:
+                        print(k[0])
+                    else:
+                        for m in k:
+                            print(m)
+            success = uu[-1] == 'CPU reset.'
+
+            if not success:
+                print('Firmware flash. Failed to upload to %s' % (port_name))
+                return False
+            else:
+                click.secho('Success in firmware flash' , fg="green")
+                return True
+        else:
+            print('Firmware update %s. Failed to find device %s' % (tag, device_name))
+            return False
 
-        if not self.num_update:
-            click.secho('System is up to date. No updates to be done', fg="yellow",bold=True)
+# ########################################################################################################3
+    def wait_on_return_to_bus(self,device_name):
+        click.secho('Checking that device %s returned to bus '%device_name)
+        print('It may take several minutes to appear on the USB bus.' )
+        ts = time.time()
+        found = False
+        ntry=30
+        for i in range(ntry):
+            if not fwu.wait_on_device(device_name, timeout=10.0):
+                print('Trying again: %d of %d\n' % (i,ntry))
+                # Bit of a hack.Sometimes after a firmware flash the device
+                # Doesn't fully present on the USB bus with a serial No for Udev to find
+                # In does present as an 'Arduino Zero' product. This will attempt to reset it
+                # and re-present to the bus
+                # time.sleep(1.0)
+                # os.system('usbreset \"Arduino Zero\"')
+                # time.sleep(1.0)
+                # print('')
+            else:
+                found = True
+                break
+        if not found:
+            click.secho('Device %s failed to return to bus after %f seconds.' % (device_name, time.time() - ts),fg="yellow", bold=True)
             return False
-        self.print_upload_warning()
-        self.fw_updated={}
-        if no_prompts or click.confirm('Proceed with update??'):
-            for device_name in self.target.keys():
-                self.fw_updated[device_name]=False
-                if self.target[device_name] is not None:
-                    self.fw_updated[device_name]=self.flash_firmware_update(device_name,self.target[device_name].to_string(),repo_path=repo_path,verbose=verbose)
-                    if not self.fw_updated[device_name]:
-                        return False
-            click.secho('---- Firmware Update Complete!', fg="cyan",bold=True)
-            success=self.post_firmware_update()
-            return success
+        else:
+            click.secho('Device %s returned to bus after %f seconds.' % (device_name, time.time() - ts),fg="green", bold=True)
+        return True
+# ########################################################################################################3
+    def verify_firmware_version(self,device_name):
+        fw_installed = FirmwareInstalled({device_name: True})  # Pull the currently installed system from fw
+        if not fw_installed.is_device_valid(device_name):  # Device may not have come back on bus
+            print('%s | No device available' % device_name.upper().ljust(25))
+            print('')
+            return False
+        else:
+            #click.secho(' Confirming Firmware Updates '.center(110, '#'), fg="cyan", bold=True)
+            v_curr = fw_installed.get_version(device_name)  # Version that is now on the board
+            if v_curr == self.target[device_name]:
+                click.secho('PASS: %s | Installed %s | Target %s ' % (device_name.upper().ljust(25), v_curr.to_string().ljust(40),self.target[device_name].to_string().ljust(40)), fg="green")
+                return True
+            else:
+                click.secho('FAIL: %s | Installed %s | Target %s ' % (device_name.upper().ljust(25), v_curr.to_string().ljust(40), self.target[device_name].to_string().ljust(40)),fg="red")
+        return False
+
+    def verify_establish_comms(self,device_name):
+        if device_name == 'hello-wacc':
+            dd = stretch_body.wacc.Wacc()
+        elif device_name == 'hello-pimu':
+            dd = stretch_body.pimu.Pimu()
+        else:
+            dd = stretch_body.stepper.Stepper('/dev/' + device_name)
+        if not dd.startup():
+            click.secho('FAIL: Unable to establish comms with device %s' % device_name.upper(), fg="red")
+            return False
+        click.secho('PASS: Established comms with device %s ' % device_name.upper(),fg="green")
+        return True
+# ########################################################################################################3
+    def flash_stepper_calibration(self, device_name):
+        if device_name == 'hello-motor-arm' or device_name == 'hello-motor-lift' or device_name == 'hello-motor-right-wheel' or device_name == 'hello-motor-left-wheel':
+            #click.secho(' Flashing Stepper Calibration: %s '.center(70, '#') % device_name, fg="cyan", bold=True)
+            if not fwu.wait_on_device(device_name):
+                click.secho('Device %s failed to return to bus.' % device_name, fg="red", bold=True)
+                return False
+            #time.sleep(1.0)
+            motor = stretch_body.stepper.Stepper('/dev/' + device_name)
+            motor.startup()
+            if not motor.hw_valid:
+                click.secho('Failed to startup stepper %s' % device_name, fg="red", bold=True)
+                return False
+            else:
+                print('Writing gains to flash...')
+                motor.write_gains_to_flash()
+                motor.push_command()
+                print('Gains written to flash')
+                print('')
+                print('Reading calibration data from YAML...')
+                data = motor.read_encoder_calibration_from_YAML()
+                print('Writing calibration data to flash...')
+                motor.write_encoder_calibration_to_flash(data)
+
+                print('Successful write of FLASH.')
+                fwu.wait_on_device(device_name)
+                motor.board_reset()
+                motor.push_command()
+                motor.transport.ser.close()
+                time.sleep(2.0) #Give time to return to bus
+                return True
+        click.secho('Successful flash of device calibration',fg="green")
         return True
+# ########################################################################################################3
 
-    def do_update_to(self,verbose=False, no_prompts=False):
+    def set_target_from_install_version(self):
         # Return True if system was upgraded
-        # Return False if system was not upgraded / error happened
-        click.secho(' Select target firmware versions '.center(60,'#'), fg="cyan", bold=True)
+        # Return False if systvt = None
+        #                     while vt == None:
+        #                         id = click.prompt('Please enter desired version id [Recommended]', default=default_id)
+        #                         if id >= 0 and id < len(vs):
+        #                             vt = vs[id]
+        #                         else:
+        #                             click.secho('Invalid ID', fg="red")
+        #                     print('Selected version %s for device %s' % (vt, device_name))em was not upgraded / error happened
+        click.secho(' Select target firmware versions '.center(60, '#'), fg="cyan", bold=True)
         for device_name in self.fw_recommended.recommended.keys():
-            if self.use_device[device_name]:
-                vs=self.fw_available.versions[device_name]
+            if self.state['use_device'][device_name]:
+                vs = self.fw_available.versions[device_name]
                 if len(vs) and self.fw_recommended.recommended[device_name] is not None:
                     print('')
-                    click.secho('---------- %s [%s]-----------'%(device_name.upper(),str(self.fw_installed.get_version(device_name))), fg="blue", bold=True)
-                    default_id=0
+                    click.secho('---------- %s [%s]-----------' % (
+                    device_name.upper(), str(self.fw_installed.get_version(device_name))), fg="blue", bold=True)
+                    default_id = 0
                     for i in range(len(vs)):
-                        if vs[i]==self.fw_recommended.recommended[device_name]:
-                            default_id=i
-                        print('%d: %s'%(i,vs[i]))
+                        if vs[i] == self.fw_recommended.recommended[device_name]:
+                            default_id = i
+                        print('%d: %s' % (i, vs[i]))
                     print('----------------------')
-                    vt=None
-                    while vt==None:
-                        id = click.prompt('Please enter desired version id [Recommended]', default=default_id)
-                        if id>=0 and id<len(vs):
-                            vt=vs[id]
-                        else:
-                            click.secho('Invalid ID', fg="red" )
-                    print('Selected version %s for device %s'%(vt,device_name))
-                    self.target[device_name]=vt
+
+                    self.target[device_name] = vt
         print('')
         print('')
-        return self.do_update(verbose=verbose, no_prompts=no_prompts)
+        return True
 
-    def do_update_to_path(self,path_name,verbose=False, no_prompts=False):
+    def set_target_from_install_path(self, path_name):
         # Burn the Head of the branch to each board regardless of what is currently installed
         click.secho('>>> Flashing firmware from path %s ' % path_name, fg="cyan", bold=True)
         # Check that version of target path is compatible
-        for device_name in self.target.keys():
-            if self.use_device[device_name]:
-                sketch_name = self.get_sketch_name(device_name)
+        for device_name in self.target:
+            if self.state['use_device'][device_name]:
+                sketch_name = fwu.get_sketch_name(device_name)
                 target_version = self.get_firmware_version_from_path(sketch_name, path_name)
                 if target_version is None:
                     return False
                 self.target[device_name] = target_version
                 path_protocol = 'p' + str(target_version.protocol)
                 if not self.fw_installed.is_protocol_supported(device_name, path_protocol):
                     click.secho('---------------------------', fg="yellow")
-                    click.secho('Target firmware path of %s is incompatible with installed Stretch Body for device %s' % (path_name, device_name), fg="yellow")
-                    x = " , ".join(["{}"] * len(self.fw_installed.get_supported_protocols(device_name))).format(*self.fw_installed.get_supported_protocols(device_name))
+                    click.secho(
+                        'Target firmware path of %s is incompatible with installed Stretch Body for device %s' % (
+                        path_name, device_name), fg="yellow")
+                    x = " , ".join(["{}"] * len(self.fw_installed.get_supported_protocols(device_name))).format(
+                        *self.fw_installed.get_supported_protocols(device_name))
                     click.secho('Installed Stretch Body supports protocols %s' % x, fg="yellow")
                     click.secho('Target path supports protocol %s' % path_protocol, fg="yellow")
                     if path_protocol > self.fw_installed.max_protocol_supported(device_name):
                         click.secho('Upgrade Stretch Body first...', fg="yellow")
                     else:
                         click.secho('Downgrade Stretch Body first...', fg="yellow")
                     return False
-        repo_path=path_name[:path_name.rfind('arduino')]
-        return self.do_update(repo_path=repo_path,verbose=verbose,no_prompts=no_prompts)
+        self.state['repo_path']=path_name[:path_name.rfind('arduino')]
+        return True
 
-    def do_update_to_branch(self,verbose=False, no_prompts=False):
+    def set_target_from_install_branch(self,):
         # Return True if system was upgraded
         # Return False if system was not upgraded / error happened
-        click.secho(' Select target branch '.center(60,'#'), fg="cyan", bold=True)
-        branches=self.fw_available.get_remote_branches()
+        click.secho(' Select target branch '.center(60, '#'), fg="cyan", bold=True)
+        branches = self.fw_available.get_remote_branches()
         for id in range(len(branches)):
             print('%d: %s' % (id, branches[id]))
         print('')
-        branch_name=None
+        branch_name = None
         while branch_name == None:
             try:
-                id = click.prompt('Please enter desired branch id',default=0)
+                id = click.prompt('Please enter desired branch id', default=0)
             except click.exceptions.Abort:
                 return False
             if id >= 0 and id < len(branches):
-                branch_name=branches[id]
+                branch_name = branches[id]
             else:
                 click.secho('Invalid ID', fg="red")
-        print('Selected branch %s'%branch_name )
-        #Check that version of target branch is compatible
-        for device_name in self.target.keys():
-            if self.use_device[device_name]:
-                sketch_name=self.get_sketch_name(device_name)
-                target_version=self.get_firmware_version_from_git(sketch_name, branch_name)
-                self.target[device_name]=target_version
-                git_protocol = 'p'+str(target_version.protocol)
-                if not self.fw_installed.is_protocol_supported(device_name,git_protocol):
+        print('Selected branch %s' % branch_name)
+        self.state['install_branch']=branch_name
+        # Check that version of target branch is compatible
+        for device_name in self.target:
+            if self.state['use_device'][device_name]:
+                sketch_name = fwu.get_sketch_name(device_name)
+                target_version = self.get_firmware_version_from_git(sketch_name, branch_name)
+                self.target[device_name] = target_version
+                git_protocol = 'p' + str(target_version.protocol)
+                if not self.fw_installed.is_protocol_supported(device_name, git_protocol):
                     click.secho('---------------------------', fg="yellow")
-                    click.secho('Target firmware branch of %s is incompatible with installed Stretch Body for device %s'%(branch_name,device_name),fg="yellow")
-                    x = " , ".join(["{}"] * len(self.fw_installed.get_supported_protocols(device_name))).format(*self.fw_installed.get_supported_protocols(device_name))
-                    click.secho('Installed Stretch Body supports protocols %s'%x,fg="yellow")
-                    click.secho('Target branch supports protocol %s'%git_protocol,fg="yellow")
-                    if git_protocol>self.fw_installed.max_protocol_supported(device_name):
-                        click.secho('Upgrade Stretch Body first...',fg="yellow")
+                    click.secho(
+                        'Target firmware branch of %s is incompatible with installed Stretch Body for device %s' % (
+                        branch_name, device_name), fg="yellow")
+                    x = " , ".join(["{}"] * len(self.fw_installed.get_supported_protocols(device_name))).format(
+                        *self.fw_installed.get_supported_protocols(device_name))
+                    click.secho('Installed Stretch Body supports protocols %s' % x, fg="yellow")
+                    click.secho('Target branch supports protocol %s' % git_protocol, fg="yellow")
+                    if git_protocol > self.fw_installed.max_protocol_supported(device_name):
+                        click.secho('Upgrade Stretch Body first...', fg="yellow")
                     else:
-                        click.secho('Downgrade Stretch Body first...',fg="yellow")
+                        click.secho('Downgrade Stretch Body first...', fg="yellow")
                     return False
-        return self.do_update(verbose=verbose,no_prompts=no_prompts)
+        return True
 
 
-    def flash_stepper_calibration(self,device_name):
-        if device_name == 'hello-motor-arm' or device_name == 'hello-motor-lift' or device_name == 'hello-motor-right-wheel' or device_name == 'hello-motor-left-wheel':
-                click.secho(' Flashing Stepper Calibration: %s '.center(110,'#') % device_name, fg="cyan",bold=True)
-                if not self.wait_on_device(device_name):
-                    click.secho('Device %s failed to return to bus' % device_name, fg="red",bold=True)
-                    return False
-                time.sleep(1.0)
-                motor = stretch_body.stepper.Stepper('/dev/' + device_name)
-                motor.startup()
-                if not motor.hw_valid:
-                    click.secho('Failed to startup stepper %s' % device_name, fg="red", bold=True)
-                    return False
-                else:
-                    print('Writing gains to flash...')
-                    motor.write_gains_to_flash()
-                    motor.push_command()
-                    print('Gains written to flash')
-                    print('')
-                    print('Reading calibration data from YAML...')
-                    data = motor.read_encoder_calibration_from_YAML()
-                    print('Writing calibration data to flash...')
-                    motor.write_encoder_calibration_to_flash(data)
-                    print('Successful write of FLASH.')
-                    self.wait_on_device(device_name)
-                    motor.board_reset()
-                    motor.push_command()
-                    motor.transport.ser.close()
-                    time.sleep(2.0)
-                    self.wait_on_device(device_name)
-                    print('Successful return of device to bus.')
-        return True
+# ########################################################################################################################
 
 
+# ########################################################################################################################
+#     def foo(self):
+#         all_success = all_success and self.verify_firmware_version(device_name)
+#         print('')
+#         print('')
+#                 # NOTE: Move to exceptions and single device flow, can track where in the flow it fails.
+#                 self.post_firmware_update(device_name)
+#
+#                 if len(no_return):
+#                     click.secho('Devices did not return to bus. Power cycle robot', fg="yellow", bold=True)
+#                     click.secho('Then run stretch_robot_system_check.py to confirm all devices present', fg="yellow",
+#                                 bold=True)
+#                     for device_name in no_stepper_return:
+#                         click.secho(
+#                             'Device %s requires calibration data to be written after power cycle.' % device_name,
+#                             fg="yellow", bold=True)
+#                         click.secho('After power cycle run: REx_stepper_calibration_YAML_to_flash.py %s' % device_name,
+#                                     fg="yellow", bold=True)
+#                     return False
+#
+#                 return all_success
+#         return True
 
 
-    def post_firmware_update(self):
-        #Return True if no errors
-        click.secho(' Performing Post Firmware Updates '.center(110, '#'), fg="cyan", bold=True)
-        StretchDeviceMgmt.reset_all_arduino()
-        s = StretchDeviceMgmt()
-        s.reset_all()
-        time.sleep(2.0)
-        flash_stepper_calibration_success={}
-        for device_name in self.target.keys():
-            if self.fw_updated[device_name]:
-                flash_stepper_calibration_success[device_name]=self.flash_stepper_calibration(device_name)
-                time.sleep(2.0)  # Give time to get back on bus
-                #s = StretchDeviceMgmt([device_name])
-                #s.reset_all()
-                # StretchDeviceMgmt.reset_all_arduino()
-                # if not self.wait_on_device(device_name):
-                #     print('Failed to return to bus')
-                #     return False
-        print('')
-        click.secho(' Confirming Firmware Updates '.center(110,'#'), fg="cyan", bold=True)
-        self.fw_installed = InstalledFirmware(self.use_device) #Pull the currently installed system from fw
-        n_failure=0
-        for device_name in self.target.keys():
-            if self.use_device[device_name]:
-                if not self.fw_installed.is_device_valid(device_name): #Device may not have come back on bus
-                    print('%s | No device available' % device_name.upper().ljust(25))
-                    n_failure=n_failure+1
+
+
+    def create_arduino_config_file(self):
+        arduino_config = {'board_manager': {'additional_urls': []},
+                          'daemon': {'port': '50051'},
+                          'directories': {'data': os.environ['HOME'] + '/.arduino15',
+                                          'downloads': os.environ['HOME'] + '/.arduino15/staging',
+                                          'user': self.fw_available.repo_path + '/arduino'},
+                          'library': {'enable_unsafe_install': False},
+                          'logging': {'file': '', 'format': 'text', 'level': 'info'},
+                          'metrics': {'addr': ':9090', 'enabled': True},
+                          'sketch': {'always_export_binaries': False},
+                          'telemetry': {'addr': ':9090', 'enabled': True}}
+        with open(self.fw_available.repo_path + '/arduino-cli.yaml', 'w') as yaml_file:
+            yaml.dump(arduino_config, yaml_file, default_flow_style=False)
+
+    def pretty_print_target(self):
+        click.secho(' UPDATING FIRMWARE TO... '.center(110, '#'), fg="cyan", bold=True)
+        for device_name in self.target:
+            if self.state['use_device'][device_name]:
+                if not self.fw_installed.is_device_valid(device_name):
+                    print('%s | No target available' % device_name.upper().ljust(25))
                 else:
-                    v_curr =self.fw_installed.get_version(device_name)  # Version that is now on the board
-                    if v_curr ==  self.target[device_name]:
-                        click.secho('%s | %s ' % (device_name.upper().ljust(25), 'Installed firmware matches target'.ljust(40)),fg="green")
+                    v_curr = self.fw_installed.get_version(device_name)
+                    v_targ = self.target[device_name]
+                    if v_targ is None:
+                        rec = 'No target available'
+                    elif v_curr > v_targ:
+                        rec = 'Downgrading to %s' % self.target[device_name]
+                    elif v_curr < v_targ:
+                        rec = 'Upgrading to %s' % self.target[device_name]
                     else:
-                        click.secho('%s | %s ' % (device_name.upper().ljust(25), 'Firmware update failure!!'.ljust(40)),fg="red", bold=True)
-                        n_failure=n_failure+1
-                    if not flash_stepper_calibration_success[device_name]:
-                        n_failure = n_failure + 1
-                        click.secho('%s | %s ' % (device_name.upper().ljust(25), 'Stepper calibration flash failure!!'.ljust(40)),fg="red", bold=True)
-                        click.secho('To manually restore stepper calibration, after power-cycling robot run ', fg="red",bold=True)
-                        click.secho('REx_stepper_calibration_YAML_to_flash.py %s' % device_name)
-        if n_failure !=0:
-            click.secho('#'*110,fg="red", bold=True)
-            click.secho('Firmware update reported %d failures.\nTo remedy failures power down and the power up the robot and try again.'%n_failure,fg="red", bold=True)
-            return False
-        return True
+                        rec = 'Reinstalling %s' % self.target[device_name]
+                    print('%s | %s ' % (device_name.upper().ljust(25), rec.ljust(40)))
+        print('')
+
+    def print_upload_warning(self):
+        click.secho('------------------------------------------------', fg="yellow", bold=True)
+        click.secho('WARNING: (1) Updating robot firmware should only be done by experienced users', fg="yellow",
+                    bold=True)
+        click.secho('WARNING: (2) Do not have other robot processes running during update', fg="yellow", bold=True)
+        click.secho('WARNING: (3) Leave robot powered on during update', fg="yellow", bold=True)
+        if self.state['use_device']['hello-motor-lift']:
+            click.secho('WARNING: (4) Ensure Lift has support clamp in place', fg="yellow", bold=True)
+            click.secho('WARNING: (5) Lift may make a loud noise during programming. This is normal.', fg="yellow",
+                        bold=True)
+        click.secho('------------------------------------------------', fg="yellow", bold=True)
+
+
+
+
+
+
+
 
     def get_firmware_version_from_path(self,sketch_name,path):
         file_path = path+'/'+sketch_name+'/Common.h'
         try:
             f=open(file_path,'r')
         except IOError:
             click.secho('Invalid path provided. Path should should have sketch directories under it',fg="red", bold=True)
@@ -659,160 +709,7 @@
         lines=f.readlines()
         for l in lines:
             if l.find('FIRMWARE_VERSION')>=0:
                 version=l[l.find('"')+1:-2] #Format of: '#define FIRMWARE_VERSION "Wacc.v0.0.1p1"\n'
                 return FirmwareVersion(version)
         return None
 
-    def get_sketch_name(self,device_name):
-        if device_name=='hello-motor-left-wheel' or device_name=='hello-motor-right-wheel' or device_name=='hello-motor-arm' or device_name=='hello-motor-lift':
-            return 'hello_stepper'
-        if device_name == 'hello-wacc':
-            return 'hello_wacc'
-        if device_name == 'hello-pimu':
-            return 'hello_pimu'
-
-    def exec_process(self,cmdline, silent, input=None, **kwargs):
-        """Execute a subprocess and returns the returncode, stdout buffer and stderr buffer.
-           Optionally prints stdout and stderr while running."""
-        try:
-            sub = Popen(cmdline, stdin=PIPE, stdout=PIPE, stderr=PIPE,
-                                   **kwargs)
-            stdout, stderr = sub.communicate(input=input)
-            returncode = sub.returncode
-            if not silent:
-                sys.stdout.write(stdout.decode('utf-8'))
-                sys.stderr.write(stderr.decode('utf-8'))
-        except OSError as e:
-            if e.errno == 2:
-                raise RuntimeError('"%s" is not present on this system' % cmdline[0])
-            else:
-                raise
-        if returncode != 0:
-            raise RuntimeError('Got return value %d while executing "%s", stderr output was:\n%s' % (
-            returncode, " ".join(cmdline), stderr.rstrip(b"\n")))
-        return stdout
-
-    # ###################################
-    def is_device_present(self,device_name):
-        try:
-            self.exec_process(['ls', '/dev/'+device_name], True)
-            return True
-        except RuntimeError as e:
-            return False
-
-    def wait_on_device(self,device_name,timeout=10.0):
-        #Wait for device to appear on bus for timeout seconds
-        print('Waiting for device %s to return to bus.'%device_name)
-        ts=time.time()
-        itr=0
-        while(time.time()-ts<timeout):
-            if self.is_device_present(device_name):
-                return True
-            itr=itr+1
-            if itr % 5 == 0:
-                sys.stdout.write('.')
-                sys.stdout.flush()
-            time.sleep(0.1)
-        return False
-
-    def get_port_name(self, device_name):
-        try:
-            port_name = Popen("ls -l /dev/" + device_name, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().strip().split()[-1]
-            if not type(port_name)==str:
-                port_name=port_name.decode('utf-8')
-            return port_name
-        except IndexError:
-            return None
-
-    def does_stepper_have_encoder_calibration_YAML(self,device_name):
-        d=stretch_body.device.Device(req_params=False)
-        sn = d.robot_params[device_name]['serial_no']
-        fn = 'calibration_steppers/' + device_name + '_' + sn + '.yaml'
-        enc_data = stretch_body.hello_utils.read_fleet_yaml(fn)
-        return len(enc_data)!=0
-
-    def flash_firmware_update(self,device_name, tag,repo_path=None,verbose=False):
-        click.secho('-------- FIRMWARE FLASH %s | %s ------------'%(device_name,tag), fg="cyan", bold=True)
-        config_file = self.fw_available.repo_path + '/arduino-cli.yaml'
-
-        user_msg_log('Config: '+str(config_file), user_display=verbose)
-        user_msg_log('Repo: '+str(repo_path), user_display=verbose)
-
-        sketch_name=None
-        if device_name == 'hello-motor-left-wheel' or device_name == 'hello-motor-right-wheel' or device_name == 'hello-motor-arm' or device_name == 'hello-motor-lift':
-            sketch_name = 'hello_stepper'
-        if device_name == 'hello-wacc':
-            sketch_name = 'hello_wacc'
-        if device_name == 'hello-pimu':
-            sketch_name = 'hello_pimu'
-
-        if sketch_name=='hello_stepper' and not self.does_stepper_have_encoder_calibration_YAML(device_name):
-            print('Encoder data has not been stored for %s and may be lost. Aborting firmware flash.'%device_name)
-            return False
-        #s = StretchDeviceMgmt([device_name])
-        #if not s.reset(device_name):
-        #    return False
-        print('Looking for device %s on bus' % device_name)
-        if not self.wait_on_device(device_name, timeout=5.0):
-            print('Failure: Device not on bus.')
-            return False
-        port_name = self.get_port_name(device_name)
-        if port_name is not None and sketch_name is not None:
-
-            print('Starting programming. This will take about 5s...')
-            if repo_path is None:
-                os.chdir(self.fw_available.repo_path)
-                os.system('git checkout '+tag+'>/dev/null 2>&1')
-                src_path=self.fw_available.repo_path
-            else:
-                src_path=repo_path
-
-            compile_command = 'arduino-cli compile --config-file %s --fqbn hello-robot:samd:%s %s/arduino/%s'%(config_file,sketch_name,src_path,sketch_name)
-            user_msg_log(compile_command,user_display=verbose)
-            c=Popen(compile_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
-            cc = c.split(b'\n')
-            user_msg_log(c, user_display=verbose)
-
-            # In version 0.18.x the last line after compile is: Sketch uses xxx bytes (58%) of program storage space. Maximum is yyy bytes.
-            #In version 0.24.x this is now on line 0.
-            #Need a more robust way to determine successful compile. Works for now.
-            success=str(cc[0]).find('Sketch uses')!=-1
-            if not success:
-                print('Firmware failed to compile %s at %s' % (sketch_name,src_path))
-                return False
-            else:
-                print('Success in firmware compile')
-
-            upload_command = 'arduino-cli upload  --config-file %s -p /dev/%s --fqbn hello-robot:samd:%s %s/arduino/%s' % (config_file, port_name, sketch_name, src_path,sketch_name)
-            user_msg_log(upload_command,user_display=verbose)
-            u = Popen(upload_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
-            uu = u.split(b'\n')
-            user_msg_log(u, user_display=False)
-            if verbose:
-                print(upload_command)
-                # Pretty print the result
-                for l in uu:
-                    k = l.split(b'\r')
-                    if len(k) == 1:
-                        print(k[0].decode('utf-8'))
-                    else:
-                        for m in k:
-                            print(m.decode('utf-8'))
-
-            success = uu[-1] == b'CPU reset.'
-            if not success:
-                print('Firmware flash. Failed to upload to %s' % (port_name))
-                return False
-            else:
-                print('Success in firmware flash.')
-                #Give time to get back on bus
-                time.sleep(3.0)
-                s = StretchDeviceMgmt.reset_all_arduino()
-
-                if not self.wait_on_device(device_name):
-                    click.secho('Device %s failed to return to bus' % device_name, fg="red",bold=True)
-                    return False
-                return True
-        else:
-            print('Firmware update %s. Failed to find device %s'%(tag,device_name))
-            return False
```

### Comparing `hello_robot_stretch_factory-0.3.9/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.0/stretch_factory/hello_device_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import time
 import requests
 import os
 from subprocess import Popen, PIPE
 import fcntl
 import subprocess
 import sys
-
+import glob
 from subprocess import Popen, PIPE
 import usb.core
 import stretch_body.hello_utils as hello_utils
 import stretch_body.robot_params
 import stretch_body.device
 
+import serial
+from colorama import Fore, Style
+
+
 # ###################################
 class stream_tee(object):
     # Based on https://gist.github.com/327585 by Anand Kunal
     # http://www.tentech.ca/2011/05/stream-tee-in-python-saving-stdout-to-file-while-keeping-the-console-alive/
     def __init__(self, stream1, stream2):
         self.stream1 = stream1
         self.stream2 = stream2
@@ -34,41 +38,48 @@
         # Emit method call to the log copy
         callable2 = getattr(self.stream2, self.__missing_method_name)
         callable2(*args, **kwargs)
 
         # Emit method call to stdout (stream 1)
         callable1 = getattr(self.stream1, self.__missing_method_name)
         return callable1(*args, **kwargs)
+
+
 # ###################################
 def check_internet():
     url = "http://github.com"
     timeout = 10
     for i in range(10):
-        print('Attempting to reach internet. Try %d of 10'%(i+1))
+        print('Attempting to reach internet. Try %d of 10' % (i + 1))
         try:
             requests.get(url, timeout=timeout)
             print("Connected to the GitHub")
-            return {'success':1}
+            return {'success': 1}
         except (requests.ConnectionError, requests.Timeout) as exception:
             print("Failed to establish internet connection.")
             time.sleep(0.5)
-    return {'success':0}
+    return {'success': 0}
+
+
 # ###################################
 def check_arduino_cli_install():
     """
     Return true if the arduino-cli is available
     """
-    res=Popen('arduino-cli version', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()[:11]
-    if not(res==b'arduino-cli'):
+    res = Popen('arduino-cli version', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()[
+          :11]
+    if not (res == b'arduino-cli'):
         print('WARNING:---------------------------------------------------------------------------------')
         print('WARNING: Tool arduino_cli not installed. See stretch_install_dev.sh (Stretch Install repo)')
         print('WARNING:---------------------------------------------------------------------------------')
         print('')
         return False
     return True
+
+
 # ###################################
 def exec_process(cmdline, silent, input=None, **kwargs):
     """Execute a subprocess and returns the returncode, stdout buffer and stderr buffer.
        Optionally prints stdout and stderr while running."""
     try:
         sub = subprocess.Popen(cmdline, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, **kwargs)
         stdout, stderr = sub.communicate(input=input)
@@ -78,125 +89,211 @@
             sys.stderr.write(stderr.decode('utf-8'))
     except OSError as e:
         if e.errno == 2:
             raise RuntimeError('"%s" is not present on this system' % cmdline[0])
         else:
             raise
     if returncode != 0:
-        raise RuntimeError('Got return value %d while executing "%s", stderr output was:\n%s' % (returncode, " ".join(cmdline), stderr.rstrip(b"\n")))
+        raise RuntimeError('Got return value %d while executing "%s", stderr output was:\n%s' % (
+        returncode, " ".join(cmdline), stderr.rstrip(b"\n")))
     return stdout
 
+
 # ###################################
+def get_device_ttyACMx(device):
+    # Return the ACMx of a symlinked device, eg 'ttyACM0' given /dev/hello-motor-arm
+    try:
+        ACMx = Popen("ls -l %s" % device, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,
+                     close_fds=True).stdout.read().strip().split()[-1]
+        ACMx = ACMx.decode("utf-8")
+        return ACMx
+    except IndexError:
+        return None
+
+
+def get_all_ttyACMx():
+    # Return list of ACMx names eg ['ttyACM0','ttyACM1']
+    ACMx_all = Popen("ls -l /dev/ttyACM*", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,
+                     close_fds=True).stdout.read().strip().split()
+    ret = []
+    for line in ACMx_all:
+        l = line.decode("utf-8")
+        if l.find('ttyACM') != -1:
+            ret.append(l[5:])
+    return ret
+
+def get_hello_ttyACMx_mapping():
+    mapping={}
+    mapping['hello'] = {'hello-motor-arm': None, 'hello-motor-right-wheel': None, 'hello-motor-left-wheel': None,'hello-pimu': None, 'hello-wacc': None, 'hello-motor-lift': None}
+    mapping['missing']=[]
+    mapping['ACMx']={}
+
+    for d in mapping['hello']:
+        x = get_device_ttyACMx('/dev/'+d)
+        if x is not None:
+            mapping['hello'][d] = x
+        else:
+            mapping['missing'].append(d)
+
+    att = get_all_ttyACMx()
+    for a in att:
+        mapping['ACMx'][a]=None
+        for h in mapping['hello']:
+            if mapping['hello'][h]==a:
+                mapping['ACMx'][a]=h
+    return mapping
+
 def is_device_present(device):
     try:
-        exec_process(['ls',device],True)
+        exec_process(['ls', device], True)
         return True
     except RuntimeError as e:
         return False
 
+
 def find_steppers_on_bus():
-    s=[]
-    device_names=['/dev/hello-motor-arm', '/dev/hello-motor-lift', '/dev/hello-motor-right-wheel', '/dev/hello-motor-left-wheel']
+    s = []
+    device_names = ['/dev/hello-motor-arm', '/dev/hello-motor-lift', '/dev/hello-motor-right-wheel',
+                    '/dev/hello-motor-left-wheel']
     for d in device_names:
         if is_device_present(d):
             s.append(d)
     return s
+
+
 # ###################################
+
+def place_arduino_in_bootloader(port):
+    print('Putting %s into bootloader mode.'%port)
+    arduino = serial.Serial(port, baudrate=1200)
+    with arduino:  # the reset part is actually optional but the sleep is nice to have either way.
+        arduino.setDTR(False)
+        time.sleep(0.1)
+        arduino.flushInput()
+        arduino.setDTR(True)
+        time.sleep(0.1)
+        arduino.setDTR(False)
+        time.sleep(0.1)
+        arduino.flushInput()
+        arduino.setDTR(True)
+        time.sleep(0.5)
+
+
 def find_arduinos():
     devs = []
     all = usb.core.find(find_all=True)
     for dev in all:
         if dev.idVendor == 0x2341 and dev.idProduct == 0x804d:
             devs.append(dev)
     return devs
 
+
 def find_ftdis():
     devs = []
     all = usb.core.find(find_all=True)
     for dev in all:
         if dev.idVendor == 0x0403 and dev.idProduct == 0x6001:
             devs.append(dev)
     return devs
 
+
 # ###################################
 def get_dmesg():
     return exec_process(['sudo', 'dmesg', '-c'], True)
 
+
 def find_arduino():
     """
     Assumes Arduino data is already on dmesg
     """
     dmesg_data = get_dmesg()
     lines = dmesg_data.split(b'\n')
     for idx in range(len(lines)):
-        if lines[idx].find(b'Product: Hello')>0:
-            board=lines[idx][lines[idx].find(b'Product: ')+9:]
-            idx=min(idx+2,len(lines)-1)
-            if lines[idx].find(b'SerialNumber') >0:
-                sn=lines[idx][lines[idx].find(b'SerialNumber')+14:]
-                if lines[idx].find(b'SerialNumber') >0:
-                    sn=lines[idx][lines[idx].find(b'SerialNumber')+14:]
-                    idx=min(idx+1,len(lines)-1)
+        if lines[idx].find(b'Product: Hello') > 0:
+            board = lines[idx][lines[idx].find(b'Product: ') + 9:]
+            idx = min(idx + 2, len(lines) - 1)
+            if lines[idx].find(b'SerialNumber') > 0:
+                sn = lines[idx][lines[idx].find(b'SerialNumber') + 14:]
+                if lines[idx].find(b'SerialNumber') > 0:
+                    sn = lines[idx][lines[idx].find(b'SerialNumber') + 14:]
+                    idx = min(idx + 1, len(lines) - 1)
                     if lines[idx].find(b'ttyACM') > 0:
-                        port = b'/dev/'+lines[idx][lines[idx].find(b'ttyACM'):lines[idx].find(b'ttyACM')+7] #only ttyACM0-9
+                        port = b'/dev/' + lines[idx][
+                                          lines[idx].find(b'ttyACM'):lines[idx].find(b'ttyACM') + 7]  # only ttyACM0-9
                         if (is_device_present(port)):
                             print('---------------------------')
-                            print('Found board %s with SerialNumber %s on port %s'%(board,sn,port))
-                            return {'board':board,'serial':sn,'port':port}
+                            print('Found board %s with SerialNumber %s on port %s' % (board, sn, port))
+                            return {'board': board, 'serial': sn, 'port': port}
     print('No Arduino device device found')
-    return {'board':None,'serial':None,'port':None}
+    return {'board': None, 'serial': None, 'port': None}
+
 
 def find_ftdi_sn():
     try:
-        x=exec_process([b'sudo',b'lsusb', b'-d', b'0403:6001',b'-v'], True).split(b'\n')
+        x = exec_process([b'sudo', b'lsusb', b'-d', b'0403:6001', b'-v'], True).split(b'\n')
         for ln in x:
-            if ln.find(b'iSerial')>=0:
-                sn=ln.split(b' ')[-1]
+            if ln.find(b'iSerial') >= 0:
+                sn = ln.split(b' ')[-1]
                 return sn
     except RuntimeError:
         print('FTDI device not found')
         return None
 
+
 def find_shoulder_hub():
-    lsusb_out = Popen("lsusb | grep '1a40:0101'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip().split()
-    #Note: User periphs using Terminus may ID false positive
+    lsusb_out = Popen("lsusb | grep '1a40:0101'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,
+                      close_fds=True).stdout.read().strip().split()
+    # Note: User periphs using Terminus may ID false positive
     if len(lsusb_out):
         bus = lsusb_out[1]
         device = lsusb_out[3][:-1]
-        port= "/dev/bus/usb/%s/%s" % (bus, device)
-        print('Found shoulder hub IC on bus at %s'%port)
-        return {'success':1}
+        port = "/dev/bus/usb/%s/%s" % (bus, device)
+        print('Found shoulder hub IC on bus at %s' % port)
+        return {'success': 1}
     else:
         print('Terminus USB2 hub not found')
-        return {'success':0}
+        return {'success': 0}
+
 
 def find_ftdi_port():
-    lsusb_out = Popen("lsusb | grep -i %s"%'Future', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip().split()
+    lsusb_out = Popen("lsusb | grep -i %s" % 'Future', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,
+                      close_fds=True).stdout.read().strip().split()
     if len(lsusb_out):
         bus = lsusb_out[1]
         device = lsusb_out[3][:-1]
         return "/dev/bus/usb/%s/%s" % (bus, device)
     else:
         print('FTDI port not found')
         return None
+
+
 # ###################################
-def compile_arduino_firmware(sketch_name,repo_path):
+
+
+def compile_arduino_firmware(sketch_name, repo_path):
     """
     :param sketch_name: eg 'hello_stepper'
     :return T if success:
     """
+    text='------------------------ Compile Arduino Firmware {} ------------------------'.format(sketch_name)
+    print(Style.BRIGHT + Fore.BLUE + text + Style.RESET_ALL)
     compile_command = 'arduino-cli compile --fqbn hello-robot:samd:%s %s/arduino/%s' % (sketch_name, repo_path, sketch_name)
     print(compile_command)
     c = Popen(compile_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
-    return c.find(b'Sketch uses')>-1
+    return c.find(b'Sketch uses') > -1
+
 
 def burn_arduino_firmware(port, sketch_name,repo_path):
-    print('-------- Flashing firmware %s | %s ------------' % (port, sketch_name))
+    text='------------------------ Flashing firmware %s | %s ------------------------' % (port, sketch_name)
+    print(Style.BRIGHT + Fore.BLUE + text + Style.RESET_ALL)
+
     port_name = Popen("ls -l " + port, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip().split()[-1]
     port_name=port_name.decode("utf-8")
+    if '/dev/' != port_name[:5]:
+        port_name = f"/dev/{port_name}"
     if port_name is not None:
         upload_command = 'arduino-cli upload -p %s --fqbn hello-robot:samd:%s %s/arduino/%s' % (port_name, sketch_name,repo_path, sketch_name)
         print('Running: %s'%upload_command)
         u = Popen(upload_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
         uu = u.split(b'\n')
         #Pretty print the result
         for l in uu:
@@ -206,102 +303,110 @@
             else:
                 for m in k:
                     print(m.decode('utf-8'))
         print('################')
         success=uu[-1]==b'CPU reset.'
         if not success:
             print('Firmware flash. Failed to upload to %s'% ( port))
+            return False
         else:
             print('Success in firmware flash')
-        return success
+        return True
     else:
         print('Firmware flash. Failed to find device %s' % ( port))
         return False
 
 def burn_bootloader(sketch):
     print('-------- Burning bootlader ------------')
     cmd = 'arduino-cli burn-bootloader -b hello-robot:samd:%s -P sam_ice' % sketch
     cmdl = ['arduino-cli', 'burn-bootloader', '-b', 'hello-robot:samd:%s' % sketch, '-P', 'sam_ice']
     print(cmd)
     u = subprocess.call(cmdl)
-    return u==0
+    return u == 0
+
 
 # ##################################
 
 def reset_arduino_usb():
     USBDEVFS_RESET = 21780
-    lsusb_out = Popen("lsusb | grep -i %s"%'Arduino', shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip().split()
-    while len(lsusb_out):
-        bus = lsusb_out[1]
-        device = lsusb_out[3][:-1]
+    lsusb_out = Popen("lsusb | grep -i Arduino", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
+    if type(lsusb_out)==bytes:
+        lsusb_out=lsusb_out.decode('utf-8')
+    lsusb_out=lsusb_out.strip().split('\n')
+    for d in lsusb_out:
+        dd=d.split(' ')
+        bus = dd[1]
+        device = dd[3][:-1]
         try:
-            print('Resetting Arduino. Bus:',bus, 'Device: ',device)
+            print('Resetting Arduino. Bus:', bus, 'Device: ', device)
             f = open("/dev/bus/usb/%s/%s" % (bus, device), 'w', os.O_WRONLY)
             fcntl.ioctl(f, USBDEVFS_RESET, 0)
         except Exception as msg:
-            print("failed to reset device: %s"%msg)
-        lsusb_out=lsusb_out[8:]
+            print("failed to reset device: %s" % msg)
+
+
 
 # ##############################################################
 
-def run_firmware_flash(port,sketch,repo_path=''):
-    #Return board serial # / success
-    print('### Running Firmware Flash on port %s and sketch %s'%(port,sketch))
+def run_firmware_flash(port, sketch, repo_path=''):
+    # Return board serial # / success
+    print('### Running Firmware Flash on port %s and sketch %s' % (port, sketch))
     print('###################################################################')
     if burn_bootloader(sketch):
         print('SUCCESS: Burned bootloader')
     else:
         print('FAIL: Could not burn bootlaoder')
-        return  {'success':0,'sn':None}
+        return {'success': 0, 'sn': None}
     time.sleep(2.0)
     if is_device_present(port):
-        print('SUCCESS: Found PCBA on %s'%port)
+        print('SUCCESS: Found PCBA on %s' % port)
     else:
-        print('FAIL: Did not find PCBA on %s'%port)
-        return  {'success':0,'sn':None}
+        print('FAIL: Did not find PCBA on %s' % port)
+        return {'success': 0, 'sn': None}
 
-    if compile_arduino_firmware(sketch,repo_path):
+    if compile_arduino_firmware(sketch, repo_path):
         print('SUCCESS: Found compiled sketch %s' % sketch)
     else:
         print('FAIL: Could not compile sketch %s' % sketch)
-        return  {'success':0,'sn':None}
+        return {'success': 0, 'sn': None}
 
     get_dmesg()
-    if burn_arduino_firmware(port,sketch,repo_path):
+    if burn_arduino_firmware(port, sketch, repo_path):
         print('SUCCESS: Flashed sketch %s' % sketch)
     else:
         print('FAIL: Could not flash sketch %s' % sketch)
-        return  {'success':0,'sn':None}
+        return {'success': 0, 'sn': None}
     time.sleep(2.0)
     x = find_arduino()
     if x['serial'] is not None:
         print('###################################################################')
         print('SUCCESS: Firmware flash complete')
         return {'success': 1, 'sn': x['serial']}
     else:
         print('###################################################################')
         print('Failure: could not find board SN')
         return {'success': 0, 'sn': x['serial']}
 
 
 # ######################## RDK Tools ##########################################
-def modify_bashrc(env_var,env_var_val):
-    f=open(os.environ['HOME']+'/.bashrc','r')
-    x=f.readlines()
-    x_out=''
+def modify_bashrc(env_var, env_var_val):
+    f = open(os.environ['HOME'] + '/.bashrc', 'r')
+    x = f.readlines()
+    x_out = ''
     for xx in x:
-        if xx.find(env_var)>0:
-            x_out=x_out+'export '+env_var+'='+env_var_val+'\n'
+        if xx.find(env_var) > 0:
+            x_out = x_out + 'export ' + env_var + '=' + env_var_val + '\n'
         else:
-            x_out=x_out+xx
+            x_out = x_out + xx
     f.close()
-    f=open(os.environ['HOME']+'/.bashrc','w')
+    f = open(os.environ['HOME'] + '/.bashrc', 'w')
     f.write(x_out)
     f.close()
 
+
 def add_arduino_udev_line_etc(device_name, serial_no):
     f = open('/etc/udev/rules.d/95-hello-arduino.rules', 'r')
     x = f.readlines()
     x_out = ''
     overwrite = False
     uline = 'KERNEL=="ttyACM*", ATTRS{idVendor}=="2341", ATTRS{idProduct}=="804d",MODE:="0666", ATTRS{serial}=="' + serial_no + '", SYMLINK+="' + device_name + '", ENV{ID_MM_DEVICE_IGNORE}="1"\n'
     for xx in x:
@@ -311,97 +416,167 @@
             print('Overwriting existing entry...')
         else:
             x_out = x_out + xx
     if not overwrite:
         print('Creating new entry...')
         x_out = x_out + uline
     f.close()
-    f = open( '/tmp/95-hello-arduino.rules', 'w')
+    f = open('/tmp/95-hello-arduino.rules', 'w')
     f.write(x_out)
     f.close()
     os.system('sudo cp /tmp/95-hello-arduino.rules /etc/udev/rules.d')
 
-def add_arduino_udev_line(device_name, serial_no,fleet_dir):
-    f = open(fleet_dir+'udev/95-hello-arduino.rules', 'r')
+
+def add_arduino_udev_line(device_name, serial_no, fleet_dir):
+    f = open(fleet_dir + 'udev/95-hello-arduino.rules', 'r')
     x = f.readlines()
     x_out = ''
-    overwrite=False
-    uline = 'KERNEL=="ttyACM*", ATTRS{idVendor}=="2341", ATTRS{idProduct}=="804d",MODE:="0666", ATTRS{serial}=="'+serial_no + '", SYMLINK+="'+device_name+'", ENV{ID_MM_DEVICE_IGNORE}="1"\n'
+    overwrite = False
+    uline = 'KERNEL=="ttyACM*", ATTRS{idVendor}=="2341", ATTRS{idProduct}=="804d",MODE:="0666", ATTRS{serial}=="' + serial_no + '", SYMLINK+="' + device_name + '", ENV{ID_MM_DEVICE_IGNORE}="1"\n'
     for xx in x:
-        if xx.find(device_name) > 0 and xx[0]!='#':
-            overwrite=True
+        if xx.find(device_name) > 0 and xx[0] != '#':
+            overwrite = True
             x_out = x_out + uline
             print('Overwriting existing entry...')
         else:
             x_out = x_out + xx
     if not overwrite:
         print('Creating new entry...')
         x_out = x_out + uline
     f.close()
-    f = open(fleet_dir+'udev/95-hello-arduino.rules', 'w')
+    f = open(fleet_dir + 'udev/95-hello-arduino.rules', 'w')
     f.write(x_out)
     f.close()
 
-def add_ftdi_udev_line(device_name, serial_no,fleet_dir):
-    f = open(fleet_dir+'udev/99-hello-dynamixel.rules', 'r')
+
+def add_ftdi_udev_line(device_name, serial_no, fleet_dir):
+    f = open(fleet_dir + 'udev/99-hello-dynamixel.rules', 'r')
     x = f.readlines()
     x_out = ''
-    overwrite=False
-    uline = 'SUBSYSTEM=="tty", ATTRS{idVendor}=="0403", ATTRS{idProduct}=="6001", ATTR{device/latency_timer}="1", ATTRS{serial}=="'+serial_no+'", SYMLINK+="'+device_name+'"'
+    overwrite = False
+    uline = 'SUBSYSTEM=="tty", ATTRS{idVendor}=="0403", ATTRS{idProduct}=="6001", ATTR{device/latency_timer}="1", ATTRS{serial}=="' + serial_no + '", SYMLINK+="' + device_name + '"'
     for xx in x:
-        if xx.find(device_name) > 0 and xx[0]!='#':
-            overwrite=True
-            x_out = x_out + uline +'\n'
+        if xx.find(device_name) > 0 and xx[0] != '#':
+            overwrite = True
+            x_out = x_out + uline + '\n'
             print('Overwriting existing entry...')
         else:
             x_out = x_out + xx
     if not overwrite:
         print('Creating new entry...')
         x_out = x_out + uline + '\n'
     f.close()
-    f = open(fleet_dir+'udev/99-hello-dynamixel.rules', 'w')
+    f = open(fleet_dir + 'udev/99-hello-dynamixel.rules', 'w')
     f.write(x_out)
     f.close()
 
-def assign_arduino_to_robot(device_name,is_stepper=False,robot_sn=None):
+
+def get_serial_nos_from_udev(udev_file_full_path, device_name):
+    sns = []
+    try:
+        f = open(udev_file_full_path, 'r')
+        x = f.readlines()
+        f.close()
+        lines = []
+        for xx in x:
+            if xx.find(device_name) > 0 and xx[0] != '#':
+                lines.append(xx)
+        for l in lines:
+            ll = l.split(',')
+            for q in ll:
+                if q.find('serial') > -1:
+                    s = q[q.find('"') + 1:q.rfind('"')]
+                    if len(s) == 8 or len(s) == 32:  # FTDI or Arduino
+                        sns.append(s)
+    except:
+        pass
+    return sns
+
+
+def assign_arduino_to_robot(device_name, is_stepper=False, robot_sn=None):
     """
     This expects only a single arduino device on the bus
     Tie the uC serial number to device_name under udev
     Also update the YAML with the serial number if a stepper
     The YAML writing requres the HELLO_FLEET_ID to be set in advance
     """
     if robot_sn is None:
-       fleet_dir=hello_utils.get_fleet_directory()
+        fleet_dir = hello_utils.get_fleet_directory()
     else:
-        fleet_dir=os.environ['HELLO_FLEET_PATH']+'/'+robot_sn+'/'
+        fleet_dir = os.environ['HELLO_FLEET_PATH'] + '/' + robot_sn + '/'
     a = find_arduinos()
     if len(a) != 1:
         print('Error: Only one Arduino should be on the bus')
     else:
-        sn=str(a[0].serial_number)
-        add_arduino_udev_line(device_name,sn,fleet_dir)
+        sn = str(a[0].serial_number)
+        add_arduino_udev_line(device_name, sn, fleet_dir)
         if is_stepper:
-            print('Setting serial number in YAML for %s to %s'%(device_name,sn))
+            print('Setting serial number in YAML for %s to %s' % (device_name, sn))
             d = stretch_body.device.Device(req_params=False)
-            d.write_configuration_param_to_YAML(device_name+'.serial_no', sn,fleet_dir=fleet_dir)
-        return  {'success': 1, 'sn': sn}
-    return  {'success': 0, 'sn':None}
+            d.write_configuration_param_to_YAML(device_name + '.serial_no', sn, fleet_dir=fleet_dir)
+        return {'success': 1, 'sn': sn}
+    return {'success': 0, 'sn': None}
+
 
 def assign_dynamixel_to_robot(device_name, robot_sn=None):
     """
     This expects only a single FTDI device on the bus
     Tie the FTDI serial number to device_name under udev
     """
-    print('A',hello_utils.get_fleet_directory())
-    print('B',os.environ['HELLO_FLEET_PATH'],robot_sn)
+    print('A', hello_utils.get_fleet_directory())
+    print('B', os.environ['HELLO_FLEET_PATH'], robot_sn)
     if robot_sn is None:
-        fleet_dir=hello_utils.get_fleet_directory()
+        fleet_dir = hello_utils.get_fleet_directory()
     else:
-        fleet_dir=os.environ['HELLO_FLEET_PATH']+'/'+robot_sn+'/'
-    f=find_ftdis()
+        fleet_dir = os.environ['HELLO_FLEET_PATH'] + '/' + robot_sn + '/'
+    f = find_ftdis()
     if len(f) != 1:
         print('Error: Only one FTDI should be on the bus')
     else:
-        sn=f[0].serial_number
-        add_ftdi_udev_line(device_name,sn,fleet_dir)
-        return  {'success': 1, 'sn': sn}
-    return  {'success': 0, 'sn':None}
+        sn = f[0].serial_number
+        add_ftdi_udev_line(device_name, sn, fleet_dir)
+        return {'success': 1, 'sn': sn}
+    return {'success': 0, 'sn': None}
+
+
+def find_tty_devices():
+    """
+    Returns a dictionary of USB device details of tty class in the ttyUSB* and ttyACM* namespace.
+    """
+    devices_dict = {}
+    ttyUSB_dev_list = glob.glob('/dev/ttyUSB*')
+    ttyACM_dev_list = glob.glob('/dev/ttyACM*')
+    for d in ttyACM_dev_list:
+        devices_dict[d] = {"serial": extract_udevadm_info(d, 'ID_SERIAL_SHORT'),
+                           "vendor": extract_udevadm_info(d, 'ID_VENDOR'),
+                           "model": extract_udevadm_info(d, 'ID_MODEL'),
+                           "path": extract_udevadm_info(d, 'DEVPATH')}
+    for d in ttyUSB_dev_list:
+        devices_dict[d] = {"serial": extract_udevadm_info(d, 'ID_SERIAL_SHORT'),
+                           "vendor": extract_udevadm_info(d, 'ID_VENDOR'),
+                           "model": extract_udevadm_info(d, 'ID_MODEL'),
+                           "path": extract_udevadm_info(d, 'DEVPATH')}
+    return devices_dict
+
+
+def extract_udevadm_info(usb_port, ID_NAME=None):
+    """
+    Extracts usb device attributes with the given attribute ID_NAME
+
+    example ID_NAME:
+    ID_SERIAL_SHORT
+    ID_MODEL
+    DEVPATH
+    ID_VENDOR_FROM_DATABASE
+    ID_VENDOR
+    """
+    value = None
+    dname = bytes(usb_port[5:], 'utf-8')
+    out = exec_process([b'udevadm', b'info', b'-n', dname], True)
+    if ID_NAME is None:
+        value = out.decode(encoding='UTF-8')
+    else:
+        for a in out.split(b'\n'):
+            a = a.decode(encoding='UTF-8')
+            if "{}=".format(ID_NAME) in a:
+                value = a.split('=')[-1]
+    return value
```

### Comparing `hello_robot_stretch_factory-0.3.9/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.0/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.0/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.0/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.0/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_D435i_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,28 +108,28 @@
               'Gyro': {'target': 900, 'sampled': 0}}}
     return target
 
 def check_install_v4l2():
     global check_log
     out = Popen("which v4l2-ctl", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
     if len(out):
-        out = Popen("v4l2-ctl --all | grep -A 3 -i 'uvcvideo'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
+        out = Popen("v4l2-ctl --all | grep -A 3 -i 'uvcvideo'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().decode("utf-8")
         check_log.append(out)
         print(out)
     else:
         print('"v4l2-utils" tool is required to be installed for logging USB video driver info.')
-        x = raw_input('Enter "y" to proceed with Installation of "v4l2-utils".\n')
+        x = input('Enter "y" to proceed with Installation of "v4l2-utils".\n')
         if x=='y' or x=='Y':
             print('Installing v4l2-utils tool.....')
             script = 'sudo apt-get install -y v4l-utils'
             os.system(script)
             check = Popen("which v4l2-ctl", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
             if check:
                 print(Fore.GREEN +'[Pass] "v4l2-utils" sucessfully installed'+Style.RESET_ALL+'\n\n')
-                out = Popen("v4l2-ctl --all | grep -A 3 -i 'uvcvideo'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
+                out = Popen("v4l2-ctl --all | grep -A 3 -i 'uvcvideo'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().decode("utf-8")
                 check_log.append(out)
                 print(out)
             else:
                 print(Fore.RED + '[Fail] "v4l2-utils" did not install.'+Style.RESET_ALL)
         else:
             print(Fore.YELLOW+'[Warning] Skip logging USB Video Drivers.'+Style.RESET_ALL)
 
@@ -139,15 +139,15 @@
     Gets the USB Bus number and device ID for monitoring
     Execute it at Start
     """
     global usbtop_cmd, check_log
     print('Starting D435i Check')
     print('====================')
     print('Searching for Realsense D435i in USB Bus...')
-    out = Popen("usb-devices | grep -B 5 -i 'RealSense' | grep -i 'Bus'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
+    out = Popen("usb-devices | grep -B 5 -i 'RealSense' | grep -i 'Bus'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
     if(len(out)):
         out_list = out.split(' ')
         bus_no = None
         dev_id = None
         usb_found = False
         for i in range(len(out_list)):
             if out_list[i].find('Bus')!=-1:
@@ -167,44 +167,44 @@
     else:
         print(Fore.RED + '[Fail] Realsense D435i not found at USB Bus'+Style.RESET_ALL)
         check_log.append('[Fail] Realsense D435i not found at USB Bus')
         sys.exit()         
 
 def check_usb():
     global check_log
-    out = Popen("rs-enumerate-devices| grep Usb | grep 3.2", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
+    out = Popen("rs-enumerate-devices| grep Usb | grep 3.2", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
     if len(out):
         print(Fore.GREEN +'[Pass] Confirmed USB 3.2 connection to device'+Style.RESET_ALL)
         check_log.append('[Pass] Confirmed USB 3.2 connection to device')
     else:
         print(Fore.RED +'[Fail] Did not find USB 3.2 connection to device'+Style.RESET_ALL)
         check_log.append('[Fail] Did not find USB 3.2 connection to device')
 
 def get_driver_versions():
     global check_log
-    fw_details = Popen("rs-fw-update -l | grep -i 'firmware'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
+    fw_details = Popen("rs-fw-update -l | grep -i 'firmware'", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
     fw_details = fw_details.split(',')[3]
     fw_version = fw_details.split(' ')[-1]
     print('D435i Firmware version: %s'%(fw_version))
-    nuc_bios_version = Popen("sudo dmidecode -s bios-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
-    system_version = Popen("sudo dmidecode -s system-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
-    baseboard_version = Popen("sudo dmidecode -s baseboard-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
-    processor_version = Popen("sudo dmidecode -s processor-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
-    kernel_version = Popen("uname -r", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read()
+    nuc_bios_version = Popen("sudo dmidecode -s bios-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
+    system_version = Popen("sudo dmidecode -s system-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
+    baseboard_version = Popen("sudo dmidecode -s baseboard-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
+    processor_version = Popen("sudo dmidecode -s processor-version", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
+    kernel_version = Popen("uname -r", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().decode("utf-8")
     check_install_v4l2()
     check_log.append('\nD435i Firmware version: %s\n'%(fw_version))
     check_log.append("Linux Kernel Version : %s"%(kernel_version))
     check_log.append("NUC Bios Version : %s"%(nuc_bios_version))
     check_log.append("NUC System Version : %s"%(system_version))
     check_log.append("NUC Baseboard Version : %s"%(baseboard_version))
     check_log.append("Processor Version : %s"%(processor_version))
     
 def check_ros():
     global check_log
-    ros_out = Popen("rostopic list", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True,stderr=PIPE).stdout.read()
+    ros_out = Popen("rostopic list", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True,stderr=PIPE).stdout.read().decode("utf-8")
     if ros_out:
         print(Fore.YELLOW+'[Warning] roscore is running in background. Recommended to stop roscore.'+Style.RESET_ALL)
         check_log.append('\nroscore is running in background')
 
 def get_frame_id_from_log_line(stream_type,line):
     if line.find(stream_type)!=0:
         return None
@@ -285,15 +285,15 @@
         print(Fore.GREEN+'[Pass] No unexpected dmesg warnings')
     print(Style.RESET_ALL)
 
 def check_dmesg_thread():
     global thread_stop, check_log, pan_tilt_pos, dmesg_log
     print('\nMonitoring the DMESG Buffer for issues while collecting camera stream.\n\n')
     while thread_stop==False:
-        out = hdu.exec_process(['sudo', 'dmesg', '-c'], True).split('\n')
+        out = hdu.exec_process(['sudo', 'dmesg', '-c'], True).decode("utf-8").split('\n')
         filtered_out = []
         filters = ['uvc','usb','input','hid']
         for o in out:
             for f in filters:
                 if f in o:
                     filtered_out.append(o)
                     break
@@ -360,15 +360,15 @@
     usbtop_proc = Popen(usbtop_cmd,stdout=PIPE,shell=True)
 
     if robot:
         scan_head_thread = Thread(target=scan_head_sequence,args=[robot,])
         scan_head_thread.start()
 
     cmd='rs-data-collect -c /tmp/d435i_confg.cfg -f /tmp/d435i_log.csv -t %d -m %d'%(target['duration'],target['nframe'])
-    out = Popen(cmd, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()    
+    out = Popen(cmd, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().decode("utf-8")
     usbtop_proc.kill()
 
     ff=open('/tmp/d435i_log.csv') 
     data=ff.readlines()
     data=data[10:] #drop preamble
     check_frames_collected(data,target)
     check_FPS(data)
@@ -525,33 +525,33 @@
     check_dmesg(dmesg_log)
     save_collected_log(check_log)
 
 def check_install_usbtop():
     """
     Function to be executed at start. Checks for usbtop and if not prompts the user for installation.
     """
-    out = Popen("which usbtop", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
+    out = Popen("which usbtop", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().decode("utf-8")
     if len(out):
         return None
     else:
         print('"usbtop" tool is required to be installed for running this test first time.')
-        x = raw_input('Enter "y" to proceed with Installation of "usbtop".\n')
+        x = input('Enter "y" to proceed with Installation of "usbtop".\n')
 
         if x=='y' or x=='Y':
             script = 'cd ~/'
             script = script+';git clone https://github.com/aguinet/usbtop.git'
             script = script+';cd usbtop'
             script = script+';sudo apt install libboost-dev libpcap-dev libboost-thread-dev libboost-system-dev cmake'
             script = script+';mkdir _build && cd _build'
             script = script+';cmake -DCMAKE_BUILD_TYPE=Release ..'
             script = script+';make'
             script = script+';sudo make install'
             print('Installing usbtop tool.....')
             os.system(script)
-            check = Popen("which usbtop", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read()
+            check = Popen("which usbtop", shell=True, bufsize=64, stdin=PIPE, stdout=PIPE,close_fds=True).stdout.read().decode("utf-8")
             if check:
                 print(Fore.GREEN +'[Pass] "usbtop" sucessfully installed'+Style.RESET_ALL+'\n\n')
             else:
                 print(Fore.RED + '[Fail] "usbtop" did not install.'+Style.RESET_ALL)
                 sys.exit()
         else:
             print('Exiting...')
```

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_guarded_contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 if args.lift:
     import stretch_body.lift
     j=stretch_body.lift.Lift()
 if args.arm:
     import stretch_body.arm
     j=stretch_body.arm.Arm()
 
-if j.robot_params['robot']['model_name']=='RE1V0':
-    print('This is tool is not yet supported for robot model RE1V0')
-    exit(1)
+check_deprecated_contact_model_prismatic_joint(j, 'REx_calibrate_guarded_contacts.py', None, None, None, None)
 
 if not j.startup(threaded=False):
     exit(1)
 
 j.pull_status()
 if not j.motor.status['pos_calibrated']:
     print('Joint not calibrated. Exiting.')
```

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_firmware_updater.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #!/usr/bin/env python
 import argparse
-from stretch_factory.firmware_updater import *
+from stretch_factory.firmware_available import FirmwareAvailable
+from stretch_factory.firmware_recommended import FirmwareRecommended
+from stretch_factory.firmware_installed import FirmwareInstalled
+from stretch_factory.firmware_updater import FirmwareUpdater
 import os
+import click
+import stretch_factory.hello_device_utils as hdu
 
 parser = argparse.ArgumentParser(description='Upload Stretch firmware to microcontrollers')
 
 group = parser.add_mutually_exclusive_group()
 group.add_argument("--current", help="Display the currently installed firmware versions", action="store_true")
 group.add_argument("--available", help="Display the available firmware versions", action="store_true")
 group.add_argument("--recommended", help="Display the recommended firmware", action="store_true")
 group.add_argument("--install", help="Install the recommended firmware", action="store_true")
 group.add_argument("--install_version", help="Install a specific firmware version", action="store_true")
 group.add_argument("--install_branch", help="Install the HEAD of a specific branch", action="store_true")
 group.add_argument("--install_path", help="Install the firmware on the provided path (eg ./stretch_firmware/arduino)", type=str)
+group.add_argument("--resume", help="Resume an install in progress", action="store_true")
 group.add_argument("--mgmt", help="Display overview on firmware management", action="store_true")
+parser.add_argument("--map", help="Print mapping from ttyACMx to Hello device", action="store_true")
 
 parser.add_argument("--pimu", help="Upload Pimu firmware", action="store_true")
 parser.add_argument("--wacc", help="Upload Wacc firmware", action="store_true")
 parser.add_argument("--arm", help="Upload Arm Stepper firmware", action="store_true")
 parser.add_argument("--lift", help="Upload Lift Stepper firmware", action="store_true")
 parser.add_argument("--left_wheel", help="Upload Left Wheel Stepper firmware", action="store_true")
 parser.add_argument("--right_wheel", help="Upload Right Wheel Stepper firmware", action="store_true")
@@ -88,45 +95,43 @@
 else:
     use_device = {'hello-motor-arm': True, 'hello-motor-right-wheel': True, 'hello-motor-left-wheel': True, 'hello-pimu': True, 'hello-wacc': True,'hello-motor-lift': True}
 
 if args.mgmt:
     print(mgmt)
     exit()
 
+if args.map:
+        mapping = hdu.get_hello_ttyACMx_mapping()
+        click.secho('------------------------------------------', fg="yellow", bold=True)
+        for k in mapping['hello']:
+            print('%s | %s' % (k, mapping['hello'][k]))
+        click.secho('------------------------------------------', fg="yellow", bold=True)
+        for k in mapping['ACMx']:
+            print('%s | %s' % (k, mapping['ACMx'][k]))
+        click.secho('------------------------------------------', fg="yellow", bold=True)
+        print('')
+        exit()
+
 if args.current:
-    c = InstalledFirmware(use_device)
+    c = FirmwareInstalled(use_device)
     c.pretty_print()
     exit()
 
 if args.recommended:
-    r = RecommendedFirmware(use_device)
+    r = FirmwareRecommended(use_device)
     r.pretty_print()
     r.print_recommended_args()
     exit()
 
 if args.available:
-    a = AvailableFirmware(use_device)
+    a = FirmwareAvailable(use_device)
     a.pretty_print()
     exit()
 
-if args.install or args.install_version or args.install_branch or args.install_path:
-    cwd=os.getcwd()
-    u = FirmwareUpdater(use_device)
-    if not u.startup():
-        exit()
-    if args.install:
-        u.fw_recommended.pretty_print()
-        print('')
-        print('')
-        u.do_update(no_prompts=args.no_prompts,verbose=args.verbose)
-    elif args.install_version:
-        u.do_update_to(verbose=args.verbose)
-    elif args.install_branch:
-        u.do_update_to_branch(verbose=args.verbose)
-    elif args.install_path:
-        if args.install_path[0]!='/':
-            u.do_update_to_path(cwd+'/'+args.install_path,verbose=args.verbose)
-        else:
-            u.do_update_to_path(args.install_path,verbose=args.verbose)
+
+if args.resume or args.install or args.install_version or args.install_branch or args.install_path:
+    u = FirmwareUpdater(use_device, args)
+    u.run()
+    exit()
 else:
     parser.print_help()
```

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.3.9/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.0/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

